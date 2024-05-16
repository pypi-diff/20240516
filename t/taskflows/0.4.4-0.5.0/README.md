# Comparing `tmp/taskflows-0.4.4-py3-none-any.whl.zip` & `tmp/taskflows-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 23894 bytes, number of entries: 16
+Zip file size: 24408 bytes, number of entries: 16
 -rw-rw-r--  2.0 unx       87 b- defN 24-Feb-15 20:59 taskflows/__init__.py
--rw-rw-r--  2.0 unx    10229 b- defN 24-May-07 20:34 taskflows/admin.py
+-rw-rw-r--  2.0 unx    10107 b- defN 24-May-15 20:52 taskflows/admin.py
 -rw-rw-r--  2.0 unx     3444 b- defN 24-May-01 00:36 taskflows/db.py
 -rw-rw-r--  2.0 unx     8937 b- defN 24-Mar-05 14:35 taskflows/tasks.py
 -rw-rw-r--  2.0 unx      564 b- defN 24-Feb-12 20:43 taskflows/utils.py
--rwxrwxr-x  2.0 unx      587 b- defN 24-May-02 17:22 taskflows/service/__init__.py
+-rwxrwxr-x  2.0 unx      699 b- defN 24-May-15 20:52 taskflows/service/__init__.py
 -rwxrwxr-x  2.0 unx     1286 b- defN 24-Feb-29 14:30 taskflows/service/commands.py
 -rwxrwxr-x  2.0 unx     1586 b- defN 24-Feb-12 20:43 taskflows/service/constraints.py
--rw-rw-r--  2.0 unx    18204 b- defN 24-Apr-22 18:48 taskflows/service/docker.py
+-rw-rw-r--  2.0 unx    21124 b- defN 24-May-15 13:34 taskflows/service/docker.py
 -rwxrwxr-x  2.0 unx     2234 b- defN 24-Feb-12 20:43 taskflows/service/schedule.py
--rwxrwxr-x  2.0 unx    18155 b- defN 24-May-07 19:56 taskflows/service/service.py
--rw-rw-r--  2.0 unx     4293 b- defN 24-May-13 18:06 taskflows-0.4.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-13 18:06 taskflows-0.4.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx      111 b- defN 24-May-13 18:06 taskflows-0.4.4.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       10 b- defN 24-May-13 18:06 taskflows-0.4.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1294 b- defN 24-May-13 18:06 taskflows-0.4.4.dist-info/RECORD
-16 files, 71113 bytes uncompressed, 21772 bytes compressed:  69.4%
+-rwxrwxr-x  2.0 unx    17746 b- defN 24-May-15 15:51 taskflows/service/service.py
+-rw-rw-r--  2.0 unx     4293 b- defN 24-May-16 00:30 taskflows-0.5.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-16 00:30 taskflows-0.5.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      111 b- defN 24-May-16 00:30 taskflows-0.5.0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       10 b- defN 24-May-16 00:30 taskflows-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1294 b- defN 24-May-16 00:30 taskflows-0.5.0.dist-info/RECORD
+16 files, 73614 bytes uncompressed, 22286 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: taskflows/service/schedule.py
 Comment: 
 
 Filename: taskflows/service/service.py
 Comment: 
 
-Filename: taskflows-0.4.4.dist-info/METADATA
+Filename: taskflows-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: taskflows-0.4.4.dist-info/WHEEL
+Filename: taskflows-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: taskflows-0.4.4.dist-info/entry_points.txt
+Filename: taskflows-0.5.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: taskflows-0.4.4.dist-info/top_level.txt
+Filename: taskflows-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: taskflows-0.4.4.dist-info/RECORD
+Filename: taskflows-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## taskflows/admin.py

```diff
@@ -1,40 +1,57 @@
 import re
 import subprocess
+from collections import defaultdict
+from fnmatch import fnmatch
 from functools import lru_cache
 from itertools import cycle
-from pprint import pformat, pprint
-from typing import Optional, Tuple
-from collections import defaultdict
+from pprint import pformat
+from typing import List, Union
 
 import click
 import sqlalchemy as sa
 from click.core import Group
-from dynamic_imports import import_module
+from dynamic_imports import class_inst
 from rich import box
 from rich.console import Console
 from rich.table import Table
 
 from .db import task_flows_db
 from .service import (
-    systemd_dir,
+    DockerService,
     Service,
     disable_service,
     enable_service,
     get_service_files,
     get_timer_files,
     remove_service,
     restart_service,
     service_cmd,
     service_runs,
     start_service,
     stop_service,
+    systemd_dir,
+    systemd_manager,
 )
 from .utils import _SYSTEMD_FILE_PREFIX
 
+
+def discover_services(search_in: str) -> List[Union[DockerService, Service]]:
+    """Search for services in a Python module or package."""
+    services = []
+    for class_t in (DockerService, Service):
+        services.extend(class_inst(class_type=class_t, search_in=search_in))
+    return services
+
+
+def get_service_names():
+    """Get names of all services that have been created."""
+    return [f.stem.replace(_SYSTEMD_FILE_PREFIX, "") for f in get_service_files()]
+
+
 cli = Group("taskflows", chain=True)
 
 
 @cli.command()
 @click.option(
     "-l",
     "--limit",
@@ -71,34 +88,40 @@
     for c in columns:
         table.add_column(c, style=column_color(c), justify="center")
     for row in rows:
         table.add_row(*[str(row[c]) for c in columns])
     console.print(table, justify="center")
 
 
-@cli.command
-@click.argument("service_name")
-def status(service_name: str):
-    """Get status of service."""
-    proc = service_cmd(service_name=service_name, command="status")
-    pprint(proc.stderr.decode().split("\n"))
-    pprint(proc.stdout.decode().split("\n"))
-    # manager.GetUnitFileState(service)
-
-
 @cli.command(name="list")
 def list_services():
     """List services."""
-    services = [f.stem.replace(_SYSTEMD_FILE_PREFIX,"") for f in get_service_files()]
+    services = get_service_names()
     if services:
         click.echo(pformat(services))
     else:
         click.echo(click.style("No services found.", fg="yellow"))
 
 
+@cli.command
+@click.argument("service_name", required=False)
+def status(service_name: str):
+    """Get status of service(s)."""
+    if service_name:
+        service_names = [service_name]
+    else:
+        service_names = get_service_names()
+    for sn in service_names:
+        proc = service_cmd(service_name=sn, command="status")
+        err = proc.stderr.decode().strip()
+        info = proc.stdout.decode().strip()
+        state = systemd_manager().GetUnitFileState(f"taskflow_{sn}.service").strip()
+        print(f"----------{sn} status----------\n{state}\n{err}\n{info}\n\n")
+
+
 @cli.command()
 @click.option(
     "-m", "--match", help="Only show for this service name or service name pattern."
 )
 def schedule(match: str = None):
     """List service schedules."""
     table = _service_schedules_table(running_only=False, match=match)
@@ -130,90 +153,74 @@
     )
     subprocess.run(
         f"journalctl --user -f -u {_SYSTEMD_FILE_PREFIX}{service_name}".split()
     )
 
 
 @cli.command()
-@click.argument("service_file", default="deployments.py")
+@click.argument("search-in")
 @click.option(
-    "-i",
-    "--include",
-    multiple=True,
-    help="Name(s) of service(s)/service list(s) that should be created.",
+    "-c",
+    "--command",
+    type=str,
+    help="Command that should be ran on discovered services (e.g. create, enable, disable, remove, restart, run, stop).",
 )
 @click.option(
-    "-im",
-    "--include-matching",
-    multiple=True,
-    help="Substring(s) of service(s)/service list(s) names that should be created.",
+    "-i",
+    "--include",
+    type=str,
+    help="Name or glob pattern of services that should be included.",
 )
 @click.option(
     "-e",
     "--exclude",
-    multiple=True,
-    help="Name(s) of service(s)/service list(s) that should not be created.",
-)
-@click.option(
-    "-em",
-    "--exclude-matching",
-    multiple=True,
-    help="Substring(s) of service(s)/service list(s) names that should not be created.",
+    type=str,
+    help="Name or glob pattern of services that should be excluded.",
 )
-def create(
-    service_file: str,
-    include: Optional[Tuple[str]] = None,
-    include_matching: Optional[Tuple[str]] = None,
-    exclude: Optional[Tuple[str]] = None,
-    exclude_matching: Optional[Tuple[str]] = None,
+def search(
+    search_in,
+    command,
+    include,
+    exclude,
 ):
-    """Create services from a Python file containing services/service lists or dict with services or service lists as values."""
-    services = {}
-    for member in import_module(service_file).__dict__.values():
-        if isinstance(member, Service):
-            services[member.name] = member
-        elif isinstance(member, (list, tuple)):
-            services.update({m.name: m for m in member if isinstance(m, Service)})
-        elif isinstance(member, dict):
-            for k, v in member.items():
-                if isinstance(v, Service):
-                    services[v.name] = v
-                    services[k] = v
-                elif isinstance(v, (list, tuple)) and (
-                    v := {m.name: m for m in v if isinstance(m, Service)}
-                ):
-                    services.update(v)
-                    services[k] = v
+    """Search for and run a command on services from a Python file or package."""
+    services = discover_services(search_in)
     if include:
-        services = {
-            k: v for k, v in services.items() if any(name == k for name in include)
-        }
-    if include_matching:
-        services = {
-            k: v
-            for k, v in services.items()
-            if any(name in k for name in include_matching)
-        }
+        services = [s for s in services if fnmatch(include, s.name)]
     if exclude:
-        services = {
-            k: v for k, v in services.items() if not any(name == k for name in exclude)
-        }
-    if exclude_matching:
-        services = {
-            k: v
-            for k, v in services.items()
-            if not any(name in k for name in exclude_matching)
-        }
-    click.echo(
-        click.style(
-            f"Creating {len(services)} service(s) from {service_file}.", fg="cyan"
+        services = [s for s in services if not fnmatch(exclude, s.name)]
+    services_str = "\n\n".join([str(s) for s in services])
+    if command:
+        click.echo(
+            click.style(
+                f"{command.title()}ing {len(services)} service(s) from {search_in}:\n{services_str}",
+                fg="cyan",
+            )
         )
-    )
-    for srv in services.values():
-        srv.create()
+        for srv in services:
+            getattr(srv, command)()
+    else:
+        click.echo(
+            click.style(
+                f"Found {len(services)} service(s) from {search_in}:\n{services_str}",
+                fg="cyan",
+            )
+        )
+    click.echo(click.style("Done!", fg="green"))
+
+
+@cli.command()
+@click.argument("service")
+def create(service: str):
+    """Create service(s).
+
+    Args:
+        service (str): Name or name pattern of service(s) to create.
+    """
+    start_service(service)
     click.echo(click.style("Done!", fg="green"))
 
 
 @cli.command()
 @click.argument("service")
 def start(service: str):
     """Start service(s).
@@ -284,24 +291,25 @@
     remove_service(service)
     click.echo(click.style("Done!", fg="green"))
 
 
 @cli.command
 @click.argument("service", required=False)
 def show(service: str):
+    """Show services file contents."""
     files = defaultdict(list)
     for f in systemd_dir.glob(f"{_SYSTEMD_FILE_PREFIX}*.service"):
         files[f.stem].append(f)
     for f in systemd_dir.glob(f"{_SYSTEMD_FILE_PREFIX}*.timer"):
         files[f.stem].append(f)
     if service:
         files = {k: v for k, v in files.items() if service in k}
     services = []
     for srvs in files.values():
-        services.append('\n'.join([s.read_text() for s in srvs]))
+        services.append("\n".join([s.read_text() for s in srvs]))
     services = "\n\n".join(services)
     click.echo(click.style(services, fg="cyan"))
 
 
 def table_column_colors():
     colors_gen = cycle(["orange3", "green", "cyan", "magenta", "dodger_blue1", "red"])
```

## taskflows/service/__init__.py

```diff
@@ -4,23 +4,33 @@
     CPUs,
     HardwareConstraint,
     IOPressure,
     Memory,
     MemoryPressure,
     SystemLoadConstraint,
 )
-from .docker import ContainerLimits, DockerContainer, DockerImage, Ulimit, Volume
+from .docker import (
+    ContainerLimits,
+    DockerContainer,
+    DockerImage,
+    DockerService,
+    DockerStartService,
+    DockerStopService,
+    Ulimit,
+    Volume,
+)
 from .schedule import Calendar, Periodic, Schedule
 from .service import (
-    systemd_dir,
     Service,
     disable_service,
     enable_service,
     get_service_files,
     get_timer_files,
     remove_service,
     restart_service,
     service_cmd,
     service_runs,
     start_service,
     stop_service,
+    systemd_dir,
+    systemd_manager,
 )
```

## taskflows/service/docker.py

```diff
@@ -1,20 +1,23 @@
 from dataclasses import asdict, dataclass
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Dict, List, Literal, Optional, Sequence, Union
 
+from dotenv import dotenv_values
+from taskflows.utils import logger
+from xxhash import xxh32
+
 import docker
 from docker.errors import ImageNotFound
 from docker.models.containers import Container
 from docker.models.images import Image
-from dotenv import dotenv_values
-from xxhash import xxh32
 
-from taskflows.utils import logger
+from .schedule import Schedule
+from .service import Service
 
 
 @lru_cache
 def get_docker_client(user_host: Optional[str] = None):
     base_url = f"ssh://{user_host}" if user_host else "unix:///var/run/docker.sock"
     return docker.DockerClient(base_url=base_url)
 
@@ -463,7 +466,104 @@
         """
         try:
             container = get_docker_client().containers.get(container_name)
         except docker.errors.NotFound:
             return
         container.remove(force=True)
         logger.info("Removed Docker container: %s", container_name)
+
+
+class DockerService:
+    """A service to start and stop a Docker container."""
+
+    def __init__(
+        self,
+        container: DockerContainer | str,
+        start_schedule: Union[Schedule, Sequence[Schedule]],
+        stop_schedule: Union[Schedule, Sequence[Schedule]],
+        start_kwargs: Optional[Dict[str, Any]] = None,
+        stop_kwargs: Optional[Dict[str, Any]] = None,
+    ):
+        start_kwargs = start_kwargs or {}
+        stop_kwargs = stop_kwargs or {}
+        self.start_service = DockerStartService(
+            container=container, schedule=start_schedule, **start_kwargs
+        )
+        self.stop_service = DockerStopService(
+            container=container, schedule=stop_schedule, **stop_kwargs
+        )
+
+    @property
+    def name(self) -> str:
+        return f"{self.start_service} + {self.stop_service}"
+
+    def create(self):
+        self.start_service.create()
+        self.stop_service.create()
+
+    def enable(self):
+        self.start_service.enable()
+        self.stop_service.enable()
+
+    def run(self):
+        self.start_service.run()
+        self.stop_service.run()
+
+    def stop(self):
+        self.start_service.stop()
+        self.stop_service.stop()
+
+    def restart(self):
+        self.start_service.restart()
+        self.stop_service.restart()
+
+    def disable(self):
+        self.start_service.disable()
+        self.stop_service.disable()
+
+    def remove(self):
+        self.start_service.remove()
+        self.stop_service.remove()
+
+    def __str__(self):
+        return f"DockerService({self.name})"
+
+    def __repr__(self):
+        return str(self)
+
+
+class DockerStartService(Service):
+    """A service to start a Docker container."""
+
+    def __init__(
+        self, container: DockerContainer | str, name: Optional[str] = None, **kwargs
+    ):
+        self.container = container
+        cname = container if isinstance(container, str) else container.name
+        if name is None:
+            name = f"{cname}-start"
+        super().__init__(
+            name=name,
+            command=f"docker start {cname}",
+            **kwargs,
+        )
+
+    def create(self):
+        if isinstance(self.container, DockerContainer):
+            if not self.container.name:
+                logger.info("Setting container name to service name: %s", self.name)
+                self.container.name = self.name
+            self.container.create()
+        super().create()
+
+
+class DockerStopService(Service):
+    """A service to start a Docker container."""
+
+    def __init__(
+        self, container: DockerContainer | str, name: Optional[str] = None, **kwargs
+    ):
+        self.container = container
+        cname = container if isinstance(container, str) else container.name
+        if name is None:
+            name = f"{cname}-stop"
+        super().__init__(name=name, command=f"docker stop {cname}", **kwargs)
```

## taskflows/service/service.py

```diff
@@ -1,42 +1,43 @@
 import re
 from collections import defaultdict
-from dataclasses import asdict
+from dataclasses import dataclass
 from datetime import datetime
 from fnmatch import fnmatch
 from pathlib import Path
 from subprocess import run
 from time import time
 from typing import Any, Dict, List, Literal, Optional, Sequence, Union
 
-import dbus
-from pydantic import BaseModel
-
 from taskflows.utils import _SYSTEMD_FILE_PREFIX, logger
 
 from .constraints import HardwareConstraint, SystemLoadConstraint
-from .docker import DockerContainer
 from .schedule import Schedule
 
-# bus = dbus.SystemBus()
-bus = dbus.SessionBus()
-systemd = bus.get_object("org.freedesktop.systemd1", "/org/freedesktop/systemd1")
-manager = dbus.Interface(systemd, "org.freedesktop.systemd1.Manager")
+
+def systemd_manager():
+    import dbus
+
+    bus = dbus.SessionBus()
+    systemd = bus.get_object("org.freedesktop.systemd1", "/org/freedesktop/systemd1")
+    return dbus.Interface(systemd, "org.freedesktop.systemd1.Manager")
 
 
 systemd_dir = Path.home().joinpath(".config", "systemd", "user")
 # systemd_dir = Path("/etc/systemd/system")
 
 ServiceNames = Optional[Union[str, Sequence[str]]]
 
 
-class Service(BaseModel):
+@dataclass
+class Service:
+    """A service to run a command on a specified schedule."""
+
     name: str
     command: str
-    container: Optional[DockerContainer] = None
     description: Optional[str] = None
     schedule: Optional[Union[Schedule, Sequence[Schedule]]] = None
     restart_policy: Optional[
         Literal[
             "always",
             "on-success",
             "on-failure",
@@ -92,29 +93,16 @@
     # Specifies a timeout (in seconds) that starts running when the queued job is actually started.
     # If limit is reached, the job will be cancelled, the unit however will not change state or even enter the "failed" mode.
     timeout: Optional[int] = None
     env_file: Optional[str] = None
     env: Optional[Dict[str, str]] = None
     working_directory: Optional[Union[str, Path]] = None
 
-    class Config:
-        arbitrary_types_allowed = True
-
     def create(self):
         logger.info("Creating service %s", self.name)
-        if self.container:
-            if not self.container.name:
-                logger.info("Setting container name to service name: %s", self.name)
-                self.container.name = self.name
-            else:
-                logger.warning(
-                    "Container name is already set. Will not change: %s",
-                    self.container.name,
-                )
-            self.container.create()
         self._write_timer_unit()
         self._write_service_unit()
         self.enable()
 
     def enable(self):
         enable_service(self.name)
 
@@ -129,23 +117,14 @@
 
     def disable(self):
         disable_service(self.name)
 
     def remove(self):
         remove_service(self.name)
 
-    def as_dict(self) -> Dict[str, Any]:
-        data = self.model_dump()
-        if self.schedule:
-            data["schedule"] = asdict(self.schedule)
-        data = {k: v for k, v in data.items() if v is not None}
-        if "working_directory" in data:
-            data["working_directory"] = str(data["working_directory"])
-        return data
-
     def _join_values(self, values: Any):
         if isinstance(values, str):
             return values
         elif isinstance(values, (list, tuple)):
             return " ".join(values)
         raise ValueError(f"Unexpected type for values: {type(values)}")
 
@@ -248,117 +227,130 @@
         )
         if file.exists():
             logger.warning("Replacing existing unit: %s", file)
         else:
             logger.info("Creating new unit: %s", file)
         file.write_text(content)
 
+    def __repr__(self):
+        return str(self)
+
+    def __str__(self):
+        meta = {
+            "name": self.name,
+            "command": self.command,
+        }
+        if self.description:
+            meta["description"] = self.description
+        if self.schedule:
+            meta["schedule"] = self.schedule
+        meta = ", ".join(f"{k}={v}" for k, v in meta.items())
+        return f"{self.__class__.__name__}({meta})"
+
 
 def enable_service(service: str):
     """Enable currently disabled service(s).
 
     Args:
         service (str): Name or name pattern of service(s) to restart.
     """
     for sf in get_service_files(service):
         logger.info("Enabling service: %s", sf)
-        manager.EnableUnitFiles([str(sf)], True, True)
+        systemd_manager().EnableUnitFiles([str(sf)], True, True)
         # user_systemctl("enable", "--now", f"{_SYSTEMD_FILE_PREFIX}{sf}.timer")
 
 
 def is_service_enabled(service):
     """
     is_service_enabled method will check if service is already enabled that is passed in this method.
     It raise exception if there is error.
     Return value, True if service is already enabled otherwise False.
 
     :param str service: name of the service
     """
     try:
-        return manager.GetUnitFileState(service) == "enabled"
+        return systemd_manager().GetUnitFileState(service) == "enabled"
     except:
         return False
 
 
 def start_service(service: str):
     """
     start method will start service that is passed in this method.
     If service is already started then it will ignore it.
     It raise exception if there is error
 
     :param str service: name of the service
     """
     for sf in get_service_files(service):
-        logger.info("Running service: %s", sf)
+        logger.info("Running service: %s", sf.name)
         # service_cmd(sf, "start")
-        manager.StartUnit(sf.name, "replace")
+        systemd_manager().StartUnit(sf.name, "replace")
 
 
 def restart_service(service: str):
     """Restart running service(s).
 
     Args:
         service (str): Name or name pattern of service(s) to restart.
     """
     for sf in get_service_files(service):
         logger.info("Restarting service: %s", sf)
         # service_cmd(sf, "restart")
-        manager.RestartUnit(sf.name, "replace")
+        systemd_manager().RestartUnit(sf.name, "replace")
 
 
 def stop_service(service: str):
     """Stop running service(s).
 
     Args:
         service (str): Name or name pattern of service(s) to stop.
     """
     for sf in get_service_files(service):
         logger.info("Stopping service: %s", sf)
         # service_cmd(sf, "stop")
         # TODO a way to not use sigkill?
-        manager.StopUnit(sf.name, "replace")
+        systemd_manager().StopUnit(sf.name, "replace")
 
 
 def disable_service(service: str):
     """Disable service(s).
 
     Args:
         service (str): Name or name pattern of service(s) to disable.
     """
     for sf in get_service_files(service):
         # user_systemctl(
         #    "disable", "--now", f"{_SYSTEMD_FILE_PREFIX}{sf}.timer"
         # )
         logger.info("Stopped and disabled service: %s", sf)
         # file = systemd_dir / f"{_SYSTEMD_FILE_PREFIX}{sf}.timer"
-        manager.DisableUnitFiles([sf.name], False)
+        systemd_manager().DisableUnitFiles([sf.name], False)
     # remove any failed status caused by stopping service.
     # user_systemctl("reset-failed")
-    manager.Reload()
+    systemd_manager().Reload()
 
 
 def remove_service(service: str):
     """Remove service(s).
 
     Args:
         service (str): Name or name pattern of service(s) to remove.
     """
-    for sf in get_service_files(service):
-        logger.info("Removing service %s", sf)
-        disable_service(sf)
-        files = list(systemd_dir.glob(f"{_SYSTEMD_FILE_PREFIX}{sf}.*"))
-        srvs = {f.stem for f in files}
-        for srv in srvs:
-            logger.info("Cleaning cache and runtime directories: %s.", srv)
-            # TODO python-dbus
-            user_systemctl("clean", srv)
+    disable_service(service)
+    for srv_file in get_service_files(service):
+        logger.info("Cleaning cache and runtime directories: %s.", srv_file)
+        # TODO python-dbus
+        user_systemctl("clean", srv_file.stem)
         # remove files.
-        for file in files:
-            logger.info("Deleting %s", file)
-            file.unlink()
+        logger.info("Deleting %s", srv_file)
+        srv_file.unlink()
+    for timer_file in get_timer_files(service):
+        logger.info("Deleting %s", timer_file)
+        timer_file.unlink()
 
 
 def service_runs(match: Optional[str] = None) -> Dict[str, Dict[str, str]]:
     """Map service name to current schedule status."""
     srv_runs = defaultdict(dict)
     # get task status.
     for info in parse_systemctl_tables(["systemctl", "--user", "list-timers"]):
@@ -398,15 +390,15 @@
     """Get names of all services."""
     return get_systemd_files("timer", match)
 
 
 def get_systemd_files(
     file_type: Literal["timer", "service"], match: Optional[str] = None
 ) -> List[Path]:
-    if match:
+    if match is not None:
         if not match.startswith(_SYSTEMD_FILE_PREFIX):
             match = f"{_SYSTEMD_FILE_PREFIX}{match}"
         if not match.endswith(file_type):
             match = f"{match}*.{file_type}"
         files = list(systemd_dir.glob(match))
     else:
         files = list(systemd_dir.glob(f"{_SYSTEMD_FILE_PREFIX}*.{file_type}"))
@@ -440,15 +432,15 @@
     """
     is_service_active method will check if service is running or not.
     It raise exception if there is service is not loaded
     Return value, True if service is running otherwise False.
     :param str service: name of the service
     """
     try:
-        manager.GetUnit(service)
+        systemd_manager().GetUnit(service)
         return True
     except:
         return False
 
 
 def user_systemctl(*args):
     """Run a systemd command as current user."""
```

## Comparing `taskflows-0.4.4.dist-info/METADATA` & `taskflows-0.5.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskflows
-Version: 0.4.4
+Version: 0.5.0
 Summary: Python task management, scheduling, alerts.
 Author-email: Dan Kelleher <kelleherjdan@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

## Comparing `taskflows-0.4.4.dist-info/RECORD` & `taskflows-0.5.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 taskflows/__init__.py,sha256=oW-FCpGdoTfDXFNZ7hlNV2lzLUzQoKSPTP2TfvDIPPk,87
-taskflows/admin.py,sha256=dXtzOrR4zFdFdpjHlZS3Gb8_HWS_Lo2CxAIKIZn38vU,10229
+taskflows/admin.py,sha256=muL5Dvh0r23UNK1afGOL2rUiyyGuHEvwAOaKIDMJGdI,10107
 taskflows/db.py,sha256=aOoWhuy1__7YobfP0bB1x-sTFEjoSM06Kdw1m6--GWc,3444
 taskflows/tasks.py,sha256=aXQxLu6_JItg5iqQpZDDYLaJKIvbI5B17_rLWQGWJFk,8937
 taskflows/utils.py,sha256=TahZKvotnW_us79SXYkjrjXoa464MwHFe6uo5SR0XuI,564
-taskflows/service/__init__.py,sha256=Epl-nKhfYN7Qn69PBBH8mvxXgYVJBywvIAcIFUK8Su8,587
+taskflows/service/__init__.py,sha256=r4gR-aa3fQf8p5_OBWh0VLqVFBi4UtZA51CZ26iXqA4,699
 taskflows/service/commands.py,sha256=t_ITtM5l5_Dtpx70p6uKBaWGixGkNZCYm13zXBlQkQw,1286
 taskflows/service/constraints.py,sha256=2N5eSAJjUg2twxmVjs3GWaqmppc-DW0dZ5MlMRqcmNw,1586
-taskflows/service/docker.py,sha256=w2VFWPCcAd5hLqkOamfdJuPagT_qeB4tBqVoFnGw5Rc,18204
+taskflows/service/docker.py,sha256=dSHitWrl-Vm4QtXqK_9JzgBU0vcCOkHynIFCNBNukZk,21124
 taskflows/service/schedule.py,sha256=84B5phVhjSoj-UTtmqHmVwKTHYVjjfuryYW3p4yuJco,2234
-taskflows/service/service.py,sha256=_tKef13I2Ge3qPF3WgJprVFAaxDxnPciCC6fMPuo2iY,18155
-taskflows-0.4.4.dist-info/METADATA,sha256=wH6QlfidgfcQ-2XEz2aYyGGMSKCUX48TTdeiB0C9xO0,4293
-taskflows-0.4.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-taskflows-0.4.4.dist-info/entry_points.txt,sha256=84ElXyA0XQ3cRfNIL-woPCmCkGk9-OV4YarSW0i-88Y,111
-taskflows-0.4.4.dist-info/top_level.txt,sha256=CipuamG5azL_xisU7bxm8aEd18vy0JSHVWx4WzswtqQ,10
-taskflows-0.4.4.dist-info/RECORD,,
+taskflows/service/service.py,sha256=2G_7U_bBGZoSvIJboruFgA_Me3tViyONnHpA_SOPw5c,17746
+taskflows-0.5.0.dist-info/METADATA,sha256=Q3BsWm1VAcd3CbqpQKVarVeVvWeSdKKrRilkIIwyfrU,4293
+taskflows-0.5.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+taskflows-0.5.0.dist-info/entry_points.txt,sha256=84ElXyA0XQ3cRfNIL-woPCmCkGk9-OV4YarSW0i-88Y,111
+taskflows-0.5.0.dist-info/top_level.txt,sha256=CipuamG5azL_xisU7bxm8aEd18vy0JSHVWx4WzswtqQ,10
+taskflows-0.5.0.dist-info/RECORD,,
```


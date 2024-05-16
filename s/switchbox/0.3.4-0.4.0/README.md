# Comparing `tmp/switchbox-0.3.4.tar.gz` & `tmp/switchbox-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "switchbox-0.3.4.tar", max compression
+gzip compressed data, was "switchbox-0.4.0.tar", max compression
```

## Comparing `switchbox-0.3.4.tar` & `switchbox-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1669 2022-09-02 11:21:11.225583 switchbox-0.3.4/README.md
--rw-r--r--   0        0        0     1141 2022-09-16 10:36:58.102088 switchbox-0.3.4/pyproject.toml
--rw-r--r--   0        0        0        0 2022-08-24 16:31:20.143789 switchbox-0.3.4/switchbox/__init__.py
--rw-r--r--   0        0        0       74 2022-09-14 10:25:32.920147 switchbox-0.3.4/switchbox/__main__.py
--rw-r--r--   0        0        0     8569 2022-09-16 10:36:58.270085 switchbox-0.3.4/switchbox/app.py
--rw-r--r--   0        0        0     5008 2022-09-16 10:37:26.257607 switchbox-0.3.4/switchbox/cli.py
--rw-r--r--   0        0        0        0 2022-08-29 19:12:46.740750 switchbox-0.3.4/switchbox/ext/__init__.py
--rw-r--r--   0        0        0     2858 2022-09-14 13:42:12.253283 switchbox-0.3.4/switchbox/ext/git.py
--rw-r--r--   0        0        0     8914 2022-09-16 10:28:33.802749 switchbox-0.3.4/switchbox/repo.py
--rw-r--r--   0        0        0        0 2022-08-25 14:28:07.113260 switchbox-0.3.4/switchbox/tests/__init__.py
--rw-r--r--   0        0        0      328 2022-08-29 19:12:46.740750 switchbox-0.3.4/switchbox/tests/test_repo.py
--rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 switchbox-0.3.4/setup.py
--rw-r--r--   0        0        0     2738 1970-01-01 00:00:00.000000 switchbox-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1754 2024-04-12 13:55:10.287122 switchbox-0.4.0/README.md
+-rw-r--r--   0        0        0     1157 2024-04-12 13:55:10.289122 switchbox-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-12 13:55:10.289122 switchbox-0.4.0/switchbox/__init__.py
+-rw-r--r--   0        0        0       74 2024-04-12 13:55:10.289122 switchbox-0.4.0/switchbox/__main__.py
+-rw-r--r--   0        0        0     8568 2024-04-12 13:55:10.289122 switchbox-0.4.0/switchbox/app.py
+-rw-r--r--   0        0        0     5009 2024-04-12 13:55:10.289122 switchbox-0.4.0/switchbox/cli.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:55:10.289122 switchbox-0.4.0/switchbox/ext/__init__.py
+-rw-r--r--   0        0        0     3068 2024-04-12 13:55:10.289122 switchbox-0.4.0/switchbox/ext/git.py
+-rw-r--r--   0        0        0     9331 2024-04-12 13:55:10.289122 switchbox-0.4.0/switchbox/repo.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:55:10.289122 switchbox-0.4.0/switchbox/tests/__init__.py
+-rw-r--r--   0        0        0      328 2024-04-12 13:55:10.289122 switchbox-0.4.0/switchbox/tests/test_repo.py
+-rw-r--r--   0        0        0     2925 1970-01-01 00:00:00.000000 switchbox-0.4.0/PKG-INFO
```

### Comparing `switchbox-0.3.4/README.md` & `switchbox-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 switchbox
 =========
 
 A collection of small tools for git workflows.
 
+![A screenshot displaying the output of 'switchbox finish'.](./docs/screenshot.png)
+
 Installation
 ------------
 
 Clone the repository and install the package with `pip`.
 
 ```zsh
 pip install --user .
```

### Comparing `switchbox-0.3.4/pyproject.toml` & `switchbox-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "switchbox"
-version = "0.3.4"
+version = "0.4.0"
 readme = "README.md"
 description = "Tools for working with Git repositories."
 homepage = "https://pypi.org/project/switchbox/"
 repository = "https://github.com/borntyping/switchbox"
 authors = ["Sam Clements <sam@borntyping.co.uk>"]
 license = "MPL-2.0"
 packages = [
@@ -28,14 +28,15 @@
 PyGithub = "^1.55"
 GitPython = "^3.1.27"
 
 [tool.poetry.dev-dependencies]
 black = "^22.6.0"
 mypy = "^0.971"
 pytest = "^7.1.2"
+pipx = "^1.1.0"
 
 [tool.poetry.scripts]
 git-switchbox = "switchbox.cli:main"
 switchbox = "switchbox.cli:main"
 
 [tool.mypy]
 files = [
```

### Comparing `switchbox-0.3.4/switchbox/app.py` & `switchbox-0.4.0/switchbox/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,32 +118,34 @@
         with output.status("Updating all remotes..."):
             self.repo.update_remotes()
         output.done("Updated all remotes.")
 
     def update_default_branch(self) -> None:
         output = Output(**self.context)
 
-        if self.repo.active_branch == self.repo.default_branch:
-            raise click.ClickException(f"Already on branch {self.repo.default_branch}")
-
         with output.status(
             "Updating branch {default_branch} "
-            "to match {default_branch}/{default_remote}."
+            "to match {default_remote}/{default_branch}."
         ):
             self.repo.update_branch_from_remote(
                 remote=self.repo.default_remote,
                 branch=self.repo.default_branch,
             )
         output.done(
             "Updated branch {default_branch} "
             "to match {default_branch}/{default_remote}."
         )
 
     def switch_default_branch(self) -> None:
         output = Output(**self.context)
+
+        if self.repo.active_branch == self.repo.default_branch:
+            output.done("Already on the {default_branch} branch.")
+            return
+
         with output.status("Switching to the {default_branch} branch..."):
             self.repo.switch(self.repo.default_branch)
         output.done("Switched to the {default_branch} branch.")
 
     def remove_merged_branches(self, dry_run: bool = True) -> None:
         self._remove_branches(
             merged="[green]merged[/]",
@@ -209,19 +211,19 @@
             "Found and removed {one} {branch} "
             "that {was} {merged} into {target}: {items}."
         )
 
     def rebase_active_branch(self) -> typing.Tuple[str, str]:
         """Rebase the active branch on top of the remote default branch."""
         output = Output(**self.context)
-        with output.status("Rebasing onto {default_branch}/{default_remote}..."):
+        with output.status("Rebasing onto {default_remote}/{default_branch}..."):
             before = self.repo.active_branch_ref()
             self.repo.rebase(upstream=self.repo.remote_default_branch)
             after = self.repo.active_branch_ref()
-        output.done("Rebased {active_branch} onto {default_branch}/{default_remote}.")
+        output.done("Rebased {active_branch} onto {default_remote}/{default_branch}.")
         return before, after
 
     def rebase_and_push_active_branch(self):
         before, after = self.rebase_active_branch()
         output = Output(**self.context)
         with output.status(
             "Force pushing from {default_branch} "
```

### Comparing `switchbox-0.3.4/switchbox/cli.py` & `switchbox-0.4.0/switchbox/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
 
 @main.command()
 @remote_update_option
 @click.option(
     "--push/--no-push",
     "push",
-    default=True,
+    default=False,
     is_flag=True,
     help="Run 'git push --force-with-lease' after rebasing.",
 )
 @click.pass_obj
 def rebase(app: Application, update_remotes: bool, push: bool) -> None:
     """
     Rebase the active branch, and force push it to the remote branch.
```

### Comparing `switchbox-0.3.4/switchbox/ext/git.py` & `switchbox-0.4.0/switchbox/ext/git.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,179 +1,192 @@
 00000000: 696d 706f 7274 206c 6f67 6769 6e67 0a69  import logging.i
 00000010: 6d70 6f72 7420 7479 7069 6e67 0a0a 696d  mport typing..im
 00000020: 706f 7274 2067 6974 0a0a 6c6f 6767 6572  port git..logger
 00000030: 203d 206c 6f67 6769 6e67 2e67 6574 4c6f   = logging.getLo
 00000040: 6767 6572 285f 5f6e 616d 655f 5f29 0a0a  gger(__name__)..
-00000050: 0a64 6566 2066 696e 645f 6d65 7267 655f  .def find_merge_
-00000060: 6261 7365 280a 2020 2020 7265 706f 3a20  base(.    repo: 
-00000070: 6769 742e 5265 706f 2c0a 2020 2020 613a  git.Repo,.    a:
-00000080: 2067 6974 2e72 6566 732e 4865 6164 2c0a   git.refs.Head,.
-00000090: 2020 2020 623a 2067 6974 2e72 6566 732e      b: git.refs.
-000000a0: 4865 6164 2c0a 2920 2d3e 2067 6974 2e6f  Head,.) -> git.o
-000000b0: 626a 6563 7473 2e63 6f6d 6d69 742e 436f  bjects.commit.Co
-000000c0: 6d6d 6974 3a0a 2020 2020 6d65 7267 655f  mmit:.    merge_
-000000d0: 6261 7365 7320 3d20 7265 706f 2e6d 6572  bases = repo.mer
-000000e0: 6765 5f62 6173 6528 612c 2062 290a 0a20  ge_base(a, b).. 
-000000f0: 2020 2069 6620 6c65 6e28 6d65 7267 655f     if len(merge_
-00000100: 6261 7365 7329 203d 3d20 303a 0a20 2020  bases) == 0:.   
-00000110: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
-00000120: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
-00000130: 2020 224e 6f20 6d65 7267 6520 6261 7365    "No merge base
-00000140: 2066 6f75 6e64 2066 6f72 2025 2861 292e   found for %(a).
-00000150: 3773 2061 6e64 2025 2862 292e 3773 2220  7s and %(b).7s" 
-00000160: 2520 7b22 6122 3a20 612c 2022 6222 3a20  % {"a": a, "b": 
-00000170: 627d 0a20 2020 2020 2020 2029 0a0a 2020  b}.        )..  
-00000180: 2020 6966 206c 656e 286d 6572 6765 5f62    if len(merge_b
-00000190: 6173 6573 2920 3e3d 2032 3a0a 2020 2020  ases) >= 2:.    
-000001a0: 2020 2020 7261 6973 6520 4578 6365 7074      raise Except
-000001b0: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
-000001c0: 2022 4d75 6c74 6970 6c65 206d 6572 6765   "Multiple merge
-000001d0: 2062 6173 6573 2066 6f75 6e64 2066 6f72   bases found for
-000001e0: 2025 2861 292e 3773 2061 6e64 2025 2862   %(a).7s and %(b
-000001f0: 292e 3773 2220 2520 7b22 6122 3a20 612c  ).7s" % {"a": a,
-00000200: 2022 6222 3a20 627d 0a20 2020 2020 2020   "b": b}.       
-00000210: 2029 0a0a 2020 2020 6d65 7267 655f 6261   )..    merge_ba
-00000220: 7365 203d 206d 6572 6765 5f62 6173 6573  se = merge_bases
-00000230: 5b30 5d0a 0a20 2020 2069 6620 6e6f 7420  [0]..    if not 
-00000240: 6973 696e 7374 616e 6365 286d 6572 6765  isinstance(merge
-00000250: 5f62 6173 652c 2067 6974 2e6f 626a 6563  _base, git.objec
-00000260: 7473 2e63 6f6d 6d69 742e 436f 6d6d 6974  ts.commit.Commit
-00000270: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
-00000280: 2045 7863 6570 7469 6f6e 2866 2255 6e6b   Exception(f"Unk
-00000290: 6e6f 776e 206d 6572 6765 2062 6173 6520  nown merge base 
-000002a0: 7479 7065 3a20 7b6d 6572 6765 5f62 6173  type: {merge_bas
-000002b0: 6521 727d 2229 0a0a 2020 2020 7265 7475  e!r}")..    retu
-000002c0: 726e 206d 6572 6765 5f62 6173 650a 0a0a  rn merge_base...
-000002d0: 6465 6620 636f 6e74 6169 6e73 5f65 7175  def contains_equ
-000002e0: 6976 616c 656e 7428 0a20 2020 2072 6570  ivalent(.    rep
-000002f0: 6f3a 2067 6974 2e52 6570 6f2c 0a20 2020  o: git.Repo,.   
-00000300: 2075 7073 7472 6561 6d3a 2067 6974 2e72   upstream: git.r
-00000310: 6566 732e 4865 6164 2c0a 2020 2020 6865  efs.Head,.    he
-00000320: 6164 3a20 6769 742e 7265 6673 2e48 6561  ad: git.refs.Hea
-00000330: 642c 0a29 202d 3e20 626f 6f6c 3a0a 2020  d,.) -> bool:.  
-00000340: 2020 2222 220a 2020 2020 5265 7475 726e    """.    Return
-00000350: 2054 7275 6520 6966 2061 6c6c 2063 6f6d   True if all com
-00000360: 6d69 7473 2069 6e20 3c68 6561 643e 2068  mits in <head> h
-00000370: 6176 6520 616e 2065 7175 6976 616c 656e  ave an equivalen
-00000380: 7420 696e 203c 7570 7374 7265 616d 3e2e  t in <upstream>.
-00000390: 0a20 2020 2068 7474 7073 3a2f 2f67 6974  .    https://git
-000003a0: 2d73 636d 2e63 6f6d 2f64 6f63 732f 6769  -scm.com/docs/gi
-000003b0: 742d 6368 6572 7279 0a20 2020 2022 2222  t-cherry.    """
-000003c0: 0a20 2020 206c 6f67 6765 722e 696e 666f  .    logger.info
-000003d0: 280a 2020 2020 2020 2020 2243 6865 636b  (.        "Check
-000003e0: 696e 6720 6966 2027 2528 7570 7374 7265  ing if '%(upstre
-000003f0: 616d 2973 2720 636f 6e74 6169 6e73 2061  am)s' contains a
-00000400: 6c6c 2063 6f6d 6d69 7473 2066 726f 6d20  ll commits from 
-00000410: 2725 2868 6561 6429 7327 222c 0a20 2020  '%(head)s'",.   
-00000420: 2020 2020 207b 2275 7073 7472 6561 6d22       {"upstream"
-00000430: 3a20 7570 7374 7265 616d 2c20 2268 6561  : upstream, "hea
-00000440: 6422 3a20 6865 6164 7d2c 0a20 2020 2029  d": head},.    )
-00000450: 0a20 2020 2073 7464 6f75 7420 3d20 7265  .    stdout = re
-00000460: 706f 2e67 6974 2e63 6865 7272 7928 7570  po.git.cherry(up
-00000470: 7374 7265 616d 2c20 6865 6164 290a 2020  stream, head).  
-00000480: 2020 7265 7475 726e 2061 6c6c 286c 696e    return all(lin
-00000490: 655b 305d 203d 3d20 222d 2220 666f 7220  e[0] == "-" for 
-000004a0: 6c69 6e65 2069 6e20 7374 646f 7574 2e73  line in stdout.s
-000004b0: 706c 6974 6c69 6e65 7328 2929 0a0a 0a64  plitlines())...d
-000004c0: 6566 2063 6f6d 6d69 7473 280a 2020 2020  ef commits(.    
-000004d0: 7265 706f 3a20 6769 742e 5265 706f 2c0a  repo: git.Repo,.
-000004e0: 2020 2020 7231 3a20 6769 742e 6f62 6a65      r1: git.obje
-000004f0: 6374 732e 436f 6d6d 6974 207c 2067 6974  cts.Commit | git
-00000500: 2e72 6566 732e 4865 6164 2c0a 2020 2020  .refs.Head,.    
-00000510: 7232 3a20 6769 742e 6f62 6a65 6374 732e  r2: git.objects.
-00000520: 436f 6d6d 6974 207c 2067 6974 2e72 6566  Commit | git.ref
-00000530: 732e 4865 6164 2c0a 2920 2d3e 206c 6973  s.Head,.) -> lis
-00000540: 745b 6769 742e 6f62 6a65 6374 732e 436f  t[git.objects.Co
-00000550: 6d6d 6974 5d3a 0a20 2020 2072 6574 7572  mmit]:.    retur
-00000560: 6e20 6c69 7374 2872 6570 6f2e 6974 6572  n list(repo.iter
-00000570: 5f63 6f6d 6d69 7473 2866 227b 7231 7d2e  _commits(f"{r1}.
-00000580: 2e7b 7232 7d22 2929 0a0a 0a64 6566 2063  .{r2}"))...def c
-00000590: 6f6e 7461 696e 735f 7371 7561 7368 5f63  ontains_squash_c
-000005a0: 6f6d 6d69 7428 0a20 2020 2072 6570 6f3a  ommit(.    repo:
-000005b0: 2067 6974 2e52 6570 6f2c 0a20 2020 2061   git.Repo,.    a
-000005c0: 3a20 6769 742e 7265 6673 2e48 6561 642c  : git.refs.Head,
-000005d0: 0a20 2020 2062 3a20 6769 742e 7265 6673  .    b: git.refs
-000005e0: 2e48 6561 642c 0a29 202d 3e20 626f 6f6c  .Head,.) -> bool
-000005f0: 207c 204e 6f6e 653a 0a20 2020 2022 2222   | None:.    """
-00000600: 0a20 2020 2043 6865 636b 7320 6966 2042  .    Checks if B
-00000610: 2068 6173 2062 6565 6e20 6d65 7267 6564   has been merged
-00000620: 2069 6e74 6f20 4120 7769 7468 2061 2073   into A with a s
-00000630: 7175 6173 6820 636f 6d6d 6974 2e0a 0a20  quash commit... 
-00000640: 2020 2054 6869 7320 776f 726b 7320 6279     This works by
-00000650: 2066 696e 6469 6e67 2074 6865 2063 6f6d   finding the com
-00000660: 6d6f 6e20 616e 6365 7374 6f72 202f 206d  mon ancestor / m
-00000670: 6572 6765 2062 6173 6520 4d2c 2061 6e64  erge base M, and
-00000680: 2063 6865 636b 696e 6720 6966 0a20 2020   checking if.   
-00000690: 2022 2222 0a20 2020 2069 6620 6120 3d3d   """.    if a ==
-000006a0: 2062 3a0a 2020 2020 2020 2020 6c6f 6767   b:.        logg
-000006b0: 6572 2e64 6562 7567 2822 4e6f 7420 6368  er.debug("Not ch
-000006c0: 6563 6b69 6e67 2066 6f72 2073 7175 6173  ecking for squas
-000006d0: 6820 636f 6d6d 6974 732c 2062 7261 6e63  h commits, branc
-000006e0: 6865 7320 6172 6520 6964 656e 7469 6361  hes are identica
-000006f0: 6c22 290a 2020 2020 2020 2020 7265 7475  l").        retu
-00000700: 726e 204e 6f6e 650a 0a20 2020 206c 6f67  rn None..    log
-00000710: 6765 722e 696e 666f 2822 4368 6563 6b69  ger.info("Checki
-00000720: 6e67 2069 6620 2725 2862 2973 2720 7761  ng if '%(b)s' wa
-00000730: 7320 7371 7561 7368 6564 2069 6e74 6f20  s squashed into 
-00000740: 2725 2861 2973 2722 2c20 7b22 6122 3a20  '%(a)s'", {"a": 
-00000750: 612c 2022 6222 3a20 627d 290a 0a20 2020  a, "b": b})..   
-00000760: 206d 6572 6765 5f62 6173 6520 3d20 6669   merge_base = fi
-00000770: 6e64 5f6d 6572 6765 5f62 6173 6528 7265  nd_merge_base(re
-00000780: 706f 2c20 612c 2062 290a 2020 2020 6272  po, a, b).    br
-00000790: 616e 6368 5f64 6966 6620 3d20 622e 636f  anch_diff = b.co
-000007a0: 6d6d 6974 2e64 6966 6628 6d65 7267 655f  mmit.diff(merge_
-000007b0: 6261 7365 290a 0a20 2020 2069 6620 6c65  base)..    if le
-000007c0: 6e28 636f 6d6d 6974 7328 7265 706f 2c20  n(commits(repo, 
-000007d0: 7231 3d6d 6572 6765 5f62 6173 652c 2072  r1=merge_base, r
-000007e0: 323d 6229 2920 3d3d 2031 3a0a 2020 2020  2=b)) == 1:.    
-000007f0: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-00000800: 0a20 2020 2020 2020 2020 2020 2022 536b  .            "Sk
-00000810: 6970 7069 6e67 2062 7261 6e63 6820 7769  ipping branch wi
-00000820: 7468 206f 6e65 2063 6f6d 6d69 742c 2022  th one commit, "
-00000830: 0a20 2020 2020 2020 2020 2020 2022 7371  .            "sq
-00000840: 7561 7368 696e 6720 616e 6420 7265 6261  uashing and reba
-00000850: 7369 6e67 2061 7265 2065 7175 6976 616c  sing are equival
-00000860: 656e 7420 696e 2074 6869 7320 6361 7365  ent in this case
-00000870: 220a 2020 2020 2020 2020 290a 2020 2020  ".        ).    
-00000880: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-00000890: 0a20 2020 2066 6f72 2063 6f6d 6d69 7420  .    for commit 
-000008a0: 696e 2063 6f6d 6d69 7473 2872 6570 6f2c  in commits(repo,
-000008b0: 2072 313d 6d65 7267 655f 6261 7365 2c20   r1=merge_base, 
-000008c0: 7232 3d61 293a 0a20 2020 2020 2020 2069  r2=a):.        i
-000008d0: 6620 6c65 6e28 636f 6d6d 6974 2e70 6172  f len(commit.par
-000008e0: 656e 7473 2920 3d3d 2030 3a0a 2020 2020  ents) == 0:.    
-000008f0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-00000900: 6562 7567 2822 536b 6970 7069 6e67 2063  ebug("Skipping c
-00000910: 6f6d 6d69 7420 7769 7468 206e 6f20 7061  ommit with no pa
-00000920: 7265 6e74 7320 2528 6329 7322 2c20 7b22  rents %(c)s", {"
-00000930: 6322 3a20 636f 6d6d 6974 7d29 0a20 2020  c": commit}).   
-00000940: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00000950: 650a 2020 2020 2020 2020 656c 6966 206c  e.        elif l
-00000960: 656e 2863 6f6d 6d69 742e 7061 7265 6e74  en(commit.parent
-00000970: 7329 203e 3d20 323a 0a20 2020 2020 2020  s) >= 2:.       
-00000980: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00000990: 6728 2253 6b69 7070 696e 6720 6d65 7267  g("Skipping merg
-000009a0: 6520 636f 6d6d 6974 2025 2863 2973 222c  e commit %(c)s",
-000009b0: 207b 2263 223a 2063 6f6d 6d69 747d 290a   {"c": commit}).
-000009c0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-000009d0: 696e 7565 0a20 2020 2020 2020 2065 6c73  inue.        els
-000009e0: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
-000009f0: 6172 656e 7420 3d20 636f 6d6d 6974 2e70  arent = commit.p
-00000a00: 6172 656e 7473 5b30 5d0a 0a20 2020 2020  arents[0]..     
-00000a10: 2020 206c 6f67 6765 722e 696e 666f 280a     logger.info(.
-00000a20: 2020 2020 2020 2020 2020 2020 2243 6865              "Che
-00000a30: 636b 696e 6720 6966 2027 2528 6229 7327  cking if '%(b)s'
-00000a40: 2077 6173 2073 7175 6173 6865 6420 696e   was squashed in
-00000a50: 746f 2027 2528 6129 7327 2062 7920 2528  to '%(a)s' by %(
-00000a60: 6329 2e37 7322 2c0a 2020 2020 2020 2020  c).7s",.        
-00000a70: 2020 2020 7b22 6122 3a20 612c 2022 6222      {"a": a, "b"
-00000a80: 3a20 622c 2022 6322 3a20 636f 6d6d 6974  : b, "c": commit
-00000a90: 7d2c 0a20 2020 2020 2020 2029 0a0a 2020  },.        )..  
-00000aa0: 2020 2020 2020 6d61 7463 6865 735f 6272        matches_br
-00000ab0: 616e 6368 5f64 6966 6620 3d20 636f 6d6d  anch_diff = comm
-00000ac0: 6974 2e64 6966 6628 7061 7265 6e74 2920  it.diff(parent) 
-00000ad0: 3d3d 2062 7261 6e63 685f 6469 6666 0a0a  == branch_diff..
-00000ae0: 2020 2020 2020 2020 6966 206d 6174 6368          if match
-00000af0: 6573 5f62 7261 6e63 685f 6469 6666 3a0a  es_branch_diff:.
-00000b00: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00000b10: 726e 2054 7275 650a 0a20 2020 2072 6574  rn True..    ret
-00000b20: 7572 6e20 4661 6c73 650a                 urn False.
+00000050: 0a63 6c61 7373 2047 6974 4578 6365 7074  .class GitExcept
+00000060: 696f 6e28 4578 6365 7074 696f 6e29 3a0a  ion(Exception):.
+00000070: 2020 2020 7061 7373 0a0a 0a63 6c61 7373      pass...class
+00000080: 204e 6f4d 6572 6765 4261 7365 2847 6974   NoMergeBase(Git
+00000090: 4578 6365 7074 696f 6e29 3a0a 2020 2020  Exception):.    
+000000a0: 7061 7373 0a0a 0a63 6c61 7373 204d 756c  pass...class Mul
+000000b0: 7469 706c 654d 6572 6765 4261 7365 7328  tipleMergeBases(
+000000c0: 4769 7445 7863 6570 7469 6f6e 293a 0a20  GitException):. 
+000000d0: 2020 2070 6173 730a 0a0a 6465 6620 6669     pass...def fi
+000000e0: 6e64 5f6d 6572 6765 5f62 6173 6528 0a20  nd_merge_base(. 
+000000f0: 2020 2072 6570 6f3a 2067 6974 2e52 6570     repo: git.Rep
+00000100: 6f2c 0a20 2020 2061 3a20 6769 742e 7265  o,.    a: git.re
+00000110: 6673 2e48 6561 642c 0a20 2020 2062 3a20  fs.Head,.    b: 
+00000120: 6769 742e 7265 6673 2e48 6561 642c 0a29  git.refs.Head,.)
+00000130: 202d 3e20 6769 742e 6f62 6a65 6374 732e   -> git.objects.
+00000140: 636f 6d6d 6974 2e43 6f6d 6d69 743a 0a20  commit.Commit:. 
+00000150: 2020 206d 6572 6765 5f62 6173 6573 203d     merge_bases =
+00000160: 2072 6570 6f2e 6d65 7267 655f 6261 7365   repo.merge_base
+00000170: 2861 2c20 6229 0a0a 2020 2020 6966 206c  (a, b)..    if l
+00000180: 656e 286d 6572 6765 5f62 6173 6573 2920  en(merge_bases) 
+00000190: 3d3d 2030 3a0a 2020 2020 2020 2020 7261  == 0:.        ra
+000001a0: 6973 6520 4e6f 4d65 7267 6542 6173 6528  ise NoMergeBase(
+000001b0: 0a20 2020 2020 2020 2020 2020 2022 4e6f  .            "No
+000001c0: 206d 6572 6765 2062 6173 6520 666f 756e   merge base foun
+000001d0: 6420 666f 7220 2528 6129 2e37 7320 616e  d for %(a).7s an
+000001e0: 6420 2528 6229 2e37 7322 2025 207b 2261  d %(b).7s" % {"a
+000001f0: 223a 2061 2c20 2262 223a 2062 7d0a 2020  ": a, "b": b}.  
+00000200: 2020 2020 2020 290a 0a20 2020 2069 6620        )..    if 
+00000210: 6c65 6e28 6d65 7267 655f 6261 7365 7329  len(merge_bases)
+00000220: 203e 3d20 323a 0a20 2020 2020 2020 2072   >= 2:.        r
+00000230: 6169 7365 204d 756c 7469 706c 654d 6572  aise MultipleMer
+00000240: 6765 4261 7365 7328 0a20 2020 2020 2020  geBases(.       
+00000250: 2020 2020 2022 4d75 6c74 6970 6c65 206d       "Multiple m
+00000260: 6572 6765 2062 6173 6573 2066 6f75 6e64  erge bases found
+00000270: 2066 6f72 2025 2861 292e 3773 2061 6e64   for %(a).7s and
+00000280: 2025 2862 292e 3773 2220 2520 7b22 6122   %(b).7s" % {"a"
+00000290: 3a20 612c 2022 6222 3a20 627d 0a20 2020  : a, "b": b}.   
+000002a0: 2020 2020 2029 0a0a 2020 2020 6d65 7267       )..    merg
+000002b0: 655f 6261 7365 203d 206d 6572 6765 5f62  e_base = merge_b
+000002c0: 6173 6573 5b30 5d0a 0a20 2020 2069 6620  ases[0]..    if 
+000002d0: 6e6f 7420 6973 696e 7374 616e 6365 286d  not isinstance(m
+000002e0: 6572 6765 5f62 6173 652c 2067 6974 2e6f  erge_base, git.o
+000002f0: 626a 6563 7473 2e63 6f6d 6d69 742e 436f  bjects.commit.Co
+00000300: 6d6d 6974 293a 0a20 2020 2020 2020 2072  mmit):.        r
+00000310: 6169 7365 2047 6974 4578 6365 7074 696f  aise GitExceptio
+00000320: 6e28 6622 556e 6b6e 6f77 6e20 6d65 7267  n(f"Unknown merg
+00000330: 6520 6261 7365 2074 7970 653a 207b 6d65  e base type: {me
+00000340: 7267 655f 6261 7365 2172 7d22 290a 0a20  rge_base!r}").. 
+00000350: 2020 2072 6574 7572 6e20 6d65 7267 655f     return merge_
+00000360: 6261 7365 0a0a 0a64 6566 2063 6f6e 7461  base...def conta
+00000370: 696e 735f 6571 7569 7661 6c65 6e74 280a  ins_equivalent(.
+00000380: 2020 2020 7265 706f 3a20 6769 742e 5265      repo: git.Re
+00000390: 706f 2c0a 2020 2020 7570 7374 7265 616d  po,.    upstream
+000003a0: 3a20 6769 742e 7265 6673 2e48 6561 642c  : git.refs.Head,
+000003b0: 0a20 2020 2068 6561 643a 2067 6974 2e72  .    head: git.r
+000003c0: 6566 732e 4865 6164 2c0a 2920 2d3e 2062  efs.Head,.) -> b
+000003d0: 6f6f 6c3a 0a20 2020 2022 2222 0a20 2020  ool:.    """.   
+000003e0: 2052 6574 7572 6e20 5472 7565 2069 6620   Return True if 
+000003f0: 616c 6c20 636f 6d6d 6974 7320 696e 203c  all commits in <
+00000400: 6865 6164 3e20 6861 7665 2061 6e20 6571  head> have an eq
+00000410: 7569 7661 6c65 6e74 2069 6e20 3c75 7073  uivalent in <ups
+00000420: 7472 6561 6d3e 2e0a 2020 2020 6874 7470  tream>..    http
+00000430: 733a 2f2f 6769 742d 7363 6d2e 636f 6d2f  s://git-scm.com/
+00000440: 646f 6373 2f67 6974 2d63 6865 7272 790a  docs/git-cherry.
+00000450: 2020 2020 2222 220a 2020 2020 6c6f 6767      """.    logg
+00000460: 6572 2e69 6e66 6f28 0a20 2020 2020 2020  er.info(.       
+00000470: 2022 4368 6563 6b69 6e67 2069 6620 2725   "Checking if '%
+00000480: 2875 7073 7472 6561 6d29 7327 2063 6f6e  (upstream)s' con
+00000490: 7461 696e 7320 616c 6c20 636f 6d6d 6974  tains all commit
+000004a0: 7320 6672 6f6d 2027 2528 6865 6164 2973  s from '%(head)s
+000004b0: 2722 2c0a 2020 2020 2020 2020 7b22 7570  '",.        {"up
+000004c0: 7374 7265 616d 223a 2075 7073 7472 6561  stream": upstrea
+000004d0: 6d2c 2022 6865 6164 223a 2068 6561 647d  m, "head": head}
+000004e0: 2c0a 2020 2020 290a 2020 2020 7374 646f  ,.    ).    stdo
+000004f0: 7574 203d 2072 6570 6f2e 6769 742e 6368  ut = repo.git.ch
+00000500: 6572 7279 2875 7073 7472 6561 6d2c 2068  erry(upstream, h
+00000510: 6561 6429 0a20 2020 2072 6574 7572 6e20  ead).    return 
+00000520: 616c 6c28 6c69 6e65 5b30 5d20 3d3d 2022  all(line[0] == "
+00000530: 2d22 2066 6f72 206c 696e 6520 696e 2073  -" for line in s
+00000540: 7464 6f75 742e 7370 6c69 746c 696e 6573  tdout.splitlines
+00000550: 2829 290a 0a0a 6465 6620 636f 6d6d 6974  ())...def commit
+00000560: 7328 0a20 2020 2072 6570 6f3a 2067 6974  s(.    repo: git
+00000570: 2e52 6570 6f2c 0a20 2020 2072 313a 2067  .Repo,.    r1: g
+00000580: 6974 2e6f 626a 6563 7473 2e43 6f6d 6d69  it.objects.Commi
+00000590: 7420 7c20 6769 742e 7265 6673 2e48 6561  t | git.refs.Hea
+000005a0: 642c 0a20 2020 2072 323a 2067 6974 2e6f  d,.    r2: git.o
+000005b0: 626a 6563 7473 2e43 6f6d 6d69 7420 7c20  bjects.Commit | 
+000005c0: 6769 742e 7265 6673 2e48 6561 642c 0a29  git.refs.Head,.)
+000005d0: 202d 3e20 6c69 7374 5b67 6974 2e6f 626a   -> list[git.obj
+000005e0: 6563 7473 2e43 6f6d 6d69 745d 3a0a 2020  ects.Commit]:.  
+000005f0: 2020 7265 7475 726e 206c 6973 7428 7265    return list(re
+00000600: 706f 2e69 7465 725f 636f 6d6d 6974 7328  po.iter_commits(
+00000610: 6622 7b72 317d 2e2e 7b72 327d 2229 290a  f"{r1}..{r2}")).
+00000620: 0a0a 6465 6620 636f 6e74 6169 6e73 5f73  ..def contains_s
+00000630: 7175 6173 685f 636f 6d6d 6974 280a 2020  quash_commit(.  
+00000640: 2020 7265 706f 3a20 6769 742e 5265 706f    repo: git.Repo
+00000650: 2c0a 2020 2020 613a 2067 6974 2e72 6566  ,.    a: git.ref
+00000660: 732e 4865 6164 2c0a 2020 2020 623a 2067  s.Head,.    b: g
+00000670: 6974 2e72 6566 732e 4865 6164 2c0a 2920  it.refs.Head,.) 
+00000680: 2d3e 2062 6f6f 6c20 7c20 4e6f 6e65 3a0a  -> bool | None:.
+00000690: 2020 2020 2222 220a 2020 2020 4368 6563      """.    Chec
+000006a0: 6b73 2069 6620 4220 6861 7320 6265 656e  ks if B has been
+000006b0: 206d 6572 6765 6420 696e 746f 2041 2077   merged into A w
+000006c0: 6974 6820 6120 7371 7561 7368 2063 6f6d  ith a squash com
+000006d0: 6d69 742e 0a0a 2020 2020 5468 6973 2077  mit...    This w
+000006e0: 6f72 6b73 2062 7920 6669 6e64 696e 6720  orks by finding 
+000006f0: 7468 6520 636f 6d6d 6f6e 2061 6e63 6573  the common ances
+00000700: 746f 7220 2f20 6d65 7267 6520 6261 7365  tor / merge base
+00000710: 204d 2c20 616e 6420 6368 6563 6b69 6e67   M, and checking
+00000720: 2069 660a 2020 2020 2222 220a 2020 2020   if.    """.    
+00000730: 6966 2061 203d 3d20 623a 0a20 2020 2020  if a == b:.     
+00000740: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+00000750: 224e 6f74 2063 6865 636b 696e 6720 666f  "Not checking fo
+00000760: 7220 7371 7561 7368 2063 6f6d 6d69 7473  r squash commits
+00000770: 2c20 6272 616e 6368 6573 2061 7265 2069  , branches are i
+00000780: 6465 6e74 6963 616c 2229 0a20 2020 2020  dentical").     
+00000790: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
+000007a0: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+000007b0: 2243 6865 636b 696e 6720 6966 2027 2528  "Checking if '%(
+000007c0: 6229 7327 2077 6173 2073 7175 6173 6865  b)s' was squashe
+000007d0: 6420 696e 746f 2027 2528 6129 7327 222c  d into '%(a)s'",
+000007e0: 207b 2261 223a 2061 2c20 2262 223a 2062   {"a": a, "b": b
+000007f0: 7d29 0a0a 2020 2020 7472 793a 0a20 2020  })..    try:.   
+00000800: 2020 2020 206d 6572 6765 5f62 6173 6520       merge_base 
+00000810: 3d20 6669 6e64 5f6d 6572 6765 5f62 6173  = find_merge_bas
+00000820: 6528 7265 706f 2c20 612c 2062 290a 2020  e(repo, a, b).  
+00000830: 2020 6578 6365 7074 204e 6f4d 6572 6765    except NoMerge
+00000840: 4261 7365 3a0a 2020 2020 2020 2020 7265  Base:.        re
+00000850: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
+00000860: 6272 616e 6368 5f64 6966 6620 3d20 622e  branch_diff = b.
+00000870: 636f 6d6d 6974 2e64 6966 6628 6d65 7267  commit.diff(merg
+00000880: 655f 6261 7365 290a 0a20 2020 2069 6620  e_base)..    if 
+00000890: 6c65 6e28 636f 6d6d 6974 7328 7265 706f  len(commits(repo
+000008a0: 2c20 7231 3d6d 6572 6765 5f62 6173 652c  , r1=merge_base,
+000008b0: 2072 323d 6229 2920 3d3d 2031 3a0a 2020   r2=b)) == 1:.  
+000008c0: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
+000008d0: 6f28 0a20 2020 2020 2020 2020 2020 2022  o(.            "
+000008e0: 536b 6970 7069 6e67 2062 7261 6e63 6820  Skipping branch 
+000008f0: 7769 7468 206f 6e65 2063 6f6d 6d69 742c  with one commit,
+00000900: 2022 0a20 2020 2020 2020 2020 2020 2022   ".            "
+00000910: 7371 7561 7368 696e 6720 616e 6420 7265  squashing and re
+00000920: 6261 7369 6e67 2061 7265 2065 7175 6976  basing are equiv
+00000930: 616c 656e 7420 696e 2074 6869 7320 6361  alent in this ca
+00000940: 7365 220a 2020 2020 2020 2020 290a 2020  se".        ).  
+00000950: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+00000960: 650a 0a20 2020 2066 6f72 2063 6f6d 6d69  e..    for commi
+00000970: 7420 696e 2063 6f6d 6d69 7473 2872 6570  t in commits(rep
+00000980: 6f2c 2072 313d 6d65 7267 655f 6261 7365  o, r1=merge_base
+00000990: 2c20 7232 3d61 293a 0a20 2020 2020 2020  , r2=a):.       
+000009a0: 2069 6620 6c65 6e28 636f 6d6d 6974 2e70   if len(commit.p
+000009b0: 6172 656e 7473 2920 3d3d 2030 3a0a 2020  arents) == 0:.  
+000009c0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+000009d0: 2e64 6562 7567 2822 536b 6970 7069 6e67  .debug("Skipping
+000009e0: 2063 6f6d 6d69 7420 7769 7468 206e 6f20   commit with no 
+000009f0: 7061 7265 6e74 7320 2528 6329 7322 2c20  parents %(c)s", 
+00000a00: 7b22 6322 3a20 636f 6d6d 6974 7d29 0a20  {"c": commit}). 
+00000a10: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+00000a20: 6e75 650a 2020 2020 2020 2020 656c 6966  nue.        elif
+00000a30: 206c 656e 2863 6f6d 6d69 742e 7061 7265   len(commit.pare
+00000a40: 6e74 7329 203e 3d20 323a 0a20 2020 2020  nts) >= 2:.     
+00000a50: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+00000a60: 6275 6728 2253 6b69 7070 696e 6720 6d65  bug("Skipping me
+00000a70: 7267 6520 636f 6d6d 6974 2025 2863 2973  rge commit %(c)s
+00000a80: 222c 207b 2263 223a 2063 6f6d 6d69 747d  ", {"c": commit}
+00000a90: 290a 2020 2020 2020 2020 2020 2020 636f  ).            co
+00000aa0: 6e74 696e 7565 0a20 2020 2020 2020 2065  ntinue.        e
+00000ab0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00000ac0: 2070 6172 656e 7420 3d20 636f 6d6d 6974   parent = commit
+00000ad0: 2e70 6172 656e 7473 5b30 5d0a 0a20 2020  .parents[0]..   
+00000ae0: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+00000af0: 280a 2020 2020 2020 2020 2020 2020 2243  (.            "C
+00000b00: 6865 636b 696e 6720 6966 2027 2528 6229  hecking if '%(b)
+00000b10: 7327 2077 6173 2073 7175 6173 6865 6420  s' was squashed 
+00000b20: 696e 746f 2027 2528 6129 7327 2062 7920  into '%(a)s' by 
+00000b30: 2528 6329 2e37 7322 2c0a 2020 2020 2020  %(c).7s",.      
+00000b40: 2020 2020 2020 7b22 6122 3a20 612c 2022        {"a": a, "
+00000b50: 6222 3a20 622c 2022 6322 3a20 636f 6d6d  b": b, "c": comm
+00000b60: 6974 7d2c 0a20 2020 2020 2020 2029 0a0a  it},.        )..
+00000b70: 2020 2020 2020 2020 6d61 7463 6865 735f          matches_
+00000b80: 6272 616e 6368 5f64 6966 6620 3d20 636f  branch_diff = co
+00000b90: 6d6d 6974 2e64 6966 6628 7061 7265 6e74  mmit.diff(parent
+00000ba0: 2920 3d3d 2062 7261 6e63 685f 6469 6666  ) == branch_diff
+00000bb0: 0a0a 2020 2020 2020 2020 6966 206d 6174  ..        if mat
+00000bc0: 6368 6573 5f62 7261 6e63 685f 6469 6666  ches_branch_diff
+00000bd0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00000be0: 7475 726e 2054 7275 650a 0a20 2020 2072  turn True..    r
+00000bf0: 6574 7572 6e20 4661 6c73 650a            eturn False.
```

### Comparing `switchbox-0.3.4/switchbox/repo.py` & `switchbox-0.4.0/switchbox/repo.py`

 * *Files 5% similar despite different names*

```diff
@@ -168,18 +168,27 @@
             "remote",
             "update",
             insert_kwargs_after="update",
             prune=True,
         )
 
     def update_branch_from_remote(self, remote: str, branch: str) -> None:
-        self.gitpython.git.branch(branch, f"{remote}/{branch}", force=True)
-        # self.repo.git.fetch(remote, f"{branch}:{branch}", "--update-head-ok")
+        if self.gitpython.active_branch.name == branch:
+            self.gitpython.remotes[remote].pull()
+        else:
+            self.gitpython.git.branch(branch, f"{remote}/{branch}", force=True)
 
     def switch(self, branch: str) -> None:
+        if self.gitpython.active_branch.name == branch:
+            logger.info(
+                "Not switching to branch %(branch), already on it",
+                {"branch", branch},
+            )
+            return
+
         self.gitpython.git.switch(branch)
 
     def discover_merged_branches(self, target: str) -> typing.Set[str]:
         """
         Find branches merged into a target branch.
 
         This uses 'git branch --merged' to find merged branches.
@@ -234,15 +243,19 @@
         if self.gitpython.active_branch.name == branch:
             raise Exception("Refusing to remove the active branch")
 
         logger.info("Deleting branch %(branch)s", {"branch": branch, "force": force})
         self.gitpython.delete_head(branch, force=force)
 
     def rebase(self, upstream: str) -> None:
-        self.gitpython.git.rebase(upstream)
+        self.gitpython.git.rebase(
+            upstream,
+            # # https://github.blog/2022-10-03-highlights-from-git-2-38/
+            # update_refs=True,
+        )
 
     def force_push(
         self, remote: str, local_branch: str, remote_branch: str, expect: str
     ) -> None:
         self.gitpython.git.push(
             remote,
             f"{local_branch}:{remote_branch}",
@@ -262,12 +275,13 @@
         )
         self.gitpython.git._call_process(
             "sparse-checkout",
             "set",
             *include,
             *exclude,
             insert_kwargs_after="set",
+            no_cone=True,
         )
         return include, exclude
 
     def sparse_checkout_reapply(self) -> None:
         self.gitpython.git._call_process("sparse-checkout", "reapply")
```

### Comparing `switchbox-0.3.4/setup.py` & `switchbox-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,96 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: switchbox
+Version: 0.4.0
+Summary: Tools for working with Git repositories.
+Home-page: https://pypi.org/project/switchbox/
+License: MPL-2.0
+Author: Sam Clements
+Author-email: sam@borntyping.co.uk
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Version Control
+Classifier: Topic :: Software Development :: Version Control :: Git
+Requires-Dist: GitPython (>=3.1.27,<4.0.0)
+Requires-Dist: PyGithub (>=1.55,<2.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: giturl (>=0.1.3,<0.2.0)
+Requires-Dist: inflect (>=6.0.0,<7.0.0)
+Requires-Dist: rich (>=12.5.1,<13.0.0)
+Project-URL: Repository, https://github.com/borntyping/switchbox
+Description-Content-Type: text/markdown
 
-packages = \
-['switchbox', 'switchbox.ext', 'switchbox.tests']
+switchbox
+=========
 
-package_data = \
-{'': ['*']}
+A collection of small tools for git workflows.
 
-install_requires = \
-['GitPython>=3.1.27,<4.0.0',
- 'PyGithub>=1.55,<2.0',
- 'click>=8.1.3,<9.0.0',
- 'giturl>=0.1.3,<0.2.0',
- 'inflect>=6.0.0,<7.0.0',
- 'rich>=12.5.1,<13.0.0']
-
-entry_points = \
-{'console_scripts': ['git-switchbox = switchbox.cli:main',
-                     'switchbox = switchbox.cli:main']}
-
-setup_kwargs = {
-    'name': 'switchbox',
-    'version': '0.3.4',
-    'description': 'Tools for working with Git repositories.',
-    'long_description': "switchbox\n=========\n\nA collection of small tools for git workflows.\n\nInstallation\n------------\n\nClone the repository and install the package with `pip`.\n\n```zsh\npip install --user .\n```\n\nUsage\n-----\n\nInvoke `switchbox` directly or run it via `git switchbox`.\n\nSwitchbox commands assume your git repository has a default branch and a\ndefault remote. When Switchbox is used for the first time (or you run\n`switchbox setup`) it will find and remember names for these.\n\n* The default branch will use a branch named `main` or `master`.\n* The default remote will use a remote named `upstream` or `origin`.\n\nSwitchbox options are set in a repository's `.git/config` file under a\n`switchbox` section.\n\n### `switchbox config`\n\nShow config options that Switchbox has set.\n\n### `switchbox config init`\n\nDetect a default branch and default remote, and save them to the repository's\ngit configuration. This will be done automatically when you first use a command\nthat works on a default branch or default remote.\n\n### `switchbox config default-branch $branch`\n\nChange the default branch.\n\n### `switchbox config default-remote $remote`\n\nChange the default remote.\n\n### `switchbox finish [--update/--no-update]`\n\n* Update all git remotes.\n* Update the local default branch to match the remote default branch.\n* Switch to the default branch.\n* Remove branches **merged** into the default branch.\n* Remove branches **squashed** into the default branch.\n\n### `switchbox tidy [--update/--no-update]`\n\n* Update all git remotes.\n* Remove branches **merged** into the default branch.\n* Remove branches **squashed** into the default branch.\n\n### `switchbox update`\n\n* Update all git remotes.\n",
-    'author': 'Sam Clements',
-    'author_email': 'sam@borntyping.co.uk',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://pypi.org/project/switchbox/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
+![A screenshot displaying the output of 'switchbox finish'.](./docs/screenshot.png)
 
+Installation
+------------
+
+Clone the repository and install the package with `pip`.
+
+```zsh
+pip install --user .
+```
+
+Usage
+-----
+
+Invoke `switchbox` directly or run it via `git switchbox`.
+
+Switchbox commands assume your git repository has a default branch and a
+default remote. When Switchbox is used for the first time (or you run
+`switchbox setup`) it will find and remember names for these.
+
+* The default branch will use a branch named `main` or `master`.
+* The default remote will use a remote named `upstream` or `origin`.
+
+Switchbox options are set in a repository's `.git/config` file under a
+`switchbox` section.
+
+### `switchbox config`
+
+Show config options that Switchbox has set.
+
+### `switchbox config init`
+
+Detect a default branch and default remote, and save them to the repository's
+git configuration. This will be done automatically when you first use a command
+that works on a default branch or default remote.
+
+### `switchbox config default-branch $branch`
+
+Change the default branch.
+
+### `switchbox config default-remote $remote`
+
+Change the default remote.
+
+### `switchbox finish [--update/--no-update]`
+
+* Update all git remotes.
+* Update the local default branch to match the remote default branch.
+* Switch to the default branch.
+* Remove branches **merged** into the default branch.
+* Remove branches **squashed** into the default branch.
+
+### `switchbox tidy [--update/--no-update]`
+
+* Update all git remotes.
+* Remove branches **merged** into the default branch.
+* Remove branches **squashed** into the default branch.
+
+### `switchbox update`
+
+* Update all git remotes.
 
-setup(**setup_kwargs)
```


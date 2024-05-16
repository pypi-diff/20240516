# Comparing `tmp/ddev-8.0.0.tar.gz` & `tmp/ddev-9.0.0.tar.gz`

## Comparing `ddev-8.0.0.tar` & `ddev-9.0.0.tar`

### file list

```diff
@@ -1,108 +1,123 @@
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/__main__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/py.typed
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/__init__.py
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/application.py
--rw-r--r--   0        0        0    17219 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/dep.py
--rw-r--r--   0        0        0    12319 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/terminal.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/ci/__init__.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/clean/__init__.py
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/config/__init__.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/docs/__init__.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/docs/build.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/docs/serve.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/env/__init__.py
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/env/agent.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/env/check.py
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/env/config.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/env/reload.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/env/shell.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/env/show.py
--rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/env/start.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/env/stop.py
--rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/env/test.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/meta/__init__.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/meta/scripts/__init__.py
--rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/meta/scripts/generate_metrics.py
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/meta/scripts/serve_openmetrics_payload.py
--rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/meta/scripts/upgrade_python.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/meta/scripts/scripts/serve.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/release/__init__.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/release/agent/__init__.py
--rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/release/agent/changelog.py
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/release/agent/common.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/release/agent/integrations.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/release/agent/integrations_changelog.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/release/changelog/__init__.py
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/release/changelog/fix.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/release/changelog/new.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/release/list_versions/__init__.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/release/show/__init__.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/release/stats/__init__.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/status/__init__.py
--rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/test/__init__.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/validate/__init__.py
--rw-r--r--   0        0        0    11991 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/validate/ci.py
--rw-r--r--   0        0        0     6209 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/validate/http.py
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/validate/labeler.py
--rw-r--r--   0        0        0    18700 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/validate/licenses.py
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/validate/licenses_utils.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/validate/manifest.py
--rw-r--r--   0        0        0    12514 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/validate/metadata.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/validate/metadata_utils.py
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/cli/validate/openmetrics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/config/__init__.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/config/constants.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/config/file.py
--rw-r--r--   0        0        0    23643 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/config/model.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/config/utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/e2e/__init__.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/e2e/config.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/e2e/constants.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/e2e/run.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/e2e/agent/__init__.py
--rw-r--r--   0        0        0    12584 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/e2e/agent/docker.py
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/e2e/agent/interface.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/integration/__init__.py
--rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/integration/core.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/integration/manifest.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/integration/metrics.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/plugin/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/plugin/api.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/plugin/specs.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/plugin/external/__init__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/plugin/external/hatch/__init__.py
--rw-r--r--   0        0        0     6991 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/plugin/external/hatch/environment_collector.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/plugin/external/starship/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/plugin/external/starship/__main__.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/plugin/external/starship/prompt.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/release/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/release/constants.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/repo/__init__.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/repo/config.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/repo/constants.py
--rw-r--r--   0        0        0     6859 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/repo/core.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/testing/__init__.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/testing/constants.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/testing/hatch.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/utils/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/utils/ci.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/utils/fs.py
--rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/utils/git.py
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/utils/github.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/utils/json.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/utils/network.py
--rw-r--r--   0        0        0     6660 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/utils/platform.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/utils/structures.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/utils/toml.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/utils/scripts/__init__.py
--rw-r--r--   0        0        0    11813 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/utils/scripts/check_pr.py
--rw-r--r--   0        0        0     9761 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/utils/scripts/ci_matrix.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/validation/__init__.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 ddev-8.0.0/src/ddev/validation/tracker.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 ddev-8.0.0/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 ddev-8.0.0/README.md
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 ddev-8.0.0/hatch.toml
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 ddev-8.0.0/pyproject.toml
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 ddev-8.0.0/PKG-INFO
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/__main__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/py.typed
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/__init__.py
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/application.py
+-rw-r--r--   0        0        0    12319 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/terminal.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/ci/__init__.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/clean/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/config/__init__.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/config/edit.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/config/explore.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/config/find.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/config/restore.py
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/config/set.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/config/show.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/config/update.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/dep/__init__.py
+-rw-r--r--   0        0        0     8730 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/dep/common.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/dep/freeze.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/dep/pin.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/dep/sync.py
+-rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/dep/updates.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/docs/__init__.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/docs/build.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/docs/serve.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/env/__init__.py
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/env/agent.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/env/check.py
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/env/config.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/env/reload.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/env/shell.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/env/show.py
+-rw-r--r--   0        0        0     7923 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/env/start.py
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/env/stop.py
+-rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/env/test.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/meta/__init__.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/meta/scripts/__init__.py
+-rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/meta/scripts/generate_metrics.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/meta/scripts/serve_openmetrics_payload.py
+-rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/meta/scripts/upgrade_python.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/meta/scripts/scripts/serve.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/release/__init__.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/release/agent/__init__.py
+-rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/release/agent/changelog.py
+-rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/release/agent/common.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/release/agent/integrations.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/release/agent/integrations_changelog.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/release/branch/__init__.py
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/release/branch/create.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/release/changelog/__init__.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/release/changelog/fix.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/release/changelog/new.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/release/list_versions/__init__.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/release/show/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/release/stats/__init__.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/status/__init__.py
+-rw-r--r--   0        0        0    10622 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/test/__init__.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/validate/__init__.py
+-rw-r--r--   0        0        0    11991 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/validate/ci.py
+-rw-r--r--   0        0        0     6209 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/validate/http.py
+-rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/validate/labeler.py
+-rw-r--r--   0        0        0    18700 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/validate/licenses.py
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/validate/licenses_utils.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/validate/manifest.py
+-rw-r--r--   0        0        0    14045 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/validate/metadata.py
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/validate/metadata_utils.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/cli/validate/openmetrics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/config/__init__.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/config/constants.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/config/file.py
+-rw-r--r--   0        0        0    23737 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/config/model.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/config/utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/e2e/__init__.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/e2e/config.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/e2e/constants.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/e2e/run.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/e2e/agent/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/e2e/agent/constants.py
+-rw-r--r--   0        0        0    12723 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/e2e/agent/docker.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/e2e/agent/interface.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/integration/__init__.py
+-rw-r--r--   0        0        0     7210 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/integration/core.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/integration/manifest.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/integration/metrics.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/plugin/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/plugin/api.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/plugin/specs.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/plugin/external/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/plugin/external/hatch/__init__.py
+-rw-r--r--   0        0        0     7000 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/plugin/external/hatch/environment_collector.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/plugin/external/starship/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/plugin/external/starship/__main__.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/plugin/external/starship/prompt.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/release/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/release/constants.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/repo/__init__.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/repo/config.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/repo/constants.py
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/repo/core.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/testing/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/testing/constants.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/testing/hatch.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/utils/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/utils/ci.py
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/utils/fs.py
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/utils/git.py
+-rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/utils/github.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/utils/json.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/utils/network.py
+-rw-r--r--   0        0        0     6660 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/utils/platform.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/utils/structures.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/utils/toml.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/utils/scripts/__init__.py
+-rw-r--r--   0        0        0    11814 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/utils/scripts/check_pr.py
+-rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/utils/scripts/ci_matrix.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/validation/__init__.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 ddev-9.0.0/src/ddev/validation/tracker.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 ddev-9.0.0/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 ddev-9.0.0/README.md
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 ddev-9.0.0/hatch.toml
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 ddev-9.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 ddev-9.0.0/PKG-INFO
```

### Comparing `ddev-8.0.0/src/ddev/cli/__init__.py` & `ddev-9.0.0/src/ddev/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/application.py` & `ddev-9.0.0/src/ddev/cli/application.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/terminal.py` & `ddev-9.0.0/src/ddev/cli/terminal.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/clean/__init__.py` & `ddev-9.0.0/src/ddev/cli/clean/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/docs/build.py` & `ddev-9.0.0/src/ddev/cli/docs/build.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/docs/serve.py` & `ddev-9.0.0/src/ddev/cli/docs/serve.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/env/__init__.py` & `ddev-9.0.0/src/ddev/cli/env/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/env/agent.py` & `ddev-9.0.0/src/ddev/cli/env/agent.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/env/check.py` & `ddev-9.0.0/src/ddev/cli/env/check.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/env/config.py` & `ddev-9.0.0/src/ddev/cli/env/config.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/env/reload.py` & `ddev-9.0.0/src/ddev/cli/env/reload.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/env/shell.py` & `ddev-9.0.0/src/ddev/cli/env/shell.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/env/show.py` & `ddev-9.0.0/src/ddev/cli/env/show.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/env/start.py` & `ddev-9.0.0/src/ddev/cli/env/start.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,39 +166,40 @@
         app.display_pair('Trigger run', app.style_info(f'ddev env agent {intg_name} {environment} check'))
         app.display_pair('Reload config', app.style_info(f'ddev env reload {intg_name} {environment}'))
         app.display_pair('Manage config', app.style_info('ddev env config'))
         app.display_pair('Config file', f'[link={env_data.config_file}]{env_data.config_file}[/]')
 
 
 def _get_agent_env_vars(org_config, metadata, extra_env_vars, dogstatsd):
+    from ddev.e2e.agent.constants import AgentEnvVars
     from ddev.e2e.constants import DEFAULT_DOGSTATSD_PORT, E2EEnvVars, E2EMetadata
 
     # Use the environment variables defined by tests as defaults so tooling can override them
     env_vars: dict[str, str] = metadata.get('env_vars', {}).copy()
 
     if api_key := org_config.get('api_key'):
-        env_vars['DD_API_KEY'] = api_key
+        env_vars[AgentEnvVars.API_KEY] = api_key
 
     if site := org_config.get('site'):
-        env_vars['DD_SITE'] = site
+        env_vars[AgentEnvVars.SITE] = site
 
     # Custom core Agent intake
     if dd_url := org_config.get('dd_url'):
-        env_vars['DD_DD_URL'] = dd_url
+        env_vars[AgentEnvVars.URL] = dd_url
 
     # Custom logs Agent intake
     if log_url := org_config.get('log_url'):
-        env_vars['DD_LOGS_CONFIG_DD_URL'] = log_url
+        env_vars[AgentEnvVars.LOGS_URL] = log_url
 
     # TODO: remove the CLI flag and exclusively rely on the metadata flag
     if metadata.get('dogstatsd') or dogstatsd:
-        env_vars['DD_DOGSTATSD_PORT'] = str(DEFAULT_DOGSTATSD_PORT)
-        env_vars['DD_DOGSTATSD_NON_LOCAL_TRAFFIC'] = 'true'
-        env_vars['DD_DOGSTATSD_METRICS_STATS_ENABLE'] = 'true'
+        env_vars[AgentEnvVars.DOGSTATSD_PORT] = str(DEFAULT_DOGSTATSD_PORT)
+        env_vars[AgentEnvVars.DOGSTATSD_NON_LOCAL_TRAFFIC] = 'true'
+        env_vars[AgentEnvVars.DOGSTATSD_METRICS_STATS] = 'true'
 
     # Enable logs Agent by default if the environment is mounting logs
     if any(ev.startswith(E2EEnvVars.LOGS_DIR_PREFIX) for ev in metadata.get(E2EMetadata.ENV_VARS, {})):
-        env_vars.setdefault('DD_LOGS_ENABLED', 'true')
+        env_vars.setdefault(AgentEnvVars.LOGS_ENABLED, 'true')
 
     env_vars.update(ev.split('=', maxsplit=1) for ev in extra_env_vars)
 
     return env_vars
```

### Comparing `ddev-8.0.0/src/ddev/cli/env/test.py` & `ddev-9.0.0/src/ddev/cli/env/test.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/meta/__init__.py` & `ddev-9.0.0/src/ddev/cli/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/meta/scripts/__init__.py` & `ddev-9.0.0/src/ddev/cli/meta/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/meta/scripts/generate_metrics.py` & `ddev-9.0.0/src/ddev/cli/meta/scripts/generate_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,17 +66,15 @@
                     overriden_values[metric.metric_name][loop % len(overriden_values[metric.metric_name])]
                     if metric.metric_name in overriden_values
                     else random.randint(0, 100)
                 )
                 type = (
                     MetricIntakeType.GAUGE
                     if metric.metric_type == 'gauge'
-                    else MetricIntakeType.COUNT
-                    if metric.metric_type == 'counter'
-                    else MetricIntakeType.UNSPECIFIED
+                    else MetricIntakeType.COUNT if metric.metric_type == 'counter' else MetricIntakeType.UNSPECIFIED
                 )
                 app.display_info(f"Metric {metric.metric_name} with value {value} and type {type}")
 
                 series.append(
                     MetricSeries(
                         metric=metric.metric_name,
                         type=type,
```

### Comparing `ddev-8.0.0/src/ddev/cli/meta/scripts/upgrade_python.py` & `ddev-9.0.0/src/ddev/cli/meta/scripts/upgrade_python.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/release/__init__.py` & `ddev-9.0.0/src/ddev/cli/release/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 from datadog_checks.dev.tooling.commands.release.build import build
 from datadog_checks.dev.tooling.commands.release.make import make
 from datadog_checks.dev.tooling.commands.release.tag import tag
 from datadog_checks.dev.tooling.commands.release.trello import trello
 from datadog_checks.dev.tooling.commands.release.upload import upload
 
 from ddev.cli.release.agent import agent
+from ddev.cli.release.branch import branch
 from ddev.cli.release.changelog import changelog
 from ddev.cli.release.list_versions import list_versions
 from ddev.cli.release.show import show
 from ddev.cli.release.stats import stats
 
 
 @click.group(short_help='Manage the release of integrations')
 def release():
     """
     Manage the release of integrations.
     """
 
 
 release.add_command(agent)
+release.add_command(branch)
 release.add_command(build)
 release.add_command(changelog)
 release.add_command(list_versions)
 release.add_command(make)
 release.add_command(show)
 release.add_command(stats)
 release.add_command(tag)
```

### Comparing `ddev-8.0.0/src/ddev/cli/release/agent/__init__.py` & `ddev-9.0.0/src/ddev/cli/release/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/release/agent/changelog.py` & `ddev-9.0.0/src/ddev/cli/release/agent/changelog.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/release/agent/common.py` & `ddev-9.0.0/src/ddev/cli/release/agent/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,23 +19,19 @@
     sorted by more recent first.
     """
     from packaging.version import parse as parse_version
 
     agent_tags = sorted(parse_version(t) for t in repo.git.filter_tags(r'^\d+\.\d+\.\d+$'))
 
     # default value for `to` is the latest tag
-    if to:
-        to = parse_version(to)
-    else:
-        to = agent_tags[-1]
-
-    since = parse_version(since)
+    to_version = parse_version(to) if to else agent_tags[-1]
+    since_version = parse_version(since)
 
     # filter out versions according to the interval [since, to]
-    agent_tags = [t for t in agent_tags if since <= t <= to]
+    agent_tags = [t for t in agent_tags if since_version <= t <= to_version]
 
     # reverse so we have descendant order
     return [str(t) for t in reversed(agent_tags)]
 
 
 def get_changes_per_agent(repo: Repository, since: str, to: str) -> AgentChangelog:
     """
```

### Comparing `ddev-8.0.0/src/ddev/cli/release/agent/integrations.py` & `ddev-9.0.0/src/ddev/cli/release/agent/integrations.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/release/agent/integrations_changelog.py` & `ddev-9.0.0/src/ddev/cli/release/agent/integrations_changelog.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/release/changelog/fix.py` & `ddev-9.0.0/src/ddev/cli/release/changelog/fix.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/release/changelog/new.py` & `ddev-9.0.0/src/ddev/cli/release/changelog/new.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,48 +14,60 @@
 @click.command(short_help='Create changelog entries')
 @click.argument('entry_type', required=False)
 @click.argument('targets', nargs=-1, required=False)
 @click.option('--message', '-m', help='The changelog text')
 @click.pass_obj
 def new(app: Application, entry_type: str | None, targets: tuple[str], message: str | None):
     """
-    This creates new changelog entries. If the entry type is not specified, you will be prompted.
+    This creates new changelog entries in Markdown format.
+
+    If the ENTRY_TYPE is not specified, you will be prompted.
 
     The `--message` option can be used to specify the changelog text. If this is not supplied, an editor
     will be opened for you to manually write the entry. The changelog text that is opened defaults to
     the PR title, followed by the most recent commit subject. If that is sufficient, then you may close
     the editor tab immediately.
 
     By default, changelog entries will be created for all integrations that have changed code. To create
     entries only for specific targets, you may pass them as additional arguments after the entry type.
     """
     from datadog_checks.dev.tooling.commands.release.changelog import towncrier
 
+    create_command = None
+
+    edited = 0
+    for check in app.repo.integrations.iter_changed_code(targets):
+        if not create_command:
+            create_command = __get_create_command(app, entry_type, message)
+
+        towncrier(check.path, *create_command)
+        edited += 1
+
+    if not edited:
+        app.display_info('No changelog entries to create')
+    else:
+        app.display_success(f'Added {edited} changelog entr{"ies" if edited > 1 else "y"}')
+
+
+def __get_create_command(app, entry_type, message):
     from ddev.release.constants import ENTRY_TYPES
 
     latest_commit = app.repo.git.latest_commit
     pr = app.github.get_pull_request(latest_commit.sha)
-    message_based_on_git = ''
     if pr is not None:
         pr_number = pr.number
         message_based_on_git = pr.title
     else:
         pr_number = app.github.get_next_issue_number()
         message_based_on_git = latest_commit.subject
 
-    if entry_type is not None:
-        if entry_type not in ENTRY_TYPES:
-            app.abort(f'Unknown entry type: {entry_type}')
-    else:
+    if entry_type is None:
         entry_type = click.prompt('Entry type?', type=click.Choice(ENTRY_TYPES, case_sensitive=False))
+    elif entry_type not in ENTRY_TYPES:
+        app.abort(f'Unknown entry type: {entry_type}')
 
-    create_cmd = [
+    return [
         'create',
         '--content',
         message or click.edit(text=message_based_on_git, require_save=False) or message_based_on_git,
         f'{pr_number}.{entry_type}',
     ]
-    edited = 0
-    for check in app.repo.integrations.iter_changed_code(targets):
-        towncrier(check.path, *create_cmd)
-        edited += 1
-    app.display_success(f'Added {edited} changelog entr{"ies" if edited > 1 else "y"}')
```

### Comparing `ddev-8.0.0/src/ddev/cli/release/list_versions/__init__.py` & `ddev-9.0.0/src/ddev/cli/release/list_versions/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/release/show/__init__.py` & `ddev-9.0.0/src/ddev/cli/release/show/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/status/__init__.py` & `ddev-9.0.0/src/ddev/cli/status/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/test/__init__.py` & `ddev-9.0.0/src/ddev/cli/test/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     junit: bool,
     hide_header: bool,
     e2e: bool,
 ):
     """
     Run unit and integration tests.
 
-    Please see these docs for to pass TARGET_SPEC and PYTEST_ARGS:
+    Please see these docs to know how to pass TARGET_SPEC and PYTEST_ARGS:
 
     \b
     https://datadoghq.dev/integrations-core/testing/
     """
     import json
     import os
     import sys
@@ -101,25 +101,32 @@
 
     # target name -> target
     targets: dict[str, Integration] = {}
     if target_name == 'changed':
         for integration in app.repo.integrations.iter_changed():
             if integration.is_testable:
                 targets[integration.name] = integration
+    elif target_name == 'all':
+        for integration in app.repo.integrations.iter_testable('all'):
+            targets[integration.name] = integration
     else:
         try:
             integration = app.repo.integrations.get(target_name)
         except OSError:
             app.abort(f'Unknown target: {target_name}')
 
         if integration.is_testable:
             targets[integration.name] = integration
 
     if not targets:
-        app.abort('No testable targets found')
+        if target_name == 'changed':
+            app.display_info('No changed testable targets found')
+            return
+        else:
+            app.abort('No testable targets found')
 
     if list_envs:
         multiple_targets = len(targets) > 1
         for target in targets.values():
             with target.path.as_cwd():
                 if multiple_targets:
                     app.display_header(target.display_name)
```

### Comparing `ddev-8.0.0/src/ddev/cli/validate/__init__.py` & `ddev-9.0.0/src/ddev/cli/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/validate/ci.py` & `ddev-9.0.0/src/ddev/cli/validate/ci.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/validate/http.py` & `ddev-9.0.0/src/ddev/cli/validate/http.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/validate/labeler.py` & `ddev-9.0.0/src/ddev/cli/validate/labeler.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,18 @@
     if not is_core:
         app.display_info(
             f"The labeler validation is only enabled for integrations-core, skipping for repo {app.repo.name}"
         )
         return
 
     valid_integrations = dict.fromkeys(i.name for i in app.repo.integrations.iter("all"))
-    # Remove this when we remove the `datadog_checks_tests_helper` package
-    valid_integrations['datadog_checks_tests_helper'] = None
+
+    include = set(app.repo.config.get('/overrides/validate/labeler/include', []))
+    for integration in include:
+        valid_integrations[integration] = None
 
     pr_labels_config_path = app.repo.path / '.github' / 'workflows' / 'config' / 'labeler.yml'
     if not pr_labels_config_path.exists():
         app.abort('Unable to find the PR Labels config file')
 
     pr_labels_config = yaml.safe_load(pr_labels_config_path.read_text())
     new_pr_labels_config = copy.deepcopy(pr_labels_config)
```

### Comparing `ddev-8.0.0/src/ddev/cli/validate/licenses.py` & `ddev-9.0.0/src/ddev/cli/validate/licenses.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/validate/licenses_utils.py` & `ddev-9.0.0/src/ddev/cli/validate/licenses_utils.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/cli/validate/manifest.py` & `ddev-9.0.0/src/ddev/cli/validate/manifest.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 @click.command(short_help='Validate integration manifests')
 @click.argument('integrations', nargs=-1)
 @click.pass_context
 def manifest(ctx: click.Context, integrations: tuple[str, ...]):
     """Validate integration manifests."""
     import httpx
-    from datadog_checks.dev.tooling.commands.validate.manifest import manifest as legacy_manifest_validation
 
     app: Application = ctx.obj
     validation_tracker = app.create_validation_tracker('Manifests')
 
     dd_url = app.config.org.config.get('dd_url', '')
     if not dd_url:
         app.abort(f'No `dd_url` has been set for org `{app.config.org.name}`')
@@ -43,9 +42,8 @@
         except Exception as e:
             validation_tracker.error((integration.display_name, 'manifest.json'), message=str(e))
 
     if validation_tracker.errors:
         validation_tracker.display()
         app.abort()
 
-    ctx.invoke(legacy_manifest_validation, check=integrations[0] if integrations else None, ignore_schema=True)
     validation_tracker.display()
```

### Comparing `ddev-8.0.0/src/ddev/cli/validate/metadata.py` & `ddev-9.0.0/src/ddev/cli/validate/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,27 +57,31 @@
 
 @click.command(short_help='Validate `metadata.csv` files')
 @click.argument('integrations', nargs=-1)
 @click.option(
     '--check-duplicates', is_flag=True, help='Output warnings if there are duplicate short names and descriptions'
 )
 @click.option('--show-warnings', '-w', is_flag=True, help='Show warnings in addition to failures')
+@click.option('--sync', is_flag=True, help='Update the file')
 @click.pass_obj
-def metadata(app: Application, integrations: tuple[str, ...], check_duplicates: bool, show_warnings: bool):
+def metadata(app: Application, integrations: tuple[str, ...], check_duplicates: bool, show_warnings: bool, sync: bool):
     """
     Validate `metadata.csv` files
 
-    If `check` is specified, only the check will be validated, if check value is
-    'changed' will only apply to changed checks, an 'all' or empty `check` value
-    will validate all README files.
+    If `integrations` is specified, only the check will be validated, an 'all' or empty value will validate all
+    metadata.csv files, a `changed` value will validate changed integrations.
     """
     from ddev.cli.validate import metadata_utils
 
+    is_core = app.repo.name == 'core'
     validation_tracker = app.create_validation_tracker('Metrics validation')
 
+    if not integrations:
+        integrations = ('all',)
+
     excluded = set(app.repo.config.get('/overrides/validate/metrics/exclude', []))
     for current_check in app.repo.integrations.iter(integrations):
         if current_check.name in excluded or not current_check.has_metrics:
             continue
 
         errors = False
         error_message = ""
@@ -101,15 +105,18 @@
         if metadata_file.stat().st_size == 0:
             errors = True
 
             error_message += (
                 f"{current_check.name} metadata file is empty. This file needs the header row at the minimum.\n"
             )
 
+        rows = []
+
         for line, row in read_metadata_rows(metadata_file):
+            rows.append(row)
             # determine if number of columns is complete by checking for None values
             # DictReader populates missing columns with None https://docs.python.org/3.8/library/csv.html#csv.DictReader
             if None in row.values():
                 errors = True
 
                 error_message += f"{current_check.name}:{line} {row['metric_name']} has the wrong number of columns.\n"
                 continue
@@ -119,20 +126,25 @@
             if all_keys != metadata_utils.ALL_HEADERS:
                 invalid_headers = all_keys.difference(metadata_utils.ALL_HEADERS)
                 if invalid_headers:
                     errors = True
 
                     error_message += f"{current_check.name}:{line} Invalid column {invalid_headers}.\n"
 
-                missing_headers = metadata_utils.ALL_HEADERS.difference(all_keys)
+                missing_headers = metadata_utils.HEADERS_TO_CHECK.difference(all_keys)
                 if missing_headers:
                     errors = True
 
                     error_message += f"{current_check.name}:{line} Missing columns {missing_headers}.\n"
-                continue
+
+                if errors:
+                    # There's now an optional sample_tag column that isn't added yet to the existing metadata.csv
+                    # all_keys will not be same as ALL_HEADERS. But since that sample_tag column is optional and not
+                    # inside HEADERS_TO_CHECK, we should only continue if there's an invalid header or missing_header.
+                    continue
 
             # check duplicate metric name
             duplicate_metric_name = check_duplicate_values(
                 current_check, line, row, 'metric_name', duplicate_name_set, fail=True
             )
             if duplicate_metric_name[0]:
                 errors = True
@@ -270,14 +282,31 @@
             errors = True
 
             error_message += (
                 f"{current_check.name}: `{prefix}` appears {count} time(s) and does not match metric_prefix "
             )
             error_message += "defined in the manifest.\n"
 
+        unsorted = set(app.repo.config.get('/overrides/validate/metrics/unsorted', []))
+
+        if is_core and current_check.name not in unsorted:
+            sorted_rows = sorted(rows, key=lambda x: x['metric_name'])
+            if sorted_rows != rows:
+                error_message = f"{current_check.name}: metadata.csv is not sorted by metric name.\n"
+
+                if not sync:
+                    errors = True
+                    error_message += f"Run `ddev validate metadata {current_check.name} --sync` to sort it.\n"
+                else:
+                    error_message += f"Sorting {metadata_file.relative_to(app.repo.path)} by metric names."
+                    with metadata_file.open(mode='w', encoding='utf-8') as f:
+                        writer = csv.DictWriter(f, fieldnames=metadata_utils.ORDERED_HEADERS)
+                        writer.writeheader()
+                        writer.writerows(sorted_rows)
+
         error_message = error_message[:-1]
         if errors:
             validation_tracker.error(
                 (current_check.display_name, str(metadata_file.relative_to(app.repo.path))),
                 message=error_message,
             )
         else:
```

### Comparing `ddev-8.0.0/src/ddev/cli/validate/metadata_utils.py` & `ddev-9.0.0/src/ddev/cli/validate/metadata_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,40 @@
 # (C) Datadog, Inc. 2023-present
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
 import re
 
 REQUIRED_HEADERS = {'metric_name', 'metric_type', 'orientation', 'integration'}
 
-OPTIONAL_HEADERS = {'description', 'interval', 'unit_name', 'per_unit_name', 'short_name', 'curated_metric'}
-
-ALL_HEADERS = REQUIRED_HEADERS | OPTIONAL_HEADERS
+OPTIONAL_HEADERS = {
+    'description',
+    'interval',
+    'unit_name',
+    'per_unit_name',
+    'short_name',
+    'curated_metric',
+}
+
+EXPERIMENTAL_HEADER = {"sample_tags"}
+ALL_HEADERS = REQUIRED_HEADERS | OPTIONAL_HEADERS | EXPERIMENTAL_HEADER
+HEADERS_TO_CHECK = REQUIRED_HEADERS | OPTIONAL_HEADERS
+
+ORDERED_HEADERS = [
+    "metric_name",
+    "metric_type",
+    "interval",
+    "unit_name",
+    "per_unit_name",
+    "description",
+    "orientation",
+    "integration",
+    "short_name",
+    "curated_metric",
+    "sample_tags",
+]
 
 VALID_METRIC_TYPE = {'count', 'gauge', 'rate'}
 
 VALID_ORIENTATION = {'0', '1', '-1'}
 
 VALID_CURATED_METRIC_TYPES = {'cpu', 'memory'}
```

### Comparing `ddev-8.0.0/src/ddev/cli/validate/openmetrics.py` & `ddev-9.0.0/src/ddev/cli/validate/openmetrics.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/config/constants.py` & `ddev-9.0.0/src/ddev/config/constants.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/config/file.py` & `ddev-9.0.0/src/ddev/config/file.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/config/model.py` & `ddev-9.0.0/src/ddev/config/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,21 +199,23 @@
 
                 for name, data in orgs.items():
                     if not isinstance(data, dict):
                         self.raise_error('must be a table', extra_steps=(name,))
 
                 self._field_orgs = orgs
             else:
+                from ddev.e2e.agent.constants import AgentEnvVars
+
                 self._field_orgs = self.raw_data['orgs'] = {
                     'default': {
-                        'api_key': os.getenv('DD_API_KEY', ''),
-                        'app_key': os.getenv('DD_APP_KEY', ''),
-                        'site': os.getenv('DD_SITE', 'datadoghq.com'),
-                        'dd_url': os.getenv('DD_DD_URL', 'https://app.datadoghq.com'),
-                        'log_url': os.getenv('DD_LOGS_CONFIG_DD_URL', ''),
+                        'api_key': os.getenv(AgentEnvVars.API_KEY, ''),
+                        'app_key': os.getenv(AgentEnvVars.APP_KEY, ''),
+                        'site': os.getenv(AgentEnvVars.SITE, 'datadoghq.com'),
+                        'dd_url': os.getenv(AgentEnvVars.URL, 'https://app.datadoghq.com'),
+                        'log_url': os.getenv(AgentEnvVars.LOGS_URL, ''),
                     },
                 }
 
         return self._field_orgs
 
     @orgs.setter
     def orgs(self, value):
```

### Comparing `ddev-8.0.0/src/ddev/config/utils.py` & `ddev-9.0.0/src/ddev/config/utils.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/e2e/config.py` & `ddev-9.0.0/src/ddev/e2e/config.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/e2e/run.py` & `ddev-9.0.0/src/ddev/e2e/run.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/e2e/agent/__init__.py` & `ddev-9.0.0/src/ddev/e2e/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/e2e/agent/docker.py` & `ddev-9.0.0/src/ddev/e2e/agent/docker.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,58 +87,60 @@
     def _show_logs(self) -> None:
         self._run_command(['docker', 'logs', self._container_name])
 
     def get_id(self) -> str:
         return self._container_name
 
     def start(self, *, agent_build: str, local_packages: dict[Path, str], env_vars: dict[str, str]) -> None:
+        from ddev.e2e.agent.constants import AgentEnvVars
+
         if not agent_build:
             agent_build = 'datadog/agent-dev:master'
 
         if agent_build.startswith("datadog/"):
             # Add a potentially missing `py` suffix for default non-RC builds
             if 'rc' not in agent_build and 'py' not in agent_build and not re.match(AGENT_VERSION_REGEX, agent_build):
                 agent_build = f'{agent_build}-py{self.python_version[0]}'
 
             if self.metadata.get('use_jmx') and not agent_build.endswith('-jmx'):
                 agent_build += '-jmx'
 
         env_vars = env_vars.copy()
 
         # Containerized agents require an API key to start
-        if 'DD_API_KEY' not in env_vars:
+        if AgentEnvVars.API_KEY not in env_vars:
             # This fake key must be the proper length
-            env_vars['DD_API_KEY'] = 'a' * 32
+            env_vars[AgentEnvVars.API_KEY] = 'a' * 32
 
         # Set Agent hostname for CI
-        env_vars['DD_HOSTNAME'] = _get_hostname()
+        env_vars[AgentEnvVars.HOSTNAME] = _get_hostname()
 
         # Run API on a random free port
-        env_vars['DD_CMD_PORT'] = str(_find_free_port())
+        env_vars[AgentEnvVars.CMD_PORT] = str(_find_free_port())
 
         # Disable trace Agent
-        env_vars['DD_APM_ENABLED'] = 'false'
+        env_vars[AgentEnvVars.APM_ENABLED] = 'false'
 
         # Set up telemetry
-        env_vars['DD_TELEMETRY_ENABLED'] = '1'
-        env_vars['DD_EXPVAR_PORT'] = '5000'
+        env_vars[AgentEnvVars.TELEMETRY_ENABLED] = '1'
+        env_vars[AgentEnvVars.EXPVAR_PORT] = '5000'
 
         # TODO: Remove this when Python 2 support is removed
         #
         # Don't write .pyc, needed to fix this issue (only Python 2):
         # More info: https://github.com/DataDog/integrations-core/pull/5454
         # When reinstalling a package, .pyc are not cleaned correctly. The issue is fixed by not writing them
         # in the first place.
         env_vars['PYTHONDONTWRITEBYTECODE'] = '1'
 
         if (proxy_data := self.metadata.get('proxy')) is not None:
             if (http_proxy := proxy_data.get('http')) is not None:
-                env_vars['DD_PROXY_HTTP'] = http_proxy
+                env_vars[AgentEnvVars.PROXY_HTTP] = http_proxy
             if (https_proxy := proxy_data.get('https')) is not None:
-                env_vars['DD_PROXY_HTTPS'] = https_proxy
+                env_vars[AgentEnvVars.PROXY_HTTPS] = https_proxy
 
         volumes = []
 
         if not self._is_windows_container:
             volumes.append('/proc:/host/proc')
 
         # Only mount the volume if the initial configuration is not set to `None`.
@@ -194,15 +196,15 @@
             command.extend(['-e', f'{key}={value}'])
 
         # The docker `--add-host` command will reliably create entries in the `/etc/hosts` file,
         # otherwise, edits to that file will be overwritten on container restarts
         for host, ip in self.metadata.get('custom_hosts', []):
             command.extend(['--add-host', f'{host}:{ip}'])
 
-        if dogstatsd_port := env_vars.get('DD_DOGSTATSD_PORT'):
+        if dogstatsd_port := env_vars.get(AgentEnvVars.DOGSTATSD_PORT):
             command.extend(['-p', f'{dogstatsd_port}:{dogstatsd_port}/udp'])
 
         # The chosen tag
         command.append(agent_build)
 
         process = self._captured_process(command)
         if process.returncode:
```

### Comparing `ddev-8.0.0/src/ddev/e2e/agent/interface.py` & `ddev-9.0.0/src/ddev/e2e/agent/interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,25 +55,20 @@
         major, minor = PYTHON_VERSION.split('.')
         return int(major), int(minor)
 
     def get_id(self) -> str:
         return f'{self.integration.name}_{self.env}'
 
     @abstractmethod
-    def start(self, *, agent_build: str, local_packages: dict[Path, str], env_vars: dict[str, str]) -> None:
-        ...
+    def start(self, *, agent_build: str, local_packages: dict[Path, str], env_vars: dict[str, str]) -> None: ...
 
     @abstractmethod
-    def stop(self) -> None:
-        ...
+    def stop(self) -> None: ...
 
     @abstractmethod
-    def restart(self) -> None:
-        ...
+    def restart(self) -> None: ...
 
     @abstractmethod
-    def invoke(self, args: list[str]) -> None:
-        ...
+    def invoke(self, args: list[str]) -> None: ...
 
     @abstractmethod
-    def enter_shell(self) -> None:
-        ...
+    def enter_shell(self) -> None: ...
```

### Comparing `ddev-8.0.0/src/ddev/integration/core.py` & `ddev-9.0.0/src/ddev/integration/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,16 +187,15 @@
 
     @cached_property
     def is_tile(self) -> bool:
         return self.is_integration and not self.is_package
 
     @cached_property
     def is_testable(self) -> bool:
-        # TODO: remove tox when the Hatch migration is complete
-        return (self.path / 'hatch.toml').is_file() or (self.path / 'tox.ini').is_file()
+        return (self.path / 'hatch.toml').is_file()
 
     @cached_property
     def is_shippable(self) -> bool:
         return self.is_package and self.path.name not in NOT_SHIPPABLE
 
     @cached_property
     def is_agent_check(self) -> bool:
```

### Comparing `ddev-8.0.0/src/ddev/plugin/external/hatch/environment_collector.py` & `ddev-9.0.0/src/ddev/plugin/external/hatch/environment_collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,29 +127,29 @@
     def get_initial_config(self):
         settings_dir = '.' if self.is_dev_package else '..'
         lint_env = {
             'detached': True,
             'scripts': {
                 'style': [
                     f'black --config {settings_dir}/pyproject.toml --check --diff .',
-                    f'ruff --config {settings_dir}/pyproject.toml .',
+                    f'ruff check --config {settings_dir}/pyproject.toml .',
                 ],
                 'fmt': [
                     f'black . --config {settings_dir}/pyproject.toml',
-                    f'ruff --config {settings_dir}/pyproject.toml --fix .',
+                    f'ruff check --config {settings_dir}/pyproject.toml --fix .',
                     'python -c "print(\'\\n[NOTE] ruff may still report style errors for things '
                     'black cannot fix, these will need to be fixed manually.\')"',
                     'style',
                 ],
                 'all': ['style'],
             },
             # We pin deps in order to make CI more stable/reliable.
             'dependencies': [
-                'black==22.12.0',
-                'ruff==0.0.257',
+                'black==24.2.0',
+                'ruff==0.3.3',
                 # Keep in sync with: /datadog_checks_base/pyproject.toml
                 'pydantic==2.0.2',
             ],
         }
         config = {'lint': lint_env}
 
         if self.check_types:
```

### Comparing `ddev-8.0.0/src/ddev/repo/core.py` & `ddev-9.0.0/src/ddev/repo/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def config(self) -> RepositoryConfig:
         from ddev.repo.config import RepositoryConfig
 
         return RepositoryConfig(self.path / CONFIG_DIRECTORY / 'config.toml')
 
     @cached_property
     def agent_requirements(self) -> Path:
-        return self.path / 'datadog_checks_base' / 'datadog_checks' / 'base' / 'data' / 'agent_requirements.in'
+        return self.path / 'agent_requirements.in'
 
     @cached_property
     def agent_release_requirements(self) -> Path:
         return self.path / 'requirements-agent-release.txt'
 
     @cached_property
     def agent_changelog(self) -> Path:
@@ -188,16 +188,17 @@
         else:
             integration = Integration(path, self.repo.path, self.repo.config)
             self.__cache[path.name] = integration
 
         return integration
 
     def __finalize_selection(self, selection: Iterable[str]) -> set[str] | None:
-        if not selection:
+        if not selection or 'changed' in selection:
             return self.__get_changed_root_entries() or None
-        elif 'all' in selection:
+
+        if 'all' in selection:
             return set()
-        else:
-            return set(selection)
+
+        return set(selection)
 
     def __get_changed_root_entries(self) -> set[str]:
         return {relative_path.split('/', 1)[0] for relative_path in self.repo.git.changed_files}
```

### Comparing `ddev-8.0.0/src/ddev/utils/fs.py` & `ddev-9.0.0/src/ddev/utils/fs.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/utils/git.py` & `ddev-9.0.0/src/ddev/utils/git.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/utils/github.py` & `ddev-9.0.0/src/ddev/utils/github.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # (C) Datadog, Inc. 2023-present
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
 from __future__ import annotations
 
+import json
 from functools import cached_property
 from time import time
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from httpx import Client
 
@@ -16,16 +17,18 @@
 
 class PullRequest:
     def __init__(self, data: dict[str, Any]):
         self.__number = data['number']
         self.__title = data['title']
         self.__html_url = data['pull_request']['html_url']
         self.__diff_url = data['pull_request']['diff_url']
-        # Normalize to remove carriage returns on Windows
-        self.__body = '\n'.join(data['body'].splitlines())
+        # Github API returns `None` for empty bodies, but we use empty string as default.
+        # Normalize to remove carriage returns on Windows.
+        raw_body = data['body']
+        self.__body = ('' if raw_body is None else raw_body).replace(r'\r', '')
         self.__author = data['user']['login']
         self.__labels = sorted(label['name'] for label in data['labels'])
 
     @property
     def number(self) -> int:
         return self.__number
 
@@ -59,14 +62,17 @@
 
     # https://docs.github.com/en/rest/search?apiVersion=2022-11-28#search-issues-and-pull-requests
     ISSUE_SEARCH_API = 'https://api.github.com/search/issues'
 
     # https://docs.github.com/en/rest/issues/issues?apiVersion=2022-11-28#list-repository-issues
     ISSUE_LIST_API = 'https://api.github.com/repos/{repo_id}/issues'
 
+    # https://docs.github.com/en/rest/issues/labels?apiVersion=2022-11-28#create-a-label
+    LABELS_API = 'https://api.github.com/repos/{repo_id}/labels'
+
     def __init__(self, repo: Repository, *, user: str, token: str, status: BorrowedStatus):
         self.__repo = repo
         self.__auth = (user, token)
         self.__status = status
         self.__repo_id = f'DataDog/{self.__repo.full_name}'
 
     @property
@@ -111,21 +117,35 @@
 
         return number
 
     def get_diff(self, pr: PullRequest) -> str:
         response = self.__api_get(pr.diff_url, follow_redirects=True)
         return response.text
 
+    def create_label(self, name, color):
+        self.__api_post(
+            self.LABELS_API.format(repo_id=self.repo_id), content=json.dumps({'name': name, 'color': color})
+        )
+
+    def get_label(self, name):
+        return self.__api_get(f'{self.LABELS_API.format(repo_id=self.repo_id)}/{name}')
+
+    def __api_post(self, *args, **kwargs):
+        return self.__api_call('post', *args, **kwargs)
+
     def __api_get(self, *args, **kwargs):
+        return self.__api_call('get', *args, **kwargs)
+
+    def __api_call(self, method, *args, **kwargs):
         from httpx import HTTPError
 
         retry_wait = 2
         while True:
             try:
-                response = self.client.get(*args, auth=self.__auth, **kwargs)
+                response = getattr(self.client, method)(*args, auth=self.__auth, **kwargs)
 
                 # https://docs.github.com/en/rest/overview/resources-in-the-rest-api?apiVersion=2022-11-28#rate-limiting
                 # https://docs.github.com/en/rest/guides/best-practices-for-integrators?apiVersion=2022-11-28#dealing-with-rate-limits
                 if response.status_code == 403 and response.headers['X-RateLimit-Remaining'] == '0':  # noqa: PLR2004
                     self.__status.wait_for(
                         float(response.headers['X-RateLimit-Reset']) - time() + 1,
                         context='GitHub API rate limit reached',
```

### Comparing `ddev-8.0.0/src/ddev/utils/json.py` & `ddev-9.0.0/src/ddev/utils/json.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/utils/platform.py` & `ddev-9.0.0/src/ddev/utils/platform.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/utils/structures.py` & `ddev-9.0.0/src/ddev/utils/structures.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/src/ddev/utils/scripts/check_pr.py` & `ddev-9.0.0/src/ddev/utils/scripts/check_pr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Running this script by itself must not use any external dependencies.
 """
+
 # (C) Datadog, Inc. 2023-present
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
 from __future__ import annotations
 
 import os
 import re
```

### Comparing `ddev-8.0.0/src/ddev/utils/scripts/ci_matrix.py` & `ddev-9.0.0/src/ddev/utils/scripts/ci_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Running this script by itself requires Python 3.11 or later and must not use any external dependencies.
 
 The logic is also imported by ddev to perform the CI validation on 3.8 which works because dependencies exist.
 """
+
 # (C) Datadog, Inc. 2023-present
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
 from __future__ import annotations
 
 import argparse
 import json
@@ -49,15 +50,15 @@
   | metadata\.csv
   | pyproject\.toml
   | datadog_checks/[^/]+/data/metrics\.yaml
   | datadog_checks/snmp/data/default_profiles/.+
     """,
     re.VERBOSE,
 )
-AGENT_REQUIREMENTS_FILE = 'datadog_checks_base/datadog_checks/base/data/agent_requirements.in'
+AGENT_REQUIREMENTS_FILE = 'agent_requirements.in'
 NON_TESTABLE_FILES = {'auto_conf.yaml'}
 DISPLAY_ORDER_OVERRIDE = {
     _d: _i
     for _i, _d in enumerate(
         (
             'ddev',
             'datadog_checks_base',
```

### Comparing `ddev-8.0.0/src/ddev/validation/tracker.py` & `ddev-9.0.0/src/ddev/validation/tracker.py`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/.gitignore` & `ddev-9.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/README.md` & `ddev-9.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ddev-8.0.0/pyproject.toml` & `ddev-9.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "click~=8.1.6",
     "coverage",
     "datadog-api-client==2.20.0",
-    "datadog-checks-dev[cli]~=31.0",
+    "datadog-checks-dev[cli]~=32.1",
     "hatch>=1.8.1",
     "httpx",
     "jsonpointer",
     "pluggy",
     "rich>=12.5.1",
     "stamina==23.2.0",
     "tomli; python_version < '3.11'",
@@ -79,14 +79,16 @@
 target-version = ["py311"]
 extend-exclude = "src/ddev/_version.py"
 
 [tool.ruff]
 exclude = []
 target-version = "py311"
 line-length = 120
+
+[tool.ruff.lint]
 # Rules were ported over from the legacy flake8 settings for parity
 # All the rules can be found here: https://beta.ruff.rs/docs/rules/
 select = [
   "B",
   "C",
   "E",
   "F",
@@ -106,16 +108,16 @@
   "C901",
 ]
 unfixable = [
   # Don't touch unused imports
   "F401",
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["ddev"]
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 #Tests can use assertions and relative imports
 "**/tests/**/*" = ["I252"]
```

### Comparing `ddev-8.0.0/PKG-INFO` & `ddev-9.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ddev
-Version: 8.0.0
+Version: 9.0.0
 Summary: The Datadog Agent integration developer tool
 Project-URL: Source, https://github.com/DataDog/integrations-core
 Author-email: Datadog <packages@datadoghq.com>
 License-Expression: BSD-3-Clause
 Keywords: agent,datadog,integration
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Requires-Dist: click~=8.1.6
 Requires-Dist: coverage
 Requires-Dist: datadog-api-client==2.20.0
-Requires-Dist: datadog-checks-dev[cli]~=31.0
+Requires-Dist: datadog-checks-dev[cli]~=32.1
 Requires-Dist: hatch>=1.8.1
 Requires-Dist: httpx
 Requires-Dist: jsonpointer
 Requires-Dist: pluggy
 Requires-Dist: rich>=12.5.1
 Requires-Dist: stamina==23.2.0
 Requires-Dist: tomli-w
```


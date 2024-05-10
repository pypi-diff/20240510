# Comparing `tmp/hypothesis-6.99.8.tar.gz` & `tmp/hypothesis-6.99.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypothesis-6.99.8.tar", last modified: Mon Mar 18 04:40:42 2024, max compression
+gzip compressed data, was "hypothesis-6.99.9.tar", last modified: Tue Mar 19 06:05:25 2024, max compression
```

## Comparing `hypothesis-6.99.8.tar` & `hypothesis-6.99.9.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 04:40:42.325899 hypothesis-6.99.8/
--rw-r--r--   0 runner    (1001) docker     (127)    17141 2024-03-18 04:40:05.000000 hypothesis-6.99.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-18 04:40:05.000000 hypothesis-6.99.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-03-18 04:40:42.325899 hypothesis-6.99.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-03-18 04:40:05.000000 hypothesis-6.99.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-18 04:40:42.325899 hypothesis-6.99.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-03-18 04:40:05.000000 hypothesis-6.99.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 04:40:42.301900 hypothesis-6.99.8/src/
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/_hypothesis_ftz_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/_hypothesis_globals.py
--rw-r--r--   0 runner    (1001) docker     (127)    19018 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/_hypothesis_pytestplugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 04:40:42.305899 hypothesis-6.99.8/src/hypothesis/
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27369 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/control.py
--rw-r--r--   0 runner    (1001) docker     (127)    73912 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    24822 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 04:40:42.309899 hypothesis-6.99.8/src/hypothesis/extra/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/extra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27678 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/extra/_array_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/extra/_patching.py
--rw-r--r--   0 runner    (1001) docker     (127)    42573 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/extra/array_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12957 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/extra/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11309 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/extra/codemods.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/extra/dateutil.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 04:40:42.309899 hypothesis-6.99.8/src/hypothesis/extra/django/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/extra/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12501 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/extra/django/_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/extra/django/_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/extra/dpcontracts.py
--rw-r--r--   0 runner    (1001) docker     (127)    71783 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/extra/ghostwriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/extra/lark.py
--rw-r--r--   0 runner    (1001) docker     (127)    51264 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/extra/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 04:40:42.309899 hypothesis-6.99.8/src/hypothesis/extra/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/extra/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28443 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/extra/pandas/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/extra/pytestplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/extra/pytz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/extra/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 04:40:42.313899 hypothesis-6.99.8/src/hypothesis/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9752 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/cathetus.py
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/charmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     8803 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 04:40:42.313899 hypothesis-6.99.8/src/hypothesis/internal/conjecture/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/conjecture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/conjecture/choicetree.py
--rw-r--r--   0 runner    (1001) docker     (127)    87693 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/conjecture/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    43861 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/conjecture/datatree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 04:40:42.313899 hypothesis-6.99.8/src/hypothesis/internal/conjecture/dfa/
--rw-r--r--   0 runner    (1001) docker     (127)    23906 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/conjecture/dfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19317 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/conjecture/dfa/lstar.py
--rw-r--r--   0 runner    (1001) docker     (127)    49048 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/conjecture/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/conjecture/floats.py
--rw-r--r--   0 runner    (1001) docker     (127)    12740 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/conjecture/junkdrawer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/conjecture/optimiser.py
--rw-r--r--   0 runner    (1001) docker     (127)    14355 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/conjecture/pareto.py
--rw-r--r--   0 runner    (1001) docker     (127)    65819 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/conjecture/shrinker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 04:40:42.317899 hypothesis-6.99.8/src/hypothesis/internal/conjecture/shrinking/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/conjecture/shrinking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/conjecture/shrinking/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11913 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/conjecture/shrinking/dfas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/conjecture/shrinking/floats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/conjecture/shrinking/integer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1848 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/conjecture/shrinking/learned_dfas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/conjecture/shrinking/lexical.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/conjecture/shrinking/ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)    13534 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/conjecture/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/escalation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/floats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)    10630 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/intervalsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/observability.py
--rw-r--r--   0 runner    (1001) docker     (127)    24899 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/reflection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/scrutineer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/internal/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/provisional.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)    39386 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 04:40:42.317899 hypothesis-6.99.8/src/hypothesis/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 04:40:42.321899 hypothesis-6.99.8/src/hypothesis/strategies/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/_internal/attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12709 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/_internal/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)   100380 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/_internal/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    20343 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/_internal/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/_internal/deferred.py
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/_internal/featureflags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/_internal/flatmapped.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/_internal/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/_internal/ipaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/_internal/lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/_internal/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    20437 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/_internal/numbers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12924 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/_internal/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/_internal/recursive.py
--rw-r--r--   0 runner    (1001) docker     (127)    21665 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/_internal/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/_internal/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)    39946 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/_internal/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)    11860 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/_internal/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)    40227 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/_internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/strategies/_internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 04:40:42.321899 hypothesis-6.99.8/src/hypothesis/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/utils/conventions.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/utils/dynamicvariables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/utils/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 04:40:42.321899 hypothesis-6.99.8/src/hypothesis/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29627 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/vendor/pretty.py
--rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-03-18 04:40:05.000000 hypothesis-6.99.8/src/hypothesis/vendor/tlds-alpha-by-domain.txt
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-18 04:40:42.000000 hypothesis-6.99.8/src/hypothesis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 04:40:42.321899 hypothesis-6.99.8/src/hypothesis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-03-18 04:40:42.000000 hypothesis-6.99.8/src/hypothesis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-03-18 04:40:42.000000 hypothesis-6.99.8/src/hypothesis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 04:40:42.000000 hypothesis-6.99.8/src/hypothesis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-18 04:40:42.000000 hypothesis-6.99.8/src/hypothesis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 04:40:42.000000 hypothesis-6.99.8/src/hypothesis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-03-18 04:40:42.000000 hypothesis-6.99.8/src/hypothesis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-18 04:40:42.000000 hypothesis-6.99.8/src/hypothesis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 04:40:42.321899 hypothesis-6.99.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-03-18 04:40:06.000000 hypothesis-6.99.8/tests/test_annotated_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 06:05:25.741117 hypothesis-6.99.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    17141 2024-03-19 06:04:47.000000 hypothesis-6.99.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-19 06:04:47.000000 hypothesis-6.99.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-03-19 06:05:25.741117 hypothesis-6.99.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-03-19 06:04:47.000000 hypothesis-6.99.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-19 06:05:25.741117 hypothesis-6.99.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-03-19 06:04:47.000000 hypothesis-6.99.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 06:05:25.717117 hypothesis-6.99.9/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/_hypothesis_ftz_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/_hypothesis_globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19018 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/_hypothesis_pytestplugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 06:05:25.721117 hypothesis-6.99.9/src/hypothesis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27369 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73912 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24822 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 06:05:25.725117 hypothesis-6.99.9/src/hypothesis/extra/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/extra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27678 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/extra/_array_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/extra/_patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42573 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/extra/array_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12957 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/extra/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11309 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/extra/codemods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/extra/dateutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 06:05:25.725117 hypothesis-6.99.9/src/hypothesis/extra/django/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/extra/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12501 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/extra/django/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/extra/django/_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/extra/dpcontracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71783 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/extra/ghostwriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/extra/lark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51264 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/extra/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 06:05:25.725117 hypothesis-6.99.9/src/hypothesis/extra/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/extra/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28443 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/extra/pandas/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/extra/pytestplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/extra/pytz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/extra/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 06:05:25.729117 hypothesis-6.99.9/src/hypothesis/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9752 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/cathetus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/charmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8803 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 06:05:25.729117 hypothesis-6.99.9/src/hypothesis/internal/conjecture/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/conjecture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/conjecture/choicetree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90008 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/conjecture/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43861 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/conjecture/datatree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 06:05:25.729117 hypothesis-6.99.9/src/hypothesis/internal/conjecture/dfa/
+-rw-r--r--   0 runner    (1001) docker     (127)    23906 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/conjecture/dfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19317 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/conjecture/dfa/lstar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49048 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/conjecture/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/conjecture/floats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12740 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/conjecture/junkdrawer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/conjecture/optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14355 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/conjecture/pareto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66976 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/conjecture/shrinker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 06:05:25.729117 hypothesis-6.99.9/src/hypothesis/internal/conjecture/shrinking/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/conjecture/shrinking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/conjecture/shrinking/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11913 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/conjecture/shrinking/dfas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/conjecture/shrinking/floats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/conjecture/shrinking/integer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1848 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/conjecture/shrinking/learned_dfas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/conjecture/shrinking/lexical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/conjecture/shrinking/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13534 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/conjecture/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/escalation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/floats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10630 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/intervalsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/observability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24899 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/scrutineer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/internal/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/provisional.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39386 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 06:05:25.729117 hypothesis-6.99.9/src/hypothesis/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 06:05:25.733117 hypothesis-6.99.9/src/hypothesis/strategies/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/_internal/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12709 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/_internal/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100380 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/_internal/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20343 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/_internal/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/_internal/deferred.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/_internal/featureflags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/_internal/flatmapped.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/_internal/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/_internal/ipaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/_internal/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/_internal/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20437 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/_internal/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12924 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/_internal/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/_internal/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21665 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/_internal/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/_internal/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39946 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/_internal/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11860 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/_internal/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40227 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/_internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/strategies/_internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 06:05:25.733117 hypothesis-6.99.9/src/hypothesis/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/utils/conventions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/utils/dynamicvariables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/utils/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 06:05:25.733117 hypothesis-6.99.9/src/hypothesis/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29627 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/vendor/pretty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-03-19 06:04:47.000000 hypothesis-6.99.9/src/hypothesis/vendor/tlds-alpha-by-domain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-19 06:05:25.000000 hypothesis-6.99.9/src/hypothesis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 06:05:25.733117 hypothesis-6.99.9/src/hypothesis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-03-19 06:05:25.000000 hypothesis-6.99.9/src/hypothesis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-03-19 06:05:25.000000 hypothesis-6.99.9/src/hypothesis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 06:05:25.000000 hypothesis-6.99.9/src/hypothesis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-19 06:05:25.000000 hypothesis-6.99.9/src/hypothesis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 06:05:25.000000 hypothesis-6.99.9/src/hypothesis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-03-19 06:05:25.000000 hypothesis-6.99.9/src/hypothesis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-19 06:05:25.000000 hypothesis-6.99.9/src/hypothesis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 06:05:25.733117 hypothesis-6.99.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-03-19 06:04:47.000000 hypothesis-6.99.9/tests/test_annotated_types.py
```

### Comparing `hypothesis-6.99.8/LICENSE.txt` & `hypothesis-6.99.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/PKG-INFO` & `hypothesis-6.99.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis
-Version: 6.99.8
+Version: 6.99.9
 Summary: A library for property-based testing
 Home-page: https://hypothesis.works
 Author: David R. MacIver and Zac Hatfield-Dodds
 Author-email: david@drmaciver.com
 License: MPL-2.0
 Project-URL: Source, https://github.com/HypothesisWorks/hypothesis/tree/master/hypothesis-python
 Project-URL: Changelog, https://hypothesis.readthedocs.io/en/latest/changes.html
```

### Comparing `hypothesis-6.99.8/README.rst` & `hypothesis-6.99.9/README.rst`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/setup.py` & `hypothesis-6.99.9/setup.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/_hypothesis_ftz_detector.py` & `hypothesis-6.99.9/src/_hypothesis_ftz_detector.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/_hypothesis_globals.py` & `hypothesis-6.99.9/src/_hypothesis_globals.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/_hypothesis_pytestplugin.py` & `hypothesis-6.99.9/src/_hypothesis_pytestplugin.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/__init__.py` & `hypothesis-6.99.9/src/hypothesis/__init__.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/_settings.py` & `hypothesis-6.99.9/src/hypothesis/_settings.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/configuration.py` & `hypothesis-6.99.9/src/hypothesis/configuration.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/control.py` & `hypothesis-6.99.9/src/hypothesis/control.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/core.py` & `hypothesis-6.99.9/src/hypothesis/core.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/database.py` & `hypothesis-6.99.9/src/hypothesis/database.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/entry_points.py` & `hypothesis-6.99.9/src/hypothesis/entry_points.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/errors.py` & `hypothesis-6.99.9/src/hypothesis/errors.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/extra/_array_helpers.py` & `hypothesis-6.99.9/src/hypothesis/extra/_array_helpers.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/extra/_patching.py` & `hypothesis-6.99.9/src/hypothesis/extra/_patching.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/extra/array_api.py` & `hypothesis-6.99.9/src/hypothesis/extra/array_api.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/extra/cli.py` & `hypothesis-6.99.9/src/hypothesis/extra/cli.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/extra/codemods.py` & `hypothesis-6.99.9/src/hypothesis/extra/codemods.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/extra/dateutil.py` & `hypothesis-6.99.9/src/hypothesis/extra/dateutil.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/extra/django/__init__.py` & `hypothesis-6.99.9/src/hypothesis/extra/django/__init__.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/extra/django/_fields.py` & `hypothesis-6.99.9/src/hypothesis/extra/django/_fields.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/extra/django/_impl.py` & `hypothesis-6.99.9/src/hypothesis/extra/django/_impl.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/extra/dpcontracts.py` & `hypothesis-6.99.9/src/hypothesis/extra/dpcontracts.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/extra/ghostwriter.py` & `hypothesis-6.99.9/src/hypothesis/extra/ghostwriter.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/extra/lark.py` & `hypothesis-6.99.9/src/hypothesis/extra/lark.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/extra/numpy.py` & `hypothesis-6.99.9/src/hypothesis/extra/numpy.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/extra/pandas/__init__.py` & `hypothesis-6.99.9/src/hypothesis/extra/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/extra/pandas/impl.py` & `hypothesis-6.99.9/src/hypothesis/extra/pandas/impl.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/extra/pytestplugin.py` & `hypothesis-6.99.9/src/hypothesis/extra/pytestplugin.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/extra/pytz.py` & `hypothesis-6.99.9/src/hypothesis/extra/pytz.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/extra/redis.py` & `hypothesis-6.99.9/src/hypothesis/extra/redis.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/cache.py` & `hypothesis-6.99.9/src/hypothesis/internal/cache.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/cathetus.py` & `hypothesis-6.99.9/src/hypothesis/internal/cathetus.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/charmap.py` & `hypothesis-6.99.9/src/hypothesis/internal/charmap.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/compat.py` & `hypothesis-6.99.9/src/hypothesis/internal/compat.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/conjecture/choicetree.py` & `hypothesis-6.99.9/src/hypothesis/internal/conjecture/choicetree.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/conjecture/data.py` & `hypothesis-6.99.9/src/hypothesis/internal/conjecture/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,14 +321,19 @@
 
     @property
     def length(self) -> int:
         """The number of bytes in this example."""
         return self.end - self.start
 
     @property
+    def ir_length(self) -> int:
+        """The number of ir nodes in this example."""
+        return self.ir_end - self.ir_start
+
+    @property
     def children(self) -> "List[Example]":
         """The list of all examples with this as a parent, in increasing index
         order."""
         return [self.owner[i] for i in self.owner.children[self.index]]
 
 
 class ExampleProperty:
@@ -461,15 +466,19 @@
 
     def freeze(self) -> None:
         self.__index_of_labels = None
 
     def record_ir_draw(self, ir_type, value, *, kwargs, was_forced):
         self.trail.append(IR_NODE_RECORD)
         node = IRNode(
-            ir_type=ir_type, value=value, kwargs=kwargs, was_forced=was_forced
+            ir_type=ir_type,
+            value=value,
+            kwargs=kwargs,
+            was_forced=was_forced,
+            index=len(self.ir_nodes),
         )
         self.ir_nodes.append(node)
 
     def start_example(self, label: int) -> None:
         assert self.__index_of_labels is not None
         try:
             i = self.__index_of_labels[label]
@@ -946,26 +955,72 @@
 
 @attr.s(slots=True, repr=False, eq=False)
 class IRNode:
     ir_type: IRTypeName = attr.ib()
     value: IRType = attr.ib()
     kwargs: IRKWargsType = attr.ib()
     was_forced: bool = attr.ib()
+    index: Optional[int] = attr.ib(default=None)
 
     def copy(self, *, with_value: IRType) -> "IRNode":
         # we may want to allow this combination in the future, but for now it's
         # a footgun.
         assert not self.was_forced, "modifying a forced node doesn't make sense"
+        # explicitly not copying index. node indices are only assigned via
+        # ExampleRecord. This prevents footguns with relying on stale indices
+        # after copying.
         return IRNode(
             ir_type=self.ir_type,
             value=with_value,
             kwargs=self.kwargs,
             was_forced=self.was_forced,
         )
 
+    @property
+    def trivial(self):
+        """
+        A node is trivial if it cannot be simplified any further. This does not
+        mean that modifying a trivial node can't produce simpler test cases when
+        viewing the tree as a whole. Just that when viewing this node in
+        isolation, this is the simplest the node can get.
+        """
+        if self.was_forced:
+            return True
+
+        if self.ir_type == "integer":
+            shrink_towards = self.kwargs["shrink_towards"]
+            min_value = self.kwargs["min_value"]
+            max_value = self.kwargs["max_value"]
+
+            if min_value is not None:
+                shrink_towards = max(min_value, shrink_towards)
+            if max_value is not None:
+                shrink_towards = min(max_value, shrink_towards)
+
+            return self.value == shrink_towards
+        if self.ir_type == "float":
+            # floats shrink "like integers" (for now, anyway), except shrink_towards
+            # is not configurable and is always 0.
+            shrink_towards = 0
+            shrink_towards = max(self.kwargs["min_value"], shrink_towards)
+            shrink_towards = min(self.kwargs["max_value"], shrink_towards)
+
+            return ir_value_equal("float", self.value, shrink_towards)
+        if self.ir_type == "boolean":
+            return self.value is False
+        if self.ir_type == "string":
+            # smallest size and contains only the smallest-in-shrink-order character.
+            minimal_char = self.kwargs["intervals"].char_in_shrink_order(0)
+            return self.value == (minimal_char * self.kwargs["min_size"])
+        if self.ir_type == "bytes":
+            # smallest size and all-zero value.
+            return len(self.value) == self.kwargs["size"] and not any(self.value)
+
+        raise NotImplementedError(f"unhandled ir_type {self.ir_type}")
+
     def __eq__(self, other):
         if not isinstance(other, IRNode):
             return NotImplemented
 
         return (
             self.ir_type == other.ir_type
             and ir_value_equal(self.ir_type, self.value, other.value)
```

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/conjecture/datatree.py` & `hypothesis-6.99.9/src/hypothesis/internal/conjecture/datatree.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/conjecture/dfa/__init__.py` & `hypothesis-6.99.9/src/hypothesis/internal/conjecture/dfa/__init__.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/conjecture/dfa/lstar.py` & `hypothesis-6.99.9/src/hypothesis/internal/conjecture/dfa/lstar.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/conjecture/engine.py` & `hypothesis-6.99.9/src/hypothesis/internal/conjecture/engine.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/conjecture/floats.py` & `hypothesis-6.99.9/src/hypothesis/internal/conjecture/floats.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/conjecture/junkdrawer.py` & `hypothesis-6.99.9/src/hypothesis/internal/conjecture/junkdrawer.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/conjecture/optimiser.py` & `hypothesis-6.99.9/src/hypothesis/internal/conjecture/optimiser.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/conjecture/pareto.py` & `hypothesis-6.99.9/src/hypothesis/internal/conjecture/pareto.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/conjecture/shrinker.py` & `hypothesis-6.99.9/src/hypothesis/internal/conjecture/shrinker.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,21 @@
 
 from hypothesis.internal.compat import int_from_bytes, int_to_bytes
 from hypothesis.internal.conjecture.choicetree import (
     ChoiceTree,
     prefix_selection_order,
     random_selection_order,
 )
-from hypothesis.internal.conjecture.data import ConjectureData, ConjectureResult, Status
+from hypothesis.internal.conjecture.data import (
+    ConjectureData,
+    ConjectureResult,
+    Status,
+    bits_to_bytes,
+    ir_value_permitted,
+)
 from hypothesis.internal.conjecture.dfa import ConcreteDFA
 from hypothesis.internal.conjecture.floats import is_simple
 from hypothesis.internal.conjecture.junkdrawer import (
     binary_search,
     find_integer,
     replace_all,
 )
@@ -373,15 +379,14 @@
     def calls(self):
         """Return the number of calls that have been made to the underlying
         test function."""
         return self.engine.call_count
 
     def consider_new_tree(self, tree):
         data = self.engine.ir_tree_to_data(tree)
-
         return self.consider_new_buffer(data.buffer)
 
     def consider_new_buffer(self, buffer):
         """Returns True if after running this buffer the result would be
         the current shrink_target."""
         buffer = bytes(buffer)
         return buffer.startswith(self.buffer) or self.incorporate_new_buffer(buffer)
@@ -821,44 +826,42 @@
         """
 
         label = chooser.choose(
             self.distinct_labels, lambda l: len(self.examples_by_label[l]) >= 2
         )
 
         ls = self.examples_by_label[label]
-
         i = chooser.choose(range(len(ls) - 1))
-
         ancestor = ls[i]
 
-        if i + 1 == len(ls) or ls[i + 1].start >= ancestor.end:
+        if i + 1 == len(ls) or ls[i + 1].ir_start >= ancestor.ir_end:
             return
 
         @self.cached(label, i)
         def descendants():
             lo = i + 1
             hi = len(ls)
             while lo + 1 < hi:
                 mid = (lo + hi) // 2
-                if ls[mid].start >= ancestor.end:
+                if ls[mid].ir_start >= ancestor.ir_end:
                     hi = mid
                 else:
                     lo = mid
-            return [t for t in ls[i + 1 : hi] if t.length < ancestor.length]
+            return [t for t in ls[i + 1 : hi] if t.ir_length < ancestor.ir_length]
 
-        descendant = chooser.choose(descendants, lambda ex: ex.length > 0)
+        descendant = chooser.choose(descendants, lambda ex: ex.ir_length > 0)
 
-        assert ancestor.start <= descendant.start
-        assert ancestor.end >= descendant.end
-        assert descendant.length < ancestor.length
-
-        self.incorporate_new_buffer(
-            self.buffer[: ancestor.start]
-            + self.buffer[descendant.start : descendant.end]
-            + self.buffer[ancestor.end :]
+        assert ancestor.ir_start <= descendant.ir_start
+        assert ancestor.ir_end >= descendant.ir_end
+        assert descendant.ir_length < ancestor.ir_length
+
+        self.consider_new_tree(
+            self.nodes[: ancestor.ir_start]
+            + self.nodes[descendant.ir_start : descendant.ir_end]
+            + self.nodes[ancestor.ir_end :]
         )
 
     def lower_common_block_offset(self):
         """Sometimes we find ourselves in a situation where changes to one part
         of the byte stream unlock changes to other parts. Sometimes this is
         good, but sometimes this can cause us to exhibit exponential slow
         downs!
@@ -1217,64 +1220,87 @@
             lambda node: node.ir_type == "float" and not node.was_forced
             # avoid shrinking integer-valued floats. In our current ordering, these
             # are already simpler than all other floats, so it's better to shrink
             # them in other passes.
             and not is_simple(node.value),
         )
 
-        i = self.nodes.index(node)
         # the Float shrinker was only built to handle positive floats. We'll
         # shrink the positive portion and reapply the sign after, which is
         # equivalent to this shrinker's previous behavior. We'll want to refactor
         # Float to handle negative floats natively in the future. (likely a pure
         # code quality change, with no shrinking impact.)
         sign = math.copysign(1.0, node.value)
         Float.shrink(
             abs(node.value),
             lambda val: self.consider_new_tree(
-                self.nodes[:i]
+                self.nodes[: node.index]
                 + [node.copy(with_value=sign * val)]
-                + self.nodes[i + 1 :]
+                + self.nodes[node.index + 1 :]
             ),
             random=self.random,
             node=node,
         )
 
     @defines_shrink_pass()
     def redistribute_block_pairs(self, chooser):
         """If there is a sum of generated integers that we need their sum
         to exceed some bound, lowering one of them requires raising the
         other. This pass enables that."""
 
-        block = chooser.choose(self.blocks, lambda b: not b.all_zero)
+        node = chooser.choose(
+            self.nodes, lambda node: node.ir_type == "integer" and not node.trivial
+        )
 
-        for j in range(block.index + 1, len(self.blocks)):
-            next_block = self.blocks[j]
-            if next_block.length == block.length:
+        # The preconditions for this pass are that the two integer draws are only
+        # separated by non-integer nodes, and have the same size value in bytes.
+        #
+        # This isn't particularly principled. For instance, this wouldn't reduce
+        # e.g. @given(integers(), integers(), integers()) where the sum property
+        # involves the first and last integers.
+        #
+        # A better approach may be choosing *two* such integer nodes arbitrarily
+        # from the list, instead of conditionally scanning forward.
+
+        for j in range(node.index + 1, len(self.nodes)):
+            next_node = self.nodes[j]
+            if next_node.ir_type == "integer" and bits_to_bytes(
+                node.value.bit_length()
+            ) == bits_to_bytes(next_node.value.bit_length()):
                 break
         else:
             return
 
-        buffer = self.buffer
+        if next_node.was_forced:
+            # avoid modifying a forced node. Note that it's fine for next_node
+            # to be trivial, because we're going to explicitly make it *not*
+            # trivial by adding to its value.
+            return
 
-        m = int_from_bytes(buffer[block.start : block.end])
-        n = int_from_bytes(buffer[next_block.start : next_block.end])
+        m = node.value
+        n = next_node.value
 
         def boost(k):
             if k > m:
                 return False
-            attempt = bytearray(buffer)
-            attempt[block.start : block.end] = int_to_bytes(m - k, block.length)
-            try:
-                attempt[next_block.start : next_block.end] = int_to_bytes(
-                    n + k, next_block.length
-                )
-            except OverflowError:
+
+            node_value = m - k
+            next_node_value = n + k
+            if (not ir_value_permitted(node_value, "integer", node.kwargs)) or (
+                not ir_value_permitted(next_node_value, "integer", next_node.kwargs)
+            ):
                 return False
-            return self.consider_new_buffer(attempt)
+
+            return self.consider_new_tree(
+                self.nodes[: node.index]
+                + [node.copy(with_value=node_value)]
+                + self.nodes[node.index + 1 : next_node.index]
+                + [next_node.copy(with_value=next_node_value)]
+                + self.nodes[next_node.index + 1 :]
+            )
 
         find_integer(boost)
 
     @defines_shrink_pass()
     def lower_blocks_together(self, chooser):
         block = chooser.choose(self.blocks, lambda b: not b.all_zero)
```

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/conjecture/shrinking/__init__.py` & `hypothesis-6.99.9/src/hypothesis/internal/conjecture/shrinking/__init__.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/conjecture/shrinking/common.py` & `hypothesis-6.99.9/src/hypothesis/internal/conjecture/shrinking/common.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/conjecture/shrinking/dfas.py` & `hypothesis-6.99.9/src/hypothesis/internal/conjecture/shrinking/dfas.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/conjecture/shrinking/floats.py` & `hypothesis-6.99.9/src/hypothesis/internal/conjecture/shrinking/floats.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/conjecture/shrinking/integer.py` & `hypothesis-6.99.9/src/hypothesis/internal/conjecture/shrinking/integer.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/conjecture/shrinking/learned_dfas.py` & `hypothesis-6.99.9/src/hypothesis/internal/conjecture/shrinking/learned_dfas.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/conjecture/shrinking/lexical.py` & `hypothesis-6.99.9/src/hypothesis/internal/conjecture/shrinking/lexical.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/conjecture/shrinking/ordering.py` & `hypothesis-6.99.9/src/hypothesis/internal/conjecture/shrinking/ordering.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/conjecture/utils.py` & `hypothesis-6.99.9/src/hypothesis/internal/conjecture/utils.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/coverage.py` & `hypothesis-6.99.9/src/hypothesis/internal/coverage.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/detection.py` & `hypothesis-6.99.9/src/hypothesis/internal/detection.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/entropy.py` & `hypothesis-6.99.9/src/hypothesis/internal/entropy.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/escalation.py` & `hypothesis-6.99.9/src/hypothesis/internal/escalation.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/filtering.py` & `hypothesis-6.99.9/src/hypothesis/internal/filtering.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/floats.py` & `hypothesis-6.99.9/src/hypothesis/internal/floats.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/healthcheck.py` & `hypothesis-6.99.9/src/hypothesis/internal/healthcheck.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/intervalsets.py` & `hypothesis-6.99.9/src/hypothesis/internal/intervalsets.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/observability.py` & `hypothesis-6.99.9/src/hypothesis/internal/observability.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/reflection.py` & `hypothesis-6.99.9/src/hypothesis/internal/reflection.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/scrutineer.py` & `hypothesis-6.99.9/src/hypothesis/internal/scrutineer.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/internal/validation.py` & `hypothesis-6.99.9/src/hypothesis/internal/validation.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/provisional.py` & `hypothesis-6.99.9/src/hypothesis/provisional.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/reporting.py` & `hypothesis-6.99.9/src/hypothesis/reporting.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/stateful.py` & `hypothesis-6.99.9/src/hypothesis/stateful.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/statistics.py` & `hypothesis-6.99.9/src/hypothesis/statistics.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/__init__.py` & `hypothesis-6.99.9/src/hypothesis/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/_internal/__init__.py` & `hypothesis-6.99.9/src/hypothesis/strategies/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/_internal/attrs.py` & `hypothesis-6.99.9/src/hypothesis/strategies/_internal/attrs.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/_internal/collections.py` & `hypothesis-6.99.9/src/hypothesis/strategies/_internal/collections.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/_internal/core.py` & `hypothesis-6.99.9/src/hypothesis/strategies/_internal/core.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/_internal/datetime.py` & `hypothesis-6.99.9/src/hypothesis/strategies/_internal/datetime.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/_internal/deferred.py` & `hypothesis-6.99.9/src/hypothesis/strategies/_internal/deferred.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/_internal/featureflags.py` & `hypothesis-6.99.9/src/hypothesis/strategies/_internal/featureflags.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/_internal/flatmapped.py` & `hypothesis-6.99.9/src/hypothesis/strategies/_internal/flatmapped.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/_internal/functions.py` & `hypothesis-6.99.9/src/hypothesis/strategies/_internal/functions.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/_internal/ipaddress.py` & `hypothesis-6.99.9/src/hypothesis/strategies/_internal/ipaddress.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/_internal/lazy.py` & `hypothesis-6.99.9/src/hypothesis/strategies/_internal/lazy.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/_internal/misc.py` & `hypothesis-6.99.9/src/hypothesis/strategies/_internal/misc.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/_internal/numbers.py` & `hypothesis-6.99.9/src/hypothesis/strategies/_internal/numbers.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/_internal/random.py` & `hypothesis-6.99.9/src/hypothesis/strategies/_internal/random.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/_internal/recursive.py` & `hypothesis-6.99.9/src/hypothesis/strategies/_internal/recursive.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/_internal/regex.py` & `hypothesis-6.99.9/src/hypothesis/strategies/_internal/regex.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/_internal/shared.py` & `hypothesis-6.99.9/src/hypothesis/strategies/_internal/shared.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/_internal/strategies.py` & `hypothesis-6.99.9/src/hypothesis/strategies/_internal/strategies.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/_internal/strings.py` & `hypothesis-6.99.9/src/hypothesis/strategies/_internal/strings.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/_internal/types.py` & `hypothesis-6.99.9/src/hypothesis/strategies/_internal/types.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/strategies/_internal/utils.py` & `hypothesis-6.99.9/src/hypothesis/strategies/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/utils/__init__.py` & `hypothesis-6.99.9/src/hypothesis/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/utils/conventions.py` & `hypothesis-6.99.9/src/hypothesis/utils/conventions.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/utils/dynamicvariables.py` & `hypothesis-6.99.9/src/hypothesis/utils/dynamicvariables.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/utils/terminal.py` & `hypothesis-6.99.9/src/hypothesis/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/vendor/pretty.py` & `hypothesis-6.99.9/src/hypothesis/vendor/pretty.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis/vendor/tlds-alpha-by-domain.txt` & `hypothesis-6.99.9/src/hypothesis/vendor/tlds-alpha-by-domain.txt`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis.egg-info/PKG-INFO` & `hypothesis-6.99.9/src/hypothesis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis
-Version: 6.99.8
+Version: 6.99.9
 Summary: A library for property-based testing
 Home-page: https://hypothesis.works
 Author: David R. MacIver and Zac Hatfield-Dodds
 Author-email: david@drmaciver.com
 License: MPL-2.0
 Project-URL: Source, https://github.com/HypothesisWorks/hypothesis/tree/master/hypothesis-python
 Project-URL: Changelog, https://hypothesis.readthedocs.io/en/latest/changes.html
```

### Comparing `hypothesis-6.99.8/src/hypothesis.egg-info/SOURCES.txt` & `hypothesis-6.99.9/src/hypothesis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/src/hypothesis.egg-info/requires.txt` & `hypothesis-6.99.9/src/hypothesis.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hypothesis-6.99.8/tests/test_annotated_types.py` & `hypothesis-6.99.9/tests/test_annotated_types.py`

 * *Files identical despite different names*


# Comparing `tmp/mosaic_widget-0.7.1.tar.gz` & `tmp/mosaic_widget-0.8.0.tar.gz`

## Comparing `mosaic_widget-0.7.1.tar` & `mosaic_widget-0.8.0.tar`

### file list

```diff
@@ -1,1419 +1,12 @@
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/package.json
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/tsconfig.json
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/vite.config.mjs
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/mosaic_widget/__init__.py
--rw-r--r--   0        0        0  1222101 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/mosaic_widget/static/index.js
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/mosaic_widget/static/style.css
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/command-line-args/LICENSE
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/command-line-args/README.md
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/command-line-args/index.d.ts
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/command-line-args/package.json
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/LICENSE
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/README.md
--rw-r--r--   0        0        0    41643 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/assert.d.ts
--rw-r--r--   0        0        0    22740 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/async_hooks.d.ts
--rw-r--r--   0        0        0   107501 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/buffer.d.ts
--rw-r--r--   0        0        0    69241 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/child_process.d.ts
--rw-r--r--   0        0        0    20851 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/cluster.d.ts
--rw-r--r--   0        0        0    18476 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/console.d.ts
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/constants.d.ts
--rw-r--r--   0        0        0   190746 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/crypto.d.ts
--rw-r--r--   0        0        0    27756 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/dgram.d.ts
--rw-r--r--   0        0        0    23158 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/diagnostics_channel.d.ts
--rw-r--r--   0        0        0    31241 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/dns.d.ts
--rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/dom-events.d.ts
--rw-r--r--   0        0        0     7820 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/domain.d.ts
--rw-r--r--   0        0        0    41792 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/events.d.ts
--rw-r--r--   0        0        0   187145 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/fs.d.ts
--rw-r--r--   0        0        0    14300 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/globals.d.ts
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/globals.global.d.ts
--rw-r--r--   0        0        0    84276 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/http.d.ts
--rw-r--r--   0        0        0   116844 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/http2.d.ts
--rw-r--r--   0        0        0    24891 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/https.d.ts
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/index.d.ts
--rw-r--r--   0        0        0   125362 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/inspector.d.ts
--rw-r--r--   0        0        0    13783 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/module.d.ts
--rw-r--r--   0        0        0    43290 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/net.d.ts
--rw-r--r--   0        0        0    18073 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/os.d.ts
--rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/package.json
--rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/path.d.ts
--rw-r--r--   0        0        0    24508 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/perf_hooks.d.ts
--rw-r--r--   0        0        0    76213 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/process.d.ts
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/punycode.d.ts
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/querystring.d.ts
--rw-r--r--   0        0        0    22983 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/readline.d.ts
--rw-r--r--   0        0        0    19536 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/repl.d.ts
--rw-r--r--   0        0        0    82656 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/stream.d.ts
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/string_decoder.d.ts
--rw-r--r--   0        0        0    59836 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/test.d.ts
--rw-r--r--   0        0        0    12279 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/timers.d.ts
--rw-r--r--   0        0        0    56857 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/tls.d.ts
--rw-r--r--   0        0        0     7928 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/trace_events.d.ts
--rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/tty.d.ts
--rw-r--r--   0        0        0    41139 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/url.d.ts
--rw-r--r--   0        0        0    85386 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/util.d.ts
--rw-r--r--   0        0        0    32211 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/v8.d.ts
--rw-r--r--   0        0        0    39089 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/vm.d.ts
--rw-r--r--   0        0        0     7837 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/wasi.d.ts
--rw-r--r--   0        0        0    33962 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/worker_threads.d.ts
--rw-r--r--   0        0        0    19551 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/zlib.d.ts
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/assert/strict.d.ts
--rw-r--r--   0        0        0    17506 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/dns/promises.d.ts
--rw-r--r--   0        0        0    54387 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/fs/promises.d.ts
--rw-r--r--   0        0        0     6117 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/readline/promises.d.ts
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/stream/consumers.d.ts
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/stream/promises.d.ts
--rw-r--r--   0        0        0    14998 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/stream/web.d.ts
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/timers/promises.d.ts
--rw-r--r--   0        0        0    41643 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/assert.d.ts
--rw-r--r--   0        0        0    22740 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/async_hooks.d.ts
--rw-r--r--   0        0        0   107501 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/buffer.d.ts
--rw-r--r--   0        0        0    69191 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/child_process.d.ts
--rw-r--r--   0        0        0    20851 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/cluster.d.ts
--rw-r--r--   0        0        0    18476 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/console.d.ts
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/constants.d.ts
--rw-r--r--   0        0        0   190746 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/crypto.d.ts
--rw-r--r--   0        0        0    27756 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/dgram.d.ts
--rw-r--r--   0        0        0    23158 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/diagnostics_channel.d.ts
--rw-r--r--   0        0        0    31241 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/dns.d.ts
--rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/dom-events.d.ts
--rw-r--r--   0        0        0     7820 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/domain.d.ts
--rw-r--r--   0        0        0    41792 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/events.d.ts
--rw-r--r--   0        0        0   187145 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/fs.d.ts
--rw-r--r--   0        0        0    14300 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/globals.d.ts
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/globals.global.d.ts
--rw-r--r--   0        0        0    84276 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/http.d.ts
--rw-r--r--   0        0        0   116844 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/http2.d.ts
--rw-r--r--   0        0        0    24891 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/https.d.ts
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/index.d.ts
--rw-r--r--   0        0        0   125362 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/inspector.d.ts
--rw-r--r--   0        0        0    13783 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/module.d.ts
--rw-r--r--   0        0        0    43290 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/net.d.ts
--rw-r--r--   0        0        0    18073 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/os.d.ts
--rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/path.d.ts
--rw-r--r--   0        0        0    24508 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/perf_hooks.d.ts
--rw-r--r--   0        0        0    76213 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/process.d.ts
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/punycode.d.ts
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/querystring.d.ts
--rw-r--r--   0        0        0    22983 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/readline.d.ts
--rw-r--r--   0        0        0    19536 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/repl.d.ts
--rw-r--r--   0        0        0    82656 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/stream.d.ts
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/string_decoder.d.ts
--rw-r--r--   0        0        0    59836 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/test.d.ts
--rw-r--r--   0        0        0    12279 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/timers.d.ts
--rw-r--r--   0        0        0    56857 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/tls.d.ts
--rw-r--r--   0        0        0     7928 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/trace_events.d.ts
--rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/tty.d.ts
--rw-r--r--   0        0        0    41139 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/url.d.ts
--rw-r--r--   0        0        0    85386 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/util.d.ts
--rw-r--r--   0        0        0    32211 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/v8.d.ts
--rw-r--r--   0        0        0    39089 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/vm.d.ts
--rw-r--r--   0        0        0     7837 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/wasi.d.ts
--rw-r--r--   0        0        0    33962 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/worker_threads.d.ts
--rw-r--r--   0        0        0    19551 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/zlib.d.ts
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/assert/strict.d.ts
--rw-r--r--   0        0        0    17506 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/dns/promises.d.ts
--rw-r--r--   0        0        0    54387 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/fs/promises.d.ts
--rw-r--r--   0        0        0     6117 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/readline/promises.d.ts
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/stream/consumers.d.ts
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/stream/promises.d.ts
--rw-r--r--   0        0        0    14998 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/stream/web.d.ts
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/@types/node/ts4.8/timers/promises.d.ts
--rw-r--r--   0        0        0    13095 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.d.mts
--rw-r--r--   0        0        0    13095 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.d.ts
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.d.ts.map
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.dom.d.mts
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.dom.d.ts
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.dom.d.ts.map
--rw-r--r--   0        0        0    24331 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.dom.js
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.dom.js.map
--rw-r--r--   0        0        0     4210 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.dom.mjs
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.dom.mjs.map
--rw-r--r--   0        0        0   172372 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.es2015.min.js
--rw-r--r--   0        0        0   479133 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.es2015.min.js.map
--rw-r--r--   0        0        0   162685 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.esnext.min.js
--rw-r--r--   0        0        0   453168 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.esnext.min.js.map
--rw-r--r--   0        0        0    39276 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.externs.es2015.min.js
--rw-r--r--   0        0        0    39276 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.externs.esnext.min.js
--rw-r--r--   0        0        0    25827 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.js
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.js.map
--rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.mjs
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.mjs.map
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.node.d.mts
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.node.d.ts
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.node.d.ts.map
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.node.js
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.node.js.map
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.node.mjs
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/Arrow.node.mjs.map
--rw-r--r--   0        0        0   110091 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/LICENSE.txt
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/NOTICE.txt
--rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/README.md
--rw-r--r--   0        0        0    10022 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder.d.mts
--rw-r--r--   0        0        0    10022 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder.d.ts
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder.d.ts.map
--rw-r--r--   0        0        0    13849 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder.js
--rw-r--r--   0        0        0     7768 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder.js.map
--rw-r--r--   0        0        0    13534 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder.mjs
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder.mjs.map
--rw-r--r--   0        0        0     9144 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/data.d.mts
--rw-r--r--   0        0        0     9144 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/data.d.ts
--rw-r--r--   0        0        0    10238 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/data.d.ts.map
--rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/data.js
--rw-r--r--   0        0        0    22025 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/data.js.map
--rw-r--r--   0        0        0    19331 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/data.mjs
--rw-r--r--   0        0        0    21939 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/data.mjs.map
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/enum.d.mts
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/enum.d.ts
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/enum.d.ts.map
--rw-r--r--   0        0        0     6848 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/enum.js
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/enum.js.map
--rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/enum.mjs
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/enum.mjs.map
--rw-r--r--   0        0        0     7041 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/factories.d.mts
--rw-r--r--   0        0        0     7041 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/factories.d.ts
--rw-r--r--   0        0        0     4171 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/factories.d.ts.map
--rw-r--r--   0        0        0    11323 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/factories.js
--rw-r--r--   0        0        0     6601 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/factories.js.map
--rw-r--r--   0        0        0    10747 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/factories.mjs
--rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/factories.mjs.map
--rw-r--r--   0        0        0    16727 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/interfaces.d.mts
--rw-r--r--   0        0        0    16727 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/interfaces.d.ts
--rw-r--r--   0        0        0    18946 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/interfaces.d.ts.map
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/interfaces.js
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/interfaces.js.map
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/interfaces.mjs
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/interfaces.mjs.map
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/package.json
--rw-r--r--   0        0        0     5219 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/recordbatch.d.mts
--rw-r--r--   0        0        0     5219 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/recordbatch.d.ts
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/recordbatch.d.ts.map
--rw-r--r--   0        0        0    12781 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/recordbatch.js
--rw-r--r--   0        0        0     9297 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/recordbatch.js.map
--rw-r--r--   0        0        0    12188 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/recordbatch.mjs
--rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/recordbatch.mjs.map
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/schema.d.mts
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/schema.d.ts
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/schema.d.ts.map
--rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/schema.js
--rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/schema.js.map
--rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/schema.mjs
--rw-r--r--   0        0        0     5772 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/schema.mjs.map
--rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/table.d.mts
--rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/table.d.ts
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/table.d.ts.map
--rw-r--r--   0        0        0    13927 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/table.js
--rw-r--r--   0        0        0    10424 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/table.js.map
--rw-r--r--   0        0        0    13280 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/table.mjs
--rw-r--r--   0        0        0    10887 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/table.mjs.map
--rw-r--r--   0        0        0    20874 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/type.d.mts
--rw-r--r--   0        0        0    20874 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/type.d.ts
--rw-r--r--   0        0        0    20212 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/type.d.ts.map
--rw-r--r--   0        0        0    24105 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/type.js
--rw-r--r--   0        0        0    22409 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/type.js.map
--rw-r--r--   0        0        0    20981 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/type.mjs
--rw-r--r--   0        0        0    22287 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/type.mjs.map
--rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/vector.d.mts
--rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/vector.d.ts
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/vector.d.ts.map
--rw-r--r--   0        0        0    16228 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/vector.js
--rw-r--r--   0        0        0    11788 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/vector.js.map
--rw-r--r--   0        0        0    15702 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/vector.mjs
--rw-r--r--   0        0        0    12064 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/vector.mjs.map
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor.d.mts
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor.d.ts
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor.d.ts.map
--rw-r--r--   0        0        0    15273 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor.js
--rw-r--r--   0        0        0    12591 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor.js.map
--rw-r--r--   0        0        0    13711 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor.mjs
--rw-r--r--   0        0        0    12664 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor.mjs.map
--rwxr-xr-x   0        0        0    15106 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/bin/arrow2csv.js
--rwxr-xr-x   0        0        0    14902 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/bin/arrow2csv.mjs
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/binary.d.mts
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/binary.d.ts
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/binary.d.ts.map
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/binary.js
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/binary.js.map
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/binary.mjs
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/binary.mjs.map
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/bool.d.mts
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/bool.d.ts
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/bool.d.ts.map
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/bool.js
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/bool.js.map
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/bool.mjs
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/bool.mjs.map
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/buffer.d.mts
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/buffer.d.ts
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/buffer.d.ts.map
--rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/buffer.js
--rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/buffer.js.map
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/buffer.mjs
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/buffer.mjs.map
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/date.d.mts
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/date.d.ts
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/date.d.ts.map
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/date.js
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/date.js.map
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/date.mjs
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/date.mjs.map
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/decimal.d.mts
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/decimal.d.ts
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/decimal.d.ts.map
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/decimal.js
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/decimal.js.map
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/decimal.mjs
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/decimal.mjs.map
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/dictionary.d.mts
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/dictionary.d.ts
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/dictionary.d.ts.map
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/dictionary.js
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/dictionary.js.map
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/dictionary.mjs
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/dictionary.mjs.map
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/duration.d.mts
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/duration.d.ts
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/duration.d.ts.map
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/duration.js
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/duration.js.map
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/duration.mjs
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/duration.mjs.map
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/fixedsizebinary.d.mts
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/fixedsizebinary.d.ts
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/fixedsizebinary.d.ts.map
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/fixedsizebinary.js
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/fixedsizebinary.js.map
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/fixedsizebinary.mjs
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/fixedsizebinary.mjs.map
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/fixedsizelist.d.mts
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/fixedsizelist.d.ts
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/fixedsizelist.d.ts.map
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/fixedsizelist.js
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/fixedsizelist.js.map
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/fixedsizelist.mjs
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/fixedsizelist.mjs.map
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/float.d.mts
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/float.d.ts
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/float.d.ts.map
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/float.js
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/float.js.map
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/float.mjs
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/float.mjs.map
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/int.d.mts
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/int.d.ts
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/int.d.ts.map
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/int.js
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/int.js.map
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/int.mjs
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/int.mjs.map
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/interval.d.mts
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/interval.d.ts
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/interval.d.ts.map
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/interval.js
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/interval.js.map
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/interval.mjs
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/interval.mjs.map
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/largebinary.d.mts
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/largebinary.d.ts
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/largebinary.d.ts.map
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/largebinary.js
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/largebinary.js.map
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/largebinary.mjs
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/largebinary.mjs.map
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/largeutf8.d.mts
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/largeutf8.d.ts
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/largeutf8.d.ts.map
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/largeutf8.js
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/largeutf8.js.map
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/largeutf8.mjs
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/largeutf8.mjs.map
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/list.d.mts
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/list.d.ts
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/list.d.ts.map
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/list.js
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/list.js.map
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/list.mjs
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/list.mjs.map
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/map.d.mts
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/map.d.ts
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/map.d.ts.map
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/map.js
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/map.js.map
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/map.mjs
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/map.mjs.map
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/null.d.mts
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/null.d.ts
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/null.d.ts.map
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/null.js
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/null.js.map
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/null.mjs
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/null.mjs.map
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/struct.d.mts
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/struct.d.ts
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/struct.d.ts.map
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/struct.js
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/struct.js.map
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/struct.mjs
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/struct.mjs.map
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/time.d.mts
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/time.d.ts
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/time.d.ts.map
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/time.js
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/time.js.map
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/time.mjs
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/time.mjs.map
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/timestamp.d.mts
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/timestamp.d.ts
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/timestamp.d.ts.map
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/timestamp.js
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/timestamp.js.map
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/timestamp.mjs
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/timestamp.mjs.map
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/union.d.mts
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/union.d.ts
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/union.d.ts.map
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/union.js
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/union.js.map
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/union.mjs
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/union.mjs.map
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/utf8.d.mts
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/utf8.d.ts
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/utf8.d.ts.map
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/utf8.js
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/utf8.js.map
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/utf8.mjs
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/utf8.mjs.map
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/valid.d.mts
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/valid.d.ts
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/valid.d.ts.map
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/valid.js
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/valid.js.map
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/valid.mjs
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/builder/valid.mjs.map
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/File_generated.d.mts
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/File_generated.d.ts
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/File_generated.d.ts.map
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/File_generated.js
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/File_generated.js.map
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/File_generated.mjs
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/File_generated.mjs.map
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/Message_generated.d.mts
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/Message_generated.d.ts
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/Message_generated.d.ts.map
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/Message_generated.js
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/Message_generated.js.map
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/Message_generated.mjs
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/Message_generated.mjs.map
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/Schema_generated.d.mts
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/Schema_generated.d.ts
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/Schema_generated.d.ts.map
--rw-r--r--   0        0        0     6818 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/Schema_generated.js
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/Schema_generated.js.map
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/Schema_generated.mjs
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/Schema_generated.mjs.map
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/SparseTensor_generated.d.mts
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/SparseTensor_generated.d.ts
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/SparseTensor_generated.d.ts.map
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/SparseTensor_generated.js
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/SparseTensor_generated.js.map
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/SparseTensor_generated.mjs
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/SparseTensor_generated.mjs.map
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/Tensor_generated.d.mts
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/Tensor_generated.d.ts
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/Tensor_generated.d.ts.map
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/Tensor_generated.js
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/Tensor_generated.js.map
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/Tensor_generated.mjs
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/Tensor_generated.mjs.map
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/binary.d.mts
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/binary.d.ts
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/binary.d.ts.map
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/binary.js
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/binary.js.map
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/binary.mjs
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/binary.mjs.map
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/block.d.mts
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/block.d.ts
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/block.d.ts.map
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/block.js
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/block.js.map
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/block.mjs
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/block.mjs.map
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/body-compression-method.d.mts
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/body-compression-method.d.ts
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/body-compression-method.d.ts.map
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/body-compression-method.js
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/body-compression-method.js.map
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/body-compression-method.mjs
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/body-compression-method.mjs.map
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/body-compression.d.mts
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/body-compression.d.ts
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/body-compression.d.ts.map
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/body-compression.js
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/body-compression.js.map
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/body-compression.mjs
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/body-compression.mjs.map
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/bool.d.mts
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/bool.d.ts
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/bool.d.ts.map
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/bool.js
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/bool.js.map
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/bool.mjs
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/bool.mjs.map
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/buffer.d.mts
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/buffer.d.ts
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/buffer.d.ts.map
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/buffer.js
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/buffer.js.map
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/buffer.mjs
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/buffer.mjs.map
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/compression-type.d.mts
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/compression-type.d.ts
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/compression-type.d.ts.map
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/compression-type.js
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/compression-type.js.map
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/compression-type.mjs
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/compression-type.mjs.map
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/date-unit.d.mts
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/date-unit.d.ts
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/date-unit.d.ts.map
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/date-unit.js
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/date-unit.js.map
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/date-unit.mjs
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/date-unit.mjs.map
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/date.d.mts
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/date.d.ts
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/date.d.ts.map
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/date.js
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/date.js.map
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/date.mjs
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/date.mjs.map
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/decimal.d.mts
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/decimal.d.ts
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/decimal.d.ts.map
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/decimal.js
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/decimal.js.map
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/decimal.mjs
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/decimal.mjs.map
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/dictionary-batch.d.mts
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/dictionary-batch.d.ts
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/dictionary-batch.d.ts.map
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/dictionary-batch.js
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/dictionary-batch.js.map
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/dictionary-batch.mjs
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/dictionary-batch.mjs.map
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/dictionary-encoding.d.mts
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/dictionary-encoding.d.ts
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/dictionary-encoding.d.ts.map
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/dictionary-encoding.js
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/dictionary-encoding.js.map
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/dictionary-encoding.mjs
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/dictionary-encoding.mjs.map
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/dictionary-kind.d.mts
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/dictionary-kind.d.ts
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/dictionary-kind.d.ts.map
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/dictionary-kind.js
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/dictionary-kind.js.map
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/dictionary-kind.mjs
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/dictionary-kind.mjs.map
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/duration.d.mts
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/duration.d.ts
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/duration.d.ts.map
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/duration.js
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/duration.js.map
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/duration.mjs
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/duration.mjs.map
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/endianness.d.mts
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/endianness.d.ts
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/endianness.d.ts.map
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/endianness.js
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/endianness.js.map
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/endianness.mjs
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/endianness.mjs.map
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/feature.d.mts
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/feature.d.ts
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/feature.d.ts.map
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/feature.js
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/feature.js.map
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/feature.mjs
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/feature.mjs.map
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/field-node.d.mts
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/field-node.d.ts
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/field-node.d.ts.map
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/field-node.js
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/field-node.js.map
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/field-node.mjs
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/field-node.mjs.map
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/field.d.mts
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/field.d.ts
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/field.d.ts.map
--rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/field.js
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/field.js.map
--rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/field.mjs
--rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/field.mjs.map
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/fixed-size-binary.d.mts
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/fixed-size-binary.d.ts
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/fixed-size-binary.d.ts.map
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/fixed-size-binary.js
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/fixed-size-binary.js.map
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/fixed-size-binary.mjs
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/fixed-size-binary.mjs.map
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/fixed-size-list.d.mts
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/fixed-size-list.d.ts
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/fixed-size-list.d.ts.map
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/fixed-size-list.js
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/fixed-size-list.js.map
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/fixed-size-list.mjs
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/fixed-size-list.mjs.map
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/floating-point.d.mts
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/floating-point.d.ts
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/floating-point.d.ts.map
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/floating-point.js
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/floating-point.js.map
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/floating-point.mjs
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/floating-point.mjs.map
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/footer.d.mts
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/footer.d.ts
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/footer.d.ts.map
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/footer.js
--rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/footer.js.map
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/footer.mjs
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/footer.mjs.map
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/int.d.mts
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/int.d.ts
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/int.d.ts.map
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/int.js
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/int.js.map
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/int.mjs
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/int.mjs.map
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/interval-unit.d.mts
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/interval-unit.d.ts
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/interval-unit.d.ts.map
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/interval-unit.js
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/interval-unit.js.map
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/interval-unit.mjs
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/interval-unit.mjs.map
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/interval.d.mts
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/interval.d.ts
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/interval.d.ts.map
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/interval.js
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/interval.js.map
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/interval.mjs
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/interval.mjs.map
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/key-value.d.mts
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/key-value.d.ts
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/key-value.d.ts.map
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/key-value.js
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/key-value.js.map
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/key-value.mjs
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/key-value.mjs.map
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/large-binary.d.mts
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/large-binary.d.ts
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/large-binary.d.ts.map
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/large-binary.js
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/large-binary.js.map
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/large-binary.mjs
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/large-binary.mjs.map
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/large-list.d.mts
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/large-list.d.ts
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/large-list.d.ts.map
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/large-list.js
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/large-list.js.map
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/large-list.mjs
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/large-list.mjs.map
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/large-utf8.d.mts
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/large-utf8.d.ts
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/large-utf8.d.ts.map
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/large-utf8.js
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/large-utf8.js.map
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/large-utf8.mjs
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/large-utf8.mjs.map
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/list.d.mts
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/list.d.ts
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/list.d.ts.map
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/list.js
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/list.js.map
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/list.mjs
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/list.mjs.map
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/map.d.mts
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/map.d.ts
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/map.d.ts.map
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/map.js
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/map.js.map
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/map.mjs
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/map.mjs.map
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/message-header.d.mts
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/message-header.d.ts
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/message-header.d.ts.map
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/message-header.js
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/message-header.js.map
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/message-header.mjs
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/message-header.mjs.map
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/message.d.mts
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/message.d.ts
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/message.d.ts.map
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/message.js
--rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/message.js.map
--rw-r--r--   0        0        0     3699 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/message.mjs
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/message.mjs.map
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/metadata-version.d.mts
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/metadata-version.d.ts
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/metadata-version.d.ts.map
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/metadata-version.js
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/metadata-version.js.map
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/metadata-version.mjs
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/metadata-version.mjs.map
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/null.d.mts
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/null.d.ts
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/null.d.ts.map
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/null.js
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/null.js.map
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/null.mjs
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/null.mjs.map
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/precision.d.mts
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/precision.d.ts
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/precision.d.ts.map
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/precision.js
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/precision.js.map
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/precision.mjs
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/precision.mjs.map
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/record-batch.d.mts
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/record-batch.d.ts
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/record-batch.d.ts.map
--rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/record-batch.js
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/record-batch.js.map
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/record-batch.mjs
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/record-batch.mjs.map
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/run-end-encoded.d.mts
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/run-end-encoded.d.ts
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/run-end-encoded.d.ts.map
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/run-end-encoded.js
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/run-end-encoded.js.map
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/run-end-encoded.mjs
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/run-end-encoded.mjs.map
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/schema.d.mts
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/schema.d.ts
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/schema.d.ts.map
--rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/schema.js
--rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/schema.js.map
--rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/schema.mjs
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/schema.mjs.map
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-matrix-compressed-axis.d.mts
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-matrix-compressed-axis.d.ts
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-matrix-compressed-axis.d.ts.map
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-matrix-compressed-axis.js
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-matrix-compressed-axis.js.map
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-matrix-compressed-axis.mjs
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-matrix-compressed-axis.mjs.map
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-matrix-index-csx.d.mts
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-matrix-index-csx.d.ts
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-matrix-index-csx.d.ts.map
--rw-r--r--   0        0        0     4678 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-matrix-index-csx.js
--rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-matrix-index-csx.js.map
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-matrix-index-csx.mjs
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-matrix-index-csx.mjs.map
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor-index-coo.d.mts
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor-index-coo.d.ts
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor-index-coo.d.ts.map
--rw-r--r--   0        0        0     4943 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor-index-coo.js
--rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor-index-coo.js.map
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor-index-coo.mjs
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor-index-coo.mjs.map
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor-index-csf.d.mts
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor-index-csf.d.ts
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor-index-csf.d.ts.map
--rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor-index-csf.js
--rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor-index-csf.js.map
--rw-r--r--   0        0        0     6864 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor-index-csf.mjs
--rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor-index-csf.mjs.map
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor-index.d.mts
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor-index.d.ts
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor-index.d.ts.map
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor-index.js
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor-index.js.map
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor-index.mjs
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor-index.mjs.map
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor.d.mts
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor.d.ts
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor.d.ts.map
--rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor.js
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor.js.map
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor.mjs
--rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/sparse-tensor.mjs.map
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/struct-.d.mts
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/struct-.d.ts
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/struct-.d.ts.map
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/struct-.js
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/struct-.js.map
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/struct-.mjs
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/struct-.mjs.map
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/tensor-dim.d.mts
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/tensor-dim.d.ts
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/tensor-dim.d.ts.map
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/tensor-dim.js
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/tensor-dim.js.map
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/tensor-dim.mjs
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/tensor-dim.mjs.map
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/tensor.d.mts
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/tensor.d.ts
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/tensor.d.ts.map
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/tensor.js
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/tensor.js.map
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/tensor.mjs
--rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/tensor.mjs.map
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/time-unit.d.mts
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/time-unit.d.ts
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/time-unit.d.ts.map
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/time-unit.js
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/time-unit.js.map
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/time-unit.mjs
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/time-unit.mjs.map
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/time.d.mts
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/time.d.ts
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/time.d.ts.map
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/time.js
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/time.js.map
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/time.mjs
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/time.mjs.map
--rw-r--r--   0        0        0     7094 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/timestamp.d.mts
--rw-r--r--   0        0        0     7094 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/timestamp.d.ts
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/timestamp.d.ts.map
--rw-r--r--   0        0        0     7568 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/timestamp.js
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/timestamp.js.map
--rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/timestamp.mjs
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/timestamp.mjs.map
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/type.d.mts
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/type.d.ts
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/type.d.ts.map
--rw-r--r--   0        0        0     6244 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/type.js
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/type.js.map
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/type.mjs
--rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/type.mjs.map
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/union-mode.d.mts
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/union-mode.d.ts
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/union-mode.d.ts.map
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/union-mode.js
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/union-mode.js.map
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/union-mode.mjs
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/union-mode.mjs.map
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/union.d.mts
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/union.d.ts
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/union.d.ts.map
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/union.js
--rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/union.js.map
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/union.mjs
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/union.mjs.map
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/utf8.d.mts
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/utf8.d.ts
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/utf8.d.ts.map
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/utf8.js
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/utf8.js.map
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/utf8.mjs
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/fb/utf8.mjs.map
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/adapters.d.mts
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/adapters.d.ts
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/adapters.d.ts.map
--rw-r--r--   0        0        0    13796 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/adapters.js
--rw-r--r--   0        0        0    10436 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/adapters.js.map
--rw-r--r--   0        0        0    13349 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/adapters.mjs
--rw-r--r--   0        0        0    10401 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/adapters.mjs.map
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/file.d.mts
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/file.d.ts
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/file.d.ts.map
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/file.js
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/file.js.map
--rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/file.mjs
--rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/file.mjs.map
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/interfaces.d.mts
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/interfaces.d.ts
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/interfaces.d.ts.map
--rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/interfaces.js
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/interfaces.js.map
--rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/interfaces.mjs
--rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/interfaces.mjs.map
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/stream.d.mts
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/stream.d.ts
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/stream.d.ts.map
--rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/stream.js
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/stream.js.map
--rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/stream.mjs
--rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/stream.mjs.map
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/builder.d.mts
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/builder.d.ts
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/builder.d.ts.map
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/builder.js
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/builder.js.map
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/builder.mjs
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/builder.mjs.map
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/iterable.d.mts
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/iterable.d.ts
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/iterable.d.ts.map
--rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/iterable.js
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/iterable.js.map
--rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/iterable.mjs
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/iterable.mjs.map
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/reader.d.mts
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/reader.d.ts
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/reader.d.ts.map
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/reader.js
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/reader.js.map
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/reader.mjs
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/reader.mjs.map
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/writer.d.mts
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/writer.d.ts
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/writer.d.ts.map
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/writer.js
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/writer.js.map
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/writer.mjs
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/node/writer.mjs.map
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/builder.d.mts
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/builder.d.ts
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/builder.d.ts.map
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/builder.js
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/builder.js.map
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/builder.mjs
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/builder.mjs.map
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/iterable.d.mts
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/iterable.d.ts
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/iterable.d.ts.map
--rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/iterable.js
--rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/iterable.js.map
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/iterable.mjs
--rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/iterable.mjs.map
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/reader.d.mts
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/reader.d.ts
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/reader.d.ts.map
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/reader.js
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/reader.js.map
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/reader.mjs
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/reader.mjs.map
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/writer.d.mts
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/writer.d.ts
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/writer.d.ts.map
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/writer.js
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/writer.js.map
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/writer.mjs
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/io/whatwg/writer.mjs.map
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/message.d.mts
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/message.d.ts
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/message.d.ts.map
--rw-r--r--   0        0        0    12888 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/message.js
--rw-r--r--   0        0        0     9938 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/message.js.map
--rw-r--r--   0        0        0    11829 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/message.mjs
--rw-r--r--   0        0        0    10170 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/message.mjs.map
--rw-r--r--   0        0        0    13510 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/reader.d.mts
--rw-r--r--   0        0        0    13510 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/reader.d.ts
--rw-r--r--   0        0        0    12257 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/reader.d.ts.map
--rw-r--r--   0        0        0    27682 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/reader.js
--rw-r--r--   0        0        0    22403 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/reader.js.map
--rw-r--r--   0        0        0    26586 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/reader.mjs
--rw-r--r--   0        0        0    22830 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/reader.mjs.map
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/serialization.d.mts
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/serialization.d.ts
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/serialization.d.ts.map
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/serialization.js
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/serialization.js.map
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/serialization.mjs
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/serialization.mjs.map
--rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/writer.d.mts
--rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/writer.d.ts
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/writer.d.ts.map
--rw-r--r--   0        0        0    17023 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/writer.js
--rw-r--r--   0        0        0    14433 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/writer.js.map
--rw-r--r--   0        0        0    16047 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/writer.mjs
--rw-r--r--   0        0        0    14883 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/writer.mjs.map
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/metadata/file.d.mts
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/metadata/file.d.ts
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/metadata/file.d.ts.map
--rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/metadata/file.js
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/metadata/file.js.map
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/metadata/file.mjs
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/metadata/file.mjs.map
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/metadata/json.d.mts
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/metadata/json.d.ts
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/metadata/json.d.ts.map
--rw-r--r--   0        0        0     8251 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/metadata/json.js
--rw-r--r--   0        0        0     7669 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/metadata/json.js.map
--rw-r--r--   0        0        0     7660 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/metadata/json.mjs
--rw-r--r--   0        0        0     8011 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/metadata/json.mjs.map
--rw-r--r--   0        0        0     5739 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/metadata/message.d.mts
--rw-r--r--   0        0        0     5739 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/metadata/message.d.ts
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/metadata/message.d.ts.map
--rw-r--r--   0        0        0    22090 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/metadata/message.js
--rw-r--r--   0        0        0    20317 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/metadata/message.js.map
--rw-r--r--   0        0        0    20144 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/metadata/message.mjs
--rw-r--r--   0        0        0    21501 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/ipc/metadata/message.mjs.map
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/row/map.d.mts
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/row/map.d.ts
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/row/map.d.ts.map
--rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/row/map.js
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/row/map.js.map
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/row/map.mjs
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/row/map.mjs.map
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/row/struct.d.mts
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/row/struct.d.ts
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/row/struct.d.ts.map
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/row/struct.js
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/row/struct.js.map
--rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/row/struct.mjs
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/row/struct.mjs.map
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/Arrow.dom.mts
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/Arrow.dom.ts
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/Arrow.mts
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/Arrow.node.mts
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/Arrow.node.ts
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/Arrow.ts
--rw-r--r--   0        0        0    16317 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder.mts
--rw-r--r--   0        0        0    16317 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder.ts
--rw-r--r--   0        0        0    29544 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/data.mts
--rw-r--r--   0        0        0    29544 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/data.ts
--rw-r--r--   0        0        0     5206 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/enum.mts
--rw-r--r--   0        0        0     5206 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/enum.ts
--rw-r--r--   0        0        0    13877 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/factories.mts
--rw-r--r--   0        0        0    13877 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/factories.ts
--rw-r--r--   0        0        0    17737 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/interfaces.mts
--rw-r--r--   0        0        0    17737 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/interfaces.ts
--rw-r--r--   0        0        0    13717 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/recordbatch.mts
--rw-r--r--   0        0        0    13717 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/recordbatch.ts
--rw-r--r--   0        0        0     7870 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/schema.mts
--rw-r--r--   0        0        0     7870 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/schema.ts
--rw-r--r--   0        0        0    16512 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/table.mts
--rw-r--r--   0        0        0    16512 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/table.ts
--rw-r--r--   0        0        0    32115 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/type.mts
--rw-r--r--   0        0        0    32115 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/type.ts
--rw-r--r--   0        0        0    17913 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/vector.mts
--rw-r--r--   0        0        0    17913 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/vector.ts
--rw-r--r--   0        0        0    16272 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor.mts
--rw-r--r--   0        0        0    16272 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor.ts
--rwxr-xr-x   0        0        0    13298 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/bin/arrow2csv.mts
--rwxr-xr-x   0        0        0    13298 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/bin/arrow2csv.ts
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/binary.mts
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/binary.ts
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/bool.mts
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/bool.ts
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/buffer.mts
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/buffer.ts
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/date.mts
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/date.ts
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/decimal.mts
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/decimal.ts
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/dictionary.mts
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/dictionary.ts
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/duration.mts
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/duration.ts
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/fixedsizebinary.mts
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/fixedsizebinary.ts
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/fixedsizelist.mts
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/fixedsizelist.ts
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/float.mts
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/float.ts
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/int.mts
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/int.ts
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/interval.mts
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/interval.ts
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/largebinary.mts
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/largebinary.ts
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/largeutf8.mts
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/largeutf8.ts
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/list.mts
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/list.ts
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/map.mts
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/map.ts
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/null.mts
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/null.ts
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/struct.mts
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/struct.ts
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/time.mts
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/time.ts
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/timestamp.mts
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/timestamp.ts
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/union.mts
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/union.ts
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/utf8.mts
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/utf8.ts
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/valid.mts
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/builder/valid.ts
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/File_generated.mts
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/File_generated.ts
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/Message_generated.mts
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/Message_generated.ts
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/Schema_generated.mts
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/Schema_generated.ts
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/SparseTensor_generated.mts
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/SparseTensor_generated.ts
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/Tensor_generated.mts
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/Tensor_generated.ts
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/binary.mts
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/binary.ts
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/block.mts
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/block.ts
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/body-compression-method.mts
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/body-compression-method.ts
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/body-compression.mts
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/body-compression.ts
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/bool.mts
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/bool.ts
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/buffer.mts
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/buffer.ts
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/compression-type.mts
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/compression-type.ts
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/date-unit.mts
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/date-unit.ts
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/date.mts
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/date.ts
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/decimal.mts
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/decimal.ts
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/dictionary-batch.mts
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/dictionary-batch.ts
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/dictionary-encoding.mts
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/dictionary-encoding.ts
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/dictionary-kind.mts
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/dictionary-kind.ts
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/duration.mts
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/duration.ts
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/endianness.mts
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/endianness.ts
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/feature.mts
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/feature.ts
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/field-node.mts
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/field-node.ts
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/field.mts
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/field.ts
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/fixed-size-binary.mts
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/fixed-size-binary.ts
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/fixed-size-list.mts
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/fixed-size-list.ts
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/floating-point.mts
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/floating-point.ts
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/footer.mts
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/footer.ts
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/int.mts
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/int.ts
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/interval-unit.mts
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/interval-unit.ts
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/interval.mts
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/interval.ts
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/key-value.mts
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/key-value.ts
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/large-binary.mts
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/large-binary.ts
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/large-list.mts
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/large-list.ts
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/large-utf8.mts
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/large-utf8.ts
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/list.mts
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/list.ts
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/map.mts
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/map.ts
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/message-header.mts
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/message-header.ts
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/message.mts
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/message.ts
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/metadata-version.mts
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/metadata-version.ts
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/null.mts
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/null.ts
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/precision.mts
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/precision.ts
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/record-batch.mts
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/record-batch.ts
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/run-end-encoded.mts
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/run-end-encoded.ts
--rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/schema.mts
--rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/schema.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/sparse-matrix-compressed-axis.mts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/sparse-matrix-compressed-axis.ts
--rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/sparse-matrix-index-csx.mts
--rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/sparse-matrix-index-csx.ts
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/sparse-tensor-index-coo.mts
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/sparse-tensor-index-coo.ts
--rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/sparse-tensor-index-csf.mts
--rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/sparse-tensor-index-csf.ts
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/sparse-tensor-index.mts
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/sparse-tensor-index.ts
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/sparse-tensor.mts
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/sparse-tensor.ts
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/struct-.mts
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/struct-.ts
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/tensor-dim.mts
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/tensor-dim.ts
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/tensor.mts
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/tensor.ts
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/time-unit.mts
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/time-unit.ts
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/time.mts
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/time.ts
--rw-r--r--   0        0        0     8021 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/timestamp.mts
--rw-r--r--   0        0        0     8021 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/timestamp.ts
--rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/type.mts
--rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/type.ts
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/union-mode.mts
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/union-mode.ts
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/union.mts
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/union.ts
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/utf8.mts
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/fb/utf8.ts
--rw-r--r--   0        0        0    13958 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/adapters.mts
--rw-r--r--   0        0        0    13958 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/adapters.ts
--rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/file.mts
--rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/file.ts
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/interfaces.mts
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/interfaces.ts
--rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/stream.mts
--rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/stream.ts
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/node/builder.mts
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/node/builder.ts
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/node/iterable.mts
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/node/iterable.ts
--rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/node/reader.mts
--rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/node/reader.ts
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/node/writer.mts
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/node/writer.ts
--rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/whatwg/builder.mts
--rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/whatwg/builder.ts
--rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/whatwg/iterable.mts
--rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/whatwg/iterable.ts
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/whatwg/reader.mts
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/whatwg/reader.ts
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/whatwg/writer.mts
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/io/whatwg/writer.ts
--rw-r--r--   0        0        0    11942 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/ipc/message.mts
--rw-r--r--   0        0        0    11942 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/ipc/message.ts
--rw-r--r--   0        0        0    34683 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/ipc/reader.mts
--rw-r--r--   0        0        0    34683 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/ipc/reader.ts
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/ipc/serialization.mts
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/ipc/serialization.ts
--rw-r--r--   0        0        0    20449 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/ipc/writer.mts
--rw-r--r--   0        0        0    20449 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/ipc/writer.ts
--rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/ipc/metadata/file.mts
--rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/ipc/metadata/file.ts
--rw-r--r--   0        0        0     8341 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/ipc/metadata/json.mts
--rw-r--r--   0        0        0     8341 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/ipc/metadata/json.ts
--rw-r--r--   0        0        0    23593 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/ipc/metadata/message.mts
--rw-r--r--   0        0        0    23593 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/ipc/metadata/message.ts
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/row/map.mts
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/row/map.ts
--rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/row/struct.mts
--rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/row/struct.ts
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/bigint.mts
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/bigint.ts
--rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/bit.mts
--rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/bit.ts
--rw-r--r--   0        0        0    11494 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/bn.mts
--rw-r--r--   0        0        0    11494 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/bn.ts
--rw-r--r--   0        0        0    14557 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/buffer.mts
--rw-r--r--   0        0        0    14557 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/buffer.ts
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/chunk.mts
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/chunk.ts
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/compat.mts
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/compat.ts
--rw-r--r--   0        0        0    14395 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/int.mts
--rw-r--r--   0        0        0    14395 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/int.ts
--rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/math.mts
--rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/math.ts
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/pretty.mts
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/pretty.ts
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/recordbatch.mts
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/recordbatch.ts
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/utf8.mts
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/utf8.ts
--rw-r--r--   0        0        0     7753 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/vector.mts
--rw-r--r--   0        0        0     7753 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/util/vector.ts
--rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/builderctor.mts
--rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/builderctor.ts
--rw-r--r--   0        0        0    21030 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/get.mts
--rw-r--r--   0        0        0    21030 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/get.ts
--rw-r--r--   0        0        0    13055 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/indexof.mts
--rw-r--r--   0        0        0    13055 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/indexof.ts
--rw-r--r--   0        0        0    11814 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/iterator.mts
--rw-r--r--   0        0        0    11814 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/iterator.ts
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/jsontypeassembler.mts
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/jsontypeassembler.ts
--rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/jsonvectorassembler.mts
--rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/jsonvectorassembler.ts
--rw-r--r--   0        0        0    23921 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/set.mts
--rw-r--r--   0        0        0    23921 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/set.ts
--rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/typeassembler.mts
--rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/typeassembler.ts
--rw-r--r--   0        0        0    14980 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/typecomparator.mts
--rw-r--r--   0        0        0    14980 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/typecomparator.ts
--rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/typector.mts
--rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/typector.ts
--rw-r--r--   0        0        0    12082 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/vectorassembler.mts
--rw-r--r--   0        0        0    12082 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/vectorassembler.ts
--rw-r--r--   0        0        0    12146 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/vectorloader.mts
--rw-r--r--   0        0        0    12146 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/src/visitor/vectorloader.ts
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/bigint.d.mts
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/bigint.d.ts
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/bigint.d.ts.map
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/bigint.js
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/bigint.js.map
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/bigint.mjs
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/bigint.mjs.map
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/bit.d.mts
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/bit.d.ts
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/bit.d.ts.map
--rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/bit.js
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/bit.js.map
--rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/bit.mjs
--rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/bit.mjs.map
--rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/bn.d.mts
--rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/bn.d.ts
--rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/bn.d.ts.map
--rw-r--r--   0        0        0     6652 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/bn.js
--rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/bn.js.map
--rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/bn.mjs
--rw-r--r--   0        0        0     6997 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/bn.mjs.map
--rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/buffer.d.mts
--rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/buffer.d.ts
--rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/buffer.d.ts.map
--rw-r--r--   0        0        0    15226 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/buffer.js
--rw-r--r--   0        0        0    11582 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/buffer.js.map
--rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/buffer.mjs
--rw-r--r--   0        0        0    11161 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/buffer.mjs.map
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/chunk.d.mts
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/chunk.d.ts
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/chunk.d.ts.map
--rw-r--r--   0        0        0     5760 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/chunk.js
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/chunk.js.map
--rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/chunk.mjs
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/chunk.mjs.map
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/compat.d.mts
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/compat.d.ts
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/compat.d.ts.map
--rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/compat.js
--rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/compat.js.map
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/compat.mjs
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/compat.mjs.map
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/int.d.mts
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/int.d.ts
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/int.d.ts.map
--rw-r--r--   0        0        0    13669 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/int.js
--rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/int.js.map
--rw-r--r--   0        0        0    13439 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/int.mjs
--rw-r--r--   0        0        0    16079 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/int.mjs.map
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/math.d.mts
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/math.d.ts
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/math.d.ts.map
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/math.js
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/math.js.map
--rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/math.mjs
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/math.mjs.map
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/pretty.d.mts
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/pretty.d.ts
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/pretty.d.ts.map
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/pretty.js
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/pretty.js.map
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/pretty.mjs
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/pretty.mjs.map
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/recordbatch.d.mts
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/recordbatch.d.ts
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/recordbatch.d.ts.map
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/recordbatch.js
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/recordbatch.js.map
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/recordbatch.mjs
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/recordbatch.mjs.map
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/utf8.d.mts
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/utf8.d.ts
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/utf8.d.ts.map
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/utf8.js
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/utf8.js.map
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/utf8.mjs
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/utf8.mjs.map
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/vector.d.mts
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/vector.d.ts
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/vector.d.ts.map
--rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/vector.js
--rw-r--r--   0        0        0     6756 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/vector.js.map
--rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/vector.mjs
--rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/util/vector.mjs.map
--rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/builderctor.d.mts
--rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/builderctor.d.ts
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/builderctor.d.ts.map
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/builderctor.js
--rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/builderctor.js.map
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/builderctor.mjs
--rw-r--r--   0        0        0     3840 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/builderctor.mjs.map
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/get.d.mts
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/get.d.ts
--rw-r--r--   0        0        0     8009 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/get.d.ts.map
--rw-r--r--   0        0        0    12503 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/get.js
--rw-r--r--   0        0        0    13251 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/get.js.map
--rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/get.mjs
--rw-r--r--   0        0        0    13499 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/get.mjs.map
--rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/indexof.d.mts
--rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/indexof.d.ts
--rw-r--r--   0        0        0     9301 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/indexof.d.ts.map
--rw-r--r--   0        0        0     6456 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/indexof.js
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/indexof.js.map
--rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/indexof.mjs
--rw-r--r--   0        0        0     4796 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/indexof.mjs.map
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/iterator.d.mts
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/iterator.d.ts
--rw-r--r--   0        0        0     7758 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/iterator.d.ts.map
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/iterator.js
--rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/iterator.js.map
--rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/iterator.mjs
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/iterator.mjs.map
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/jsontypeassembler.d.mts
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/jsontypeassembler.d.ts
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/jsontypeassembler.d.ts.map
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/jsontypeassembler.js
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/jsontypeassembler.js.map
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/jsontypeassembler.mjs
--rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/jsontypeassembler.mjs.map
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/jsonvectorassembler.d.mts
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/jsonvectorassembler.d.ts
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/jsonvectorassembler.d.ts.map
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/jsonvectorassembler.js
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/jsonvectorassembler.js.map
--rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/jsonvectorassembler.mjs
--rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/jsonvectorassembler.mjs.map
--rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/set.d.mts
--rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/set.d.ts
--rw-r--r--   0        0        0    10537 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/set.d.ts.map
--rw-r--r--   0        0        0    17276 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/set.js
--rw-r--r--   0        0        0    17209 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/set.js.map
--rw-r--r--   0        0        0    14081 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/set.mjs
--rw-r--r--   0        0        0    16790 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/set.mjs.map
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/typeassembler.d.mts
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/typeassembler.d.ts
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/typeassembler.d.ts.map
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/typeassembler.js
--rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/typeassembler.js.map
--rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/typeassembler.mjs
--rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/typeassembler.mjs.map
--rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/typecomparator.d.mts
--rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/typecomparator.d.ts
--rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/typecomparator.d.ts.map
--rw-r--r--   0        0        0     8376 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/typecomparator.js
--rw-r--r--   0        0        0     7591 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/typecomparator.js.map
--rw-r--r--   0        0        0     7953 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/typecomparator.mjs
--rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/typecomparator.mjs.map
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/typector.d.mts
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/typector.d.ts
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/typector.d.ts.map
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/typector.js
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/typector.js.map
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/typector.mjs
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/typector.mjs.map
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/vectorassembler.d.mts
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/vectorassembler.d.ts
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/vectorassembler.d.ts.map
--rw-r--r--   0        0        0     9928 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/vectorassembler.js
--rw-r--r--   0        0        0     7605 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/vectorassembler.js.map
--rw-r--r--   0        0        0     9564 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/vectorassembler.mjs
--rw-r--r--   0        0        0     7827 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/vectorassembler.mjs.map
--rw-r--r--   0        0        0     4366 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/vectorloader.d.mts
--rw-r--r--   0        0        0     4366 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/vectorloader.d.ts
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/vectorloader.d.ts.map
--rw-r--r--   0        0        0    11080 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/vectorloader.js
--rw-r--r--   0        0        0    11042 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/vectorloader.js.map
--rw-r--r--   0        0        0    10141 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/vectorloader.mjs
--rw-r--r--   0        0        0    11097 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/node_modules/apache-arrow/visitor/vectorloader.mjs.map
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/src/index.js
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/src/style.css
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/.gitignore
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/README.md
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 mosaic_widget-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 mosaic_widget-0.8.0/jsconfig.json
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 mosaic_widget-0.8.0/package.json
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 mosaic_widget-0.8.0/vite.config.mjs
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 mosaic_widget-0.8.0/mosaic_widget/__init__.py
+-rw-r--r--   0        0        0  1222101 2020-02-02 00:00:00.000000 mosaic_widget-0.8.0/mosaic_widget/static/index.js
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 mosaic_widget-0.8.0/mosaic_widget/static/style.css
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 mosaic_widget-0.8.0/src/index.js
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 mosaic_widget-0.8.0/src/style.css
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mosaic_widget-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 mosaic_widget-0.8.0/README.md
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 mosaic_widget-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 mosaic_widget-0.8.0/PKG-INFO
```

### Comparing `mosaic_widget-0.7.1/package.json` & `mosaic_widget-0.8.0/package.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8875%*

 * *Differences: {"'dependencies'": "{'@uwdata/vgplot': '^0.8.0', 'apache-arrow': '^15.0.2', '@uwdata/mosaic-spec': "*

 * *                   "'^0.8.0'}",*

 * * "'devDependencies'": "{'anywidget': '^0.9.10'}",*

 * * "'scripts'": "{'test': 'tsc -p jsconfig.json', 'lint': 'eslint src', 'publish': 'hatch publish "*

 * *              "--user __token__'}",*

 * * "'version'": "'0.8.0'"}*

```diff
@@ -1,28 +1,29 @@
 {
     "author": "Dominik Moritz (https://www.domoritz.de)",
     "dependencies": {
-        "@uwdata/vgplot": "^0.7.1",
-        "apache-arrow": "^15.0.0",
+        "@uwdata/mosaic-spec": "^0.8.0",
+        "@uwdata/vgplot": "^0.8.0",
+        "apache-arrow": "^15.0.2",
         "uuid": "^9.0.1"
     },
     "devDependencies": {
-        "anywidget": "^0.9.3"
+        "anywidget": "^0.9.10"
     },
     "license": "BSD-3-Clause",
     "name": "mosaic-widget",
     "private": true,
     "repository": {
         "type": "git",
         "url": "https://github.com/uwdata/mosaic.git"
     },
     "scripts": {
         "build": "vite build",
         "dev": "vite",
-        "lint": "eslint src --ext .js",
+        "lint": "eslint src",
         "prepublishOnly": "npm run test && npm run lint && hatch fmt --check && npm run build && hatch build",
-        "publish": "hatch publish",
-        "test": "tsc"
+        "publish": "hatch publish --user __token__",
+        "test": "tsc -p jsconfig.json"
     },
     "type": "module",
-    "version": "0.7.1"
+    "version": "0.8.0"
 }
```

### Comparing `mosaic_widget-0.7.1/mosaic_widget/__init__.py` & `mosaic_widget-0.8.0/mosaic_widget/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaic_widget-0.7.1/mosaic_widget/static/index.js` & `mosaic_widget-0.8.0/mosaic_widget/static/index.js`

 * *Files identical despite different names*

### Comparing `mosaic_widget-0.7.1/mosaic_widget/static/style.css` & `mosaic_widget-0.8.0/mosaic_widget/static/style.css`

 * *Files identical despite different names*

### Comparing `mosaic_widget-0.7.1/src/index.js` & `mosaic_widget-0.8.0/src/index.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,28 +1,29 @@
-// @ts-check
-
 import {
     coordinator,
     namedPlots
 } from '@uwdata/vgplot';
 import {
+    isSelection
+} from '@uwdata/mosaic-core';
+import {
     parseSpec,
     astToDOM
 } from '@uwdata/mosaic-spec';
 import * as arrow from 'apache-arrow';
 import './style.css';
 import {
     v4 as uuidv4
 } from 'uuid';
 
 /**
  * @typedef {Record<string, {value: unknown, predicate?: string}>} Params
  *
  * @typedef Model
- * @prop {Record<any, unknown>} spec the current specification
+ * @prop {import('@uwdata/mosaic-spec').Spec} spec the current specification
  * @prop {boolean} temp_indexes whether data cube indexes should be created as temp tables
  * @prop {Params} params the current params
  */
 
 export default {
     /** @type {import('anywidget/types').Initialize<Model>} */
     // eslint-disable-next-line no-unused-vars
@@ -81,23 +82,25 @@
 
             /** @type Params */
             const params = {};
 
             for (const [name, param] of dom.params) {
                 params[name] = {
                     value: param.value,
-                    ...(param.predicate ? {
+                    ...(isSelection(param) ? {
                         predicate: String(param.predicate())
                     } : {}),
                 };
 
                 param.addEventListener('value', (value) => {
                     params[name] = {
                         value,
-                        predicate: String(param.predicate())
+                        ...(isSelection(param) ? {
+                            predicate: String(param.predicate())
+                        } : {}),
                     };
                     view.model.set('params', params);
                     view.model.save_changes();
                 });
             }
 
             view.model.set('params', params);
@@ -158,12 +161,11 @@
         return () => {
             // cleanup
             reset();
         };
     },
 };
 
-/** @param {Record<any, unknown>} spec */
 function instantiateSpec(spec) {
     const ast = parseSpec(spec);
     return astToDOM(ast);
 }
```

### Comparing `mosaic_widget-0.7.1/src/style.css` & `mosaic_widget-0.8.0/src/style.css`

 * *Files identical despite different names*

### Comparing `mosaic_widget-0.7.1/README.md` & `mosaic_widget-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `mosaic_widget-0.7.1/pyproject.toml` & `mosaic_widget-0.8.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "mosaic-widget"
 description = "A Jupyter widget for Mosaic"
 dynamic = ["version"]
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
   "anywidget>=0.9.0",
-  "duckdb==0.10.0",
+  "duckdb==0.10.2",
   "pyarrow"
 ]
 
 [project.urls]
 homepage = "https://github.com/uwdata/mosaic"
 
 [tool.hatch.build]
@@ -28,14 +28,15 @@
   "pandas",
   "pyyaml"
 ]
 
 [tool.hatch.envs.default]
 python = "3.11"
 features = ["dev"]
+uv = true
 
 [tool.hatch.version]
 path = "package.json"
 pattern = "\"version\": \"(?P<version>.+?)\""
 
 [tool.ruff]
 extend-include = ["*.ipynb"]
```

### Comparing `mosaic_widget-0.7.1/PKG-INFO` & `mosaic_widget-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mosaic-widget
-Version: 0.7.1
+Version: 0.8.0
 Summary: A Jupyter widget for Mosaic
 Project-URL: homepage, https://github.com/uwdata/mosaic
 Requires-Python: >=3.9
 Requires-Dist: anywidget>=0.9.0
-Requires-Dist: duckdb==0.10.0
+Requires-Dist: duckdb==0.10.2
 Requires-Dist: pyarrow
 Provides-Extra: dev
 Requires-Dist: jupyterlab; extra == 'dev'
 Requires-Dist: pandas; extra == 'dev'
 Requires-Dist: pyyaml; extra == 'dev'
 Description-Content-Type: text/markdown
```


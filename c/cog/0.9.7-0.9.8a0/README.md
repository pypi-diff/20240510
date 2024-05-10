# Comparing `tmp/cog-0.9.7-py3-none-any.whl.zip` & `tmp/cog-0.9.8a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,111 +1,111 @@
-Zip file size: 96039 bytes, number of entries: 109
--rw-r--r--  2.0 unx       13 b- defN 24-May-06 20:09 cog/.gitignore
--rw-r--r--  2.0 unx      384 b- defN 24-May-06 20:09 cog/__init__.py
--rw-r--r--  2.0 unx      411 b- defN 24-May-06 20:10 cog/_version.py
--rw-r--r--  2.0 unx    10313 b- defN 24-May-06 20:09 cog/code_xforms.py
--rw-r--r--  2.0 unx      286 b- defN 24-May-06 20:09 cog/errors.py
--rw-r--r--  2.0 unx     2124 b- defN 24-May-06 20:09 cog/files.py
--rw-r--r--  2.0 unx     1945 b- defN 24-May-06 20:09 cog/json.py
--rw-r--r--  2.0 unx     3171 b- defN 24-May-06 20:09 cog/logging.py
--rw-r--r--  2.0 unx    17163 b- defN 24-May-06 20:09 cog/predictor.py
--rw-r--r--  2.0 unx     3308 b- defN 24-May-06 20:09 cog/schema.py
--rw-r--r--  2.0 unx      645 b- defN 24-May-06 20:09 cog/suppress_output.py
--rw-r--r--  2.0 unx     8993 b- defN 24-May-06 20:09 cog/types.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-06 20:09 cog/command/__init__.py
--rw-r--r--  2.0 unx    18782 b- defN 24-May-06 20:09 cog/command/ast_openapi_schema.py
--rw-r--r--  2.0 unx     1934 b- defN 24-May-06 20:09 cog/command/openapi_schema.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-06 20:09 cog/server/__init__.py
--rw-r--r--  2.0 unx      593 b- defN 24-May-06 20:09 cog/server/eventtypes.py
--rw-r--r--  2.0 unx      149 b- defN 24-May-06 20:09 cog/server/exceptions.py
--rw-r--r--  2.0 unx     5349 b- defN 24-May-06 20:09 cog/server/helpers.py
--rw-r--r--  2.0 unx    16945 b- defN 24-May-06 20:09 cog/server/http.py
--rw-r--r--  2.0 unx      971 b- defN 24-May-06 20:09 cog/server/probes.py
--rw-r--r--  2.0 unx      689 b- defN 24-May-06 20:09 cog/server/response_throttler.py
--rw-r--r--  2.0 unx    15515 b- defN 24-May-06 20:09 cog/server/runner.py
--rw-r--r--  2.0 unx     3326 b- defN 24-May-06 20:09 cog/server/webhook.py
--rw-r--r--  2.0 unx     8050 b- defN 24-May-06 20:09 cog/server/worker.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-06 20:09 tests/__init__.py
--rw-r--r--  2.0 unx      536 b- defN 24-May-06 20:09 tests/conftest.py
--rw-r--r--  2.0 unx     1737 b- defN 24-May-06 20:09 tests/test_json.py
--rw-r--r--  2.0 unx     1154 b- defN 24-May-06 20:09 tests/test_predictor.py
--rw-r--r--  2.0 unx     4895 b- defN 24-May-06 20:09 tests/test_types.py
--rw-r--r--  2.0 unx      113 b- defN 24-May-06 20:09 tests/fixtures/argv_override.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-06 20:09 tests/server/__init__.py
--rw-r--r--  2.0 unx     2800 b- defN 24-May-06 20:09 tests/server/conftest.py
--rw-r--r--  2.0 unx     2564 b- defN 24-May-06 20:09 tests/server/test_code_xforms.py
--rw-r--r--  2.0 unx     4692 b- defN 24-May-06 20:09 tests/server/test_helpers.py
--rw-r--r--  2.0 unx    16956 b- defN 24-May-06 20:09 tests/server/test_http.py
--rw-r--r--  2.0 unx     9181 b- defN 24-May-06 20:09 tests/server/test_http_input.py
--rw-r--r--  2.0 unx     4020 b- defN 24-May-06 20:09 tests/server/test_http_output.py
--rw-r--r--  2.0 unx     2775 b- defN 24-May-06 20:09 tests/server/test_predictor.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-06 20:09 tests/server/test_probes.py
--rw-r--r--  2.0 unx     1210 b- defN 24-May-06 20:09 tests/server/test_response_throttler.py
--rw-r--r--  2.0 unx    10931 b- defN 24-May-06 20:09 tests/server/test_runner.py
--rw-r--r--  2.0 unx     3225 b- defN 24-May-06 20:09 tests/server/test_webhook.py
--rw-r--r--  2.0 unx    16162 b- defN 24-May-06 20:09 tests/server/test_worker.py
--rw-r--r--  2.0 unx      209 b- defN 24-May-06 20:09 tests/server/fixtures/async_setup_uses_same_loop_as_predict.py
--rw-r--r--  2.0 unx      198 b- defN 24-May-06 20:09 tests/server/fixtures/catch_in_predict.py
--rw-r--r--  2.0 unx      232 b- defN 24-May-06 20:09 tests/server/fixtures/complex_output.py
--rw-r--r--  2.0 unx      131 b- defN 24-May-06 20:09 tests/server/fixtures/count_up.py
--rw-r--r--  2.0 unx      136 b- defN 24-May-06 20:09 tests/server/fixtures/exc_in_predict.py
--rw-r--r--  2.0 unx      133 b- defN 24-May-06 20:09 tests/server/fixtures/exc_in_setup.py
--rw-r--r--  2.0 unx      151 b- defN 24-May-06 20:09 tests/server/fixtures/exc_in_setup_and_predict.py
--rw-r--r--  2.0 unx       56 b- defN 24-May-06 20:09 tests/server/fixtures/exc_on_import.py
--rw-r--r--  2.0 unx      122 b- defN 24-May-06 20:09 tests/server/fixtures/exit_in_predict.py
--rw-r--r--  2.0 unx      124 b- defN 24-May-06 20:09 tests/server/fixtures/exit_in_setup.py
--rw-r--r--  2.0 unx       23 b- defN 24-May-06 20:09 tests/server/fixtures/exit_on_import.py
--rw-r--r--  2.0 unx       58 b- defN 24-May-06 20:09 tests/server/fixtures/function.py
--rw-r--r--  2.0 unx      159 b- defN 24-May-06 20:09 tests/server/fixtures/hello_world.py
--rw-r--r--  2.0 unx      197 b- defN 24-May-06 20:09 tests/server/fixtures/input_choices.py
--rw-r--r--  2.0 unx      153 b- defN 24-May-06 20:09 tests/server/fixtures/input_choices_integer.py
--rw-r--r--  2.0 unx      139 b- defN 24-May-06 20:09 tests/server/fixtures/input_file.py
--rw-r--r--  2.0 unx      160 b- defN 24-May-06 20:09 tests/server/fixtures/input_ge_le.py
--rw-r--r--  2.0 unx      126 b- defN 24-May-06 20:09 tests/server/fixtures/input_integer.py
--rw-r--r--  2.0 unx      152 b- defN 24-May-06 20:09 tests/server/fixtures/input_integer_default.py
--rw-r--r--  2.0 unx      317 b- defN 24-May-06 20:09 tests/server/fixtures/input_multiple.py
--rw-r--r--  2.0 unx      118 b- defN 24-May-06 20:09 tests/server/fixtures/input_none.py
--rw-r--r--  2.0 unx      236 b- defN 24-May-06 20:09 tests/server/fixtures/input_path.py
--rw-r--r--  2.0 unx      137 b- defN 24-May-06 20:09 tests/server/fixtures/input_path_2.py
--rw-r--r--  2.0 unx      159 b- defN 24-May-06 20:09 tests/server/fixtures/input_secret.py
--rw-r--r--  2.0 unx      125 b- defN 24-May-06 20:09 tests/server/fixtures/input_string.py
--rw-r--r--  2.0 unx      262 b- defN 24-May-06 20:09 tests/server/fixtures/input_union_integer_or_list_of_integers.py
--rw-r--r--  2.0 unx      266 b- defN 24-May-06 20:09 tests/server/fixtures/input_union_string_or_list_of_strings.py
--rw-r--r--  2.0 unx      205 b- defN 24-May-06 20:09 tests/server/fixtures/input_unsupported_type.py
--rw-r--r--  2.0 unx      122 b- defN 24-May-06 20:09 tests/server/fixtures/input_untyped.py
--rw-r--r--  2.0 unx      160 b- defN 24-May-06 20:09 tests/server/fixtures/killed_in_predict.py
--rw-r--r--  2.0 unx      882 b- defN 24-May-06 20:09 tests/server/fixtures/logging.py
--rw-r--r--  2.0 unx      109 b- defN 24-May-06 20:09 tests/server/fixtures/missing_predict.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-06 20:09 tests/server/fixtures/missing_predictor.py
--rw-r--r--  2.0 unx      482 b- defN 24-May-06 20:09 tests/server/fixtures/openapi_complex_input.py
--rw-r--r--  2.0 unx      332 b- defN 24-May-06 20:09 tests/server/fixtures/openapi_custom_output_type.py
--rw-r--r--  2.0 unx      169 b- defN 24-May-06 20:09 tests/server/fixtures/openapi_input_int_choices.py
--rw-r--r--  2.0 unx      153 b- defN 24-May-06 20:09 tests/server/fixtures/openapi_output_list.py
--rw-r--r--  2.0 unx      374 b- defN 24-May-06 20:09 tests/server/fixtures/openapi_output_type.py
--rw-r--r--  2.0 unx      161 b- defN 24-May-06 20:09 tests/server/fixtures/openapi_output_yield.py
--rw-r--r--  2.0 unx      264 b- defN 24-May-06 20:09 tests/server/fixtures/output_complex.py
--rw-r--r--  2.0 unx      148 b- defN 24-May-06 20:09 tests/server/fixtures/output_file.py
--rw-r--r--  2.0 unx      192 b- defN 24-May-06 20:09 tests/server/fixtures/output_file_named.py
--rw-r--r--  2.0 unx      257 b- defN 24-May-06 20:09 tests/server/fixtures/output_iterator_complex.py
--rw-r--r--  2.0 unx      151 b- defN 24-May-06 20:09 tests/server/fixtures/output_numpy.py
--rw-r--r--  2.0 unx      355 b- defN 24-May-06 20:09 tests/server/fixtures/output_path_image.py
--rw-r--r--  2.0 unx      323 b- defN 24-May-06 20:09 tests/server/fixtures/output_path_text.py
--rw-r--r--  2.0 unx      115 b- defN 24-May-06 20:09 tests/server/fixtures/output_wrong_type.py
--rw-r--r--  2.0 unx      175 b- defN 24-May-06 20:09 tests/server/fixtures/setup.py
--rw-r--r--  2.0 unx      262 b- defN 24-May-06 20:09 tests/server/fixtures/setup_uses_async.py
--rw-r--r--  2.0 unx      167 b- defN 24-May-06 20:09 tests/server/fixtures/setup_weights.py
--rw-r--r--  2.0 unx      118 b- defN 24-May-06 20:09 tests/server/fixtures/simple.py
--rw-r--r--  2.0 unx      193 b- defN 24-May-06 20:09 tests/server/fixtures/sleep.py
--rw-r--r--  2.0 unx      219 b- defN 24-May-06 20:09 tests/server/fixtures/slow_predict.py
--rw-r--r--  2.0 unx      122 b- defN 24-May-06 20:09 tests/server/fixtures/slow_setup.py
--rw-r--r--  2.0 unx      290 b- defN 24-May-06 20:09 tests/server/fixtures/steps.py
--rw-r--r--  2.0 unx      359 b- defN 24-May-06 20:09 tests/server/fixtures/train.py
--rw-r--r--  2.0 unx      263 b- defN 24-May-06 20:09 tests/server/fixtures/yield_concatenate_iterator.py
--rw-r--r--  2.0 unx      506 b- defN 24-May-06 20:09 tests/server/fixtures/yield_files.py
--rw-r--r--  2.0 unx      245 b- defN 24-May-06 20:09 tests/server/fixtures/yield_strings.py
--rw-r--r--  2.0 unx      339 b- defN 24-May-06 20:09 tests/server/fixtures/yield_strings_file_input.py
--rw-r--r--  2.0 unx    11347 b- defN 24-May-06 20:10 cog-0.9.7.dist-info/LICENSE
--rw-r--r--  2.0 unx    36704 b- defN 24-May-06 20:10 cog-0.9.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-06 20:10 cog-0.9.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-May-06 20:10 cog-0.9.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     9629 b- defN 24-May-06 20:10 cog-0.9.7.dist-info/RECORD
-109 files, 275617 bytes uncompressed, 80627 bytes compressed:  70.7%
+Zip file size: 96063 bytes, number of entries: 109
+-rw-r--r--  2.0 unx       13 b- defN 24-May-10 17:11 cog/.gitignore
+-rw-r--r--  2.0 unx      384 b- defN 24-May-10 17:11 cog/__init__.py
+-rw-r--r--  2.0 unx      413 b- defN 24-May-10 17:12 cog/_version.py
+-rw-r--r--  2.0 unx    10313 b- defN 24-May-10 17:11 cog/code_xforms.py
+-rw-r--r--  2.0 unx      286 b- defN 24-May-10 17:11 cog/errors.py
+-rw-r--r--  2.0 unx     2124 b- defN 24-May-10 17:11 cog/files.py
+-rw-r--r--  2.0 unx     1945 b- defN 24-May-10 17:11 cog/json.py
+-rw-r--r--  2.0 unx     3171 b- defN 24-May-10 17:11 cog/logging.py
+-rw-r--r--  2.0 unx    17163 b- defN 24-May-10 17:11 cog/predictor.py
+-rw-r--r--  2.0 unx     3308 b- defN 24-May-10 17:11 cog/schema.py
+-rw-r--r--  2.0 unx      645 b- defN 24-May-10 17:11 cog/suppress_output.py
+-rw-r--r--  2.0 unx     8993 b- defN 24-May-10 17:11 cog/types.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-10 17:11 cog/command/__init__.py
+-rw-r--r--  2.0 unx    18782 b- defN 24-May-10 17:11 cog/command/ast_openapi_schema.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-May-10 17:11 cog/command/openapi_schema.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-10 17:11 cog/server/__init__.py
+-rw-r--r--  2.0 unx      593 b- defN 24-May-10 17:11 cog/server/eventtypes.py
+-rw-r--r--  2.0 unx      149 b- defN 24-May-10 17:11 cog/server/exceptions.py
+-rw-r--r--  2.0 unx     5349 b- defN 24-May-10 17:11 cog/server/helpers.py
+-rw-r--r--  2.0 unx    16945 b- defN 24-May-10 17:11 cog/server/http.py
+-rw-r--r--  2.0 unx      971 b- defN 24-May-10 17:11 cog/server/probes.py
+-rw-r--r--  2.0 unx      689 b- defN 24-May-10 17:11 cog/server/response_throttler.py
+-rw-r--r--  2.0 unx    15515 b- defN 24-May-10 17:11 cog/server/runner.py
+-rw-r--r--  2.0 unx     3326 b- defN 24-May-10 17:11 cog/server/webhook.py
+-rw-r--r--  2.0 unx     8050 b- defN 24-May-10 17:11 cog/server/worker.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-10 17:11 tests/__init__.py
+-rw-r--r--  2.0 unx      536 b- defN 24-May-10 17:11 tests/conftest.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-May-10 17:11 tests/test_json.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-May-10 17:11 tests/test_predictor.py
+-rw-r--r--  2.0 unx     4895 b- defN 24-May-10 17:11 tests/test_types.py
+-rw-r--r--  2.0 unx      113 b- defN 24-May-10 17:11 tests/fixtures/argv_override.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-10 17:11 tests/server/__init__.py
+-rw-r--r--  2.0 unx     2800 b- defN 24-May-10 17:11 tests/server/conftest.py
+-rw-r--r--  2.0 unx     2564 b- defN 24-May-10 17:11 tests/server/test_code_xforms.py
+-rw-r--r--  2.0 unx     4692 b- defN 24-May-10 17:11 tests/server/test_helpers.py
+-rw-r--r--  2.0 unx    16956 b- defN 24-May-10 17:11 tests/server/test_http.py
+-rw-r--r--  2.0 unx     9181 b- defN 24-May-10 17:11 tests/server/test_http_input.py
+-rw-r--r--  2.0 unx     4020 b- defN 24-May-10 17:11 tests/server/test_http_output.py
+-rw-r--r--  2.0 unx     2775 b- defN 24-May-10 17:11 tests/server/test_predictor.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-10 17:11 tests/server/test_probes.py
+-rw-r--r--  2.0 unx     1210 b- defN 24-May-10 17:11 tests/server/test_response_throttler.py
+-rw-r--r--  2.0 unx    10931 b- defN 24-May-10 17:11 tests/server/test_runner.py
+-rw-r--r--  2.0 unx     3225 b- defN 24-May-10 17:11 tests/server/test_webhook.py
+-rw-r--r--  2.0 unx    16162 b- defN 24-May-10 17:11 tests/server/test_worker.py
+-rw-r--r--  2.0 unx      209 b- defN 24-May-10 17:11 tests/server/fixtures/async_setup_uses_same_loop_as_predict.py
+-rw-r--r--  2.0 unx      198 b- defN 24-May-10 17:11 tests/server/fixtures/catch_in_predict.py
+-rw-r--r--  2.0 unx      232 b- defN 24-May-10 17:11 tests/server/fixtures/complex_output.py
+-rw-r--r--  2.0 unx      131 b- defN 24-May-10 17:11 tests/server/fixtures/count_up.py
+-rw-r--r--  2.0 unx      136 b- defN 24-May-10 17:11 tests/server/fixtures/exc_in_predict.py
+-rw-r--r--  2.0 unx      133 b- defN 24-May-10 17:11 tests/server/fixtures/exc_in_setup.py
+-rw-r--r--  2.0 unx      151 b- defN 24-May-10 17:11 tests/server/fixtures/exc_in_setup_and_predict.py
+-rw-r--r--  2.0 unx       56 b- defN 24-May-10 17:11 tests/server/fixtures/exc_on_import.py
+-rw-r--r--  2.0 unx      122 b- defN 24-May-10 17:11 tests/server/fixtures/exit_in_predict.py
+-rw-r--r--  2.0 unx      124 b- defN 24-May-10 17:11 tests/server/fixtures/exit_in_setup.py
+-rw-r--r--  2.0 unx       23 b- defN 24-May-10 17:11 tests/server/fixtures/exit_on_import.py
+-rw-r--r--  2.0 unx       58 b- defN 24-May-10 17:11 tests/server/fixtures/function.py
+-rw-r--r--  2.0 unx      159 b- defN 24-May-10 17:11 tests/server/fixtures/hello_world.py
+-rw-r--r--  2.0 unx      197 b- defN 24-May-10 17:11 tests/server/fixtures/input_choices.py
+-rw-r--r--  2.0 unx      153 b- defN 24-May-10 17:11 tests/server/fixtures/input_choices_integer.py
+-rw-r--r--  2.0 unx      139 b- defN 24-May-10 17:11 tests/server/fixtures/input_file.py
+-rw-r--r--  2.0 unx      160 b- defN 24-May-10 17:11 tests/server/fixtures/input_ge_le.py
+-rw-r--r--  2.0 unx      126 b- defN 24-May-10 17:11 tests/server/fixtures/input_integer.py
+-rw-r--r--  2.0 unx      152 b- defN 24-May-10 17:11 tests/server/fixtures/input_integer_default.py
+-rw-r--r--  2.0 unx      317 b- defN 24-May-10 17:11 tests/server/fixtures/input_multiple.py
+-rw-r--r--  2.0 unx      118 b- defN 24-May-10 17:11 tests/server/fixtures/input_none.py
+-rw-r--r--  2.0 unx      236 b- defN 24-May-10 17:11 tests/server/fixtures/input_path.py
+-rw-r--r--  2.0 unx      137 b- defN 24-May-10 17:11 tests/server/fixtures/input_path_2.py
+-rw-r--r--  2.0 unx      159 b- defN 24-May-10 17:11 tests/server/fixtures/input_secret.py
+-rw-r--r--  2.0 unx      125 b- defN 24-May-10 17:11 tests/server/fixtures/input_string.py
+-rw-r--r--  2.0 unx      262 b- defN 24-May-10 17:11 tests/server/fixtures/input_union_integer_or_list_of_integers.py
+-rw-r--r--  2.0 unx      266 b- defN 24-May-10 17:11 tests/server/fixtures/input_union_string_or_list_of_strings.py
+-rw-r--r--  2.0 unx      205 b- defN 24-May-10 17:11 tests/server/fixtures/input_unsupported_type.py
+-rw-r--r--  2.0 unx      122 b- defN 24-May-10 17:11 tests/server/fixtures/input_untyped.py
+-rw-r--r--  2.0 unx      160 b- defN 24-May-10 17:11 tests/server/fixtures/killed_in_predict.py
+-rw-r--r--  2.0 unx      882 b- defN 24-May-10 17:11 tests/server/fixtures/logging.py
+-rw-r--r--  2.0 unx      109 b- defN 24-May-10 17:11 tests/server/fixtures/missing_predict.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-10 17:11 tests/server/fixtures/missing_predictor.py
+-rw-r--r--  2.0 unx      482 b- defN 24-May-10 17:11 tests/server/fixtures/openapi_complex_input.py
+-rw-r--r--  2.0 unx      332 b- defN 24-May-10 17:11 tests/server/fixtures/openapi_custom_output_type.py
+-rw-r--r--  2.0 unx      169 b- defN 24-May-10 17:11 tests/server/fixtures/openapi_input_int_choices.py
+-rw-r--r--  2.0 unx      153 b- defN 24-May-10 17:11 tests/server/fixtures/openapi_output_list.py
+-rw-r--r--  2.0 unx      374 b- defN 24-May-10 17:11 tests/server/fixtures/openapi_output_type.py
+-rw-r--r--  2.0 unx      161 b- defN 24-May-10 17:11 tests/server/fixtures/openapi_output_yield.py
+-rw-r--r--  2.0 unx      264 b- defN 24-May-10 17:11 tests/server/fixtures/output_complex.py
+-rw-r--r--  2.0 unx      148 b- defN 24-May-10 17:11 tests/server/fixtures/output_file.py
+-rw-r--r--  2.0 unx      192 b- defN 24-May-10 17:11 tests/server/fixtures/output_file_named.py
+-rw-r--r--  2.0 unx      257 b- defN 24-May-10 17:11 tests/server/fixtures/output_iterator_complex.py
+-rw-r--r--  2.0 unx      151 b- defN 24-May-10 17:11 tests/server/fixtures/output_numpy.py
+-rw-r--r--  2.0 unx      355 b- defN 24-May-10 17:11 tests/server/fixtures/output_path_image.py
+-rw-r--r--  2.0 unx      323 b- defN 24-May-10 17:11 tests/server/fixtures/output_path_text.py
+-rw-r--r--  2.0 unx      115 b- defN 24-May-10 17:11 tests/server/fixtures/output_wrong_type.py
+-rw-r--r--  2.0 unx      175 b- defN 24-May-10 17:11 tests/server/fixtures/setup.py
+-rw-r--r--  2.0 unx      262 b- defN 24-May-10 17:11 tests/server/fixtures/setup_uses_async.py
+-rw-r--r--  2.0 unx      167 b- defN 24-May-10 17:11 tests/server/fixtures/setup_weights.py
+-rw-r--r--  2.0 unx      118 b- defN 24-May-10 17:11 tests/server/fixtures/simple.py
+-rw-r--r--  2.0 unx      193 b- defN 24-May-10 17:11 tests/server/fixtures/sleep.py
+-rw-r--r--  2.0 unx      219 b- defN 24-May-10 17:11 tests/server/fixtures/slow_predict.py
+-rw-r--r--  2.0 unx      122 b- defN 24-May-10 17:11 tests/server/fixtures/slow_setup.py
+-rw-r--r--  2.0 unx      290 b- defN 24-May-10 17:11 tests/server/fixtures/steps.py
+-rw-r--r--  2.0 unx      359 b- defN 24-May-10 17:11 tests/server/fixtures/train.py
+-rw-r--r--  2.0 unx      263 b- defN 24-May-10 17:11 tests/server/fixtures/yield_concatenate_iterator.py
+-rw-r--r--  2.0 unx      506 b- defN 24-May-10 17:11 tests/server/fixtures/yield_files.py
+-rw-r--r--  2.0 unx      245 b- defN 24-May-10 17:11 tests/server/fixtures/yield_strings.py
+-rw-r--r--  2.0 unx      339 b- defN 24-May-10 17:11 tests/server/fixtures/yield_strings_file_input.py
+-rw-r--r--  2.0 unx    11347 b- defN 24-May-10 17:12 cog-0.9.8a0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    36706 b- defN 24-May-10 17:12 cog-0.9.8a0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-10 17:12 cog-0.9.8a0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-May-10 17:12 cog-0.9.8a0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     9639 b- defN 24-May-10 17:12 cog-0.9.8a0.dist-info/RECORD
+109 files, 275631 bytes uncompressed, 80631 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -306,23 +306,23 @@
 
 Filename: tests/server/fixtures/yield_strings.py
 Comment: 
 
 Filename: tests/server/fixtures/yield_strings_file_input.py
 Comment: 
 
-Filename: cog-0.9.7.dist-info/LICENSE
+Filename: cog-0.9.8a0.dist-info/LICENSE
 Comment: 
 
-Filename: cog-0.9.7.dist-info/METADATA
+Filename: cog-0.9.8a0.dist-info/METADATA
 Comment: 
 
-Filename: cog-0.9.7.dist-info/WHEEL
+Filename: cog-0.9.8a0.dist-info/WHEEL
 Comment: 
 
-Filename: cog-0.9.7.dist-info/top_level.txt
+Filename: cog-0.9.8a0.dist-info/top_level.txt
 Comment: 
 
-Filename: cog-0.9.7.dist-info/RECORD
+Filename: cog-0.9.8a0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cog/_version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '0.9.7'
-__version_tuple__ = version_tuple = (0, 9, 7)
+__version__ = version = '0.9.8a0'
+__version_tuple__ = version_tuple = (0, 9, 8)
```

## Comparing `cog-0.9.7.dist-info/LICENSE` & `cog-0.9.8a0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cog-0.9.7.dist-info/METADATA` & `cog-0.9.8a0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cog
-Version: 0.9.7
+Version: 0.9.8a0
 Summary: Containers for machine learning
 Author-email: Replicate <team@replicate.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

## Comparing `cog-0.9.7.dist-info/RECORD` & `cog-0.9.8a0.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 cog/.gitignore,sha256=OIzCsCr9oYv3wBtJU_TppxWi-OhuDmwCBrrUqcE6kfY,13
 cog/__init__.py,sha256=QcRZ-RsRIoasGN4JsxgKSxfhtMyWbiOCn0sjQAQimB4,384
-cog/_version.py,sha256=4XC29QIe8f6Nj4TIXVcWdhsy0tKD5guALT5XGZC9sso,411
+cog/_version.py,sha256=86viJm00gkhn-XuC4vbew1a8LT1hsIbo2Ny2AICZHkg,413
 cog/code_xforms.py,sha256=ZCiXn1bN5fIoY_GU91mwNeZr7B4rmE_GXiJVcZONyaM,10313
 cog/errors.py,sha256=pB29TjzvXmyqbqi3zPOlLobFJnVWb6GJ9WsLE-77TIQ,286
 cog/files.py,sha256=8PENbdvtuVl6sbgsoZSAHId60TSM8iU-dNMpNPS9h1A,2124
 cog/json.py,sha256=xNwlgqYY7egcHZzcWs94S17q3KbtZVyaDe5gCyZG-Vo,1945
 cog/logging.py,sha256=3I7jOG1HKU5oh6-xJF1dh_qFMJMBrjo9Z60zM6sr3qU,3171
 cog/predictor.py,sha256=4L5lGT89FJAeCo0n4GzM4zy0wwFSEc-1OuokEd2J2AE,17163
 cog/schema.py,sha256=NaVXnqMQ-duhWkS8vomg2NrXhdLn9nEkFKHPnhRtb7A,3308
@@ -98,12 +98,12 @@
 tests/server/fixtures/slow_setup.py,sha256=vHIq6spLzpo-bLmgXlyazLWljQz53JamJDHcpTl_XJo,122
 tests/server/fixtures/steps.py,sha256=WbD27CUVQE8Zj_SVOtOqtleG3Y8meSJVAn-vkhpKst8,290
 tests/server/fixtures/train.py,sha256=5LmmIK9Cd7uSJIIjl-6zZkz4BRNbXCpMW5iBYRXLhKU,359
 tests/server/fixtures/yield_concatenate_iterator.py,sha256=2X582IGdiprIALwIs5e-EZO4i1eBUdM7CI4FCPf-CAo,263
 tests/server/fixtures/yield_files.py,sha256=QpIl1SOFsaakNZJlShl_XkjBGyB_MyuQgv5-J2Vm75U,506
 tests/server/fixtures/yield_strings.py,sha256=7Y9cTGZ7WE0iKlr-ZQmhkeg30mXt-fEpY9U0AQ0QMAQ,245
 tests/server/fixtures/yield_strings_file_input.py,sha256=rNxZHFXLhzqkNiG35JfcyihSA4Lx6s3bp86YRGPztX8,339
-cog-0.9.7.dist-info/LICENSE,sha256=DFJczlBRunZam8mzaMaTNN-4K9KyTIsXadU5_ijFpms,11347
-cog-0.9.7.dist-info/METADATA,sha256=5UWm__Kj3irEYVNfxvp5L86o5ZcdNdSpoYpW1gt56yU,36704
-cog-0.9.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-cog-0.9.7.dist-info/top_level.txt,sha256=gNf7F5ClydQZjQsWAVaX2nQwigQiONHlsrQGZrLOm5U,10
-cog-0.9.7.dist-info/RECORD,,
+cog-0.9.8a0.dist-info/LICENSE,sha256=DFJczlBRunZam8mzaMaTNN-4K9KyTIsXadU5_ijFpms,11347
+cog-0.9.8a0.dist-info/METADATA,sha256=wHFOKWLySzJCNDwVUE3QFVk5qrmawih_n59ELCD_glI,36706
+cog-0.9.8a0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+cog-0.9.8a0.dist-info/top_level.txt,sha256=gNf7F5ClydQZjQsWAVaX2nQwigQiONHlsrQGZrLOm5U,10
+cog-0.9.8a0.dist-info/RECORD,,
```


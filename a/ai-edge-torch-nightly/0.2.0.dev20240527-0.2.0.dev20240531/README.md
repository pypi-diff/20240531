# Comparing `tmp/ai_edge_torch_nightly-0.2.0.dev20240527-py3-none-any.whl.zip` & `tmp/ai_edge_torch_nightly-0.2.0.dev20240531-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,101 +1,109 @@
-Zip file size: 149786 bytes, number of entries: 99
--rw-r--r--  2.0 unx     1008 b- defN 24-May-22 17:27 ai_edge_torch/__init__.py
--rw-r--r--  2.0 unx     4243 b- defN 24-May-22 17:27 ai_edge_torch/model.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/convert/__init__.py
--rw-r--r--  2.0 unx     4043 b- defN 24-May-22 17:27 ai_edge_torch/convert/conversion.py
--rw-r--r--  2.0 unx    11021 b- defN 24-May-22 17:27 ai_edge_torch/convert/conversion_utils.py
--rw-r--r--  2.0 unx     6927 b- defN 24-May-22 17:27 ai_edge_torch/convert/converter.py
--rw-r--r--  2.0 unx     2825 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/__init__.py
--rw-r--r--  2.0 unx     1652 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/_pass_base.py
--rw-r--r--  2.0 unx     6150 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/build_aten_composite_pass.py
--rw-r--r--  2.0 unx     2607 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/build_upsample_bilinear2d_composite_pass.py
--rw-r--r--  2.0 unx     1673 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/canonicalize_pass.py
--rw-r--r--  2.0 unx     2448 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/inject_mlir_debuginfo_pass.py
--rw-r--r--  2.0 unx      795 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/__init__.py
--rw-r--r--  2.0 unx     6870 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_check.py
--rw-r--r--  2.0 unx     1560 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_mark.py
--rw-r--r--  2.0 unx    12438 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_rewrite.py
--rw-r--r--  2.0 unx      982 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/op_func_registry.py
--rw-r--r--  2.0 unx    10030 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/pass_body.py
--rw-r--r--  2.0 unx     2076 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/utils.py
--rw-r--r--  2.0 unx      715 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/__init__.py
--rw-r--r--  2.0 unx     2279 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/greedy.py
--rw-r--r--  2.0 unx     6432 b- defN 24-May-22 17:27 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/min_cut.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/convert/test/__init__.py
--rw-r--r--  2.0 unx     8092 b- defN 24-May-22 17:27 ai_edge_torch/convert/test/test_convert.py
--rw-r--r--  2.0 unx     6403 b- defN 24-May-22 17:27 ai_edge_torch/convert/test/test_convert_composites.py
--rw-r--r--  2.0 unx     4537 b- defN 24-May-22 17:27 ai_edge_torch/convert/test/test_convert_multisig.py
--rw-r--r--  2.0 unx      707 b- defN 24-May-22 17:27 ai_edge_torch/debug/__init__.py
--rw-r--r--  2.0 unx    12789 b- defN 24-May-22 17:27 ai_edge_torch/debug/culprit.py
--rw-r--r--  2.0 unx     1430 b- defN 24-May-22 17:27 ai_edge_torch/debug/utils.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/debug/test/__init__.py
--rw-r--r--  2.0 unx     3731 b- defN 24-May-22 17:27 ai_edge_torch/debug/test/test_culprit.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/experimental/__init__.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/generative/__init__.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/__init__.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/gemma/__init__.py
--rw-r--r--  2.0 unx     2538 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/gemma/convert_to_tflite.py
--rw-r--r--  2.0 unx     5913 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/gemma/gemma.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/phi2/__init__.py
--rw-r--r--  2.0 unx     2512 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/phi2/convert_to_tflite.py
--rw-r--r--  2.0 unx     5540 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/phi2/phi2.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-28 05:28 ai_edge_torch/generative/examples/stable_diffusion/__init__.py
--rw-r--r--  2.0 unx     3535 b- defN 24-May-28 05:28 ai_edge_torch/generative/examples/stable_diffusion/attention.py
--rw-r--r--  2.0 unx     2410 b- defN 24-May-28 05:28 ai_edge_torch/generative/examples/stable_diffusion/clip.py
--rw-r--r--  2.0 unx     3239 b- defN 24-May-28 05:28 ai_edge_torch/generative/examples/stable_diffusion/decoder.py
--rw-r--r--  2.0 unx    16200 b- defN 24-May-28 05:28 ai_edge_torch/generative/examples/stable_diffusion/diffusion.py
--rw-r--r--  2.0 unx     2251 b- defN 24-May-28 05:28 ai_edge_torch/generative/examples/stable_diffusion/encoder.py
--rw-r--r--  2.0 unx     2046 b- defN 24-May-28 05:28 ai_edge_torch/generative/examples/stable_diffusion/util.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/t5/__init__.py
--rw-r--r--  2.0 unx     4536 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/t5/convert_to_tflite.py
--rw-r--r--  2.0 unx    21065 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/t5/t5.py
--rw-r--r--  2.0 unx     8998 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/t5/t5_attention.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/test_models/__init__.py
--rw-r--r--  2.0 unx     3791 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/test_models/toy_model.py
--rw-r--r--  2.0 unx     4831 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/test_models/toy_model_with_kv_cache.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/tiny_llama/__init__.py
--rw-r--r--  2.0 unx     2566 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/tiny_llama/convert_to_tflite.py
--rw-r--r--  2.0 unx     5629 b- defN 24-May-22 17:27 ai_edge_torch/generative/examples/tiny_llama/tiny_llama.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/generative/layers/__init__.py
--rw-r--r--  2.0 unx     9127 b- defN 24-May-22 17:27 ai_edge_torch/generative/layers/attention.py
--rw-r--r--  2.0 unx     6350 b- defN 24-May-22 17:27 ai_edge_torch/generative/layers/attention_utils.py
--rw-r--r--  2.0 unx     3201 b- defN 24-May-22 17:27 ai_edge_torch/generative/layers/builder.py
--rw-r--r--  2.0 unx     2820 b- defN 24-May-22 17:27 ai_edge_torch/generative/layers/feed_forward.py
--rw-r--r--  2.0 unx     3090 b- defN 24-May-22 17:27 ai_edge_torch/generative/layers/kv_cache.py
--rw-r--r--  2.0 unx     4064 b- defN 24-May-22 17:27 ai_edge_torch/generative/layers/model_config.py
--rw-r--r--  2.0 unx     1867 b- defN 24-May-22 17:27 ai_edge_torch/generative/layers/normalization.py
--rw-r--r--  2.0 unx     1383 b- defN 24-May-22 17:27 ai_edge_torch/generative/layers/rotary_position_embedding.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/generative/quantize/__init__.py
--rw-r--r--  2.0 unx     1543 b- defN 24-May-22 17:27 ai_edge_torch/generative/quantize/example.py
--rw-r--r--  2.0 unx     1862 b- defN 24-May-22 17:27 ai_edge_torch/generative/quantize/quant_attrs.py
--rw-r--r--  2.0 unx     3327 b- defN 24-May-22 17:27 ai_edge_torch/generative/quantize/quant_recipe.py
--rw-r--r--  2.0 unx     1913 b- defN 24-May-22 17:27 ai_edge_torch/generative/quantize/quant_recipe_utils.py
--rw-r--r--  2.0 unx     1798 b- defN 24-May-22 17:27 ai_edge_torch/generative/quantize/quant_recipes.py
--rw-r--r--  2.0 unx     1345 b- defN 24-May-22 17:27 ai_edge_torch/generative/quantize/supported_schemes.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/generative/test/__init__.py
--rw-r--r--  2.0 unx     3317 b- defN 24-May-22 17:27 ai_edge_torch/generative/test/loader_test.py
--rw-r--r--  2.0 unx     6500 b- defN 24-May-22 17:27 ai_edge_torch/generative/test/test_model_conversion.py
--rw-r--r--  2.0 unx     3728 b- defN 24-May-22 17:27 ai_edge_torch/generative/test/test_quantize.py
--rw-r--r--  2.0 unx      720 b- defN 24-May-22 17:27 ai_edge_torch/generative/utilities/__init__.py
--rw-r--r--  2.0 unx    10107 b- defN 24-May-22 17:27 ai_edge_torch/generative/utilities/loader.py
--rw-r--r--  2.0 unx    16156 b- defN 24-May-22 17:27 ai_edge_torch/generative/utilities/t5_loader.py
--rw-r--r--  2.0 unx      752 b- defN 24-May-22 17:27 ai_edge_torch/hlfb/__init__.py
--rw-r--r--  2.0 unx     4799 b- defN 24-May-22 17:27 ai_edge_torch/hlfb/mark_pattern/__init__.py
--rw-r--r--  2.0 unx     1539 b- defN 24-May-22 17:27 ai_edge_torch/hlfb/mark_pattern/passes.py
--rw-r--r--  2.0 unx     9206 b- defN 24-May-22 17:27 ai_edge_torch/hlfb/mark_pattern/pattern.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/hlfb/test/__init__.py
--rw-r--r--  2.0 unx     4262 b- defN 24-May-22 17:27 ai_edge_torch/hlfb/test/test_mark_pattern.py
--rw-r--r--  2.0 unx     8190 b- defN 24-May-22 17:27 ai_edge_torch/hlfb/test/test_stablehlo_composite_builder.py
--rw-r--r--  2.0 unx      714 b- defN 24-May-22 17:27 ai_edge_torch/quantize/__init__.py
--rw-r--r--  2.0 unx    15602 b- defN 24-May-22 17:27 ai_edge_torch/quantize/pt2e_quantizer.py
--rw-r--r--  2.0 unx    36046 b- defN 24-May-22 17:27 ai_edge_torch/quantize/pt2e_quantizer_utils.py
--rw-r--r--  2.0 unx     3435 b- defN 24-May-22 17:27 ai_edge_torch/quantize/quant_config.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-22 17:27 ai_edge_torch/testing/__init__.py
--rw-r--r--  2.0 unx      765 b- defN 24-May-22 17:27 ai_edge_torch/testing/model_coverage/__init__.py
--rw-r--r--  2.0 unx     4286 b- defN 24-May-22 17:27 ai_edge_torch/testing/model_coverage/model_coverage.py
--rw-r--r--  2.0 unx    11358 b- defN 24-May-28 19:38 ai_edge_torch_nightly-0.2.0.dev20240527.dist-info/LICENSE
--rw-r--r--  2.0 unx     1748 b- defN 24-May-28 19:38 ai_edge_torch_nightly-0.2.0.dev20240527.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-28 19:38 ai_edge_torch_nightly-0.2.0.dev20240527.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 24-May-28 19:38 ai_edge_torch_nightly-0.2.0.dev20240527.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    10661 b- defN 24-May-28 19:38 ai_edge_torch_nightly-0.2.0.dev20240527.dist-info/RECORD
-99 files, 432486 bytes uncompressed, 132056 bytes compressed:  69.5%
+Zip file size: 161644 bytes, number of entries: 107
+-rw-r--r--  2.0 unx     1008 b- defN 24-May-31 10:14 ai_edge_torch/__init__.py
+-rw-r--r--  2.0 unx     4243 b- defN 24-May-31 10:14 ai_edge_torch/model.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-31 10:14 ai_edge_torch/convert/__init__.py
+-rw-r--r--  2.0 unx     4043 b- defN 24-May-31 10:14 ai_edge_torch/convert/conversion.py
+-rw-r--r--  2.0 unx    11021 b- defN 24-May-31 10:14 ai_edge_torch/convert/conversion_utils.py
+-rw-r--r--  2.0 unx     6927 b- defN 24-May-31 10:14 ai_edge_torch/convert/converter.py
+-rw-r--r--  2.0 unx     2825 b- defN 24-May-31 10:14 ai_edge_torch/convert/fx_passes/__init__.py
+-rw-r--r--  2.0 unx     1652 b- defN 24-May-31 10:14 ai_edge_torch/convert/fx_passes/_pass_base.py
+-rw-r--r--  2.0 unx     6213 b- defN 24-May-31 10:14 ai_edge_torch/convert/fx_passes/build_aten_composite_pass.py
+-rw-r--r--  2.0 unx     2607 b- defN 24-May-31 10:14 ai_edge_torch/convert/fx_passes/build_upsample_bilinear2d_composite_pass.py
+-rw-r--r--  2.0 unx     1673 b- defN 24-May-31 10:14 ai_edge_torch/convert/fx_passes/canonicalize_pass.py
+-rw-r--r--  2.0 unx     2448 b- defN 24-May-31 10:14 ai_edge_torch/convert/fx_passes/inject_mlir_debuginfo_pass.py
+-rw-r--r--  2.0 unx      795 b- defN 24-May-31 10:14 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/__init__.py
+-rw-r--r--  2.0 unx     6870 b- defN 24-May-31 10:14 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_check.py
+-rw-r--r--  2.0 unx     1560 b- defN 24-May-31 10:14 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_mark.py
+-rw-r--r--  2.0 unx    12438 b- defN 24-May-31 10:14 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_rewrite.py
+-rw-r--r--  2.0 unx      982 b- defN 24-May-31 10:14 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/op_func_registry.py
+-rw-r--r--  2.0 unx    10030 b- defN 24-May-31 10:14 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/pass_body.py
+-rw-r--r--  2.0 unx     2076 b- defN 24-May-31 10:14 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/utils.py
+-rw-r--r--  2.0 unx      715 b- defN 24-May-31 10:14 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/__init__.py
+-rw-r--r--  2.0 unx     2279 b- defN 24-May-31 10:14 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/greedy.py
+-rw-r--r--  2.0 unx     6432 b- defN 24-May-31 10:14 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/min_cut.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-31 10:14 ai_edge_torch/convert/test/__init__.py
+-rw-r--r--  2.0 unx     8092 b- defN 24-May-31 10:14 ai_edge_torch/convert/test/test_convert.py
+-rw-r--r--  2.0 unx     6616 b- defN 24-May-31 10:14 ai_edge_torch/convert/test/test_convert_composites.py
+-rw-r--r--  2.0 unx     4537 b- defN 24-May-31 10:14 ai_edge_torch/convert/test/test_convert_multisig.py
+-rw-r--r--  2.0 unx      707 b- defN 24-May-31 10:14 ai_edge_torch/debug/__init__.py
+-rw-r--r--  2.0 unx    12789 b- defN 24-May-31 10:14 ai_edge_torch/debug/culprit.py
+-rw-r--r--  2.0 unx     1430 b- defN 24-May-31 10:14 ai_edge_torch/debug/utils.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-31 10:14 ai_edge_torch/debug/test/__init__.py
+-rw-r--r--  2.0 unx     3731 b- defN 24-May-31 10:14 ai_edge_torch/debug/test/test_culprit.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-31 10:14 ai_edge_torch/experimental/__init__.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-31 10:14 ai_edge_torch/generative/__init__.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/__init__.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/gemma/__init__.py
+-rw-r--r--  2.0 unx     2538 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/gemma/convert_to_tflite.py
+-rw-r--r--  2.0 unx     5913 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/gemma/gemma.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/phi2/__init__.py
+-rw-r--r--  2.0 unx     2512 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/phi2/convert_to_tflite.py
+-rw-r--r--  2.0 unx     5540 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/phi2/phi2.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/stable_diffusion/__init__.py
+-rw-r--r--  2.0 unx     3535 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/stable_diffusion/attention.py
+-rw-r--r--  2.0 unx     2434 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/stable_diffusion/clip.py
+-rw-r--r--  2.0 unx     3633 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/stable_diffusion/convert_to_tflite.py
+-rw-r--r--  2.0 unx     3276 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/stable_diffusion/decoder.py
+-rw-r--r--  2.0 unx    16224 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/stable_diffusion/diffusion.py
+-rw-r--r--  2.0 unx     2341 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/stable_diffusion/encoder.py
+-rw-r--r--  2.0 unx     8277 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/stable_diffusion/pipeline.py
+-rw-r--r--  2.0 unx     3397 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/stable_diffusion/tokenizer.py
+-rw-r--r--  2.0 unx     2397 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/stable_diffusion/util.py
+-rw-r--r--  2.0 unx      830 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/stable_diffusion/samplers/__init__.py
+-rw-r--r--  2.0 unx     2310 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/stable_diffusion/samplers/k_euler.py
+-rw-r--r--  2.0 unx     2513 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/stable_diffusion/samplers/k_euler_ancestral.py
+-rw-r--r--  2.0 unx     2788 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/stable_diffusion/samplers/k_lms.py
+-rw-r--r--  2.0 unx     1340 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/stable_diffusion/samplers/sampler.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/t5/__init__.py
+-rw-r--r--  2.0 unx     4536 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/t5/convert_to_tflite.py
+-rw-r--r--  2.0 unx    21065 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/t5/t5.py
+-rw-r--r--  2.0 unx     8998 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/t5/t5_attention.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/test_models/__init__.py
+-rw-r--r--  2.0 unx     3791 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/test_models/toy_model.py
+-rw-r--r--  2.0 unx     4831 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/test_models/toy_model_with_kv_cache.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/tiny_llama/__init__.py
+-rw-r--r--  2.0 unx     2566 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/tiny_llama/convert_to_tflite.py
+-rw-r--r--  2.0 unx     5629 b- defN 24-May-31 10:14 ai_edge_torch/generative/examples/tiny_llama/tiny_llama.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-31 10:14 ai_edge_torch/generative/layers/__init__.py
+-rw-r--r--  2.0 unx     9127 b- defN 24-May-31 10:14 ai_edge_torch/generative/layers/attention.py
+-rw-r--r--  2.0 unx     6350 b- defN 24-May-31 10:14 ai_edge_torch/generative/layers/attention_utils.py
+-rw-r--r--  2.0 unx     3201 b- defN 24-May-31 10:14 ai_edge_torch/generative/layers/builder.py
+-rw-r--r--  2.0 unx     2820 b- defN 24-May-31 10:14 ai_edge_torch/generative/layers/feed_forward.py
+-rw-r--r--  2.0 unx     3090 b- defN 24-May-31 10:14 ai_edge_torch/generative/layers/kv_cache.py
+-rw-r--r--  2.0 unx     4064 b- defN 24-May-31 10:14 ai_edge_torch/generative/layers/model_config.py
+-rw-r--r--  2.0 unx     1867 b- defN 24-May-31 10:14 ai_edge_torch/generative/layers/normalization.py
+-rw-r--r--  2.0 unx     1383 b- defN 24-May-31 10:14 ai_edge_torch/generative/layers/rotary_position_embedding.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-31 10:14 ai_edge_torch/generative/quantize/__init__.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-May-31 10:14 ai_edge_torch/generative/quantize/example.py
+-rw-r--r--  2.0 unx     1862 b- defN 24-May-31 10:14 ai_edge_torch/generative/quantize/quant_attrs.py
+-rw-r--r--  2.0 unx     3327 b- defN 24-May-31 10:14 ai_edge_torch/generative/quantize/quant_recipe.py
+-rw-r--r--  2.0 unx     1913 b- defN 24-May-31 10:14 ai_edge_torch/generative/quantize/quant_recipe_utils.py
+-rw-r--r--  2.0 unx     1798 b- defN 24-May-31 10:14 ai_edge_torch/generative/quantize/quant_recipes.py
+-rw-r--r--  2.0 unx     1345 b- defN 24-May-31 10:14 ai_edge_torch/generative/quantize/supported_schemes.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-31 10:14 ai_edge_torch/generative/test/__init__.py
+-rw-r--r--  2.0 unx     3317 b- defN 24-May-31 10:14 ai_edge_torch/generative/test/loader_test.py
+-rw-r--r--  2.0 unx     6500 b- defN 24-May-31 10:14 ai_edge_torch/generative/test/test_model_conversion.py
+-rw-r--r--  2.0 unx     3728 b- defN 24-May-31 10:14 ai_edge_torch/generative/test/test_quantize.py
+-rw-r--r--  2.0 unx      720 b- defN 24-May-31 10:14 ai_edge_torch/generative/utilities/__init__.py
+-rw-r--r--  2.0 unx    10107 b- defN 24-May-31 10:14 ai_edge_torch/generative/utilities/loader.py
+-rw-r--r--  2.0 unx    16156 b- defN 24-May-31 10:14 ai_edge_torch/generative/utilities/t5_loader.py
+-rw-r--r--  2.0 unx      752 b- defN 24-May-31 10:14 ai_edge_torch/hlfb/__init__.py
+-rw-r--r--  2.0 unx     4799 b- defN 24-May-31 10:14 ai_edge_torch/hlfb/mark_pattern/__init__.py
+-rw-r--r--  2.0 unx     1539 b- defN 24-May-31 10:14 ai_edge_torch/hlfb/mark_pattern/passes.py
+-rw-r--r--  2.0 unx     9206 b- defN 24-May-31 10:14 ai_edge_torch/hlfb/mark_pattern/pattern.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-31 10:14 ai_edge_torch/hlfb/test/__init__.py
+-rw-r--r--  2.0 unx     4262 b- defN 24-May-31 10:14 ai_edge_torch/hlfb/test/test_mark_pattern.py
+-rw-r--r--  2.0 unx     8190 b- defN 24-May-31 10:14 ai_edge_torch/hlfb/test/test_stablehlo_composite_builder.py
+-rw-r--r--  2.0 unx      714 b- defN 24-May-31 10:14 ai_edge_torch/quantize/__init__.py
+-rw-r--r--  2.0 unx    15602 b- defN 24-May-31 10:14 ai_edge_torch/quantize/pt2e_quantizer.py
+-rw-r--r--  2.0 unx    36046 b- defN 24-May-31 10:14 ai_edge_torch/quantize/pt2e_quantizer_utils.py
+-rw-r--r--  2.0 unx     3435 b- defN 24-May-31 10:14 ai_edge_torch/quantize/quant_config.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-31 10:14 ai_edge_torch/testing/__init__.py
+-rw-r--r--  2.0 unx      765 b- defN 24-May-31 10:14 ai_edge_torch/testing/model_coverage/__init__.py
+-rw-r--r--  2.0 unx     4286 b- defN 24-May-31 10:14 ai_edge_torch/testing/model_coverage/model_coverage.py
+-rw-r--r--  2.0 unx    11358 b- defN 24-May-31 10:14 ai_edge_torch_nightly-0.2.0.dev20240531.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1748 b- defN 24-May-31 10:14 ai_edge_torch_nightly-0.2.0.dev20240531.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-31 10:14 ai_edge_torch_nightly-0.2.0.dev20240531.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-May-31 10:14 ai_edge_torch_nightly-0.2.0.dev20240531.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    11671 b- defN 24-May-31 10:14 ai_edge_torch_nightly-0.2.0.dev20240531.dist-info/RECORD
+107 files, 459386 bytes uncompressed, 142196 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -123,26 +123,50 @@
 
 Filename: ai_edge_torch/generative/examples/stable_diffusion/attention.py
 Comment: 
 
 Filename: ai_edge_torch/generative/examples/stable_diffusion/clip.py
 Comment: 
 
+Filename: ai_edge_torch/generative/examples/stable_diffusion/convert_to_tflite.py
+Comment: 
+
 Filename: ai_edge_torch/generative/examples/stable_diffusion/decoder.py
 Comment: 
 
 Filename: ai_edge_torch/generative/examples/stable_diffusion/diffusion.py
 Comment: 
 
 Filename: ai_edge_torch/generative/examples/stable_diffusion/encoder.py
 Comment: 
 
+Filename: ai_edge_torch/generative/examples/stable_diffusion/pipeline.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/stable_diffusion/tokenizer.py
+Comment: 
+
 Filename: ai_edge_torch/generative/examples/stable_diffusion/util.py
 Comment: 
 
+Filename: ai_edge_torch/generative/examples/stable_diffusion/samplers/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/stable_diffusion/samplers/k_euler.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/stable_diffusion/samplers/k_euler_ancestral.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/stable_diffusion/samplers/k_lms.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/stable_diffusion/samplers/sampler.py
+Comment: 
+
 Filename: ai_edge_torch/generative/examples/t5/__init__.py
 Comment: 
 
 Filename: ai_edge_torch/generative/examples/t5/convert_to_tflite.py
 Comment: 
 
 Filename: ai_edge_torch/generative/examples/t5/t5.py
@@ -276,23 +300,23 @@
 
 Filename: ai_edge_torch/testing/model_coverage/__init__.py
 Comment: 
 
 Filename: ai_edge_torch/testing/model_coverage/model_coverage.py
 Comment: 
 
-Filename: ai_edge_torch_nightly-0.2.0.dev20240527.dist-info/LICENSE
+Filename: ai_edge_torch_nightly-0.2.0.dev20240531.dist-info/LICENSE
 Comment: 
 
-Filename: ai_edge_torch_nightly-0.2.0.dev20240527.dist-info/METADATA
+Filename: ai_edge_torch_nightly-0.2.0.dev20240531.dist-info/METADATA
 Comment: 
 
-Filename: ai_edge_torch_nightly-0.2.0.dev20240527.dist-info/WHEEL
+Filename: ai_edge_torch_nightly-0.2.0.dev20240531.dist-info/WHEEL
 Comment: 
 
-Filename: ai_edge_torch_nightly-0.2.0.dev20240527.dist-info/top_level.txt
+Filename: ai_edge_torch_nightly-0.2.0.dev20240531.dist-info/top_level.txt
 Comment: 
 
-Filename: ai_edge_torch_nightly-0.2.0.dev20240527.dist-info/RECORD
+Filename: ai_edge_torch_nightly-0.2.0.dev20240531.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ai_edge_torch/convert/fx_passes/build_aten_composite_pass.py

```diff
@@ -137,16 +137,19 @@
     # to the default behaviour here.
     if not full_kwargs["stride"]:
       full_kwargs["stride"] = full_kwargs["kernel_size"]
 
     # Only wrap in a composite when the underlying converter can handle it.
     # TODO We should be able to remove this if the converter can inline composites when it can not handle them.
 
-    # We don't cover any cases where ceil_mode is True or divisor_override is set.
-    if full_kwargs["ceil_mode"] or full_kwargs["divisor_override"] is not None:
+    # We don't cover any cases where the divisor_override is set.
+    if full_kwargs["divisor_override"] is not None:
+      return op(*args, **kwargs)
+
+    if full_kwargs["ceil_mode"] and not full_kwargs["count_include_pad"]:
       return op(*args, **kwargs)
 
     # We also can not cover a case where count_include_pad is False but the padding is custom.
     if (
         not full_kwargs["count_include_pad"]
         and not is_valid_padding(full_kwargs["padding"])
         and not is_same_padding(
```

## ai_edge_torch/convert/test/test_convert_composites.py

```diff
@@ -47,14 +47,15 @@
     torch_module = torch.nn.Hardswish().eval()
     edge_model = ai_edge_torch.convert(torch_module, args)
 
     self.assertTrue(model_coverage.compare_tflite_torch(edge_model, torch_module, args))
 
   @parameterized.parameterized.expand(
       [
+          # input_size, kernel_size, stride, padding, ceil_mode, count_include_pad, divisor_override
           # no padding, stride = 1
           ([1, 3, 6, 6], [3, 3], [1, 1], [0, 0], False, True, None),
           # add stride
           ([1, 3, 6, 6], [3, 3], [2, 2], [0, 0], False, True, None),
           # default values
           ([1, 3, 6, 6], [3, 3]),
           # add padding
@@ -63,14 +64,16 @@
           ([1, 3, 6, 6], [3, 3], [1, 1], [0, 1], False, True, None),
           # add both stride and padding
           ([1, 3, 6, 6], [3, 3], [2, 2], [1, 1], False, True, None),
           # count_include_pad = False
           ([1, 3, 6, 6], [3, 3], [1, 1], [1, 1], False, False, None),
           # ceil_mode = True
           ([1, 3, 6, 6], [3, 3], [1, 1], [1, 1], True, True, None),
+          # ceil_mode = True, stride=[3, 3]
+          ([1, 3, 6, 6], [3, 3], [3, 3], [1, 1], True, True, None),
           # set divisor_override
           ([1, 3, 6, 6], [3, 3], [1, 1], 0, False, True, 6),
           # padding set to one number
           ([1, 3, 6, 6], [3, 3], [1, 1], 1, False, True, None),
       ]
   )
   def test_convert_avg_pool2d(self, input_size, *args):
```

## ai_edge_torch/generative/examples/stable_diffusion/clip.py

```diff
@@ -64,14 +64,15 @@
 
   def __init__(self):
     super().__init__()
     self.embedding = CLIPEmbedding(49408, 768, 77)
     self.layers = nn.ModuleList([CLIPLayer(12, 768) for i in range(12)])
     self.layernorm = nn.LayerNorm(768)
 
+  @torch.inference_mode
   def forward(self, tokens: torch.LongTensor) -> torch.FloatTensor:
     tokens = tokens.type(torch.long)
 
     state = self.embedding(tokens)
     for layer in self.layers:
       state = layer(state)
     output = self.layernorm(state)
```

## ai_edge_torch/generative/examples/stable_diffusion/decoder.py

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
+import torch
 from torch import nn
 from torch.nn import functional as F
 
 from ai_edge_torch.generative.examples.stable_diffusion.attention import SelfAttention  # NOQA
 
 
 class AttentionBlock(nn.Module):
@@ -100,12 +101,13 @@
         ResidualBlock(128, 128),
         ResidualBlock(128, 128),
         nn.GroupNorm(32, 128),
         nn.SiLU(),
         nn.Conv2d(128, 3, kernel_size=3, padding=1),
     )
 
+  @torch.inference_mode
   def forward(self, x):
     x = x / 0.18215
     for module in self:
       x = module(x)
     return x
```

## ai_edge_torch/generative/examples/stable_diffusion/diffusion.py

```diff
@@ -425,14 +425,15 @@
 
   def __init__(self):
     super().__init__()
     self.time_embedding = TimeEmbedding(320)
     self.unet = UNet()
     self.final = FinalLayer(320, 4)
 
+  @torch.inference_mode
   def forward(self, latent, context, time):
     time = self.time_embedding(time)
     # print('time:')
     # print(list(time.shape))
     output = self.unet(latent, context, time)
     output = self.final(output)
     return output
```

## ai_edge_torch/generative/examples/stable_diffusion/encoder.py

```diff
@@ -15,14 +15,15 @@
 
 import torch
 from torch import nn
 from torch.nn import functional as F
 
 from ai_edge_torch.generative.examples.stable_diffusion.decoder import AttentionBlock  # NOQA
 from ai_edge_torch.generative.examples.stable_diffusion.decoder import ResidualBlock  # NOQA
+import ai_edge_torch.generative.utilities.loader as loading_utils
 
 
 class Encoder(nn.Sequential):
 
   def __init__(self):
     super().__init__(
         nn.Conv2d(3, 128, kernel_size=3, padding=1),
@@ -42,14 +43,15 @@
         ResidualBlock(512, 512),
         nn.GroupNorm(32, 512),
         nn.SiLU(),
         nn.Conv2d(512, 8, kernel_size=3, padding=1),
         nn.Conv2d(8, 8, kernel_size=1, padding=0),
     )
 
+  @torch.inference_mode
   def forward(self, x, noise):
     for module in self:
       if getattr(module, 'stride', None) == (
           2,
           2,
       ):  # Padding at downsampling should be asymmetric (see #8)
         x = F.pad(x, (0, 1, 0, 1))
```

## ai_edge_torch/generative/examples/stable_diffusion/util.py

```diff
@@ -40,23 +40,32 @@
   parent_location = os.path.dirname(module_location)
   file_location = os.path.join(parent_location, "data", filename)
   return file_location
 
 
 def move_channel(image, to):
   if to == "first":
-    return image.permute(0, 3, 1, 2)  # (N, H, W, C) -> (N, C, H, W)
+    if isinstance(image, torch.Tensor):
+      return image.permute(0, 3, 1, 2)  # (N, H, W, C) -> (N, C, H, W)
+    if isinstance(image, np.ndarray):
+      return image.transpose(0, 3, 1, 2)
   elif to == "last":
-    return image.permute(0, 2, 3, 1)  # (N, C, H, W) -> (N, H, W, C)
+    if isinstance(image, torch.Tensor):
+      return image.permute(0, 2, 3, 1)  # (N, C, H, W) -> (N, H, W, C)
+    if isinstance(image, np.ndarray):
+      return image.transpose(0, 2, 3, 1)
   else:
     raise ValueError("to must be one of the following: first, last")
 
 
 def rescale(x, old_range, new_range, clamp=False):
   old_min, old_max = old_range
   new_min, new_max = new_range
   x -= old_min
   x *= (new_max - new_min) / (old_max - old_min)
   x += new_min
   if clamp:
-    x = x.clamp(new_min, new_max)
+    if isinstance(x, torch.Tensor):
+      x = x.clamp(new_min, new_max)
+    elif isinstance(x, np.ndarray):
+      x = x.clip(new_min, new_max)
   return x
```

## Comparing `ai_edge_torch_nightly-0.2.0.dev20240527.dist-info/LICENSE` & `ai_edge_torch_nightly-0.2.0.dev20240531.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ai_edge_torch_nightly-0.2.0.dev20240527.dist-info/METADATA` & `ai_edge_torch_nightly-0.2.0.dev20240531.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-edge-torch-nightly
-Version: 0.2.0.dev20240527
+Version: 0.2.0.dev20240531
 Summary: Supporting PyTorch models with the Google AI Edge TFLite runtime.
 Home-page: https://github.com/google-ai-edge/ai-edge-torch
 Keywords: On-Device ML,AI,Google,TFLite,PyTorch,LLMs,GenAI
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

## Comparing `ai_edge_torch_nightly-0.2.0.dev20240527.dist-info/RECORD` & `ai_edge_torch_nightly-0.2.0.dev20240531.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ai_edge_torch/model.py,sha256=kmcgELjsYl8YzF8nUF6P7q4i8MWS-pLGpfsy-yTUXmE,4243
 ai_edge_torch/convert/__init__.py,sha256=hHLluseD2R0Hh4W6XZRIXY_dRQeYudjsrKGf6LZz65g,671
 ai_edge_torch/convert/conversion.py,sha256=OlqiB17iTXBxUWX0LX4OU8OmZzLP94STk66LR-QF_V8,4043
 ai_edge_torch/convert/conversion_utils.py,sha256=NpVm3Ms81_cIW5IYgGsr0BVganJJgBKWVBDe5h_ZaGE,11021
 ai_edge_torch/convert/converter.py,sha256=bjj5TV5_g4sGyuSh8ThEDydlNMqhkGSY4SzXK6vwhqI,6927
 ai_edge_torch/convert/fx_passes/__init__.py,sha256=Ll2nNwufjcV5nSruQPXiloq7F1E7pWJ2T5clXmy1lk8,2825
 ai_edge_torch/convert/fx_passes/_pass_base.py,sha256=ijVyDclPnd6a0DWWUJkwR4igj6f82S-cE1-83QGPvgw,1652
-ai_edge_torch/convert/fx_passes/build_aten_composite_pass.py,sha256=quuPsyRtOeumB4SVRYoj2UmSWfrGzJ6Q2ZqjWeG3UPI,6150
+ai_edge_torch/convert/fx_passes/build_aten_composite_pass.py,sha256=wHVWNNMu5h_ya6GnnJn0cNif9xmdSqr8Vm-R7lllxZM,6213
 ai_edge_torch/convert/fx_passes/build_upsample_bilinear2d_composite_pass.py,sha256=76XYoIlFDgrzp5QemoaEalPFcEbfszkEH_PLvO1ASCk,2607
 ai_edge_torch/convert/fx_passes/canonicalize_pass.py,sha256=UX6dJsxCqSkftXXvNBV-i7Bjk6H7qTyqzUnE640Itfg,1673
 ai_edge_torch/convert/fx_passes/inject_mlir_debuginfo_pass.py,sha256=aRT8hTS3n9ie28lgu6mygtFO6Ypwu0qjNb0c81v9HLs,2448
 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/__init__.py,sha256=VA9bekxPVhLk4MYlIRXnOzrSnbCtUmGj7OQ_fJcKQtc,795
 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_check.py,sha256=pG-zLvO5vGs3gjNXa3RxGNwvC-_Azei2anxe2VdKsnY,6870
 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_mark.py,sha256=uXCHC23pWN-3JmDtAErWbSUnL8jjlQgUAy4gqtfDsQU,1560
 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_rewrite.py,sha256=RAgU31B98PQmXEIM3GOjgS0q9aRe2whJhGXpW2EjoqY,12438
@@ -18,15 +18,15 @@
 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/pass_body.py,sha256=wr59GFss8fP8Vy--BaBj34Bto0N16gXxQj6OuTXH8cE,10030
 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/utils.py,sha256=bItkXVaPA9THcFypAmqldpkLuD8WpOFmKlhVbBJJkPk,2076
 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/__init__.py,sha256=B-zisphkH7aRCUOJNdwHnTA0fQXuDpN08q3Qjy5bL6E,715
 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/greedy.py,sha256=8uHJbIwPMTgeSfYVba163pkXSQkHLxFwar_8A1AhgAM,2279
 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/min_cut.py,sha256=FlNKt2EhIKnlVEeUWTiv5sz446YKU6Yy1H0Gd6VRgkU,6432
 ai_edge_torch/convert/test/__init__.py,sha256=hHLluseD2R0Hh4W6XZRIXY_dRQeYudjsrKGf6LZz65g,671
 ai_edge_torch/convert/test/test_convert.py,sha256=USduDO6PaO3nlA82jMihTct--mCU_ugILZDin00lcJ8,8092
-ai_edge_torch/convert/test/test_convert_composites.py,sha256=gFUa_lKNUfeYMgtulqJvRAtWIvzy3f3eXptMBiJDbms,6403
+ai_edge_torch/convert/test/test_convert_composites.py,sha256=SrVn_cEMtQhYYCMOUKK0K7M57MQNQX-lOUwieln0HGA,6616
 ai_edge_torch/convert/test/test_convert_multisig.py,sha256=kMaGnHe9ylfyU68qCifYcaGwJqyejKz--QQt9jS2oUA,4537
 ai_edge_torch/debug/__init__.py,sha256=TKvmnjVk3asvYcVh6C-LPr6srgAF_nppSAupWEXqwPY,707
 ai_edge_torch/debug/culprit.py,sha256=vklaxBUfINdo44OsH7csILK70N41gEThCGchGEfbTZw,12789
 ai_edge_torch/debug/utils.py,sha256=hjVmQVVl1dKxEF0D6KB4a3ouQ3wBkTsebOX2YsUObZM,1430
 ai_edge_torch/debug/test/__init__.py,sha256=hHLluseD2R0Hh4W6XZRIXY_dRQeYudjsrKGf6LZz65g,671
 ai_edge_torch/debug/test/test_culprit.py,sha256=9An_n9p_RWTAYdHYTCO-__EJlbnjclCDo8tDhOzMlwk,3731
 ai_edge_torch/experimental/__init__.py,sha256=hHLluseD2R0Hh4W6XZRIXY_dRQeYudjsrKGf6LZz65g,671
@@ -36,19 +36,27 @@
 ai_edge_torch/generative/examples/gemma/convert_to_tflite.py,sha256=dZv3r24uHsTMokEdnl3nf7LpmV0q7FLnVtCuHn5AuUs,2538
 ai_edge_torch/generative/examples/gemma/gemma.py,sha256=YF4Ua-1lnL3qhQnh1sY5-HlYw2Dq6ZRm227XyDe7WAw,5913
 ai_edge_torch/generative/examples/phi2/__init__.py,sha256=hHLluseD2R0Hh4W6XZRIXY_dRQeYudjsrKGf6LZz65g,671
 ai_edge_torch/generative/examples/phi2/convert_to_tflite.py,sha256=6nOuwx9q3AUlYcjXRRXSr_3M2JKqdJ-vUf-uE3VFYHE,2512
 ai_edge_torch/generative/examples/phi2/phi2.py,sha256=VvigzPQ_LJHeADTsMliwFwPe2BcnOhFgKDqr_WZ2JQ8,5540
 ai_edge_torch/generative/examples/stable_diffusion/__init__.py,sha256=hHLluseD2R0Hh4W6XZRIXY_dRQeYudjsrKGf6LZz65g,671
 ai_edge_torch/generative/examples/stable_diffusion/attention.py,sha256=Lo4Dq7a3Kg-lyH56iqGtqCo5UaClQHRCTDdNagXGTo8,3535
-ai_edge_torch/generative/examples/stable_diffusion/clip.py,sha256=8W4X9PKdnMsWGxXbBfm5OX6mX4XhvaMZ2gZw8yCTScY,2410
-ai_edge_torch/generative/examples/stable_diffusion/decoder.py,sha256=beLCtogA32oYT2nlATpyT-1xzkyPF8zi4v3kfHpw6Mc,3239
-ai_edge_torch/generative/examples/stable_diffusion/diffusion.py,sha256=nnsfgjSeL16U3TVdjTkRycaoWA2ChFeitx2RjGLpwyA,16200
-ai_edge_torch/generative/examples/stable_diffusion/encoder.py,sha256=X6ekByU19KNHNh5OaztZEROv-QwcCwVm1xiJjm2SCoo,2251
-ai_edge_torch/generative/examples/stable_diffusion/util.py,sha256=pG_dsV4xIaB7B8MgoRgSXBvLCVqDlF6bNunPN3GIm-s,2046
+ai_edge_torch/generative/examples/stable_diffusion/clip.py,sha256=KR1Ci4rlJeeGfsFRliCxUve9K7RTJLZfTRMgFtfQ4MU,2434
+ai_edge_torch/generative/examples/stable_diffusion/convert_to_tflite.py,sha256=6REAYy1Bv-Iv5zcmA_m_W6fH6jt5a3IS6Vge18jS_Wo,3633
+ai_edge_torch/generative/examples/stable_diffusion/decoder.py,sha256=AgVAdUbSkHXONVUjAyBQEXhIUUlinf9kNljcBpWnj3A,3276
+ai_edge_torch/generative/examples/stable_diffusion/diffusion.py,sha256=nq94VpQ103eOimnmdyg7u3Xk1LH1IxGlmIbr2AttRIk,16224
+ai_edge_torch/generative/examples/stable_diffusion/encoder.py,sha256=L6hLaMQGb8-_BwSvTLIuDnZwfTqn0K4swBUjfPnYWZo,2341
+ai_edge_torch/generative/examples/stable_diffusion/pipeline.py,sha256=FCbnwlkpYYb-tF7KscbSYjNEdg7XnuLju1cDuIRoQv8,8277
+ai_edge_torch/generative/examples/stable_diffusion/tokenizer.py,sha256=r9RqbyNvuvXOGu3ojtl7ZmbC7o4Pt8aUKAhN1yCdtEc,3397
+ai_edge_torch/generative/examples/stable_diffusion/util.py,sha256=NFpOfA4KN0JpShm5QvuYbQYZ844NzexWD8nV3WjMOZM,2397
+ai_edge_torch/generative/examples/stable_diffusion/samplers/__init__.py,sha256=uQWKzCD_49ackNFrt50H04dkDXxfAwUCtMWWQre5SVE,830
+ai_edge_torch/generative/examples/stable_diffusion/samplers/k_euler.py,sha256=w9C2iVFAn4F2SLJiFdjwR9rRPf5wc3OBS1t0GIOEy08,2310
+ai_edge_torch/generative/examples/stable_diffusion/samplers/k_euler_ancestral.py,sha256=24aIPj6AoK_vSPqmpfmYd-IA8-Uvq6wHLwdVS34Pwtc,2513
+ai_edge_torch/generative/examples/stable_diffusion/samplers/k_lms.py,sha256=iPYX9ZSaxwSak2KI44j6TEr_g4pdxS3xpka4u0trjbo,2788
+ai_edge_torch/generative/examples/stable_diffusion/samplers/sampler.py,sha256=5iRfU5MO6GR6K3WrdddIU_9U7ZZGEEb7zGKVY1WFl-8,1340
 ai_edge_torch/generative/examples/t5/__init__.py,sha256=hHLluseD2R0Hh4W6XZRIXY_dRQeYudjsrKGf6LZz65g,671
 ai_edge_torch/generative/examples/t5/convert_to_tflite.py,sha256=bWtwtUacvJOEDUpuYvLTgkP7oTkXKJA-Tf4FPxlD1Cw,4536
 ai_edge_torch/generative/examples/t5/t5.py,sha256=q2gG5RRo7RgNzvHXYC0Juh6Tgt5d_RTMSWFaYvOKiZU,21065
 ai_edge_torch/generative/examples/t5/t5_attention.py,sha256=anR99IrzR21x6yswFHYG5QQtPDZ7rVicf6STfMp54fU,8998
 ai_edge_torch/generative/examples/test_models/__init__.py,sha256=hHLluseD2R0Hh4W6XZRIXY_dRQeYudjsrKGf6LZz65g,671
 ai_edge_torch/generative/examples/test_models/toy_model.py,sha256=EV07_MEG3fv9g0ZGu9gbBd5BjjrGkxCT1pv7dvhz4TI,3791
 ai_edge_torch/generative/examples/test_models/toy_model_with_kv_cache.py,sha256=MUr6fSj2hBuYSlNbZtrBBpzqB_0WY-l_xYcd_TFFUjY,4831
@@ -88,12 +96,12 @@
 ai_edge_torch/quantize/__init__.py,sha256=aB5dXot04bqyUhpsDFvxt9CIi15QAC4euvqOndJ0XLU,714
 ai_edge_torch/quantize/pt2e_quantizer.py,sha256=ye1f5vAZ0Vr4RWAtfrgU1o3JLs03Sa4inHRq3YxJDGo,15602
 ai_edge_torch/quantize/pt2e_quantizer_utils.py,sha256=yjzKoptnfEeW_sN7sODUfj3nCtUMXVzq3vHKxblsd5Y,36046
 ai_edge_torch/quantize/quant_config.py,sha256=ExThdTXqnWmGC3-F6sdXbXr8nYzkEe_qCziCfhsoMPA,3435
 ai_edge_torch/testing/__init__.py,sha256=hHLluseD2R0Hh4W6XZRIXY_dRQeYudjsrKGf6LZz65g,671
 ai_edge_torch/testing/model_coverage/__init__.py,sha256=5P8J6Zk5YYtDvTBucFvB9NGSRI7Gw_24WnrbhXgycEE,765
 ai_edge_torch/testing/model_coverage/model_coverage.py,sha256=EIyKz-HY70DguWuSrJal8LpYXQ5ZSEUf3ZrVl7jikFM,4286
-ai_edge_torch_nightly-0.2.0.dev20240527.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-ai_edge_torch_nightly-0.2.0.dev20240527.dist-info/METADATA,sha256=nbZoIm0s6CWdrMkaffTrpz-XooKzTR1q0SQ17rs-AKU,1748
-ai_edge_torch_nightly-0.2.0.dev20240527.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ai_edge_torch_nightly-0.2.0.dev20240527.dist-info/top_level.txt,sha256=5KXRaF2hwkApYxf7Y8y_tVb9aulGTlbOoNdbx1aKRkE,14
-ai_edge_torch_nightly-0.2.0.dev20240527.dist-info/RECORD,,
+ai_edge_torch_nightly-0.2.0.dev20240531.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+ai_edge_torch_nightly-0.2.0.dev20240531.dist-info/METADATA,sha256=6KuCs10nnKDOfcImlGIvopbwXSuXdiQnWuBf_iTTs3w,1748
+ai_edge_torch_nightly-0.2.0.dev20240531.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ai_edge_torch_nightly-0.2.0.dev20240531.dist-info/top_level.txt,sha256=5KXRaF2hwkApYxf7Y8y_tVb9aulGTlbOoNdbx1aKRkE,14
+ai_edge_torch_nightly-0.2.0.dev20240531.dist-info/RECORD,,
```


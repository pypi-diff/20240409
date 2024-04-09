# Comparing `tmp/angr-9.2.97.tar.gz` & `tmp/angr-9.2.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angr-9.2.97.tar", last modified: Tue Apr  2 17:02:57 2024, max compression
+gzip compressed data, was "angr-9.2.98.tar", last modified: Tue Apr  9 17:03:02 2024, max compression
```

## Comparing `angr-9.2.97.tar` & `angr-9.2.98.tar`

### file list

```diff
@@ -1,1399 +1,1401 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.082492 angr-9.2.97/
--rw-r--r--   0 vsts      (1001) docker     (127)     1327 2024-04-02 17:01:36.000000 angr-9.2.97/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      107 2024-04-02 17:01:36.000000 angr-9.2.97/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     4769 2024-04-02 17:02:57.082492 angr-9.2.97/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2603 2024-04-02 17:01:36.000000 angr-9.2.97/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.678491 angr-9.2.97/angr/
--rw-r--r--   0 vsts      (1001) docker     (127)     3992 2024-04-02 17:01:44.000000 angr-9.2.97/angr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1887 2024-04-02 17:01:36.000000 angr-9.2.97/angr/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.686491 angr-9.2.97/angr/analyses/
--rw-r--r--   0 vsts      (1001) docker     (127)     1773 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12277 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27287 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/backward_slice.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26267 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/binary_optimizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    51815 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/bindiff.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2448 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/boyscout.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2835 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/callee_cleanup_finder.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40039 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/calling_convention.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6361 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cdg.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.686491 angr-9.2.97/angr/analyses/cfg/
--rw-r--r--   0 vsts      (1001) docker     (127)      321 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15450 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/cfb.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3146 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/cfg.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3112 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/cfg_arch_options.py
--rw-r--r--   0 vsts      (1001) docker     (127)   122546 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/cfg_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)   152842 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/cfg_emulated.py
--rw-r--r--   0 vsts      (1001) docker     (127)   218220 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/cfg_fast.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26047 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/cfg_fast_soot.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5989 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/cfg_job_base.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.690491 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/
--rw-r--r--   0 vsts      (1001) docker     (127)      361 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2083 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/amd64_elf_got.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1777 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/amd64_pe_iat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5231 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/arm_elf_fast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5273 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/const_resolver.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1441 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/default_resolvers.py
--rw-r--r--   0 vsts      (1001) docker     (127)   101955 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/jumptable.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19350 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/mips_elf_fast.py
--rw-r--r--   0 vsts      (1001) docker     (127)      880 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/propagator_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3019 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/resolver.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2971 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/x86_elf_pic_plt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1621 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/x86_pe_iat.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.690491 angr-9.2.97/angr/analyses/cfg_slice_to_sink/
--rw-r--r--   0 vsts      (1001) docker     (127)      120 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg_slice_to_sink/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3982 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg_slice_to_sink/cfg_slice_to_sink.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3560 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg_slice_to_sink/graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg_slice_to_sink/transitions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2969 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/class_identifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3641 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/code_tagging.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18492 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/complete_calling_conventions.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16456 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/congruency_check.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.690491 angr-9.2.97/angr/analyses/data_dep/
--rw-r--r--   0 vsts      (1001) docker     (127)      180 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/data_dep/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25296 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/data_dep/data_dependency_analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4650 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/data_dep/dep_nodes.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1527 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/data_dep/sim_act_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3386 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/datagraph_meta.py
--rw-r--r--   0 vsts      (1001) docker     (127)    63426 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/ddg.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.698491 angr-9.2.97/angr/analyses/decompiler/
--rw-r--r--   0 vsts      (1001) docker     (127)      540 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61504 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/ail_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1595 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/ailgraph_walker.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10576 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/block_io_finder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6531 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/block_similarity.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17199 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/block_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1205 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/call_counter.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15083 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/callsite_maker.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.698491 angr-9.2.97/angr/analyses/decompiler/ccall_rewriters/
--rw-r--r--   0 vsts      (1001) docker     (127)      102 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/ccall_rewriters/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21551 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/ccall_rewriters/amd64_ccalls.py
--rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/ccall_rewriters/rewriter_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)    87477 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/clinic.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49596 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/condition_processor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/decompilation_cache.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8240 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/decompilation_options.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22137 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/decompiler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7368 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/empty_node_remover.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2867 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/expression_counters.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3545 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/expression_narrower.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2485 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/goto_manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16502 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/graph_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1181 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/jump_target_collector.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/jumptable_entry_condition_rewriter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.702491 angr-9.2.97/angr/analyses/decompiler/optimization_passes/
--rw-r--r--   0 vsts      (1001) docker     (127)     3811 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5289 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/base_ptr_save_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15319 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/code_motion.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10593 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/const_derefs.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4033 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/cross_jump_reverter.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17442 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/div_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10388 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/engine_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4701 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/expr_op_swapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3946 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/flip_boolean_cmp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7756 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/ite_expr_converter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6762 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/ite_region_converter.py
--rw-r--r--   0 vsts      (1001) docker     (127)    34328 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/lowered_switch_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3124 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/mod_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10420 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/multi_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14331 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/optimization_pass.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7398 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/register_save_area_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6470 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/ret_addr_save_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7828 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/ret_deduplicator.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18394 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/return_duplicator_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1803 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/return_duplicator_high.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4973 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/return_duplicator_low.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12559 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/stack_canary_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4523 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/switch_default_case_duplicator.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12304 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/win_stack_canary_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/x86_gcc_getpc_simplifier.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.714491 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/
--rw-r--r--   0 vsts      (1001) docker     (127)     3208 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1727 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_div_const_add_a_mul_n_div_const.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1365 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_mul_const_div_shr_const.py
--rw-r--r--   0 vsts      (1001) docker     (127)      988 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_shl_const_sub_a.py
--rw-r--r--   0 vsts      (1001) docker     (127)      953 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2050 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div_const_mul_const.py
--rw-r--r--   0 vsts      (1001) docker     (127)      619 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_sub_a_sub_n.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9333 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/arm_cmpf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3538 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/base.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1056 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_add_n.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_and_mask.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1298 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/bitwise_or_to_logical_or.py
--rw-r--r--   0 vsts      (1001) docker     (127)      991 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/bool_expr_xor_1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6238 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/bswap.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1020 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/coalesce_same_cascading_ifs.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3691 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/const_mull_a_shift.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1583 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/constant_derefs.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2578 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/conv_a_sub0_shr_and.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2070 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/conv_shl_shr.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10131 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/eager_eval.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2015 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/extended_byte_and_mask.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2601 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/inlined_strcpy.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4676 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/inlined_strcpy_consolidation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2084 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/invert_negated_logical_conjuction_disjunction.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1136 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/one_sub_bool.py
--rw-r--r--   0 vsts      (1001) docker     (127)      591 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_cascading_conversions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1560 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_empty_if_body.py
--rw-r--r--   0 vsts      (1001) docker     (127)      739 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_noop_conversions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1635 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_bitmasks.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6583 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_conversions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1189 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_ite_branch.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1869 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_ite_comparisons.py
--rw-r--r--   0 vsts      (1001) docker     (127)      503 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_nots.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1394 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_reinterprets.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1665 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_shifts.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1578 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_shifts_around_comparators.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3327 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/rewrite_bit_extractions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1809 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/rewrite_mips_gp_loads.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2814 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/rol_ror.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5282 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/sar_to_signed_div.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1477 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/simplify_pc_relative_loads.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1837 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/single_bit_cond_to_boolexpr.py
--rw-r--r--   0 vsts      (1001) docker     (127)      940 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/single_bit_xor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4833 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/tidy_stack_addr.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5385 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/redundant_label_remover.py
--rw-r--r--   0 vsts      (1001) docker     (127)    45489 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_identifier.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.714491 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/
--rw-r--r--   0 vsts      (1001) docker     (127)       48 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3721 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/cascading_cond_transformer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2490 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/cascading_ifs.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24008 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/expr_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6032 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/goto.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5034 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/if_.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3681 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/ifelse.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5861 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/loop.py
--rw-r--r--   0 vsts      (1001) docker     (127)      565 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/node_address_finder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8209 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/region_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24545 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/switch_cluster_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3327 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/switch_expr_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)      717 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_walker.py
--rw-r--r--   0 vsts      (1001) docker     (127)      529 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/seq_to_blocks.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8428 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/sequence_walker.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.714491 angr-9.2.97/angr/analyses/decompiler/structured_codegen/
--rw-r--r--   0 vsts      (1001) docker     (127)      290 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structured_codegen/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3845 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structured_codegen/base.py
--rw-r--r--   0 vsts      (1001) docker     (127)   135109 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structured_codegen/c.py
--rw-r--r--   0 vsts      (1001) docker     (127)      535 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structured_codegen/dummy.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6773 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structured_codegen/dwarf_import.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.718491 angr-9.2.97/angr/analyses/decompiler/structuring/
--rw-r--r--   0 vsts      (1001) docker     (127)      371 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structuring/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    48400 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structuring/dream.py
--rw-r--r--   0 vsts      (1001) docker     (127)   119472 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structuring/phoenix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7078 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structuring/recursive_structurer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41330 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structuring/structurer_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11964 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structuring/structurer_nodes.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27930 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    45941 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/disassembly.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2989 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/disassembly_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1245 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/dominance_frontier.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10158 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/find_objects_static.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7847 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/flirt.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.718491 angr-9.2.97/angr/analyses/forward_analysis/
--rw-r--r--   0 vsts      (1001) docker     (127)      144 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/forward_analysis/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19939 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/forward_analysis/forward_analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1579 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/forward_analysis/job_info.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.718491 angr-9.2.97/angr/analyses/forward_analysis/visitors/
--rw-r--r--   0 vsts      (1001) docker     (127)      174 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/forward_analysis/visitors/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      713 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/forward_analysis/visitors/call_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2739 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/forward_analysis/visitors/function_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8067 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/forward_analysis/visitors/graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)      711 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/forward_analysis/visitors/loop.py
--rw-r--r--   0 vsts      (1001) docker     (127)      768 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/forward_analysis/visitors/single_node_graph.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.722491 angr-9.2.97/angr/analyses/identifier/
--rw-r--r--   0 vsts      (1001) docker     (127)       33 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4757 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/custom_callable.py
--rw-r--r--   0 vsts      (1001) docker     (127)      157 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/errors.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1749 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/func.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.726491 angr-9.2.97/angr/analyses/identifier/functions/
--rw-r--r--   0 vsts      (1001) docker     (127)     1059 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2110 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/atoi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3294 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/based_atoi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4353 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/fdprintf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1941 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/free.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8665 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/int2str.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3845 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/malloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1953 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/memcmp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3166 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/memcpy.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1188 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/memset.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4307 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/printf.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11564 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/recv_until.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2356 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/skip_calloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3186 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/skip_realloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2886 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/skip_recv_n.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4179 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/snprintf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4119 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/sprintf.py
--rw-r--r--   0 vsts      (1001) docker     (127)      806 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/strcasecmp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3459 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/strcmp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1187 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/strcpy.py
--rw-r--r--   0 vsts      (1001) docker     (127)      753 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/strlen.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3297 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/strncmp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2008 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/strncpy.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2426 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/strtol.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33287 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/identify.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13739 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/runner.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8531 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/init_finder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9412 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/loop_analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7122 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/loopfinder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.726491 angr-9.2.97/angr/analyses/propagator/
--rw-r--r--   0 vsts      (1001) docker     (127)       43 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/propagator/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    68660 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/propagator/engine_ail.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1735 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/propagator/engine_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12491 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/propagator/engine_vex.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6890 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/propagator/outdated_definition_walker.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16134 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/propagator/propagator.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/propagator/tmpvar_finder.py
--rw-r--r--   0 vsts      (1001) docker     (127)      359 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/propagator/top_checker_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/propagator/values.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1433 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/propagator/vex_vars.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16323 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/proximity_graph.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.730491 angr-9.2.97/angr/analyses/reaching_definitions/
--rw-r--r--   0 vsts      (1001) docker     (127)     1989 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2217 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/call_trace.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14886 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/dep_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)    45997 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/engine_ail.py
--rw-r--r--   0 vsts      (1001) docker     (127)    42934 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/engine_vex.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/external_codeloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26839 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/function_handler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2634 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/heap_allocator.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11224 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/rd_initializer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23986 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/rd_state.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23988 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/reaching_definitions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1995 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/subject.py
--rw-r--r--   0 vsts      (1001) docker     (127)   100412 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reassembler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8941 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/soot_class_hierarchy.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29868 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/stack_pointer_tracker.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1711 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/static_hooker.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.730491 angr-9.2.97/angr/analyses/typehoon/
--rw-r--r--   0 vsts      (1001) docker     (127)       31 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/typehoon/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3519 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/typehoon/dfa.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2805 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/typehoon/lifter.py
--rw-r--r--   0 vsts      (1001) docker     (127)    48619 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/typehoon/simple_solver.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8610 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/typehoon/translator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7030 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/typehoon/typeconsts.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9353 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/typehoon/typehoon.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15783 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/typehoon/typevars.py
--rw-r--r--   0 vsts      (1001) docker     (127)      158 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/typehoon/variance.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.734491 angr-9.2.97/angr/analyses/variable_recovery/
--rw-r--r--   0 vsts      (1001) docker     (127)      105 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/variable_recovery/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1403 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/variable_recovery/annotations.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25716 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/variable_recovery/engine_ail.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41633 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/variable_recovery/engine_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19046 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/variable_recovery/engine_vex.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4701 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/variable_recovery/irsb_scanner.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21802 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/variable_recovery/variable_recovery.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14960 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/variable_recovery/variable_recovery_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24125 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/variable_recovery/variable_recovery_fast.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25224 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/veritesting.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75256 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/vfg.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16173 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/vsa_ddg.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3874 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/vtable.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9714 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/xrefs.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.734491 angr-9.2.97/angr/angrdb/
--rw-r--r--   0 vsts      (1001) docker     (127)      231 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6459 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/db.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4750 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/models.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.738491 angr-9.2.97/angr/angrdb/serializers/
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/serializers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1297 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/serializers/cfg_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1531 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/serializers/comments.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1696 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/serializers/funcs.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3688 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/serializers/kb.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1425 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/serializers/labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2494 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/serializers/loader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4190 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/serializers/structured_code.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2383 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/serializers/variables.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1180 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/serializers/xrefs.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10818 2024-04-02 17:01:36.000000 angr-9.2.97/angr/annocfg.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15519 2024-04-02 17:01:36.000000 angr-9.2.97/angr/blade.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14468 2024-04-02 17:01:36.000000 angr-9.2.97/angr/block.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6034 2024-04-02 17:01:36.000000 angr-9.2.97/angr/callable.py
--rw-r--r--   0 vsts      (1001) docker     (127)    91291 2024-04-02 17:01:36.000000 angr-9.2.97/angr/calling_conventions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5476 2024-04-02 17:01:36.000000 angr-9.2.97/angr/code_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3784 2024-04-02 17:01:36.000000 angr-9.2.97/angr/codenode.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.742491 angr-9.2.97/angr/concretization_strategies/
--rw-r--r--   0 vsts      (1001) docker     (127)     3727 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      438 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/any.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1341 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/any_named.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2218 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/controlled_data.py
--rw-r--r--   0 vsts      (1001) docker     (127)      617 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/eval.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/logging.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1035 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/max.py
--rw-r--r--   0 vsts      (1001) docker     (127)      536 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/nonzero.py
--rw-r--r--   0 vsts      (1001) docker     (127)      784 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/nonzero_range.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1435 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/norepeats.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1564 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/norepeats_range.py
--rw-r--r--   0 vsts      (1001) docker     (127)      555 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/range.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/signed_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/single.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/solutions.py
--rw-r--r--   0 vsts      (1001) docker     (127)      529 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/unlimited_range.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.742491 angr-9.2.97/angr/distributed/
--rw-r--r--   0 vsts      (1001) docker     (127)      140 2024-04-02 17:01:36.000000 angr-9.2.97/angr/distributed/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6682 2024-04-02 17:01:36.000000 angr-9.2.97/angr/distributed/server.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6075 2024-04-02 17:01:36.000000 angr-9.2.97/angr/distributed/worker.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.742491 angr-9.2.97/angr/engines/
--rw-r--r--   0 vsts      (1001) docker     (127)     1066 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7468 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/concrete.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8109 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/engine.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/failure.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2546 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/hook.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.746491 angr-9.2.97/angr/engines/light/
--rw-r--r--   0 vsts      (1001) docker     (127)      186 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/light/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23132 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/light/data.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40918 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/light/engine.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.746491 angr-9.2.97/angr/engines/pcode/
--rw-r--r--   0 vsts      (1001) docker     (127)       83 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/pcode/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28720 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/pcode/behavior.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2994 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/pcode/cc.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16718 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/pcode/emulate.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10551 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/pcode/engine.py
--rw-r--r--   0 vsts      (1001) docker     (127)    52362 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/pcode/lifter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/procedure.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.746491 angr-9.2.97/angr/engines/soot/
--rw-r--r--   0 vsts      (1001) docker     (127)       30 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17238 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/engine.py
--rw-r--r--   0 vsts      (1001) docker     (127)      221 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.754491 angr-9.2.97/angr/engines/soot/expressions/
--rw-r--r--   0 vsts      (1001) docker     (127)     1706 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      857 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/arrayref.py
--rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/base.py
--rw-r--r--   0 vsts      (1001) docker     (127)      781 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/binop.py
--rw-r--r--   0 vsts      (1001) docker     (127)      753 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/cast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1260 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/condition.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1387 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)      313 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/instanceOf.py
--rw-r--r--   0 vsts      (1001) docker     (127)      234 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/instancefieldref.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4525 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/invoke.py
--rw-r--r--   0 vsts      (1001) docker     (127)      189 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/length.py
--rw-r--r--   0 vsts      (1001) docker     (127)      215 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/local.py
--rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/new.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1970 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/newArray.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3400 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/newMultiArray.py
--rw-r--r--   0 vsts      (1001) docker     (127)      224 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/paramref.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1192 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/phi.py
--rw-r--r--   0 vsts      (1001) docker     (127)      232 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/staticfieldref.py
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/thisref.py
--rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/unsupported.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1940 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/field_dispatcher.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1780 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/method_dispatcher.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.762491 angr-9.2.97/angr/engines/soot/statements/
--rw-r--r--   0 vsts      (1001) docker     (127)      893 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/statements/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1271 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/statements/assign.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2094 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/statements/base.py
--rw-r--r--   0 vsts      (1001) docker     (127)      325 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/statements/goto.py
--rw-r--r--   0 vsts      (1001) docker     (127)      421 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/statements/identity.py
--rw-r--r--   0 vsts      (1001) docker     (127)      560 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/statements/if_.py
--rw-r--r--   0 vsts      (1001) docker     (127)      284 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/statements/invoke.py
--rw-r--r--   0 vsts      (1001) docker     (127)      466 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/statements/return_.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1301 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/statements/switch.py
--rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/statements/throw.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.766491 angr-9.2.97/angr/engines/soot/values/
--rw-r--r--   0 vsts      (1001) docker     (127)      792 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/values/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4427 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/values/arrayref.py
--rw-r--r--   0 vsts      (1001) docker     (127)      121 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/values/base.py
--rw-r--r--   0 vsts      (1001) docker     (127)      403 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/values/constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1593 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/values/instancefieldref.py
--rw-r--r--   0 vsts      (1001) docker     (127)      385 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/values/local.py
--rw-r--r--   0 vsts      (1001) docker     (127)      413 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/values/paramref.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1240 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/values/staticfieldref.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1107 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/values/strref.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5739 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/values/thisref.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23679 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/successors.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2177 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/syscall.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24447 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/unicorn.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.766491 angr-9.2.97/angr/engines/vex/
--rw-r--r--   0 vsts      (1001) docker     (127)       95 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.766491 angr-9.2.97/angr/engines/vex/claripy/
--rw-r--r--   0 vsts      (1001) docker     (127)       40 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/claripy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    82570 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/claripy/ccall.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5123 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/claripy/datalayer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    46171 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/claripy/irop.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.770491 angr-9.2.97/angr/engines/vex/heavy/
--rw-r--r--   0 vsts      (1001) docker     (127)      201 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/heavy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8871 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/heavy/actions.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14702 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/heavy/concretizers.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18699 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/heavy/dirty.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15822 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/heavy/heavy.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2317 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/heavy/inspect.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3737 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/heavy/resilience.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1180 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/heavy/super_fastpath.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17132 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/lifter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.770491 angr-9.2.97/angr/engines/vex/light/
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/light/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21729 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/light/light.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2002 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/light/resilience.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2023 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/light/slicing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8299 2024-04-02 17:01:36.000000 angr-9.2.97/angr/errors.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.774491 angr-9.2.97/angr/exploration_techniques/
--rw-r--r--   0 vsts      (1001) docker     (127)     6980 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2588 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/bucketizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2262 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1167 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/dfs.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17917 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/director.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3531 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/driller_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6163 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/explorer.py
--rw-r--r--   0 vsts      (1001) docker     (127)      550 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/lengthlimiter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2583 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/local_loop_seer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11640 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/loop_seer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3091 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/manual_mergepoint.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1271 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/memory_watcher.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3520 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/oppologist.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5126 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/slicecutor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9382 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/spiller.py
--rw-r--r--   0 vsts      (1001) docker     (127)      818 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/spiller_db.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2059 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/stochastic.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6969 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/suggestions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3122 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/symbion.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1586 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/tech_builder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2976 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/threading.py
--rw-r--r--   0 vsts      (1001) docker     (127)      923 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/timeout.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50249 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/tracer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4413 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/unique.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1350 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/veritesting.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17411 2024-04-02 17:01:36.000000 angr-9.2.97/angr/factory.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.774491 angr-9.2.97/angr/flirt/
--rw-r--r--   0 vsts      (1001) docker     (127)     4428 2024-04-02 17:01:36.000000 angr-9.2.97/angr/flirt/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10109 2024-04-02 17:01:36.000000 angr-9.2.97/angr/flirt/build_sig.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:36.000000 angr-9.2.97/angr/graph_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18129 2024-04-02 17:01:36.000000 angr-9.2.97/angr/keyed_region.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.778491 angr-9.2.97/angr/knowledge_base/
--rw-r--r--   0 vsts      (1001) docker     (127)       42 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_base/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4623 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_base/knowledge_base.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.778491 angr-9.2.97/angr/knowledge_plugins/
--rw-r--r--   0 vsts      (1001) docker     (127)      697 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1597 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/callsite_prototypes.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.778491 angr-9.2.97/angr/knowledge_plugins/cfg/
--rw-r--r--   0 vsts      (1001) docker     (127)      382 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/cfg/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2302 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/cfg/cfg_manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41756 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/cfg/cfg_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17229 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/cfg/cfg_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2145 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/cfg/indirect_jump.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5040 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/cfg/memory_data.py
--rw-r--r--   0 vsts      (1001) docker     (127)      304 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/comments.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1027 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/custom_strings.py
--rw-r--r--   0 vsts      (1001) docker     (127)      839 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/data.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8189 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/debug_variables.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.782491 angr-9.2.97/angr/knowledge_plugins/functions/
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/functions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    66932 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/functions/function.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18990 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/functions/function_manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11916 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/functions/function_parser.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4971 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/functions/soot_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1024 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/indirect_jumps.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.786491 angr-9.2.97/angr/knowledge_plugins/key_definitions/
--rw-r--r--   0 vsts      (1001) docker     (127)      397 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9753 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/atoms.py
--rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8661 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/definition.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3907 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/environment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      922 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/heap_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3251 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/key_definition_manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40482 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/live_definitions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7140 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/liveness.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7312 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/rd_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1682 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/tag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1236 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/undefined.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1510 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/unknown_size.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7468 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/uses.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3137 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4373 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/patches.py
--rw-r--r--   0 vsts      (1001) docker     (127)      733 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/plugin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.786491 angr-9.2.97/angr/knowledge_plugins/propagations/
--rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/propagations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7706 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/propagations/prop_value.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2122 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/propagations/propagation_manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2786 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/propagations/propagation_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39023 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/propagations/states.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.786491 angr-9.2.97/angr/knowledge_plugins/structured_code/
--rw-r--r--   0 vsts      (1001) docker     (127)       43 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/structured_code/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2071 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/structured_code/manager.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.786491 angr-9.2.97/angr/knowledge_plugins/sync/
--rw-r--r--   0 vsts      (1001) docker     (127)       44 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/sync/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9276 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/sync/sync_controller.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2038 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.786491 angr-9.2.97/angr/knowledge_plugins/variables/
--rw-r--r--   0 vsts      (1001) docker     (127)       60 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/variables/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3751 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/variables/variable_access.py
--rw-r--r--   0 vsts      (1001) docker     (127)    45603 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/variables/variable_manager.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.794491 angr-9.2.97/angr/knowledge_plugins/xrefs/
--rw-r--r--   0 vsts      (1001) docker     (127)       94 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/xrefs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4963 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/xrefs/xref.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4009 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/xrefs/xref_manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)      271 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/xrefs/xref_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.798491 angr-9.2.97/angr/misc/
--rw-r--r--   0 vsts      (1001) docker     (127)      237 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      807 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/ansi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3426 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/autoimport.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4241 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/bug_report.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4486 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/hookset.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1943 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/import_hooks.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4225 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/loggers.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1276 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/picklable_lock.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9370 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/plugins.py
--rw-r--r--   0 vsts      (1001) docker     (127)      509 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/range.py
--rw-r--r--   0 vsts      (1001) docker     (127)      593 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/testing.py
--rw-r--r--   0 vsts      (1001) docker     (127)      701 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/ux.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1453 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/weakpatch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.798491 angr-9.2.97/angr/procedures/
--rw-r--r--   0 vsts      (1001) docker     (127)      119 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.798491 angr-9.2.97/angr/procedures/advapi32/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/advapi32/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.798491 angr-9.2.97/angr/procedures/cgc/
--rw-r--r--   0 vsts      (1001) docker     (127)       76 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/cgc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      224 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/cgc/_terminate.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3371 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/cgc/allocate.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1984 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/cgc/deallocate.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2802 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/cgc/fdwait.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2334 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/cgc/random.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3758 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/cgc/receive.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2368 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/cgc/transmit.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.946492 angr-9.2.97/angr/procedures/definitions/
--rw-r--r--   0 vsts      (1001) docker     (127)    32023 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/cgc.py
--rw-r--r--   0 vsts      (1001) docker     (127)   394191 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/glibc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/gnulib.py
--rw-r--r--   0 vsts      (1001) docker     (127)      700 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/libstdcpp.py
--rw-r--r--   0 vsts      (1001) docker     (127)   238887 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/linux_kernel.py
--rw-r--r--   0 vsts      (1001) docker     (127)      219 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/linux_loader.py
--rw-r--r--   0 vsts      (1001) docker     (127)      601 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/msvcr.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1795 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/parse_syscalls_from_local_system.py
--rw-r--r--   0 vsts      (1001) docker     (127)   110573 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/parse_win32json.py
--rw-r--r--   0 vsts      (1001) docker     (127)  9998064 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/types_win32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1458 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_api-ms-win-dx-d3dkmt-l1-1-4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1000 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_api-ms-win-dx-d3dkmt-l1-1-6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22852 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_clfs.py
--rw-r--r--   0 vsts      (1001) docker     (127)   111981 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_fltmgr.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1730 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_fwpkclnt.py
--rw-r--r--   0 vsts      (1001) docker     (127)    68446 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_fwpuclnt.py
--rw-r--r--   0 vsts      (1001) docker     (127)    37307 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_gdi32.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11415 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_hal.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12527 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_ksecdd.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33948 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_ndis.py
--rw-r--r--   0 vsts      (1001) docker     (127)   593050 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_ntoskrnl.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9862 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_offreg.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1980 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_pshed.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3478 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_secur32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1942 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_vhfum.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1553 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_aclui.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7877 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_activeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)   310929 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_advapi32.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22314 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_advpack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3430 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_amsi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3769 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3051 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-3.py
--rw-r--r--   0 vsts      (1001) docker     (127)      922 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-6.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-apiquery-l2-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1060 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-backgroundtask-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1134 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1167 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1488 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-enclave-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1037 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-errorhandling-l1-1-3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2317 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1217 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4874 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-file-fromapp-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1125 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-handle-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5164 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-ioring-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2219 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-marshal-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2528 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1492 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-5.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3867 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-6.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2362 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-7.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2378 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-8.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8406 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-path-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1547 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1562 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1429 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1850 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1281 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-slapi-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1682 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-state-helpers-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1540 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-synch-l1-2-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)      995 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1184 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1467 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-4.py
--rw-r--r--   0 vsts      (1001) docker     (127)      951 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-6.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1537 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-util-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3268 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3777 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3228 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1162 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-registration-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)      901 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-robuffer-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1694 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-roparameterizediid-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10986 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1550 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1653 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-wow64-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6949 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6680 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-dx-d3dkmt-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1043 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-deviceinformation-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1347 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-expandedresources-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3983 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1753 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5014 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2233 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4359 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1207 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-mm-misc-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3912 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-net-isolation-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1434 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-security-base-l1-2-2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1041 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1100 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1289 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1344 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1833 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-5.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1687 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2545 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)      994 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1817 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-shcore-stream-winrt-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3586 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-wsl-api-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1117 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_apphelp.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17589 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_authz.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2884 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_avicap32.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18938 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_avifil32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5529 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_avrt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1328 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_bcp47mrm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24333 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_bcrypt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1325 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_bcryptprimitives.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17641 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_bluetoothapis.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10950 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_bthprops.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3094 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_bthprops_cpl.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16642 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_cabinet.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6820 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_certadm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4345 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_certpoleng.py
--rw-r--r--   0 vsts      (1001) docker     (127)   101560 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_cfgmgr32.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26407 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_chakra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14271 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_cldapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24138 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_clfsw32.py
--rw-r--r--   0 vsts      (1001) docker     (127)   111741 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_clusapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43365 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_comctl32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4894 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_comdlg32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2651 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_compstui.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19474 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_computecore.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16032 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_computenetwork.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4405 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_computestorage.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2241 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_comsvcs.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1201 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_coremessaging.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11823 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_credui.py
--rw-r--r--   0 vsts      (1001) docker     (127)   105559 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_crypt32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3864 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_cryptnet.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4935 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_cryptui.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9065 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_cryptxml.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1769 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_cscapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5253 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_d2d1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11546 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_d3d10.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_d3d10_1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3575 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_d3d11.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4078 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_d3d12.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3002 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_d3d9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13432 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_d3dcompiler_47.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4827 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_d3dcsx.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7266 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_davclnt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2063 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dbgeng.py
--rw-r--r--   0 vsts      (1001) docker     (127)   109042 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dbghelp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1028 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dbgmodel.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7151 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dciman32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4837 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dcomp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4233 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ddraw.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1134 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_deviceaccess.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1145 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dflayout.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5570 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dhcpcsvc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2967 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dhcpcsvc6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    81410 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dhcpsapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13697 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_diagnosticdataquery.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1243 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dinput8.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1621 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_directml.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1261 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dmprocessxmlfiltered.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22815 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dnsapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5579 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_drt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3373 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_drtprov.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1445 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_drttransport.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5367 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dsound.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11582 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dsparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2935 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dsprop.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6189 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dssec.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1855 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dsuiext.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9715 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dwmapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1120 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dwrite.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1484 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dxcompiler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1061 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dxcore.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2185 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dxgi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14554 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dxva2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10117 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_eappcfg.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9178 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_eappprxy.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1311 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_efswrt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2446 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_elscore.py
--rw-r--r--   0 vsts      (1001) docker     (127)   105927 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_esent.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3146 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_evr.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1687 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_faultrep.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2401 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_fhsvcctl.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2011 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_firewallapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12020 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_fltlib.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4105 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_fontsub.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1227 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_forceinline.py
--rw-r--r--   0 vsts      (1001) docker     (127)    93548 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_fwpuclnt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1129 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_fxsutility.py
--rw-r--r--   0 vsts      (1001) docker     (127)   148174 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_gdi32.py
--rw-r--r--   0 vsts      (1001) docker     (127)   247483 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_gdiplus.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16771 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_glu32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2162 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_gpedit.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1678 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_hhctrl_ocx.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21797 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_hid.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12512 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_hlink.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1027 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_hrtfapo.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19733 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_httpapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12533 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_icm32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1161 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_icmui.py
--rw-r--r--   0 vsts      (1001) docker     (127)   373759 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_icu.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10129 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ieframe.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11559 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_imagehlp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3884 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_imgutil.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28246 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_imm32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8100 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_infocardapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8943 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_inkobjcore.py
--rw-r--r--   0 vsts      (1001) docker     (127)    65729 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_iphlpapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28599 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_iscsidsc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1293 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_isolatedwindowsenvironmentutils.py
--rw-r--r--   0 vsts      (1001) docker     (127)   505053 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_kernel32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3158 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_kernelbase.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2060 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_keycredmgr.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3689 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ksproxy_ax.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4328 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ksuser.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14607 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ktmw32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1582 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_licenseprotection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4334 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_loadperf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6878 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_magnification.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25169 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mapi32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1411 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mdmlocalmanagement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4765 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mdmregistration.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17507 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1358 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mfcore.py
--rw-r--r--   0 vsts      (1001) docker     (127)    45685 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mfplat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1326 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mfplay.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2429 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mfreadwrite.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4363 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mfsensorgroup.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1451 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mfsrcsnk.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4531 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mgmtapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1232 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1326 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mmdevapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19241 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mpr.py
--rw-r--r--   0 vsts      (1001) docker     (127)    47666 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mprapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13037 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mqrt.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11736 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mrmsupport.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19430 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msacm32.py
--rw-r--r--   0 vsts      (1001) docker     (127)   183424 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msajapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    34895 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mscms.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11975 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mscoree.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1327 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msctfmonitor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7687 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msdelta.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4589 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msdmo.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39076 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msdrm.py
--rw-r--r--   0 vsts      (1001) docker     (127)   103106 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2796 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msimg32.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11181 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mspatcha.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6011 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mspatchc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2844 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msports.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7471 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msrating.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7594 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mssign32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mstask.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16749 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msvfw32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9190 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mswsock.py
--rw-r--r--   0 vsts      (1001) docker     (127)      973 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mtxdm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19693 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ncrypt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6200 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ndfapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86057 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_netapi32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3436 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_netsh.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1151 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_netshell.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6101 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_newdev.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11168 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ninput.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_normaliz.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27742 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ntdll.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1087 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ntdllk.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35639 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ntdsapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4407 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ntlanman.py
--rw-r--r--   0 vsts      (1001) docker     (127)    94760 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_odbc32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8509 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_odbcbcp.py
--rw-r--r--   0 vsts      (1001) docker     (127)   103812 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ole32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7007 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_oleacc.py
--rw-r--r--   0 vsts      (1001) docker     (127)   123410 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_oleaut32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6811 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_oledlg.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2609 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ondemandconnroutehelper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75467 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_opengl32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1461 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_opmxbox.py
--rw-r--r--   0 vsts      (1001) docker     (127)    32523 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_p2p.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12455 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_p2pgraph.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39415 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_pdh.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14293 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_peerdist.py
--rw-r--r--   0 vsts      (1001) docker     (127)    32180 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_powrprof.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_prntvpt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7998 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_projectedfslib.py
--rw-r--r--   0 vsts      (1001) docker     (127)    69946 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_propsys.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10760 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_psapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1362 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_quartz.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2051 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_query.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5253 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_qwave.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30989 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_rasapi32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2820 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_rasdlg.py
--rw-r--r--   0 vsts      (1001) docker     (127)    54566 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_resutils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1012 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_rometadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22447 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_rpcns4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1683 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_rpcproxy.py
--rw-r--r--   0 vsts      (1001) docker     (127)   148359 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_rpcrt4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4988 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_rstrtmgr.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36043 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_rtm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15136 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_rtutils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9078 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_rtworkq.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_sas.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1646 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_scarddlg.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3588 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_schannel.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1712 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_sechost.py
--rw-r--r--   0 vsts      (1001) docker     (127)    37550 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_secur32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1495 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_sensapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13284 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_sensorsutilsv2.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157765 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_setupapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2546 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_sfc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1932 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_shdocvw.py
--rw-r--r--   0 vsts      (1001) docker     (127)    81141 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_shell32.py
--rw-r--r--   0 vsts      (1001) docker     (127)   108109 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_shlwapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14350 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_slc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2850 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_slcext.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1143 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_slwga.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6443 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_snmpapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9685 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_spoolss.py
--rw-r--r--   0 vsts      (1001) docker     (127)      954 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_srclient.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3752 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_srpapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3032 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_sspicli.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1150 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_sti.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9597 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_t2embed.py
--rw-r--r--   0 vsts      (1001) docker     (127)    94966 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_tapi32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4951 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_tbs.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11389 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_tdh.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4744 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_tokenbinding.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8278 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_traffic.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4327 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_txfw32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1627 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ualapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    31556 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_uiautomationcore.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27741 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_urlmon.py
--rw-r--r--   0 vsts      (1001) docker     (127)   252469 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_user32.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15838 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_userenv.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23757 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_usp10.py
--rw-r--r--   0 vsts      (1001) docker     (127)    31235 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_uxtheme.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1567 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_verifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7235 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3659 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_vertdll.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13507 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_virtdisk.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6032 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_vmdevicehost.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17637 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_vmsavedstatedumpprovider.py
--rw-r--r--   0 vsts      (1001) docker     (127)      987 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_vssapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2698 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wcmapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3339 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wdsbp.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13944 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wdsclientapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2846 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wdsmc.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13248 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wdspxe.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4149 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wdstptc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4708 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_webauthn.py
--rw-r--r--   0 vsts      (1001) docker     (127)   106080 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_webservices.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7433 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_websocket.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6419 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wecapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7708 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16155 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wevtapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21479 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winbio.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1003 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_windows_ai_machinelearning.py
--rw-r--r--   0 vsts      (1001) docker     (127)      929 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_windows_data_pdf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3260 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_windows_media_mediacontrol.py
--rw-r--r--   0 vsts      (1001) docker     (127)      965 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_windows_networking.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1722 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_windows_ui_xaml.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4488 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_windowscodecs.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22678 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winfax.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22808 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winhttp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2752 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winhvemulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40942 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winhvplatform.py
--rw-r--r--   0 vsts      (1001) docker     (127)   116017 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wininet.py
--rw-r--r--   0 vsts      (1001) docker     (127)      969 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winml.py
--rw-r--r--   0 vsts      (1001) docker     (127)    55061 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winmm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29221 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winscard.py
--rw-r--r--   0 vsts      (1001) docker     (127)   114656 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winspool.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70042 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winspool_drv.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22342 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wintrust.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14539 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winusb.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30095 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wlanapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1412 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wlanui.py
--rw-r--r--   0 vsts      (1001) docker     (127)    97431 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wldap32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4202 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wldp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3239 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wmvcore.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1385 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wnvapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5271 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wofutil.py
--rw-r--r--   0 vsts      (1001) docker     (127)    65609 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ws2_32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2275 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wscapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1471 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wsclient.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11200 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wsdapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16329 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wsmsvc.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17715 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wsnmp32.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25864 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wtsapi32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1876 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_xaudio2_8.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2916 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_xinput1_4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4574 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_xinputuap.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3101 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_xmllite.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3094 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_xolehlp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2387 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_xpsprint.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.946492 angr-9.2.97/angr/procedures/glibc/
--rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/glibc/__ctype_b_loc.py
--rw-r--r--   0 vsts      (1001) docker     (127)      791 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/glibc/__ctype_tolower_loc.py
--rw-r--r--   0 vsts      (1001) docker     (127)      791 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/glibc/__ctype_toupper_loc.py
--rw-r--r--   0 vsts      (1001) docker     (127)      157 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/glibc/__errno_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      110 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/glibc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1520 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/glibc/__libc_init.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11094 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/glibc/__libc_start_main.py
--rw-r--r--   0 vsts      (1001) docker     (127)      660 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/glibc/dynamic_loading.py
--rw-r--r--   0 vsts      (1001) docker     (127)      146 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/glibc/scanf.py
--rw-r--r--   0 vsts      (1001) docker     (127)       75 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/glibc/sscanf.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.950492 angr-9.2.97/angr/procedures/gnulib/
--rw-r--r--   0 vsts      (1001) docker     (127)      115 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/gnulib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      181 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/gnulib/xalloc_die.py
--rw-r--r--   0 vsts      (1001) docker     (127)      239 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/gnulib/xstrtol_fatal.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.950492 angr-9.2.97/angr/procedures/java/
--rw-r--r--   0 vsts      (1001) docker     (127)     1224 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3381 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java/unconstrained.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.950492 angr-9.2.97/angr/procedures/java_io/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_io/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      335 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_io/read.py
--rw-r--r--   0 vsts      (1001) docker     (127)      613 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_io/write.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.954492 angr-9.2.97/angr/procedures/java_jni/
--rw-r--r--   0 vsts      (1001) docker     (127)    21472 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_jni/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10385 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_jni/array_operations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1056 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_jni/class_and_interface_operations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4789 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_jni/field_access.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_jni/global_and_local_refs.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9597 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_jni/method_calls.py
--rw-r--r--   0 vsts      (1001) docker     (127)      932 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_jni/not_implemented.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2725 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_jni/object_operations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2602 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_jni/string_operations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      229 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_jni/version_information.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.958492 angr-9.2.97/angr/procedures/java_lang/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      983 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/character.py
--rw-r--r--   0 vsts      (1001) docker     (127)      734 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/double.py
--rw-r--r--   0 vsts      (1001) docker     (127)      255 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/exit.py
--rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/getsimplename.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1497 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/integer.py
--rw-r--r--   0 vsts      (1001) docker     (127)      241 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/load_library.py
--rw-r--r--   0 vsts      (1001) docker     (127)      346 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/math.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3174 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1579 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/stringbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)      413 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/system.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.958492 angr-9.2.97/angr/procedures/java_util/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1229 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_util/collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1605 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_util/iterator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3727 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_util/list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4870 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_util/map.py
--rw-r--r--   0 vsts      (1001) docker     (127)      373 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_util/random.py
--rw-r--r--   0 vsts      (1001) docker     (127)      797 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_util/scanner_nextline.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.994492 angr-9.2.97/angr/procedures/libc/
--rw-r--r--   0 vsts      (1001) docker     (127)       95 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      105 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/abort.py
--rw-r--r--   0 vsts      (1001) docker     (127)      285 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/access.py
--rw-r--r--   0 vsts      (1001) docker     (127)      365 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/atoi.py
--rw-r--r--   0 vsts      (1001) docker     (127)      296 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/atol.py
--rw-r--r--   0 vsts      (1001) docker     (127)      185 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/calloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)      183 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/closelog.py
--rw-r--r--   0 vsts      (1001) docker     (127)      430 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/err.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2276 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/error.py
--rw-r--r--   0 vsts      (1001) docker     (127)      198 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/exit.py
--rw-r--r--   0 vsts      (1001) docker     (127)      590 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fclose.py
--rw-r--r--   0 vsts      (1001) docker     (127)      572 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/feof.py
--rw-r--r--   0 vsts      (1001) docker     (127)      223 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fflush.py
--rw-r--r--   0 vsts      (1001) docker     (127)      615 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fgetc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2805 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fgets.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2598 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fopen.py
--rw-r--r--   0 vsts      (1001) docker     (127)      730 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fprintf.py
--rw-r--r--   0 vsts      (1001) docker     (127)      537 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fputc.py
--rw-r--r--   0 vsts      (1001) docker     (127)      662 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fputs.py
--rw-r--r--   0 vsts      (1001) docker     (127)      614 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fread.py
--rw-r--r--   0 vsts      (1001) docker     (127)      159 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/free.py
--rw-r--r--   0 vsts      (1001) docker     (127)      649 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fscanf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fseek.py
--rw-r--r--   0 vsts      (1001) docker     (127)      515 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/ftell.py
--rw-r--r--   0 vsts      (1001) docker     (127)      508 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fwrite.py
--rw-r--r--   0 vsts      (1001) docker     (127)      315 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/getchar.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4047 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/getdelim.py
--rw-r--r--   0 vsts      (1001) docker     (127)      126 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/getegid.py
--rw-r--r--   0 vsts      (1001) docker     (127)      126 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/geteuid.py
--rw-r--r--   0 vsts      (1001) docker     (127)      125 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/getgid.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2636 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/gets.py
--rw-r--r--   0 vsts      (1001) docker     (127)      125 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/getuid.py
--rw-r--r--   0 vsts      (1001) docker     (127)      221 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/malloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3226 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/memcmp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1460 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/memcpy.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2395 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/memset.py
--rw-r--r--   0 vsts      (1001) docker     (127)      206 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/openlog.py
--rw-r--r--   0 vsts      (1001) docker     (127)      333 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/perror.py
--rw-r--r--   0 vsts      (1001) docker     (127)      846 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/printf.py
--rw-r--r--   0 vsts      (1001) docker     (127)      275 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/putchar.py
--rw-r--r--   0 vsts      (1001) docker     (127)      449 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/puts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      196 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/rand.py
--rw-r--r--   0 vsts      (1001) docker     (127)      167 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/realloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)      237 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/rewind.py
--rw-r--r--   0 vsts      (1001) docker     (127)      513 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/scanf.py
--rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/setbuf.py
--rw-r--r--   0 vsts      (1001) docker     (127)      110 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/setvbuf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1175 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/snprintf.py
--rw-r--r--   0 vsts      (1001) docker     (127)      675 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/sprintf.py
--rw-r--r--   0 vsts      (1001) docker     (127)       90 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/srand.py
--rw-r--r--   0 vsts      (1001) docker     (127)      353 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/sscanf.py
--rw-r--r--   0 vsts      (1001) docker     (127)      485 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/stpcpy.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strcat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1771 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strchr.py
--rw-r--r--   0 vsts      (1001) docker     (127)      818 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strcmp.py
--rw-r--r--   0 vsts      (1001) docker     (127)      412 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strcpy.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3540 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strlen.py
--rw-r--r--   0 vsts      (1001) docker     (127)      501 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strncat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7653 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strncmp.py
--rw-r--r--   0 vsts      (1001) docker     (127)      600 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strncpy.py
--rw-r--r--   0 vsts      (1001) docker     (127)      384 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strnlen.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3676 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strstr.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11852 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strtol.py
--rw-r--r--   0 vsts      (1001) docker     (127)      273 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strtoul.py
--rw-r--r--   0 vsts      (1001) docker     (127)      340 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/system.py
--rw-r--r--   0 vsts      (1001) docker     (127)      264 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/time.py
--rw-r--r--   0 vsts      (1001) docker     (127)      512 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/tmpnam.py
--rw-r--r--   0 vsts      (1001) docker     (127)      206 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/tolower.py
--rw-r--r--   0 vsts      (1001) docker     (127)      207 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/toupper.py
--rw-r--r--   0 vsts      (1001) docker     (127)      625 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/ungetc.py
--rw-r--r--   0 vsts      (1001) docker     (127)      415 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/vsnprintf.py
--rw-r--r--   0 vsts      (1001) docker     (127)      538 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/wchar.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.994492 angr-9.2.97/angr/procedures/libstdcpp/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libstdcpp/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      181 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libstdcpp/_unwind_resume.py
--rw-r--r--   0 vsts      (1001) docker     (127)      321 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libstdcpp/std____throw_bad_alloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)      320 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libstdcpp/std____throw_bad_cast.py
--rw-r--r--   0 vsts      (1001) docker     (127)      379 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libstdcpp/std____throw_length_error.py
--rw-r--r--   0 vsts      (1001) docker     (127)      378 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libstdcpp/std____throw_logic_error.py
--rw-r--r--   0 vsts      (1001) docker     (127)      268 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libstdcpp/std__terminate.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.006492 angr-9.2.97/angr/procedures/linux_kernel/
--rw-r--r--   0 vsts      (1001) docker     (127)      111 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      569 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/access.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1045 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/arch_prctl.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1558 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/arm_user_helpers.py
--rw-r--r--   0 vsts      (1001) docker     (127)      329 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/brk.py
--rw-r--r--   0 vsts      (1001) docker     (127)      719 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/cwd.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5177 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/fstat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6392 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/fstat64.py
--rw-r--r--   0 vsts      (1001) docker     (127)      524 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/futex.py
--rw-r--r--   0 vsts      (1001) docker     (127)      375 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/getegid.py
--rw-r--r--   0 vsts      (1001) docker     (127)      375 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/geteuid.py
--rw-r--r--   0 vsts      (1001) docker     (127)      373 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/getgid.py
--rw-r--r--   0 vsts      (1001) docker     (127)      229 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/getpid.py
--rw-r--r--   0 vsts      (1001) docker     (127)      779 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/getrlimit.py
--rw-r--r--   0 vsts      (1001) docker     (127)      141 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/gettid.py
--rw-r--r--   0 vsts      (1001) docker     (127)      373 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/getuid.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1450 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/iovec.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1190 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/lseek.py
--rw-r--r--   0 vsts      (1001) docker     (127)      484 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/mmap.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1396 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/mprotect.py
--rw-r--r--   0 vsts      (1001) docker     (127)      186 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/munmap.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1076 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/openat.py
--rw-r--r--   0 vsts      (1001) docker     (127)      205 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/set_tid_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)      618 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/sigaction.py
--rw-r--r--   0 vsts      (1001) docker     (127)      748 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/sigprocmask.py
--rw-r--r--   0 vsts      (1001) docker     (127)      666 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/stat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2205 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/sysinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      236 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/tgkill.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1000 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/time.py
--rw-r--r--   0 vsts      (1001) docker     (127)      764 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/uid.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1127 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/uname.py
--rw-r--r--   0 vsts      (1001) docker     (127)      708 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/unlink.py
--rw-r--r--   0 vsts      (1001) docker     (127)      492 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/vsyscall.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.006492 angr-9.2.97/angr/procedures/linux_loader/
--rw-r--r--   0 vsts      (1001) docker     (127)      115 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_loader/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      129 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_loader/_dl_initial_error_catch_tsd.py
--rw-r--r--   0 vsts      (1001) docker     (127)      337 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_loader/_dl_rtld_lock.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1876 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_loader/sim_loader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1548 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_loader/tls.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.006492 angr-9.2.97/angr/procedures/msvcr/
--rw-r--r--   0 vsts      (1001) docker     (127)      691 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/msvcr/__getmainargs.py
--rw-r--r--   0 vsts      (1001) docker     (127)      116 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/msvcr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1363 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/msvcr/_initterm.py
--rw-r--r--   0 vsts      (1001) docker     (127)      752 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/msvcr/fmode.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.010492 angr-9.2.97/angr/procedures/ntdll/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/ntdll/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2693 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/ntdll/exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.022492 angr-9.2.97/angr/procedures/posix/
--rw-r--r--   0 vsts      (1001) docker     (127)       66 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1246 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/accept.py
--rw-r--r--   0 vsts      (1001) docker     (127)      316 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/bind.py
--rw-r--r--   0 vsts      (1001) docker     (127)      174 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/bzero.py
--rw-r--r--   0 vsts      (1001) docker     (127)      739 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/chroot.py
--rw-r--r--   0 vsts      (1001) docker     (127)      200 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/close.py
--rw-r--r--   0 vsts      (1001) docker     (127)       64 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/closedir.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1917 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/dup.py
--rw-r--r--   0 vsts      (1001) docker     (127)      314 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/fcntl.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2850 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/fdopen.py
--rw-r--r--   0 vsts      (1001) docker     (127)      414 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/fileno.py
--rw-r--r--   0 vsts      (1001) docker     (127)      292 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/fork.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1383 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/getenv.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1573 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/gethostbyname.py
--rw-r--r--   0 vsts      (1001) docker     (127)      484 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/getpass.py
--rw-r--r--   0 vsts      (1001) docker     (127)      187 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/getsockopt.py
--rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/htonl.py
--rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/htons.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1950 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/inet_ntoa.py
--rw-r--r--   0 vsts      (1001) docker     (127)      315 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/listen.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5042 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/mmap.py
--rw-r--r--   0 vsts      (1001) docker     (127)      537 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/open.py
--rw-r--r--   0 vsts      (1001) docker     (127)      291 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/opendir.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2247 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/poll.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1355 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/pread64.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2402 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/pthread.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1362 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/pwrite64.py
--rw-r--r--   0 vsts      (1001) docker     (127)      252 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/read.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2161 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/readdir.py
--rw-r--r--   0 vsts      (1001) docker     (127)      275 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/recv.py
--rw-r--r--   0 vsts      (1001) docker     (127)      298 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/recvfrom.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1979 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/select.py
--rw-r--r--   0 vsts      (1001) docker     (127)      711 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/send.py
--rw-r--r--   0 vsts      (1001) docker     (127)      167 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/setsockopt.py
--rw-r--r--   0 vsts      (1001) docker     (127)      784 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/sigaction.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1654 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/sim_time.py
--rw-r--r--   0 vsts      (1001) docker     (127)      145 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/sleep.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/socket.py
--rw-r--r--   0 vsts      (1001) docker     (127)      678 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/strcasecmp.py
--rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/strdup.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2791 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/strtok_r.py
--rw-r--r--   0 vsts      (1001) docker     (127)      430 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/syslog.py
--rw-r--r--   0 vsts      (1001) docker     (127)      260 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/tz.py
--rw-r--r--   0 vsts      (1001) docker     (127)      282 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/unlink.py
--rw-r--r--   0 vsts      (1001) docker     (127)      140 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/usleep.py
--rw-r--r--   0 vsts      (1001) docker     (127)      254 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/write.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1865 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/procedure_dict.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.026492 angr-9.2.97/angr/procedures/stubs/
--rw-r--r--   0 vsts      (1001) docker     (127)      219 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/CallReturn.py
--rw-r--r--   0 vsts      (1001) docker     (127)      413 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/NoReturnUnconstrained.py
--rw-r--r--   0 vsts      (1001) docker     (127)       76 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/Nop.py
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/PathTerminator.py
--rw-r--r--   0 vsts      (1001) docker     (127)      439 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/Redirect.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/ReturnChar.py
--rw-r--r--   0 vsts      (1001) docker     (127)      774 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/ReturnUnconstrained.py
--rw-r--r--   0 vsts      (1001) docker     (127)      153 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/UnresolvableCallTarget.py
--rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/UnresolvableJumpTarget.py
--rw-r--r--   0 vsts      (1001) docker     (127)      561 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/UserHook.py
--rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      342 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/b64_decode.py
--rw-r--r--   0 vsts      (1001) docker     (127)      343 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/caller.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/crazy_scanf.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28192 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/format_parser.py
--rw-r--r--   0 vsts      (1001) docker     (127)      902 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/syscall_stub.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.026492 angr-9.2.97/angr/procedures/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/testing/manyargs.py
--rw-r--r--   0 vsts      (1001) docker     (127)      171 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/testing/retreg.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.030492 angr-9.2.97/angr/procedures/tracer/
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/tracer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      232 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/tracer/random.py
--rw-r--r--   0 vsts      (1001) docker     (127)      573 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/tracer/receive.py
--rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/tracer/transmit.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.030492 angr-9.2.97/angr/procedures/uclibc/
--rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/uclibc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      293 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/uclibc/__uClibc_main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.038492 angr-9.2.97/angr/procedures/win32/
--rw-r--r--   0 vsts      (1001) docker     (127)       97 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/EncodePointer.py
--rw-r--r--   0 vsts      (1001) docker     (127)      134 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/ExitProcess.py
--rw-r--r--   0 vsts      (1001) docker     (127)      228 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/GetCommandLine.py
--rw-r--r--   0 vsts      (1001) docker     (127)      105 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/GetCurrentProcessId.py
--rw-r--r--   0 vsts      (1001) docker     (127)      104 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/GetCurrentThreadId.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/GetLastInputInfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      940 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/GetModuleHandle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1124 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/GetProcessAffinityMask.py
--rw-r--r--   0 vsts      (1001) docker     (127)      557 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/InterlockedExchange.py
--rw-r--r--   0 vsts      (1001) docker     (127)      201 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/IsProcessorFeaturePresent.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3985 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/VirtualAlloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2274 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/VirtualProtect.py
--rw-r--r--   0 vsts      (1001) docker     (127)       86 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      277 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/critical_section.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3424 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/dynamic_loading.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1455 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/file_handles.py
--rw-r--r--   0 vsts      (1001) docker     (127)      318 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/gethostbyname.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1541 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/heap.py
--rw-r--r--   0 vsts      (1001) docker     (127)      757 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/is_bad_ptr.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2130 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/local_storage.py
--rw-r--r--   0 vsts      (1001) docker     (127)      177 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/mutex.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5332 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/sim_time.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1238 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/system_paths.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.038492 angr-9.2.97/angr/procedures/win32_kernel/
--rw-r--r--   0 vsts      (1001) docker     (127)      423 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32_kernel/ExAllocatePool.py
--rw-r--r--   0 vsts      (1001) docker     (127)      225 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32_kernel/ExFreePoolWithTag.py
--rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32_kernel/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.038492 angr-9.2.97/angr/procedures/win_user32/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win_user32/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win_user32/chars.py
--rw-r--r--   0 vsts      (1001) docker     (127)      377 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win_user32/keyboard.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1717 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win_user32/messagebox.py
--rw-r--r--   0 vsts      (1001) docker     (127)    37186 2024-04-02 17:01:36.000000 angr-9.2.97/angr/project.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.042492 angr-9.2.97/angr/protos/
--rw-r--r--   0 vsts      (1001) docker     (127)      378 2024-04-02 17:01:36.000000 angr-9.2.97/angr/protos/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2389 2024-04-02 17:01:36.000000 angr-9.2.97/angr/protos/cfg_pb2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2146 2024-04-02 17:01:36.000000 angr-9.2.97/angr/protos/function_pb2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8527 2024-04-02 17:01:36.000000 angr-9.2.97/angr/protos/primitives_pb2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8112 2024-04-02 17:01:36.000000 angr-9.2.97/angr/protos/variables_pb2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1247 2024-04-02 17:01:36.000000 angr-9.2.97/angr/protos/xrefs_pb2.py
--rw-r--r--   0 vsts      (1001) docker     (127)        8 2024-04-02 17:01:36.000000 angr-9.2.97/angr/py.typed
--rw-r--r--   0 vsts      (1001) docker     (127)     1502 2024-04-02 17:01:36.000000 angr-9.2.97/angr/serializable.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1102 2024-04-02 17:01:36.000000 angr-9.2.97/angr/service.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39300 2024-04-02 17:01:36.000000 angr-9.2.97/angr/sim_manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18057 2024-04-02 17:01:36.000000 angr-9.2.97/angr/sim_options.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26081 2024-04-02 17:01:36.000000 angr-9.2.97/angr/sim_procedure.py
--rw-r--r--   0 vsts      (1001) docker     (127)    37826 2024-04-02 17:01:36.000000 angr-9.2.97/angr/sim_state.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12530 2024-04-02 17:01:36.000000 angr-9.2.97/angr/sim_state_options.py
--rw-r--r--   0 vsts      (1001) docker     (127)   121935 2024-04-02 17:01:36.000000 angr-9.2.97/angr/sim_type.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17228 2024-04-02 17:01:36.000000 angr-9.2.97/angr/sim_variable.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.046492 angr-9.2.97/angr/simos/
--rw-r--r--   0 vsts      (1001) docker     (127)      755 2024-04-02 17:01:36.000000 angr-9.2.97/angr/simos/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5568 2024-04-02 17:01:36.000000 angr-9.2.97/angr/simos/cgc.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21461 2024-04-02 17:01:36.000000 angr-9.2.97/angr/simos/javavm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23327 2024-04-02 17:01:36.000000 angr-9.2.97/angr/simos/linux.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18275 2024-04-02 17:01:36.000000 angr-9.2.97/angr/simos/simos.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5679 2024-04-02 17:01:36.000000 angr-9.2.97/angr/simos/snimmuc_nxp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7351 2024-04-02 17:01:36.000000 angr-9.2.97/angr/simos/userland.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26047 2024-04-02 17:01:36.000000 angr-9.2.97/angr/simos/windows.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10640 2024-04-02 17:01:36.000000 angr-9.2.97/angr/slicer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8467 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_hierarchy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.054492 angr-9.2.97/angr/state_plugins/
--rw-r--r--   0 vsts      (1001) docker     (127)      735 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12092 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/callstack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4247 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/cgc.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13310 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/concrete.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6844 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/debug_variables.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15902 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/filesystem.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5125 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/gdb.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1507 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/globals.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.054492 angr-9.2.97/angr/state_plugins/heap/
--rw-r--r--   0 vsts      (1001) docker     (127)      136 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/heap/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6229 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/heap/heap_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5412 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/heap/heap_brk.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7886 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/heap/heap_freelist.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1858 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/heap/heap_libc.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28967 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/heap/heap_ptmalloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)      793 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/heap/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19104 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/history.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11317 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/inspect.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/javavm_classloader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3403 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/jni_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23586 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/libc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6747 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/light_registers.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2364 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/log.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4209 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/loop_data.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6187 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/plugin.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27145 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/posix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8053 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/preconstrainer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6178 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/scratch.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9763 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/sim_action.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4268 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/sim_action_object.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2061 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/sim_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)    45221 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/solver.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11039 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/symbolizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30091 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/trace_additions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2643 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/uc_manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)    78095 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/unicorn_engine.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12361 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/view.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.058493 angr-9.2.97/angr/storage/
--rw-r--r--   0 vsts      (1001) docker     (127)      182 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    48379 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/file.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.066492 angr-9.2.97/angr/storage/memory_mixins/
--rw-r--r--   0 vsts      (1001) docker     (127)    11944 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1944 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/__init__.pyi
--rw-r--r--   0 vsts      (1001) docker     (127)     3402 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/actions_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16569 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/address_concretization_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2901 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/bvv_conversion_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5496 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/clouseau_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)      929 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/conditional_store_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10302 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/convenient_mappings_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6034 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/default_filler_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)      317 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/dirty_addrs_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3668 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/hex_dumper_mixin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.066492 angr-9.2.97/angr/storage/memory_mixins/javavm_memory/
--rw-r--r--   0 vsts      (1001) docker     (127)       51 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/javavm_memory/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15456 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/javavm_memory/javavm_memory_mixin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.066492 angr-9.2.97/angr/storage/memory_mixins/keyvalue_memory/
--rw-r--r--   0 vsts      (1001) docker     (127)       55 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/keyvalue_memory/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      906 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/keyvalue_memory/keyvalue_memory_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)      858 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/label_merger_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3036 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/multi_value_merger_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3412 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/name_resolution_mixin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.070492 angr-9.2.97/angr/storage/memory_mixins/paged_memory/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10282 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/page_backer_mixins.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29219 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/paged_memory_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2192 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/paged_memory_multivalue_mixin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.070492 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/
--rw-r--r--   0 vsts      (1001) docker     (127)     1469 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12776 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/cooperation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3039 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/history_tracking_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2050 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/ispo_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14108 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/list_page.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11302 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/multi_values.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17647 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/mv_list_page.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/permissions_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1701 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/refcount_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19139 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/ultra_page.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1541 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/privileged_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3283 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/stack_allocation_mixin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.074493 angr-9.2.97/angr/storage/memory_mixins/regioned_memory/
--rw-r--r--   0 vsts      (1001) docker     (127)      351 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/regioned_memory/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1098 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/regioned_memory/abstract_address_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1313 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/regioned_memory/abstract_merger_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)      128 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/regioned_memory/region_category_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9196 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/regioned_memory/region_data.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4355 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/regioned_memory/region_meta_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4891 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/regioned_memory/regioned_address_concretization_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18638 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/regioned_memory/regioned_memory_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2240 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/regioned_memory/static_find_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2492 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/simple_interface_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)      502 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/simplification_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5659 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/size_resolution_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4884 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/slotted_memory.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5655 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/smart_find_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)      411 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/symbolic_merger_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)      659 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/top_merger_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2590 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/underconstrained_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1027 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/unwrapper_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6253 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_object.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1940 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/pcap.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3239 2024-04-02 17:01:36.000000 angr-9.2.97/angr/tablespecs.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.078492 angr-9.2.97/angr/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)      980 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      995 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/algo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      209 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2160 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/cowdict.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3107 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/dynamic_dictlist.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2091 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/enums_conv.py
--rw-r--r--   0 vsts      (1001) docker     (127)      363 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/env.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4217 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/formatting.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5240 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/funcid.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28417 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)      308 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/lazy_import.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7202 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/library.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1944 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/loader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1825 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/mp.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20431 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/segment_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1334 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/timing.py
--rw-r--r--   0 vsts      (1001) docker     (127)      417 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9701 2024-04-02 17:01:36.000000 angr-9.2.97/angr/vaults.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.078492 angr-9.2.97/angr.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     4769 2024-04-02 17:02:56.000000 angr-9.2.97/angr.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)    56598 2024-04-02 17:02:56.000000 angr-9.2.97/angr.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-02 17:02:56.000000 angr-9.2.97/angr.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       44 2024-04-02 17:02:56.000000 angr-9.2.97/angr.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      567 2024-04-02 17:02:56.000000 angr-9.2.97/angr.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-04-02 17:02:56.000000 angr-9.2.97/angr.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.078492 angr-9.2.97/native/
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-02 17:01:36.000000 angr-9.2.97/native/Makefile
--rw-r--r--   0 vsts      (1001) docker     (127)      320 2024-04-02 17:01:36.000000 angr-9.2.97/native/Makefile-win
--rw-r--r--   0 vsts      (1001) docker     (127)     1431 2024-04-02 17:01:36.000000 angr-9.2.97/native/angr_native.def
--rw-r--r--   0 vsts      (1001) docker     (127)     3940 2024-04-02 17:01:36.000000 angr-9.2.97/native/log.c
--rw-r--r--   0 vsts      (1001) docker     (127)     2754 2024-04-02 17:01:36.000000 angr-9.2.97/native/log.h
--rw-r--r--   0 vsts      (1001) docker     (127)   119496 2024-04-02 17:01:36.000000 angr-9.2.97/native/sim_unicorn.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    28878 2024-04-02 17:01:36.000000 angr-9.2.97/native/sim_unicorn.hpp
--rw-r--r--   0 vsts      (1001) docker     (127)      855 2024-04-02 17:01:44.000000 angr-9.2.97/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     1634 2024-04-02 17:02:57.082492 angr-9.2.97/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     3580 2024-04-02 17:01:36.000000 angr-9.2.97/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.078492 angr-9.2.97/tests/
--rwxr-xr-x   0 vsts      (1001) docker     (127)     3392 2024-04-02 17:01:36.000000 angr-9.2.97/tests/test_calling_conventions.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)    14468 2024-04-02 17:01:36.000000 angr-9.2.97/tests/test_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.272811 angr-9.2.98/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1327 2024-04-09 17:01:34.000000 angr-9.2.98/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      107 2024-04-09 17:01:34.000000 angr-9.2.98/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     4769 2024-04-09 17:03:02.272811 angr-9.2.98/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2603 2024-04-09 17:01:34.000000 angr-9.2.98/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:01.940810 angr-9.2.98/angr/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3992 2024-04-09 17:01:43.000000 angr-9.2.98/angr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1887 2024-04-09 17:01:34.000000 angr-9.2.98/angr/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:01.948810 angr-9.2.98/angr/analyses/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1773 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12277 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27287 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/backward_slice.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26267 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/binary_optimizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    51815 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/bindiff.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2448 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/boyscout.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2835 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/callee_cleanup_finder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40039 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/calling_convention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6361 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cdg.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:01.952810 angr-9.2.98/angr/analyses/cfg/
+-rw-r--r--   0 vsts      (1001) docker     (127)      321 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15450 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg/cfb.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3146 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg/cfg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3112 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg/cfg_arch_options.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   123056 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg/cfg_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   152842 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg/cfg_emulated.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   218220 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg/cfg_fast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26047 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg/cfg_fast_soot.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5989 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg/cfg_job_base.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:01.956810 angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      361 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2083 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/amd64_elf_got.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1777 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/amd64_pe_iat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5231 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/arm_elf_fast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5273 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/const_resolver.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1441 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/default_resolvers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   101955 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/jumptable.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19350 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/mips_elf_fast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/propagator_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3019 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/resolver.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2971 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/x86_elf_pic_plt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1621 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/x86_pe_iat.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:01.956810 angr-9.2.98/angr/analyses/cfg_slice_to_sink/
+-rw-r--r--   0 vsts      (1001) docker     (127)      120 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg_slice_to_sink/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3982 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg_slice_to_sink/cfg_slice_to_sink.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3560 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg_slice_to_sink/graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/cfg_slice_to_sink/transitions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2969 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/class_identifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3641 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/code_tagging.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18492 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/complete_calling_conventions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16456 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/congruency_check.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:01.956810 angr-9.2.98/angr/analyses/data_dep/
+-rw-r--r--   0 vsts      (1001) docker     (127)      180 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/data_dep/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25296 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/data_dep/data_dependency_analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4650 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/data_dep/dep_nodes.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1527 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/data_dep/sim_act_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3386 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/datagraph_meta.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    63426 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/ddg.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:01.964810 angr-9.2.98/angr/analyses/decompiler/
+-rw-r--r--   0 vsts      (1001) docker     (127)      540 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61504 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/ail_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1595 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/ailgraph_walker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10576 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/block_io_finder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6531 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/block_similarity.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17199 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/block_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1205 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/call_counter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15083 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/callsite_maker.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:01.964810 angr-9.2.98/angr/analyses/decompiler/ccall_rewriters/
+-rw-r--r--   0 vsts      (1001) docker     (127)      102 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/ccall_rewriters/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21551 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/ccall_rewriters/amd64_ccalls.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/ccall_rewriters/rewriter_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    87477 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/clinic.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49596 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/condition_processor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/decompilation_cache.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8240 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/decompilation_options.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22137 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/decompiler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7368 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/empty_node_remover.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2867 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/expression_counters.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3545 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/expression_narrower.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2485 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/goto_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16502 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/graph_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1181 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/jump_target_collector.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/jumptable_entry_condition_rewriter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:01.972810 angr-9.2.98/angr/analyses/decompiler/optimization_passes/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3954 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5289 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/base_ptr_save_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15319 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/code_motion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10593 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/const_derefs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4033 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/cross_jump_reverter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17442 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/div_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10388 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/engine_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4701 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/expr_op_swapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3946 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/flip_boolean_cmp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16281 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/inlined_string_transformation_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7756 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/ite_expr_converter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6762 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/ite_region_converter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34328 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/lowered_switch_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3124 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/mod_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10420 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/multi_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14331 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/optimization_pass.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7398 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/register_save_area_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6470 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/ret_addr_save_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7828 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/ret_deduplicator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18394 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/return_duplicator_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1803 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/return_duplicator_high.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4973 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/return_duplicator_low.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12559 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/stack_canary_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4523 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/switch_default_case_duplicator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12304 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/win_stack_canary_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3067 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/optimization_passes/x86_gcc_getpc_simplifier.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:01.984810 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3252 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1727 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/a_div_const_add_a_mul_n_div_const.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1365 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/a_mul_const_div_shr_const.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      988 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/a_shl_const_sub_a.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      953 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2050 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div_const_mul_const.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      619 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/a_sub_a_sub_n.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9333 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/arm_cmpf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3538 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1056 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_add_n.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_and_mask.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1298 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/bitwise_or_to_logical_or.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      991 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/bool_expr_xor_1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6238 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/bswap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1020 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/coalesce_same_cascading_ifs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3691 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/const_mull_a_shift.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1583 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/constant_derefs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2578 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/conv_a_sub0_shr_and.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2070 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/conv_shl_shr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10131 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/eager_eval.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2015 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/extended_byte_and_mask.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5765 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/inlined_strcpy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4676 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/inlined_strcpy_consolidation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6283 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/inlined_wstrcpy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2084 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/invert_negated_logical_conjuction_disjunction.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1136 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/one_sub_bool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      591 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/remove_cascading_conversions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1560 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/remove_empty_if_body.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      739 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/remove_noop_conversions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1635 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/remove_redundant_bitmasks.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6583 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/remove_redundant_conversions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1189 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/remove_redundant_ite_branch.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1869 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/remove_redundant_ite_comparisons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      503 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/remove_redundant_nots.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1394 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/remove_redundant_reinterprets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1665 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/remove_redundant_shifts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1578 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/remove_redundant_shifts_around_comparators.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3327 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/rewrite_bit_extractions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1809 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/rewrite_mips_gp_loads.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2814 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/rol_ror.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5282 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/sar_to_signed_div.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1477 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/simplify_pc_relative_loads.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1837 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/single_bit_cond_to_boolexpr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      940 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/single_bit_xor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4833 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/tidy_stack_addr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5385 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/redundant_label_remover.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    45489 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/region_identifier.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:01.984810 angr-9.2.98/angr/analyses/decompiler/region_simplifiers/
+-rw-r--r--   0 vsts      (1001) docker     (127)       48 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/region_simplifiers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3721 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/region_simplifiers/cascading_cond_transformer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2490 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/region_simplifiers/cascading_ifs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24008 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/region_simplifiers/expr_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6032 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/region_simplifiers/goto.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5034 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/region_simplifiers/if_.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3681 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/region_simplifiers/ifelse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5861 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/region_simplifiers/loop.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      565 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/region_simplifiers/node_address_finder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8209 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/region_simplifiers/region_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24545 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/region_simplifiers/switch_cluster_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3327 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/region_simplifiers/switch_expr_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      717 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/region_walker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      529 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/seq_to_blocks.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8428 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/sequence_walker.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:01.988810 angr-9.2.98/angr/analyses/decompiler/structured_codegen/
+-rw-r--r--   0 vsts      (1001) docker     (127)      313 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/structured_codegen/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3845 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/structured_codegen/base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   134738 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/structured_codegen/c.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      535 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/structured_codegen/dummy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6773 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/structured_codegen/dwarf_import.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:01.988810 angr-9.2.98/angr/analyses/decompiler/structuring/
+-rw-r--r--   0 vsts      (1001) docker     (127)      371 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/structuring/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    48400 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/structuring/dream.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   119472 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/structuring/phoenix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7078 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/structuring/recursive_structurer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41330 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/structuring/structurer_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11964 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/structuring/structurer_nodes.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28116 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/decompiler/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    45941 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/disassembly.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2989 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/disassembly_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1245 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/dominance_frontier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10158 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/find_objects_static.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7847 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/flirt.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:01.988810 angr-9.2.98/angr/analyses/forward_analysis/
+-rw-r--r--   0 vsts      (1001) docker     (127)      144 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/forward_analysis/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19939 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/forward_analysis/forward_analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1579 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/forward_analysis/job_info.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:01.992810 angr-9.2.98/angr/analyses/forward_analysis/visitors/
+-rw-r--r--   0 vsts      (1001) docker     (127)      174 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/forward_analysis/visitors/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      713 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/forward_analysis/visitors/call_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2739 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/forward_analysis/visitors/function_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8067 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/forward_analysis/visitors/graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      711 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/forward_analysis/visitors/loop.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      768 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/forward_analysis/visitors/single_node_graph.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:01.992810 angr-9.2.98/angr/analyses/identifier/
+-rw-r--r--   0 vsts      (1001) docker     (127)       33 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4757 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/custom_callable.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      157 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/errors.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1749 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/func.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:01.996810 angr-9.2.98/angr/analyses/identifier/functions/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1059 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2110 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/atoi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3294 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/based_atoi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4353 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/fdprintf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1941 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/free.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8665 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/int2str.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3845 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/malloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1953 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/memcmp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3166 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/memcpy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1188 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/memset.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4307 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/printf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11564 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/recv_until.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2356 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/skip_calloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3186 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/skip_realloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2886 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/skip_recv_n.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4179 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/snprintf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4119 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/sprintf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      806 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/strcasecmp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3459 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/strcmp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1187 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/strcpy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      753 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/strlen.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3297 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/strncmp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2008 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/strncpy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2426 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/functions/strtol.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33287 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/identify.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13739 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/identifier/runner.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8531 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/init_finder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9412 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/loop_analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7122 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/loopfinder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.000810 angr-9.2.98/angr/analyses/propagator/
+-rw-r--r--   0 vsts      (1001) docker     (127)       43 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/propagator/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    68660 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/propagator/engine_ail.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1735 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/propagator/engine_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12900 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/propagator/engine_vex.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6890 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/propagator/outdated_definition_walker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16134 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/propagator/propagator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/propagator/tmpvar_finder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      359 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/propagator/top_checker_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/propagator/values.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1433 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/propagator/vex_vars.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16323 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/proximity_graph.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.004810 angr-9.2.98/angr/analyses/reaching_definitions/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1989 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/reaching_definitions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2217 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/reaching_definitions/call_trace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14886 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/reaching_definitions/dep_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    45997 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/reaching_definitions/engine_ail.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43124 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/reaching_definitions/engine_vex.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/reaching_definitions/external_codeloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26839 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/reaching_definitions/function_handler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2634 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/reaching_definitions/heap_allocator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11224 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/reaching_definitions/rd_initializer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23986 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/reaching_definitions/rd_state.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23988 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/reaching_definitions/reaching_definitions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1995 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/reaching_definitions/subject.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   100412 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/reassembler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8941 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/soot_class_hierarchy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29868 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/stack_pointer_tracker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1711 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/static_hooker.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.008810 angr-9.2.98/angr/analyses/typehoon/
+-rw-r--r--   0 vsts      (1001) docker     (127)       31 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/typehoon/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3519 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/typehoon/dfa.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2805 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/typehoon/lifter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    48619 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/typehoon/simple_solver.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8610 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/typehoon/translator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7030 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/typehoon/typeconsts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9353 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/typehoon/typehoon.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15783 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/typehoon/typevars.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      158 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/typehoon/variance.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.008810 angr-9.2.98/angr/analyses/variable_recovery/
+-rw-r--r--   0 vsts      (1001) docker     (127)      105 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/variable_recovery/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1403 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/variable_recovery/annotations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25716 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/variable_recovery/engine_ail.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41633 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/variable_recovery/engine_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19215 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/variable_recovery/engine_vex.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4907 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/variable_recovery/irsb_scanner.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21802 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/variable_recovery/variable_recovery.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14960 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/variable_recovery/variable_recovery_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24125 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/variable_recovery/variable_recovery_fast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25224 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/veritesting.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75256 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/vfg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16173 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/vsa_ddg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3874 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/vtable.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9714 2024-04-09 17:01:34.000000 angr-9.2.98/angr/analyses/xrefs.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.016810 angr-9.2.98/angr/angrdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)      231 2024-04-09 17:01:34.000000 angr-9.2.98/angr/angrdb/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6459 2024-04-09 17:01:34.000000 angr-9.2.98/angr/angrdb/db.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4750 2024-04-09 17:01:34.000000 angr-9.2.98/angr/angrdb/models.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.020810 angr-9.2.98/angr/angrdb/serializers/
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-09 17:01:34.000000 angr-9.2.98/angr/angrdb/serializers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1297 2024-04-09 17:01:34.000000 angr-9.2.98/angr/angrdb/serializers/cfg_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1531 2024-04-09 17:01:34.000000 angr-9.2.98/angr/angrdb/serializers/comments.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1696 2024-04-09 17:01:34.000000 angr-9.2.98/angr/angrdb/serializers/funcs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3688 2024-04-09 17:01:34.000000 angr-9.2.98/angr/angrdb/serializers/kb.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1425 2024-04-09 17:01:34.000000 angr-9.2.98/angr/angrdb/serializers/labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2494 2024-04-09 17:01:34.000000 angr-9.2.98/angr/angrdb/serializers/loader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4190 2024-04-09 17:01:34.000000 angr-9.2.98/angr/angrdb/serializers/structured_code.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2383 2024-04-09 17:01:34.000000 angr-9.2.98/angr/angrdb/serializers/variables.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1180 2024-04-09 17:01:34.000000 angr-9.2.98/angr/angrdb/serializers/xrefs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10818 2024-04-09 17:01:34.000000 angr-9.2.98/angr/annocfg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15519 2024-04-09 17:01:34.000000 angr-9.2.98/angr/blade.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14468 2024-04-09 17:01:34.000000 angr-9.2.98/angr/block.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6034 2024-04-09 17:01:34.000000 angr-9.2.98/angr/callable.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    91291 2024-04-09 17:01:34.000000 angr-9.2.98/angr/calling_conventions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5476 2024-04-09 17:01:34.000000 angr-9.2.98/angr/code_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3784 2024-04-09 17:01:34.000000 angr-9.2.98/angr/codenode.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.024810 angr-9.2.98/angr/concretization_strategies/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3727 2024-04-09 17:01:34.000000 angr-9.2.98/angr/concretization_strategies/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      438 2024-04-09 17:01:34.000000 angr-9.2.98/angr/concretization_strategies/any.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1341 2024-04-09 17:01:34.000000 angr-9.2.98/angr/concretization_strategies/any_named.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2218 2024-04-09 17:01:34.000000 angr-9.2.98/angr/concretization_strategies/controlled_data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      617 2024-04-09 17:01:34.000000 angr-9.2.98/angr/concretization_strategies/eval.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-09 17:01:34.000000 angr-9.2.98/angr/concretization_strategies/logging.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1035 2024-04-09 17:01:34.000000 angr-9.2.98/angr/concretization_strategies/max.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      536 2024-04-09 17:01:34.000000 angr-9.2.98/angr/concretization_strategies/nonzero.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      784 2024-04-09 17:01:34.000000 angr-9.2.98/angr/concretization_strategies/nonzero_range.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1435 2024-04-09 17:01:34.000000 angr-9.2.98/angr/concretization_strategies/norepeats.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1564 2024-04-09 17:01:34.000000 angr-9.2.98/angr/concretization_strategies/norepeats_range.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      555 2024-04-09 17:01:34.000000 angr-9.2.98/angr/concretization_strategies/range.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-09 17:01:34.000000 angr-9.2.98/angr/concretization_strategies/signed_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-04-09 17:01:34.000000 angr-9.2.98/angr/concretization_strategies/single.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-09 17:01:34.000000 angr-9.2.98/angr/concretization_strategies/solutions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      529 2024-04-09 17:01:34.000000 angr-9.2.98/angr/concretization_strategies/unlimited_range.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.024810 angr-9.2.98/angr/distributed/
+-rw-r--r--   0 vsts      (1001) docker     (127)      140 2024-04-09 17:01:34.000000 angr-9.2.98/angr/distributed/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6682 2024-04-09 17:01:34.000000 angr-9.2.98/angr/distributed/server.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6075 2024-04-09 17:01:34.000000 angr-9.2.98/angr/distributed/worker.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.024810 angr-9.2.98/angr/engines/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1066 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7468 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/concrete.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8109 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/engine.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/failure.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2546 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/hook.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.024810 angr-9.2.98/angr/engines/light/
+-rw-r--r--   0 vsts      (1001) docker     (127)      186 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/light/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23132 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/light/data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    44929 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/light/engine.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.028810 angr-9.2.98/angr/engines/pcode/
+-rw-r--r--   0 vsts      (1001) docker     (127)       83 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/pcode/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28720 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/pcode/behavior.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2994 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/pcode/cc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16718 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/pcode/emulate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10551 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/pcode/engine.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    52362 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/pcode/lifter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/procedure.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.028810 angr-9.2.98/angr/engines/soot/
+-rw-r--r--   0 vsts      (1001) docker     (127)       30 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17238 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/engine.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      221 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.032810 angr-9.2.98/angr/engines/soot/expressions/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1706 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/expressions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      857 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/expressions/arrayref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/expressions/base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      781 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/expressions/binop.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      753 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/expressions/cast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1260 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/expressions/condition.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1387 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/expressions/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      313 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/expressions/instanceOf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      234 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/expressions/instancefieldref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4525 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/expressions/invoke.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      189 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/expressions/length.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      215 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/expressions/local.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/expressions/new.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1970 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/expressions/newArray.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3400 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/expressions/newMultiArray.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      224 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/expressions/paramref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1192 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/expressions/phi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      232 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/expressions/staticfieldref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/expressions/thisref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/expressions/unsupported.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1940 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/field_dispatcher.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1780 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/method_dispatcher.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.036810 angr-9.2.98/angr/engines/soot/statements/
+-rw-r--r--   0 vsts      (1001) docker     (127)      893 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/statements/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1271 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/statements/assign.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2094 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/statements/base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      325 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/statements/goto.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      421 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/statements/identity.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      560 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/statements/if_.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      284 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/statements/invoke.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      466 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/statements/return_.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1301 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/statements/switch.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/statements/throw.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.036810 angr-9.2.98/angr/engines/soot/values/
+-rw-r--r--   0 vsts      (1001) docker     (127)      792 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/values/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4427 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/values/arrayref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      121 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/values/base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      403 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/values/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1593 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/values/instancefieldref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      385 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/values/local.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      413 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/values/paramref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1240 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/values/staticfieldref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1107 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/values/strref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5739 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/soot/values/thisref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23679 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/successors.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2177 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/syscall.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24447 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/unicorn.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.036810 angr-9.2.98/angr/engines/vex/
+-rw-r--r--   0 vsts      (1001) docker     (127)       95 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/vex/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.040810 angr-9.2.98/angr/engines/vex/claripy/
+-rw-r--r--   0 vsts      (1001) docker     (127)       40 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/vex/claripy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    82570 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/vex/claripy/ccall.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5123 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/vex/claripy/datalayer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    46171 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/vex/claripy/irop.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.040810 angr-9.2.98/angr/engines/vex/heavy/
+-rw-r--r--   0 vsts      (1001) docker     (127)      201 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/vex/heavy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8871 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/vex/heavy/actions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14702 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/vex/heavy/concretizers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18699 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/vex/heavy/dirty.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15822 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/vex/heavy/heavy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2317 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/vex/heavy/inspect.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3737 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/vex/heavy/resilience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1180 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/vex/heavy/super_fastpath.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17132 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/vex/lifter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.040810 angr-9.2.98/angr/engines/vex/light/
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/vex/light/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21729 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/vex/light/light.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2002 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/vex/light/resilience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2023 2024-04-09 17:01:34.000000 angr-9.2.98/angr/engines/vex/light/slicing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8299 2024-04-09 17:01:34.000000 angr-9.2.98/angr/errors.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.048810 angr-9.2.98/angr/exploration_techniques/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6980 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2588 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/bucketizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2262 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1167 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/dfs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17917 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/director.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3531 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/driller_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6163 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/explorer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      550 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/lengthlimiter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2583 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/local_loop_seer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11640 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/loop_seer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3091 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/manual_mergepoint.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1271 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/memory_watcher.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3520 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/oppologist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5126 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/slicecutor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9382 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/spiller.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      818 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/spiller_db.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2059 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/stochastic.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6969 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/suggestions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3122 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/symbion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1586 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/tech_builder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2976 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/threading.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      923 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/timeout.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50249 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/tracer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4413 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/unique.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1350 2024-04-09 17:01:34.000000 angr-9.2.98/angr/exploration_techniques/veritesting.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17411 2024-04-09 17:01:34.000000 angr-9.2.98/angr/factory.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.048810 angr-9.2.98/angr/flirt/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4428 2024-04-09 17:01:34.000000 angr-9.2.98/angr/flirt/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10109 2024-04-09 17:01:34.000000 angr-9.2.98/angr/flirt/build_sig.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-09 17:01:34.000000 angr-9.2.98/angr/graph_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18129 2024-04-09 17:01:34.000000 angr-9.2.98/angr/keyed_region.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.048810 angr-9.2.98/angr/knowledge_base/
+-rw-r--r--   0 vsts      (1001) docker     (127)       42 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_base/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4623 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_base/knowledge_base.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.052810 angr-9.2.98/angr/knowledge_plugins/
+-rw-r--r--   0 vsts      (1001) docker     (127)      697 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1597 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/callsite_prototypes.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.052810 angr-9.2.98/angr/knowledge_plugins/cfg/
+-rw-r--r--   0 vsts      (1001) docker     (127)      382 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/cfg/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2302 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/cfg/cfg_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41756 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/cfg/cfg_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17229 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/cfg/cfg_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2145 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/cfg/indirect_jump.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5040 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/cfg/memory_data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      304 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/comments.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1027 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/custom_strings.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      839 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8189 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/debug_variables.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.052810 angr-9.2.98/angr/knowledge_plugins/functions/
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/functions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    67184 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/functions/function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18990 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/functions/function_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11916 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/functions/function_parser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4971 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/functions/soot_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1024 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/indirect_jumps.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.056810 angr-9.2.98/angr/knowledge_plugins/key_definitions/
+-rw-r--r--   0 vsts      (1001) docker     (127)      397 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/key_definitions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9753 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/key_definitions/atoms.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/key_definitions/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8661 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/key_definitions/definition.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3907 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/key_definitions/environment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      922 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/key_definitions/heap_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3251 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/key_definitions/key_definition_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40482 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/key_definitions/live_definitions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7140 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/key_definitions/liveness.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7312 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/key_definitions/rd_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1682 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/key_definitions/tag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1236 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/key_definitions/undefined.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1510 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/key_definitions/unknown_size.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7468 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/key_definitions/uses.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3137 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4373 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/patches.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      733 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/plugin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.056810 angr-9.2.98/angr/knowledge_plugins/propagations/
+-rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/propagations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7706 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/propagations/prop_value.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2122 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/propagations/propagation_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2786 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/propagations/propagation_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39023 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/propagations/states.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.056810 angr-9.2.98/angr/knowledge_plugins/structured_code/
+-rw-r--r--   0 vsts      (1001) docker     (127)       43 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/structured_code/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2071 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/structured_code/manager.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.060810 angr-9.2.98/angr/knowledge_plugins/sync/
+-rw-r--r--   0 vsts      (1001) docker     (127)       44 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/sync/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9276 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/sync/sync_controller.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2038 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.060810 angr-9.2.98/angr/knowledge_plugins/variables/
+-rw-r--r--   0 vsts      (1001) docker     (127)       60 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/variables/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3751 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/variables/variable_access.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    45603 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/variables/variable_manager.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.060810 angr-9.2.98/angr/knowledge_plugins/xrefs/
+-rw-r--r--   0 vsts      (1001) docker     (127)       94 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/xrefs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4963 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/xrefs/xref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4009 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/xrefs/xref_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      271 2024-04-09 17:01:34.000000 angr-9.2.98/angr/knowledge_plugins/xrefs/xref_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.064810 angr-9.2.98/angr/misc/
+-rw-r--r--   0 vsts      (1001) docker     (127)      237 2024-04-09 17:01:34.000000 angr-9.2.98/angr/misc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      807 2024-04-09 17:01:34.000000 angr-9.2.98/angr/misc/ansi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3426 2024-04-09 17:01:34.000000 angr-9.2.98/angr/misc/autoimport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4241 2024-04-09 17:01:34.000000 angr-9.2.98/angr/misc/bug_report.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4486 2024-04-09 17:01:34.000000 angr-9.2.98/angr/misc/hookset.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1943 2024-04-09 17:01:34.000000 angr-9.2.98/angr/misc/import_hooks.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4225 2024-04-09 17:01:34.000000 angr-9.2.98/angr/misc/loggers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1276 2024-04-09 17:01:34.000000 angr-9.2.98/angr/misc/picklable_lock.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9370 2024-04-09 17:01:34.000000 angr-9.2.98/angr/misc/plugins.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      509 2024-04-09 17:01:34.000000 angr-9.2.98/angr/misc/range.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      593 2024-04-09 17:01:34.000000 angr-9.2.98/angr/misc/testing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      701 2024-04-09 17:01:34.000000 angr-9.2.98/angr/misc/ux.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1453 2024-04-09 17:01:34.000000 angr-9.2.98/angr/misc/weakpatch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.064810 angr-9.2.98/angr/procedures/
+-rw-r--r--   0 vsts      (1001) docker     (127)      119 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.064810 angr-9.2.98/angr/procedures/advapi32/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/advapi32/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.064810 angr-9.2.98/angr/procedures/cgc/
+-rw-r--r--   0 vsts      (1001) docker     (127)       76 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/cgc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      224 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/cgc/_terminate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3371 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/cgc/allocate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1984 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/cgc/deallocate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2802 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/cgc/fdwait.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2334 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/cgc/random.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3758 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/cgc/receive.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2368 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/cgc/transmit.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.184811 angr-9.2.98/angr/procedures/definitions/
+-rw-r--r--   0 vsts      (1001) docker     (127)    32023 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/cgc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   394191 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/glibc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/gnulib.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      700 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/libstdcpp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   238887 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/linux_kernel.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      219 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/linux_loader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      601 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/msvcr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1795 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/parse_syscalls_from_local_system.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   110573 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/parse_win32json.py
+-rw-r--r--   0 vsts      (1001) docker     (127)  9998064 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/types_win32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1458 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/wdk_api-ms-win-dx-d3dkmt-l1-1-4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1000 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/wdk_api-ms-win-dx-d3dkmt-l1-1-6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22852 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/wdk_clfs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   111981 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/wdk_fltmgr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1730 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/wdk_fwpkclnt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    68446 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/wdk_fwpuclnt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    37307 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/wdk_gdi32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11415 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/wdk_hal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12527 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/wdk_ksecdd.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33948 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/wdk_ndis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   593050 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/wdk_ntoskrnl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9862 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/wdk_offreg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1980 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/wdk_pshed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3478 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/wdk_secur32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1942 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/wdk_vhfum.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1553 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_aclui.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7877 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_activeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   310929 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_advapi32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22314 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_advpack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3430 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_amsi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3769 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3051 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      922 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-apiquery-l2-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1060 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-backgroundtask-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1134 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1167 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1488 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-enclave-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1037 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-errorhandling-l1-1-3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2317 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1217 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4874 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-file-fromapp-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1125 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-handle-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5164 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-ioring-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2219 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-marshal-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2528 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1492 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3867 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2362 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2378 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8406 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-path-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1547 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1562 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1429 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1850 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1281 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-slapi-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1682 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-state-helpers-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1540 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-synch-l1-2-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      995 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1184 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1467 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      951 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1537 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-util-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3268 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3777 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3228 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-winrt-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1162 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-winrt-registration-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      901 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-winrt-robuffer-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1694 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-winrt-roparameterizediid-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10986 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1550 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1653 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-wow64-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6949 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6680 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-dx-d3dkmt-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1043 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-gaming-deviceinformation-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1347 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-gaming-expandedresources-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3983 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1753 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5014 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2233 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4359 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1207 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-mm-misc-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3912 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-net-isolation-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1434 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-security-base-l1-2-2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1041 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1100 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1289 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1344 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1833 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1687 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2545 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      994 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1817 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-shcore-stream-winrt-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3586 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-wsl-api-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1117 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_apphelp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17589 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_authz.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2884 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_avicap32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18938 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_avifil32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5529 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_avrt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1328 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_bcp47mrm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24333 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_bcrypt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1325 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_bcryptprimitives.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17641 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_bluetoothapis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10950 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_bthprops.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3094 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_bthprops_cpl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16642 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_cabinet.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6820 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_certadm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4345 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_certpoleng.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   101560 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_cfgmgr32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26407 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_chakra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14271 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_cldapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24138 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_clfsw32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   111741 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_clusapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43365 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_comctl32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4894 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_comdlg32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2651 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_compstui.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19474 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_computecore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16032 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_computenetwork.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4405 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_computestorage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2241 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_comsvcs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1201 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_coremessaging.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11823 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_credui.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   105559 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_crypt32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3864 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_cryptnet.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4935 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_cryptui.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9065 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_cryptxml.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1769 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_cscapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5253 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_d2d1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11546 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_d3d10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_d3d10_1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3575 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_d3d11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4078 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_d3d12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3002 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_d3d9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13432 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_d3dcompiler_47.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4827 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_d3dcsx.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7266 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_davclnt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2063 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dbgeng.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   109042 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dbghelp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1028 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dbgmodel.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7151 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dciman32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4837 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dcomp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4233 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_ddraw.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1134 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_deviceaccess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1145 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dflayout.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5570 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dhcpcsvc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2967 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dhcpcsvc6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    81410 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dhcpsapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13697 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_diagnosticdataquery.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1243 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dinput8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1621 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_directml.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1261 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dmprocessxmlfiltered.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22815 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dnsapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5579 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_drt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3373 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_drtprov.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1445 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_drttransport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5367 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dsound.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11582 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dsparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2935 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dsprop.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6189 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dssec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1855 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dsuiext.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9715 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dwmapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1120 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dwrite.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1484 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dxcompiler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1061 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dxcore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2185 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dxgi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14554 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_dxva2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10117 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_eappcfg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9178 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_eappprxy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1311 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_efswrt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2446 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_elscore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   105927 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_esent.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3146 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_evr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1687 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_faultrep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2401 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_fhsvcctl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2011 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_firewallapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12020 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_fltlib.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4105 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_fontsub.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1227 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_forceinline.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    93548 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_fwpuclnt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1129 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_fxsutility.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   148174 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_gdi32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   247483 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_gdiplus.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16771 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_glu32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2162 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_gpedit.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1678 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_hhctrl_ocx.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21797 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_hid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12512 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_hlink.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1027 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_hrtfapo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19733 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_httpapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12533 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_icm32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1161 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_icmui.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   373759 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_icu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10129 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_ieframe.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11559 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_imagehlp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3884 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_imgutil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28246 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_imm32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8100 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_infocardapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8943 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_inkobjcore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    65729 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_iphlpapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28599 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_iscsidsc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1293 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_isolatedwindowsenvironmentutils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   505053 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_kernel32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3158 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_kernelbase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2060 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_keycredmgr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3689 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_ksproxy_ax.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4328 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_ksuser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14607 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_ktmw32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1582 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_licenseprotection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4334 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_loadperf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6878 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_magnification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25169 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mapi32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1411 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mdmlocalmanagement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4765 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mdmregistration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17507 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1358 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mfcore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    45685 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mfplat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1326 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mfplay.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2429 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mfreadwrite.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4363 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mfsensorgroup.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1451 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mfsrcsnk.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4531 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mgmtapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1232 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1326 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mmdevapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19241 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mpr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    47666 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mprapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13037 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mqrt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11736 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mrmsupport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19430 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_msacm32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   183424 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_msajapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34895 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mscms.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11975 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mscoree.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1327 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_msctfmonitor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7687 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_msdelta.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4589 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_msdmo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39076 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_msdrm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   103106 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_msi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2796 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_msimg32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11181 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mspatcha.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6011 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mspatchc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2844 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_msports.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7471 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_msrating.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7594 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mssign32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mstask.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16749 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_msvfw32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9190 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mswsock.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      973 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_mtxdm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19693 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_ncrypt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6200 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_ndfapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86057 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_netapi32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3436 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_netsh.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1151 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_netshell.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6101 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_newdev.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11168 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_ninput.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_normaliz.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27742 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_ntdll.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1087 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_ntdllk.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    35639 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_ntdsapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4407 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_ntlanman.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    94760 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_odbc32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8509 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_odbcbcp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   103812 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_ole32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7007 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_oleacc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   123410 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_oleaut32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6811 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_oledlg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2609 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_ondemandconnroutehelper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75467 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_opengl32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1461 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_opmxbox.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    32523 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_p2p.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12455 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_p2pgraph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39415 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_pdh.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14293 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_peerdist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    32180 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_powrprof.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_prntvpt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7998 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_projectedfslib.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    69946 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_propsys.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10760 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_psapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1362 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_quartz.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2051 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_query.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5253 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_qwave.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30989 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_rasapi32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2820 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_rasdlg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    54566 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_resutils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1012 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_rometadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22447 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_rpcns4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1683 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_rpcproxy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   148359 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_rpcrt4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4988 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_rstrtmgr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36043 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_rtm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15136 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_rtutils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9078 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_rtworkq.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_sas.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1646 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_scarddlg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3588 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_schannel.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1712 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_sechost.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    37550 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_secur32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1495 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_sensapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13284 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_sensorsutilsv2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157765 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_setupapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2546 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_sfc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1932 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_shdocvw.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    81141 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_shell32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   108109 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_shlwapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14350 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_slc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2850 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_slcext.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1143 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_slwga.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6443 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_snmpapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9685 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_spoolss.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      954 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_srclient.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3752 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_srpapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3032 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_sspicli.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1150 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_sti.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9597 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_t2embed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    94966 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_tapi32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4951 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_tbs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11389 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_tdh.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4744 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_tokenbinding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8278 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_traffic.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4327 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_txfw32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1627 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_ualapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    31556 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_uiautomationcore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27741 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_urlmon.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   252469 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_user32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15838 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_userenv.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23757 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_usp10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    31235 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_uxtheme.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1567 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_verifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7235 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3659 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_vertdll.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13507 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_virtdisk.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6032 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_vmdevicehost.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17637 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_vmsavedstatedumpprovider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      987 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_vssapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2698 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wcmapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3339 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wdsbp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13944 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wdsclientapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2846 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wdsmc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13248 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wdspxe.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4149 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wdstptc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4708 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_webauthn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   106080 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_webservices.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7433 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_websocket.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6419 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wecapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7708 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16155 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wevtapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21479 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_winbio.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1003 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_windows_ai_machinelearning.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      929 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_windows_data_pdf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3260 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_windows_media_mediacontrol.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      965 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_windows_networking.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1722 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_windows_ui_xaml.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4488 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_windowscodecs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22678 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_winfax.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22808 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_winhttp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2752 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_winhvemulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40942 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_winhvplatform.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   116017 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wininet.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      969 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_winml.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    55061 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_winmm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29221 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_winscard.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   114656 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_winspool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70042 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_winspool_drv.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22342 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wintrust.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14539 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_winusb.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30095 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wlanapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1412 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wlanui.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    97431 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wldap32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4202 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wldp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3239 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wmvcore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1385 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wnvapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5271 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wofutil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    65609 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_ws2_32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2275 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wscapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1471 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wsclient.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11200 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wsdapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16329 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wsmsvc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17715 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wsnmp32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25864 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_wtsapi32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1876 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_xaudio2_8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2916 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_xinput1_4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4574 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_xinputuap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3101 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_xmllite.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3094 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_xolehlp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2387 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/definitions/win32_xpsprint.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.184811 angr-9.2.98/angr/procedures/glibc/
+-rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/glibc/__ctype_b_loc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      791 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/glibc/__ctype_tolower_loc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      791 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/glibc/__ctype_toupper_loc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      157 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/glibc/__errno_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      110 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/glibc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1520 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/glibc/__libc_init.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11094 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/glibc/__libc_start_main.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      660 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/glibc/dynamic_loading.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      146 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/glibc/scanf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       75 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/glibc/sscanf.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.184811 angr-9.2.98/angr/procedures/gnulib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      115 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/gnulib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      181 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/gnulib/xalloc_die.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      239 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/gnulib/xstrtol_fatal.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.188811 angr-9.2.98/angr/procedures/java/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1224 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3381 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java/unconstrained.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.188811 angr-9.2.98/angr/procedures/java_io/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_io/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      335 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_io/read.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      613 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_io/write.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.188811 angr-9.2.98/angr/procedures/java_jni/
+-rw-r--r--   0 vsts      (1001) docker     (127)    21472 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_jni/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10385 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_jni/array_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1056 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_jni/class_and_interface_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4789 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_jni/field_access.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_jni/global_and_local_refs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9597 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_jni/method_calls.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      932 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_jni/not_implemented.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2725 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_jni/object_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2602 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_jni/string_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      229 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_jni/version_information.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.192811 angr-9.2.98/angr/procedures/java_lang/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_lang/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      983 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_lang/character.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      734 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_lang/double.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      255 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_lang/exit.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_lang/getsimplename.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1497 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_lang/integer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      241 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_lang/load_library.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      346 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_lang/math.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3174 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_lang/string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1579 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_lang/stringbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      413 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_lang/system.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.192811 angr-9.2.98/angr/procedures/java_util/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1229 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_util/collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1605 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_util/iterator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3727 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_util/list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4870 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_util/map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      373 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_util/random.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      797 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/java_util/scanner_nextline.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.208811 angr-9.2.98/angr/procedures/libc/
+-rw-r--r--   0 vsts      (1001) docker     (127)       95 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      105 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/abort.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      285 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/access.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      365 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/atoi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      296 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/atol.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      185 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/calloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      183 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/closelog.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      430 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/err.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2276 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/error.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      198 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/exit.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      590 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/fclose.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      572 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/feof.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      223 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/fflush.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      615 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/fgetc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2805 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/fgets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2598 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/fopen.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      730 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/fprintf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      537 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/fputc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      662 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/fputs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      614 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/fread.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      159 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/free.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      649 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/fscanf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/fseek.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      515 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/ftell.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      508 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/fwrite.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      315 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/getchar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4047 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/getdelim.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      126 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/getegid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      126 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/geteuid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      125 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/getgid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2636 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/gets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      125 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/getuid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      221 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/malloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3226 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/memcmp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1460 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/memcpy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2395 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/memset.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      206 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/openlog.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      333 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/perror.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      846 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/printf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      275 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/putchar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      449 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/puts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      196 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/rand.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      167 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/realloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      237 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/rewind.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      513 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/scanf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/setbuf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      110 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/setvbuf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1175 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/snprintf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      675 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/sprintf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       90 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/srand.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      353 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/sscanf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      485 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/stpcpy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/strcat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1771 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/strchr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      818 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/strcmp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      412 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/strcpy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3540 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/strlen.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      501 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/strncat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7653 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/strncmp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      600 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/strncpy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      384 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/strnlen.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3676 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/strstr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11852 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/strtol.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      273 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/strtoul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      340 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/system.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      264 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/time.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      512 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/tmpnam.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      206 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/tolower.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      207 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/toupper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      625 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/ungetc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      415 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/vsnprintf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      538 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libc/wchar.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.208811 angr-9.2.98/angr/procedures/libstdcpp/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libstdcpp/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      181 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libstdcpp/_unwind_resume.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      321 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libstdcpp/std____throw_bad_alloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      320 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libstdcpp/std____throw_bad_cast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      379 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libstdcpp/std____throw_length_error.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      378 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libstdcpp/std____throw_logic_error.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      268 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/libstdcpp/std__terminate.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.216811 angr-9.2.98/angr/procedures/linux_kernel/
+-rw-r--r--   0 vsts      (1001) docker     (127)      111 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      569 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/access.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1045 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/arch_prctl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1558 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/arm_user_helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      329 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/brk.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      719 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/cwd.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5177 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/fstat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6392 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/fstat64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      524 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/futex.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      375 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/getegid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      375 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/geteuid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      373 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/getgid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      229 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/getpid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      779 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/getrlimit.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      141 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/gettid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      373 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/getuid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1450 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/iovec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1190 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/lseek.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      484 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/mmap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1396 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/mprotect.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      186 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/munmap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1076 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/openat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      205 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/set_tid_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      618 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/sigaction.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      748 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/sigprocmask.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      666 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/stat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2205 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/sysinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      236 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/tgkill.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1000 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/time.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      764 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/uid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1127 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/uname.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      708 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/unlink.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      492 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_kernel/vsyscall.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.216811 angr-9.2.98/angr/procedures/linux_loader/
+-rw-r--r--   0 vsts      (1001) docker     (127)      115 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_loader/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      129 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_loader/_dl_initial_error_catch_tsd.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      337 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_loader/_dl_rtld_lock.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1876 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_loader/sim_loader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1548 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/linux_loader/tls.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.216811 angr-9.2.98/angr/procedures/msvcr/
+-rw-r--r--   0 vsts      (1001) docker     (127)      691 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/msvcr/__getmainargs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      116 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/msvcr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1363 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/msvcr/_initterm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      752 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/msvcr/fmode.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.220811 angr-9.2.98/angr/procedures/ntdll/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/ntdll/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2693 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/ntdll/exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.228811 angr-9.2.98/angr/procedures/posix/
+-rw-r--r--   0 vsts      (1001) docker     (127)       66 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1246 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/accept.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      316 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/bind.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      174 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/bzero.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      739 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/chroot.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      200 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/close.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       64 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/closedir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1917 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/dup.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      314 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/fcntl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2850 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/fdopen.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      414 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/fileno.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      292 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/fork.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1383 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/getenv.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1573 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/gethostbyname.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      484 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/getpass.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      187 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/getsockopt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/htonl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/htons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1950 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/inet_ntoa.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      315 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/listen.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5042 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/mmap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      537 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/open.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      291 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/opendir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2247 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/poll.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1355 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/pread64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2402 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/pthread.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1362 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/pwrite64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      252 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/read.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2161 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/readdir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      275 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/recv.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      298 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/recvfrom.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1979 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/select.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      711 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/send.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      167 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/setsockopt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      784 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/sigaction.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1654 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/sim_time.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      145 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/sleep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/socket.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      678 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/strcasecmp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/strdup.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2791 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/strtok_r.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      430 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/syslog.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      260 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/tz.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      282 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/unlink.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      140 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/usleep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      254 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/posix/write.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1865 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/procedure_dict.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.232811 angr-9.2.98/angr/procedures/stubs/
+-rw-r--r--   0 vsts      (1001) docker     (127)      219 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/stubs/CallReturn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      413 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/stubs/NoReturnUnconstrained.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       76 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/stubs/Nop.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/stubs/PathTerminator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      439 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/stubs/Redirect.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/stubs/ReturnChar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      774 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/stubs/ReturnUnconstrained.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      153 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/stubs/UnresolvableCallTarget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/stubs/UnresolvableJumpTarget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      561 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/stubs/UserHook.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/stubs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      342 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/stubs/b64_decode.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      343 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/stubs/caller.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/stubs/crazy_scanf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28192 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/stubs/format_parser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      902 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/stubs/syscall_stub.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.232811 angr-9.2.98/angr/procedures/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/testing/manyargs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      171 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/testing/retreg.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.232811 angr-9.2.98/angr/procedures/tracer/
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/tracer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      232 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/tracer/random.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      573 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/tracer/receive.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/tracer/transmit.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.232811 angr-9.2.98/angr/procedures/uclibc/
+-rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/uclibc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      293 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/uclibc/__uClibc_main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.240811 angr-9.2.98/angr/procedures/win32/
+-rw-r--r--   0 vsts      (1001) docker     (127)       97 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/EncodePointer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      134 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/ExitProcess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      228 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/GetCommandLine.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      105 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/GetCurrentProcessId.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      104 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/GetCurrentThreadId.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/GetLastInputInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      940 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/GetModuleHandle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1124 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/GetProcessAffinityMask.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      557 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/InterlockedExchange.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      201 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/IsProcessorFeaturePresent.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3985 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/VirtualAlloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2274 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/VirtualProtect.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       86 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      277 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/critical_section.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3424 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/dynamic_loading.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1455 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/file_handles.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      318 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/gethostbyname.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1541 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/heap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      757 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/is_bad_ptr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2130 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/local_storage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      177 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/mutex.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5332 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/sim_time.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1238 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32/system_paths.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.240811 angr-9.2.98/angr/procedures/win32_kernel/
+-rw-r--r--   0 vsts      (1001) docker     (127)      423 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32_kernel/ExAllocatePool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      225 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32_kernel/ExFreePoolWithTag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win32_kernel/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.240811 angr-9.2.98/angr/procedures/win_user32/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win_user32/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win_user32/chars.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      377 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win_user32/keyboard.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1717 2024-04-09 17:01:34.000000 angr-9.2.98/angr/procedures/win_user32/messagebox.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    37186 2024-04-09 17:01:34.000000 angr-9.2.98/angr/project.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.240811 angr-9.2.98/angr/protos/
+-rw-r--r--   0 vsts      (1001) docker     (127)      378 2024-04-09 17:01:34.000000 angr-9.2.98/angr/protos/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2389 2024-04-09 17:01:34.000000 angr-9.2.98/angr/protos/cfg_pb2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2146 2024-04-09 17:01:34.000000 angr-9.2.98/angr/protos/function_pb2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8527 2024-04-09 17:01:34.000000 angr-9.2.98/angr/protos/primitives_pb2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8112 2024-04-09 17:01:34.000000 angr-9.2.98/angr/protos/variables_pb2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1247 2024-04-09 17:01:34.000000 angr-9.2.98/angr/protos/xrefs_pb2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        8 2024-04-09 17:01:34.000000 angr-9.2.98/angr/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (127)     1502 2024-04-09 17:01:34.000000 angr-9.2.98/angr/serializable.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1102 2024-04-09 17:01:34.000000 angr-9.2.98/angr/service.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39300 2024-04-09 17:01:34.000000 angr-9.2.98/angr/sim_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18057 2024-04-09 17:01:34.000000 angr-9.2.98/angr/sim_options.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26081 2024-04-09 17:01:34.000000 angr-9.2.98/angr/sim_procedure.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    37826 2024-04-09 17:01:34.000000 angr-9.2.98/angr/sim_state.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12530 2024-04-09 17:01:34.000000 angr-9.2.98/angr/sim_state_options.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   121935 2024-04-09 17:01:34.000000 angr-9.2.98/angr/sim_type.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17228 2024-04-09 17:01:34.000000 angr-9.2.98/angr/sim_variable.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.244811 angr-9.2.98/angr/simos/
+-rw-r--r--   0 vsts      (1001) docker     (127)      755 2024-04-09 17:01:34.000000 angr-9.2.98/angr/simos/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5568 2024-04-09 17:01:34.000000 angr-9.2.98/angr/simos/cgc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21461 2024-04-09 17:01:34.000000 angr-9.2.98/angr/simos/javavm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23327 2024-04-09 17:01:34.000000 angr-9.2.98/angr/simos/linux.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18275 2024-04-09 17:01:34.000000 angr-9.2.98/angr/simos/simos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5679 2024-04-09 17:01:34.000000 angr-9.2.98/angr/simos/snimmuc_nxp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7351 2024-04-09 17:01:34.000000 angr-9.2.98/angr/simos/userland.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26047 2024-04-09 17:01:34.000000 angr-9.2.98/angr/simos/windows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10640 2024-04-09 17:01:34.000000 angr-9.2.98/angr/slicer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8467 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_hierarchy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.252811 angr-9.2.98/angr/state_plugins/
+-rw-r--r--   0 vsts      (1001) docker     (127)      735 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12092 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/callstack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4247 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/cgc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13310 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/concrete.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6844 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/debug_variables.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15902 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/filesystem.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5125 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/gdb.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1507 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/globals.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.252811 angr-9.2.98/angr/state_plugins/heap/
+-rw-r--r--   0 vsts      (1001) docker     (127)      136 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/heap/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6229 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/heap/heap_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5412 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/heap/heap_brk.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7886 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/heap/heap_freelist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1858 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/heap/heap_libc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28967 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/heap/heap_ptmalloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      793 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/heap/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19104 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/history.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11317 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/inspect.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/javavm_classloader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3403 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/jni_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23586 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/libc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6747 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/light_registers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2364 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4209 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/loop_data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6187 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27145 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/posix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8053 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/preconstrainer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6178 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/scratch.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9763 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/sim_action.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4268 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/sim_action_object.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2061 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/sim_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    45221 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/solver.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11039 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/symbolizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30091 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/trace_additions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2643 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/uc_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    78095 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/unicorn_engine.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12361 2024-04-09 17:01:34.000000 angr-9.2.98/angr/state_plugins/view.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.252811 angr-9.2.98/angr/storage/
+-rw-r--r--   0 vsts      (1001) docker     (127)      182 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    48379 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/file.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.256811 angr-9.2.98/angr/storage/memory_mixins/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11944 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1944 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/__init__.pyi
+-rw-r--r--   0 vsts      (1001) docker     (127)     3402 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/actions_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16569 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/address_concretization_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2901 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/bvv_conversion_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5496 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/clouseau_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      929 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/conditional_store_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10302 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/convenient_mappings_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6034 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/default_filler_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      317 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/dirty_addrs_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3668 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/hex_dumper_mixin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.256811 angr-9.2.98/angr/storage/memory_mixins/javavm_memory/
+-rw-r--r--   0 vsts      (1001) docker     (127)       51 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/javavm_memory/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15456 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/javavm_memory/javavm_memory_mixin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.260811 angr-9.2.98/angr/storage/memory_mixins/keyvalue_memory/
+-rw-r--r--   0 vsts      (1001) docker     (127)       55 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/keyvalue_memory/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      906 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/keyvalue_memory/keyvalue_memory_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      858 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/label_merger_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3036 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/multi_value_merger_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3412 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/name_resolution_mixin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.260811 angr-9.2.98/angr/storage/memory_mixins/paged_memory/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/paged_memory/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10282 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/paged_memory/page_backer_mixins.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29219 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/paged_memory/paged_memory_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2192 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/paged_memory/paged_memory_multivalue_mixin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.260811 angr-9.2.98/angr/storage/memory_mixins/paged_memory/pages/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1469 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/paged_memory/pages/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12776 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/paged_memory/pages/cooperation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3039 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/paged_memory/pages/history_tracking_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2050 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/paged_memory/pages/ispo_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14644 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/paged_memory/pages/list_page.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11302 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/paged_memory/pages/multi_values.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17713 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/paged_memory/pages/mv_list_page.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/paged_memory/pages/permissions_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1701 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/paged_memory/pages/refcount_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19139 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/paged_memory/pages/ultra_page.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1541 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/paged_memory/privileged_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3283 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/paged_memory/stack_allocation_mixin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.264811 angr-9.2.98/angr/storage/memory_mixins/regioned_memory/
+-rw-r--r--   0 vsts      (1001) docker     (127)      351 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/regioned_memory/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1098 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/regioned_memory/abstract_address_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1313 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/regioned_memory/abstract_merger_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      128 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/regioned_memory/region_category_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9196 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/regioned_memory/region_data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4355 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/regioned_memory/region_meta_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4891 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/regioned_memory/regioned_address_concretization_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18638 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/regioned_memory/regioned_memory_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2240 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/regioned_memory/static_find_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2596 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/simple_interface_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      502 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/simplification_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5659 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/size_resolution_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4884 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/slotted_memory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5655 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/smart_find_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      411 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/symbolic_merger_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      659 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/top_merger_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2590 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/underconstrained_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1027 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_mixins/unwrapper_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6253 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/memory_object.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1940 2024-04-09 17:01:34.000000 angr-9.2.98/angr/storage/pcap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3239 2024-04-09 17:01:34.000000 angr-9.2.98/angr/tablespecs.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.268811 angr-9.2.98/angr/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)      980 2024-04-09 17:01:34.000000 angr-9.2.98/angr/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      995 2024-04-09 17:01:34.000000 angr-9.2.98/angr/utils/algo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      209 2024-04-09 17:01:34.000000 angr-9.2.98/angr/utils/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2160 2024-04-09 17:01:34.000000 angr-9.2.98/angr/utils/cowdict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3107 2024-04-09 17:01:34.000000 angr-9.2.98/angr/utils/dynamic_dictlist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2091 2024-04-09 17:01:34.000000 angr-9.2.98/angr/utils/enums_conv.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      363 2024-04-09 17:01:34.000000 angr-9.2.98/angr/utils/env.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4217 2024-04-09 17:01:34.000000 angr-9.2.98/angr/utils/formatting.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5240 2024-04-09 17:01:34.000000 angr-9.2.98/angr/utils/funcid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28417 2024-04-09 17:01:34.000000 angr-9.2.98/angr/utils/graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      308 2024-04-09 17:01:34.000000 angr-9.2.98/angr/utils/lazy_import.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7202 2024-04-09 17:01:34.000000 angr-9.2.98/angr/utils/library.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1944 2024-04-09 17:01:34.000000 angr-9.2.98/angr/utils/loader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1825 2024-04-09 17:01:34.000000 angr-9.2.98/angr/utils/mp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20431 2024-04-09 17:01:34.000000 angr-9.2.98/angr/utils/segment_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1334 2024-04-09 17:01:34.000000 angr-9.2.98/angr/utils/timing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      417 2024-04-09 17:01:34.000000 angr-9.2.98/angr/utils/typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9701 2024-04-09 17:01:34.000000 angr-9.2.98/angr/vaults.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.268811 angr-9.2.98/angr.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4769 2024-04-09 17:03:01.000000 angr-9.2.98/angr.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    56754 2024-04-09 17:03:01.000000 angr-9.2.98/angr.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-09 17:03:01.000000 angr-9.2.98/angr.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       44 2024-04-09 17:03:01.000000 angr-9.2.98/angr.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      567 2024-04-09 17:03:01.000000 angr-9.2.98/angr.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-04-09 17:03:01.000000 angr-9.2.98/angr.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.268811 angr-9.2.98/native/
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-09 17:01:34.000000 angr-9.2.98/native/Makefile
+-rw-r--r--   0 vsts      (1001) docker     (127)      320 2024-04-09 17:01:34.000000 angr-9.2.98/native/Makefile-win
+-rw-r--r--   0 vsts      (1001) docker     (127)     1431 2024-04-09 17:01:34.000000 angr-9.2.98/native/angr_native.def
+-rw-r--r--   0 vsts      (1001) docker     (127)     3940 2024-04-09 17:01:34.000000 angr-9.2.98/native/log.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     2754 2024-04-09 17:01:34.000000 angr-9.2.98/native/log.h
+-rw-r--r--   0 vsts      (1001) docker     (127)   119496 2024-04-09 17:01:34.000000 angr-9.2.98/native/sim_unicorn.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    28878 2024-04-09 17:01:34.000000 angr-9.2.98/native/sim_unicorn.hpp
+-rw-r--r--   0 vsts      (1001) docker     (127)      855 2024-04-09 17:01:43.000000 angr-9.2.98/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1634 2024-04-09 17:03:02.272811 angr-9.2.98/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     3580 2024-04-09 17:01:34.000000 angr-9.2.98/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:02.268811 angr-9.2.98/tests/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     3392 2024-04-09 17:01:34.000000 angr-9.2.98/tests/test_calling_conventions.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)    14468 2024-04-09 17:01:34.000000 angr-9.2.98/tests/test_types.py
```

### Comparing `angr-9.2.97/LICENSE` & `angr-9.2.98/LICENSE`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/PKG-INFO` & `angr-9.2.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angr
-Version: 9.2.97
+Version: 9.2.98
 Summary: A multi-architecture binary analysis toolkit, with the ability to perform dynamic symbolic execution and various static analyses on binaries
 Home-page: https://github.com/angr/angr
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -13,31 +13,31 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: CppHeaderParser
 Requires-Dist: GitPython
-Requires-Dist: ailment==9.2.97
-Requires-Dist: archinfo==9.2.97
+Requires-Dist: ailment==9.2.98
+Requires-Dist: archinfo==9.2.98
 Requires-Dist: cachetools
 Requires-Dist: capstone==5.0.0.post1
 Requires-Dist: cffi>=1.14.0
-Requires-Dist: claripy==9.2.97
-Requires-Dist: cle==9.2.97
+Requires-Dist: claripy==9.2.98
+Requires-Dist: cle==9.2.98
 Requires-Dist: dpkt
 Requires-Dist: itanium-demangler
 Requires-Dist: mulpyplexer
 Requires-Dist: nampa
 Requires-Dist: networkx!=2.8.1,>=2.0
 Requires-Dist: protobuf>=3.19.0
 Requires-Dist: psutil
 Requires-Dist: pycparser>=2.18
 Requires-Dist: pyformlang
-Requires-Dist: pyvex==9.2.97
+Requires-Dist: pyvex==9.2.98
 Requires-Dist: rich>=13.1.0
 Requires-Dist: rpyc
 Requires-Dist: sortedcontainers
 Requires-Dist: sympy
 Requires-Dist: unicorn==2.0.1.post1
 Requires-Dist: unique-log-filter
 Requires-Dist: colorama; platform_system == "Windows"
```

### Comparing `angr-9.2.97/README.md` & `angr-9.2.98/README.md`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/__init__.py` & `angr-9.2.98/angr/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=wildcard-import
 # pylint: disable=wrong-import-position
 
-__version__ = "9.2.97"
+__version__ = "9.2.98"
 
 if bytes is str:
     raise Exception(
         """
 
 =-=-=-=-=-=-=-=-=-=-=-=-=  WELCOME TO THE FUTURE!  =-=-=-=-=-=-=-=-=-=-=-=-=-=
```

### Comparing `angr-9.2.97/angr/__main__.py` & `angr-9.2.98/angr/__main__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/__init__.py` & `angr-9.2.98/angr/analyses/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/analysis.py` & `angr-9.2.98/angr/analyses/analysis.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/backward_slice.py` & `angr-9.2.98/angr/analyses/backward_slice.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/binary_optimizer.py` & `angr-9.2.98/angr/analyses/binary_optimizer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/bindiff.py` & `angr-9.2.98/angr/analyses/bindiff.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/boyscout.py` & `angr-9.2.98/angr/analyses/boyscout.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/callee_cleanup_finder.py` & `angr-9.2.98/angr/analyses/callee_cleanup_finder.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/calling_convention.py` & `angr-9.2.98/angr/analyses/calling_convention.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/cdg.py` & `angr-9.2.98/angr/analyses/cdg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/cfg/cfb.py` & `angr-9.2.98/angr/analyses/cfg/cfb.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/cfg/cfg.py` & `angr-9.2.98/angr/analyses/cfg/cfg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/cfg/cfg_arch_options.py` & `angr-9.2.98/angr/analyses/cfg/cfg_arch_options.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/cfg/cfg_base.py` & `angr-9.2.98/angr/analyses/cfg/cfg_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from collections import defaultdict
 
 import networkx
 from sortedcontainers import SortedDict
 
 import pyvex
 from claripy.utils.orderedset import OrderedSet
-from cle import ELF, PE, Blob, TLSObject, MachO, ExternObject, KernelObject, FunctionHintSource, Hex, Coff, SRec
+from cle import ELF, PE, Blob, TLSObject, MachO, ExternObject, KernelObject, FunctionHintSource, Hex, Coff, SRec, XBE
 from cle.backends import NamedRegion
 import archinfo
 from archinfo.arch_soot import SootAddressDescriptor
 from archinfo.arch_arm import is_arm_arch, get_real_address_if_arm
 
 from angr.knowledge_plugins.functions.function_manager import FunctionManager
 from angr.knowledge_plugins.functions.function import Function
@@ -774,14 +774,25 @@
 
             elif isinstance(b, (Coff, PE)):
                 for section in b.sections:
                     if section.is_executable:
                         tpl = (section.min_addr, section.max_addr + 1)
                         memory_regions.append(tpl)
 
+            elif isinstance(b, XBE):
+                # some XBE files will mark the data sections as executable
+                for section in b.sections:
+                    if (
+                        section.is_executable
+                        and not section.is_writable
+                        and section.name not in {".data", ".rdata", ".rodata"}
+                    ):
+                        tpl = (section.min_addr, section.max_addr + 1)
+                        memory_regions.append(tpl)
+
             elif isinstance(b, MachO):
                 if b.segments:
                     # Get all executable segments
                     for seg in b.segments:
                         if seg.is_executable:
                             # Take all sections from this segment (MachO style)
                             for section in seg.sections:
@@ -793,17 +804,19 @@
                     for region_addr, region_size in b.regions:
                         memory_regions.append((region_addr, region_addr + region_size))
 
             elif isinstance(b, Blob):
                 # a blob is entirely executable
                 tpl = (b.min_addr, b.max_addr + 1)
                 memory_regions.append(tpl)
+
             elif isinstance(b, NamedRegion):
                 # NamedRegions have no content! Ignore
                 pass
+
             elif isinstance(b, self._cle_pseudo_objects):
                 pass
 
             else:
                 l.warning('Unsupported object format "%s". Treat it as an executable.', b.__class__.__name__)
 
                 tpl = (b.min_addr, b.max_addr + 1)
```

### Comparing `angr-9.2.97/angr/analyses/cfg/cfg_emulated.py` & `angr-9.2.98/angr/analyses/cfg/cfg_emulated.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/cfg/cfg_fast.py` & `angr-9.2.98/angr/analyses/cfg/cfg_fast.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/cfg/cfg_fast_soot.py` & `angr-9.2.98/angr/analyses/cfg/cfg_fast_soot.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/cfg/cfg_job_base.py` & `angr-9.2.98/angr/analyses/cfg/cfg_job_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/amd64_elf_got.py` & `angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/amd64_elf_got.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/amd64_pe_iat.py` & `angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/amd64_pe_iat.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/arm_elf_fast.py` & `angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/arm_elf_fast.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/const_resolver.py` & `angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/const_resolver.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/default_resolvers.py` & `angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/default_resolvers.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/jumptable.py` & `angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/jumptable.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/mips_elf_fast.py` & `angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/mips_elf_fast.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/propagator_utils.py` & `angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/propagator_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,18 @@
     def __init__(self, project):
         self.project = project
 
     def propagator_load_callback(self, addr, size) -> bool:  # pylint:disable=unused-argument
         # only allow loading if the address falls into a read-only region
         if isinstance(addr, claripy.ast.BV) and addr.op == "BVV":
             addr_v = addr.args[0]
-            section = self.project.loader.find_section_containing(addr_v)
-            if section is not None:
-                return section.is_readable and not section.is_writable
-            segment = self.project.loader.find_segment_containing(addr_v)
-            if segment is not None:
-                return segment.is_readable and not segment.is_writable
+        elif isinstance(addr, int):
+            addr_v = addr
+        else:
+            return False
+        section = self.project.loader.find_section_containing(addr_v)
+        if section is not None:
+            return section.is_readable and not section.is_writable
+        segment = self.project.loader.find_segment_containing(addr_v)
+        if segment is not None:
+            return segment.is_readable and not segment.is_writable
         return False
```

### Comparing `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/resolver.py` & `angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/resolver.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/x86_elf_pic_plt.py` & `angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/x86_elf_pic_plt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/x86_pe_iat.py` & `angr-9.2.98/angr/analyses/cfg/indirect_jump_resolvers/x86_pe_iat.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/cfg_slice_to_sink/cfg_slice_to_sink.py` & `angr-9.2.98/angr/analyses/cfg_slice_to_sink/cfg_slice_to_sink.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/cfg_slice_to_sink/graph.py` & `angr-9.2.98/angr/analyses/cfg_slice_to_sink/graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/cfg_slice_to_sink/transitions.py` & `angr-9.2.98/angr/analyses/cfg_slice_to_sink/transitions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/class_identifier.py` & `angr-9.2.98/angr/analyses/class_identifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/code_tagging.py` & `angr-9.2.98/angr/analyses/code_tagging.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/complete_calling_conventions.py` & `angr-9.2.98/angr/analyses/complete_calling_conventions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/congruency_check.py` & `angr-9.2.98/angr/analyses/congruency_check.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/data_dep/data_dependency_analysis.py` & `angr-9.2.98/angr/analyses/data_dep/data_dependency_analysis.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/data_dep/dep_nodes.py` & `angr-9.2.98/angr/analyses/data_dep/dep_nodes.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/data_dep/sim_act_location.py` & `angr-9.2.98/angr/analyses/data_dep/sim_act_location.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/datagraph_meta.py` & `angr-9.2.98/angr/analyses/datagraph_meta.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/ddg.py` & `angr-9.2.98/angr/analyses/ddg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/__init__.py` & `angr-9.2.98/angr/analyses/decompiler/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/ail_simplifier.py` & `angr-9.2.98/angr/analyses/decompiler/ail_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/ailgraph_walker.py` & `angr-9.2.98/angr/analyses/decompiler/ailgraph_walker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/block_io_finder.py` & `angr-9.2.98/angr/analyses/decompiler/block_io_finder.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/block_similarity.py` & `angr-9.2.98/angr/analyses/decompiler/block_similarity.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/block_simplifier.py` & `angr-9.2.98/angr/analyses/decompiler/block_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/call_counter.py` & `angr-9.2.98/angr/analyses/decompiler/call_counter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/callsite_maker.py` & `angr-9.2.98/angr/analyses/decompiler/callsite_maker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/ccall_rewriters/amd64_ccalls.py` & `angr-9.2.98/angr/analyses/decompiler/ccall_rewriters/amd64_ccalls.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/clinic.py` & `angr-9.2.98/angr/analyses/decompiler/clinic.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/condition_processor.py` & `angr-9.2.98/angr/analyses/decompiler/condition_processor.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/decompilation_cache.py` & `angr-9.2.98/angr/analyses/decompiler/decompilation_cache.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/decompilation_options.py` & `angr-9.2.98/angr/analyses/decompiler/decompilation_options.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/decompiler.py` & `angr-9.2.98/angr/analyses/decompiler/decompiler.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/empty_node_remover.py` & `angr-9.2.98/angr/analyses/decompiler/empty_node_remover.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/expression_counters.py` & `angr-9.2.98/angr/analyses/decompiler/expression_counters.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/expression_narrower.py` & `angr-9.2.98/angr/analyses/decompiler/expression_narrower.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/goto_manager.py` & `angr-9.2.98/angr/analyses/decompiler/goto_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/graph_region.py` & `angr-9.2.98/angr/analyses/decompiler/graph_region.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/jump_target_collector.py` & `angr-9.2.98/angr/analyses/decompiler/jump_target_collector.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/jumptable_entry_condition_rewriter.py` & `angr-9.2.98/angr/analyses/decompiler/jumptable_entry_condition_rewriter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/__init__.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from .x86_gcc_getpc_simplifier import X86GccGetPcSimplifier
 from .flip_boolean_cmp import FlipBooleanCmp
 from .ret_deduplicator import ReturnDeduplicator
 from .win_stack_canary_simplifier import WinStackCanarySimplifier
 from .cross_jump_reverter import CrossJumpReverter
 from .code_motion import CodeMotionOptimization
 from .switch_default_case_duplicator import SwitchDefaultCaseDuplicator
+from .inlined_string_transformation_simplifier import InlinedStringTransformationSimplifier
 
 # order matters!
 _all_optimization_passes = [
     (RegisterSaveAreaSimplifier, True),
     (StackCanarySimplifier, True),
     (WinStackCanarySimplifier, True),
     (BasePointerSaveSimplifier, True),
@@ -45,14 +46,15 @@
     (SwitchDefaultCaseDuplicator, True),
     (LoweredSwitchSimplifier, False),
     (ReturnDuplicatorLow, True),
     (ReturnDeduplicator, True),
     (CodeMotionOptimization, True),
     (CrossJumpReverter, True),
     (FlipBooleanCmp, True),
+    (InlinedStringTransformationSimplifier, True),
 ]
 
 # these passes may duplicate code to remove gotos or improve the structure of the graph
 DUPLICATING_OPTS = [ReturnDuplicatorLow, ReturnDuplicatorHigh, CrossJumpReverter]
 # these passes may destroy blocks by merging them into semantically equivalent blocks
 CONDENSING_OPTS = [CodeMotionOptimization, ReturnDeduplicator]
```

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/base_ptr_save_simplifier.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/base_ptr_save_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/code_motion.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/code_motion.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/const_derefs.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/const_derefs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/cross_jump_reverter.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/cross_jump_reverter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/div_simplifier.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/div_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/engine_base.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/engine_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/expr_op_swapper.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/expr_op_swapper.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/flip_boolean_cmp.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/flip_boolean_cmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/ite_expr_converter.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/ite_expr_converter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/ite_region_converter.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/ite_region_converter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/lowered_switch_simplifier.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/lowered_switch_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/mod_simplifier.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/mod_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/multi_simplifier.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/multi_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/optimization_pass.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/optimization_pass.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/register_save_area_simplifier.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/register_save_area_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/ret_addr_save_simplifier.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/ret_addr_save_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/ret_deduplicator.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/ret_deduplicator.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/return_duplicator_base.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/return_duplicator_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/return_duplicator_high.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/return_duplicator_high.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/return_duplicator_low.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/return_duplicator_low.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/stack_canary_simplifier.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/stack_canary_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/switch_default_case_duplicator.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/switch_default_case_duplicator.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/win_stack_canary_simplifier.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/win_stack_canary_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/optimization_passes/x86_gcc_getpc_simplifier.py` & `angr-9.2.98/angr/analyses/decompiler/optimization_passes/x86_gcc_getpc_simplifier.py`

 * *Files 9% similar despite different names*

```diff
@@ -72,13 +72,16 @@
         for key, block in self._blocks_by_addr_and_idx.items():
             if (
                 block.statements
                 and isinstance(block.statements[-1], ailment.Stmt.Call)
                 and isinstance(block.statements[-1].target, ailment.Expr.Const)
             ):
                 call_func_addr = block.statements[-1].target.value
-                call_func = self.kb.functions.get_by_addr(call_func_addr)
+                try:
+                    call_func = self.kb.functions.get_by_addr(call_func_addr)
+                except KeyError:
+                    continue
                 if "get_pc" in call_func.info:
                     results.append(
                         (key, len(block.statements) - 1, call_func.info["get_pc"], block.addr + block.original_size),
                     )
         return results
```

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/__init__.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from .single_bit_cond_to_boolexpr import SingleBitCondToBoolExpr
 from .sar_to_signed_div import SarToSignedDiv
 from .tidy_stack_addr import TidyStackAddr
 from .invert_negated_logical_conjuction_disjunction import InvertNegatedLogicalConjunctionsAndDisjunctions
 from .rol_ror import RolRorRewriter
 from .inlined_strcpy import InlinedStrcpy
 from .inlined_strcpy_consolidation import InlinedStrcpyConsolidation
+from .inlined_wstrcpy import InlinedWstrcpy
 
 from .base import PeepholeOptimizationExprBase, PeepholeOptimizationStmtBase, PeepholeOptimizationMultiStmtBase
 
 MULTI_STMT_OPTS: List[Type[PeepholeOptimizationMultiStmtBase]] = []
 STMT_OPTS: List[Type[PeepholeOptimizationStmtBase]] = []
 EXPR_OPTS: List[Type[PeepholeOptimizationExprBase]] = []
```

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_div_const_add_a_mul_n_div_const.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/a_div_const_add_a_mul_n_div_const.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_mul_const_div_shr_const.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/a_mul_const_div_shr_const.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_shl_const_sub_a.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/a_shl_const_sub_a.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div_const_mul_const.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div_const_mul_const.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_sub_a_sub_n.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/a_sub_a_sub_n.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/arm_cmpf.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/arm_cmpf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/base.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_add_n.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_add_n.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_and_mask.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_and_mask.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/bitwise_or_to_logical_or.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/bitwise_or_to_logical_or.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/bool_expr_xor_1.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/bool_expr_xor_1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/bswap.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/bswap.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/coalesce_same_cascading_ifs.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/coalesce_same_cascading_ifs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/const_mull_a_shift.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/const_mull_a_shift.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/constant_derefs.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/constant_derefs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/conv_a_sub0_shr_and.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/conv_a_sub0_shr_and.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/conv_shl_shr.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/conv_shl_shr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/eager_eval.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/eager_eval.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/extended_byte_and_mask.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/extended_byte_and_mask.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/inlined_strcpy_consolidation.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/inlined_strcpy_consolidation.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/invert_negated_logical_conjuction_disjunction.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/invert_negated_logical_conjuction_disjunction.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/one_sub_bool.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/one_sub_bool.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_cascading_conversions.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/remove_cascading_conversions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_empty_if_body.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/remove_empty_if_body.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_noop_conversions.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/remove_noop_conversions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_bitmasks.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/remove_redundant_bitmasks.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_conversions.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/remove_redundant_conversions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_ite_branch.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/remove_redundant_ite_branch.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_ite_comparisons.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/remove_redundant_ite_comparisons.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_reinterprets.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/remove_redundant_reinterprets.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_shifts.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/remove_redundant_shifts.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_shifts_around_comparators.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/remove_redundant_shifts_around_comparators.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/rewrite_bit_extractions.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/rewrite_bit_extractions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/rewrite_mips_gp_loads.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/rewrite_mips_gp_loads.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/rol_ror.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/rol_ror.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/sar_to_signed_div.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/sar_to_signed_div.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/simplify_pc_relative_loads.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/simplify_pc_relative_loads.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/single_bit_cond_to_boolexpr.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/single_bit_cond_to_boolexpr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/single_bit_xor.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/single_bit_xor.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/tidy_stack_addr.py` & `angr-9.2.98/angr/analyses/decompiler/peephole_optimizations/tidy_stack_addr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/redundant_label_remover.py` & `angr-9.2.98/angr/analyses/decompiler/redundant_label_remover.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/region_identifier.py` & `angr-9.2.98/angr/analyses/decompiler/region_identifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/cascading_cond_transformer.py` & `angr-9.2.98/angr/analyses/decompiler/region_simplifiers/cascading_cond_transformer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/cascading_ifs.py` & `angr-9.2.98/angr/analyses/decompiler/region_simplifiers/cascading_ifs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/expr_folding.py` & `angr-9.2.98/angr/analyses/decompiler/region_simplifiers/expr_folding.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/goto.py` & `angr-9.2.98/angr/analyses/decompiler/region_simplifiers/goto.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/if_.py` & `angr-9.2.98/angr/analyses/decompiler/region_simplifiers/if_.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/ifelse.py` & `angr-9.2.98/angr/analyses/decompiler/region_simplifiers/ifelse.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/loop.py` & `angr-9.2.98/angr/analyses/decompiler/region_simplifiers/loop.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/node_address_finder.py` & `angr-9.2.98/angr/analyses/decompiler/region_simplifiers/node_address_finder.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/region_simplifier.py` & `angr-9.2.98/angr/analyses/decompiler/region_simplifiers/region_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/switch_cluster_simplifier.py` & `angr-9.2.98/angr/analyses/decompiler/region_simplifiers/switch_cluster_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/switch_expr_simplifier.py` & `angr-9.2.98/angr/analyses/decompiler/region_simplifiers/switch_expr_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/region_walker.py` & `angr-9.2.98/angr/analyses/decompiler/region_walker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/seq_to_blocks.py` & `angr-9.2.98/angr/analyses/decompiler/seq_to_blocks.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/sequence_walker.py` & `angr-9.2.98/angr/analyses/decompiler/sequence_walker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/structured_codegen/base.py` & `angr-9.2.98/angr/analyses/decompiler/structured_codegen/base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/structured_codegen/c.py` & `angr-9.2.98/angr/analyses/decompiler/structured_codegen/c.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint:disable=missing-class-docstring,too-many-boolean-expressions,unused-argument
+# pylint:disable=missing-class-docstring,too-many-boolean-expressions,unused-argument,no-self-use
 from typing import Optional, Dict, List, Tuple, Set, Any, Union, TYPE_CHECKING, Callable
 from collections import defaultdict
 import logging
 import struct
 
 from ailment import Block, Expr, Stmt, Tmp
 from ailment.expression import StackBaseOffset, BinaryOp
@@ -2520,17 +2520,17 @@
             self._variables_in_use,
             self._variable_kb.variables[self._func.addr],
             demangled_name=self._func.demangled_name,
             show_demangled_name=self.show_demangled_name,
             codegen=self,
             omit_header=self.omit_func_header,
         )
-        self.cfunc = FieldReferenceCleanup.handle(self.cfunc)
-        self.cfunc = PointerArithmeticFixer.handle(self.cfunc)
-        self.cfunc = MakeTypecastsImplicit.handle(self.cfunc)
+        self.cfunc = FieldReferenceCleanup().handle(self.cfunc)
+        self.cfunc = PointerArithmeticFixer().handle(self.cfunc)
+        self.cfunc = MakeTypecastsImplicit().handle(self.cfunc)
 
         # TODO store extern fallback size somewhere lol
         self.cexterns = {
             self._variable(v, 1)
             for v in self.externs
             if v not in self._inlined_strings and v not in self._function_pointers
         }
@@ -3550,128 +3550,108 @@
         # FIXME
         stack_base = CFakeVariable("stack_base", SimTypePointer(SimTypeBottom()), codegen=self)
         ptr = CBinaryOp("Add", stack_base, CConstant(expr.offset, SimTypeInt(), codegen=self), codegen=self)
         return ptr
 
 
 class CStructuredCodeWalker:
-    @classmethod
-    def handle(cls, obj):
-        handler = getattr(cls, "handle_" + type(obj).__name__, cls.handle_default)
+    def handle(self, obj):
+        handler = getattr(self, "handle_" + type(obj).__name__, self.handle_default)
         return handler(obj)
 
-    @classmethod
-    def handle_default(cls, obj):
+    def handle_default(self, obj):
         return obj
 
-    @classmethod
-    def handle_CFunction(cls, obj):
-        obj.statements = cls.handle(obj.statements)
+    def handle_CFunction(self, obj):
+        obj.statements = self.handle(obj.statements)
         return obj
 
-    @classmethod
-    def handle_CStatements(cls, obj):
-        obj.statements = [cls.handle(stmt) for stmt in obj.statements]
+    def handle_CStatements(self, obj):
+        obj.statements = [self.handle(stmt) for stmt in obj.statements]
         return obj
 
-    @classmethod
-    def handle_CWhileLoop(cls, obj):
-        obj.condition = cls.handle(obj.condition)
-        obj.body = cls.handle(obj.body)
+    def handle_CWhileLoop(self, obj):
+        obj.condition = self.handle(obj.condition)
+        obj.body = self.handle(obj.body)
         return obj
 
-    @classmethod
-    def handle_CDoWhileLoop(cls, obj):
-        obj.condition = cls.handle(obj.condition)
-        obj.body = cls.handle(obj.body)
+    def handle_CDoWhileLoop(self, obj):
+        obj.condition = self.handle(obj.condition)
+        obj.body = self.handle(obj.body)
         return obj
 
-    @classmethod
-    def handle_CForLoop(cls, obj):
-        obj.initializer = cls.handle(obj.initializer)
-        obj.condition = cls.handle(obj.condition)
-        obj.iterator = cls.handle(obj.iterator)
-        obj.body = cls.handle(obj.body)
+    def handle_CForLoop(self, obj):
+        obj.initializer = self.handle(obj.initializer)
+        obj.condition = self.handle(obj.condition)
+        obj.iterator = self.handle(obj.iterator)
+        obj.body = self.handle(obj.body)
         return obj
 
-    @classmethod
-    def handle_CIfElse(cls, obj):
+    def handle_CIfElse(self, obj):
         obj.condition_and_nodes = [
-            (cls.handle(condition), cls.handle(node)) for condition, node in obj.condition_and_nodes
+            (self.handle(condition), self.handle(node)) for condition, node in obj.condition_and_nodes
         ]
-        obj.else_node = cls.handle(obj.else_node)
+        obj.else_node = self.handle(obj.else_node)
         return obj
 
-    @classmethod
-    def handle_CIfBreak(cls, obj):
-        obj.condition = cls.handle(obj.condition)
+    def handle_CIfBreak(self, obj):
+        obj.condition = self.handle(obj.condition)
         return obj
 
-    @classmethod
-    def handle_CSwitchCase(cls, obj):
-        obj.switch = cls.handle(obj.switch)
-        obj.cases = [(case, cls.handle(body)) for case, body in obj.cases]
-        obj.default = cls.handle(obj.default)
+    def handle_CSwitchCase(self, obj):
+        obj.switch = self.handle(obj.switch)
+        obj.cases = [(case, self.handle(body)) for case, body in obj.cases]
+        obj.default = self.handle(obj.default)
         return obj
 
-    @classmethod
-    def handle_CAssignment(cls, obj):
-        obj.lhs = cls.handle(obj.lhs)
-        obj.rhs = cls.handle(obj.rhs)
+    def handle_CAssignment(self, obj):
+        obj.lhs = self.handle(obj.lhs)
+        obj.rhs = self.handle(obj.rhs)
         return obj
 
-    @classmethod
-    def handle_CFunctionCall(cls, obj):
-        obj.callee_target = cls.handle(obj.callee_target)
-        obj.args = [cls.handle(arg) for arg in obj.args]
-        obj.ret_expr = cls.handle(obj.ret_expr)
+    def handle_CFunctionCall(self, obj):
+        obj.callee_target = self.handle(obj.callee_target)
+        obj.args = [self.handle(arg) for arg in obj.args]
+        obj.ret_expr = self.handle(obj.ret_expr)
         return obj
 
-    @classmethod
-    def handle_CReturn(cls, obj):
-        obj.retval = cls.handle(obj.retval)
+    def handle_CReturn(self, obj):
+        obj.retval = self.handle(obj.retval)
         return obj
 
-    @classmethod
-    def handle_CGoto(cls, obj):
-        obj.target = cls.handle(obj.target)
+    def handle_CGoto(self, obj):
+        obj.target = self.handle(obj.target)
         return obj
 
-    @classmethod
-    def handle_CIndexedVariable(cls, obj):
-        obj.variable = cls.handle(obj.variable)
-        obj.index = cls.handle(obj.index)
+    def handle_CIndexedVariable(self, obj):
+        obj.variable = self.handle(obj.variable)
+        obj.index = self.handle(obj.index)
         return obj
 
-    @classmethod
-    def handle_CVariableField(cls, obj):
-        obj.variable = cls.handle(obj.variable)
+    def handle_CVariableField(self, obj):
+        obj.variable = self.handle(obj.variable)
         return obj
 
-    @classmethod
-    def handle_CUnaryOp(cls, obj):
-        obj.operand = cls.handle(obj.operand)
+    def handle_CUnaryOp(self, obj):
+        obj.operand = self.handle(obj.operand)
         return obj
 
-    @classmethod
-    def handle_CBinaryOp(cls, obj):
-        obj.lhs = cls.handle(obj.lhs)
-        obj.rhs = cls.handle(obj.rhs)
+    def handle_CBinaryOp(self, obj):
+        obj.lhs = self.handle(obj.lhs)
+        obj.rhs = self.handle(obj.rhs)
         return obj
 
-    @classmethod
-    def handle_CTypeCast(cls, obj):
-        obj.expr = cls.handle(obj.expr)
+    def handle_CTypeCast(self, obj):
+        obj.expr = self.handle(obj.expr)
         return obj
 
-    @classmethod
-    def handle_CITE(cls, obj):
-        obj.cond = cls.handle(obj.cond)
-        obj.iftrue = cls.handle(obj.iftrue)
-        obj.iffalse = cls.handle(obj.iffalse)
+    def handle_CITE(self, obj):
+        obj.cond = self.handle(obj.cond)
+        obj.iftrue = self.handle(obj.iftrue)
+        obj.iffalse = self.handle(obj.iffalse)
         return obj
 
 
 class MakeTypecastsImplicit(CStructuredCodeWalker):
     @classmethod
     def collapse(cls, dst_ty: SimType, child: CExpression) -> CExpression:
         result = child
@@ -3698,71 +3678,65 @@
                 # more cases go here...
 
         if result is not child:
             # TODO this is not the best since it prohibits things like the BinaryOp optimizer from working incrementally
             return cls.collapse(dst_ty, result)
         return result
 
-    @classmethod
-    def handle_CAssignment(cls, obj):
-        obj.rhs = cls.collapse(obj.lhs.type, obj.rhs)
+    def handle_CAssignment(self, obj):
+        obj.rhs = self.collapse(obj.lhs.type, obj.rhs)
         return super().handle_CAssignment(obj)
 
-    @classmethod
-    def handle_CFunctionCall(cls, obj: CFunctionCall):
+    def handle_CFunctionCall(self, obj: CFunctionCall):
         for i, (c_arg, arg_ty) in enumerate(zip(obj.args, obj.prototype.args)):
-            obj.args[i] = cls.collapse(arg_ty, c_arg)
+            obj.args[i] = self.collapse(arg_ty, c_arg)
         return super().handle_CFunctionCall(obj)
 
-    @classmethod
-    def handle_CReturn(cls, obj: CReturn):
-        obj.retval = cls.collapse(obj.codegen._func.prototype.returnty, obj.retval)
+    def handle_CReturn(self, obj: CReturn):
+        obj.retval = self.collapse(obj.codegen._func.prototype.returnty, obj.retval)
         return super().handle_CReturn(obj)
 
-    @classmethod
-    def handle_CBinaryOp(cls, obj: CBinaryOp):
+    def handle_CBinaryOp(self, obj: CBinaryOp):
         obj = super().handle_CBinaryOp(obj)
         while True:
-            new_lhs = cls.collapse(obj.common_type, obj.lhs)
+            new_lhs = self.collapse(obj.common_type, obj.lhs)
             if (
                 new_lhs is not obj.lhs
                 and CBinaryOp.compute_common_type(obj.op, new_lhs.type, obj.rhs.type) == obj.common_type
             ):
                 obj.lhs = new_lhs
             else:
-                new_rhs = cls.collapse(obj.common_type, obj.rhs)
+                new_rhs = self.collapse(obj.common_type, obj.rhs)
                 if (
                     new_rhs is not obj.rhs
                     and CBinaryOp.compute_common_type(obj.op, obj.lhs.type, new_rhs.type) == obj.common_type
                 ):
                     obj.rhs = new_rhs
                 else:
                     break
         return obj
 
-    @classmethod
-    def handle_CTypeCast(cls, obj: CTypeCast):
+    def handle_CTypeCast(self, obj: CTypeCast):
         # note that the expression that this method returns may no longer be a CTypeCast
         obj = super().handle_CTypeCast(obj)
-        inner = cls.collapse(obj.dst_type, obj.expr)
+        inner = self.collapse(obj.dst_type, obj.expr)
         if inner is not obj.expr:
             obj.src_type = inner.type
             obj.expr = inner
         if obj.src_type == obj.dst_type or qualifies_for_implicit_cast(obj.src_type, obj.dst_type):
             return obj.expr
         return obj
 
 
 class FieldReferenceCleanup(CStructuredCodeWalker):
-    @classmethod
-    def handle_CTypeCast(cls, obj):
+    def handle_CTypeCast(self, obj):
         if isinstance(obj.dst_type, SimTypePointer) and not isinstance(obj.dst_type.pts_to, SimTypeBottom):
             obj = obj.codegen._access_reference(obj.expr, obj.dst_type.pts_to)
             if not isinstance(obj, CTypeCast):
-                return cls.handle(obj)
+                return self.handle(obj)
         return super().handle_CTypeCast(obj)
 
 
 class PointerArithmeticFixer(CStructuredCodeWalker):
     """
     Before calling this fixer class, pointer arithmetics are purely integer-based and ignoring the pointer type.
 
@@ -3772,16 +3746,15 @@
     a_ptr = a_ptr + 24;
 
     It means adding 24 to the address of a_ptr, without considering the size of struct A. This fixer class will make
     pointer arithmetics aware of the pointer type. In this case, the fixer class will convert the code to
     a_ptr = a_ptr + 1.
     """
 
-    @classmethod
-    def handle_CBinaryOp(cls, obj):
+    def handle_CBinaryOp(self, obj):
         obj: CBinaryOp = super().handle_CBinaryOp(obj)
         if (
             obj.op in ("Add", "Sub")
             and isinstance(obj.type, SimTypePointer)
             and not isinstance(obj.type.pts_to, SimTypeBottom)
         ):
             out = obj.codegen._access_reference(obj, obj.type.pts_to)
```

### Comparing `angr-9.2.97/angr/analyses/decompiler/structured_codegen/dummy.py` & `angr-9.2.98/angr/analyses/decompiler/structured_codegen/dummy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/structured_codegen/dwarf_import.py` & `angr-9.2.98/angr/analyses/decompiler/structured_codegen/dwarf_import.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/structuring/dream.py` & `angr-9.2.98/angr/analyses/decompiler/structuring/dream.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/structuring/phoenix.py` & `angr-9.2.98/angr/analyses/decompiler/structuring/phoenix.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/structuring/recursive_structurer.py` & `angr-9.2.98/angr/analyses/decompiler/structuring/recursive_structurer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/structuring/structurer_base.py` & `angr-9.2.98/angr/analyses/decompiler/structuring/structurer_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/structuring/structurer_nodes.py` & `angr-9.2.98/angr/analyses/decompiler/structuring/structurer_nodes.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/decompiler/utils.py` & `angr-9.2.98/angr/analyses/decompiler/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -565,15 +565,18 @@
 
 
 def peephole_optimize_stmts(block, stmt_opts):
     any_update = False
     statements = []
 
     # run statement optimizers
-    for stmt_idx, stmt in enumerate(block.statements):
+    # note that an optimizer may optionally edit or remove statements whose statement IDs are greater than stmt_idx
+    stmt_idx = 0
+    while stmt_idx < len(block.statements):
+        stmt = block.statements[stmt_idx]
         old_stmt = stmt
         redo = True
         while redo:
             redo = False
             for opt in stmt_opts:
                 if isinstance(stmt, opt.stmt_classes):
                     r = opt.optimize(stmt, stmt_idx=stmt_idx, block=block)
@@ -583,14 +586,15 @@
                         break
 
         if stmt is not None and stmt is not old_stmt:
             statements.append(stmt)
             any_update = True
         else:
             statements.append(old_stmt)
+        stmt_idx += 1
 
     return statements, any_update
 
 
 def match_stmt_classes(all_stmts: List, idx: int, stmt_class_seq: Iterable[type]) -> bool:
     for i, cls in enumerate(stmt_class_seq):
         if idx + i >= len(all_stmts):
```

### Comparing `angr-9.2.97/angr/analyses/disassembly.py` & `angr-9.2.98/angr/analyses/disassembly.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/disassembly_utils.py` & `angr-9.2.98/angr/analyses/disassembly_utils.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/dominance_frontier.py` & `angr-9.2.98/angr/analyses/dominance_frontier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/find_objects_static.py` & `angr-9.2.98/angr/analyses/find_objects_static.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/flirt.py` & `angr-9.2.98/angr/analyses/flirt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/forward_analysis/forward_analysis.py` & `angr-9.2.98/angr/analyses/forward_analysis/forward_analysis.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/forward_analysis/job_info.py` & `angr-9.2.98/angr/analyses/forward_analysis/job_info.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/forward_analysis/visitors/call_graph.py` & `angr-9.2.98/angr/analyses/forward_analysis/visitors/call_graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/forward_analysis/visitors/function_graph.py` & `angr-9.2.98/angr/analyses/forward_analysis/visitors/function_graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/forward_analysis/visitors/graph.py` & `angr-9.2.98/angr/analyses/forward_analysis/visitors/graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/forward_analysis/visitors/loop.py` & `angr-9.2.98/angr/analyses/forward_analysis/visitors/loop.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/forward_analysis/visitors/single_node_graph.py` & `angr-9.2.98/angr/analyses/forward_analysis/visitors/single_node_graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/custom_callable.py` & `angr-9.2.98/angr/analyses/identifier/custom_callable.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/func.py` & `angr-9.2.98/angr/analyses/identifier/func.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/__init__.py` & `angr-9.2.98/angr/analyses/identifier/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/atoi.py` & `angr-9.2.98/angr/analyses/identifier/functions/atoi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/based_atoi.py` & `angr-9.2.98/angr/analyses/identifier/functions/based_atoi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/fdprintf.py` & `angr-9.2.98/angr/analyses/identifier/functions/fdprintf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/free.py` & `angr-9.2.98/angr/analyses/identifier/functions/free.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/int2str.py` & `angr-9.2.98/angr/analyses/identifier/functions/int2str.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/malloc.py` & `angr-9.2.98/angr/analyses/identifier/functions/malloc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/memcmp.py` & `angr-9.2.98/angr/analyses/identifier/functions/memcmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/memcpy.py` & `angr-9.2.98/angr/analyses/identifier/functions/memcpy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/memset.py` & `angr-9.2.98/angr/analyses/identifier/functions/memset.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/printf.py` & `angr-9.2.98/angr/analyses/identifier/functions/printf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/recv_until.py` & `angr-9.2.98/angr/analyses/identifier/functions/recv_until.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/skip_calloc.py` & `angr-9.2.98/angr/analyses/identifier/functions/skip_calloc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/skip_realloc.py` & `angr-9.2.98/angr/analyses/identifier/functions/skip_realloc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/skip_recv_n.py` & `angr-9.2.98/angr/analyses/identifier/functions/skip_recv_n.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/snprintf.py` & `angr-9.2.98/angr/analyses/identifier/functions/snprintf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/sprintf.py` & `angr-9.2.98/angr/analyses/identifier/functions/sprintf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/strcasecmp.py` & `angr-9.2.98/angr/analyses/identifier/functions/strcasecmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/strcmp.py` & `angr-9.2.98/angr/analyses/identifier/functions/strcmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/strcpy.py` & `angr-9.2.98/angr/analyses/identifier/functions/strcpy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/strlen.py` & `angr-9.2.98/angr/analyses/identifier/functions/strlen.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/strncmp.py` & `angr-9.2.98/angr/analyses/identifier/functions/strncmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/strncpy.py` & `angr-9.2.98/angr/analyses/identifier/functions/strncpy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/functions/strtol.py` & `angr-9.2.98/angr/analyses/identifier/functions/strtol.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/identify.py` & `angr-9.2.98/angr/analyses/identifier/identify.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/identifier/runner.py` & `angr-9.2.98/angr/analyses/identifier/runner.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/init_finder.py` & `angr-9.2.98/angr/analyses/init_finder.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/loop_analysis.py` & `angr-9.2.98/angr/analyses/loop_analysis.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/loopfinder.py` & `angr-9.2.98/angr/analyses/loopfinder.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/propagator/engine_ail.py` & `angr-9.2.98/angr/analyses/propagator/engine_ail.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/propagator/engine_base.py` & `angr-9.2.98/angr/analyses/propagator/engine_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/propagator/engine_vex.py` & `angr-9.2.98/angr/analyses/propagator/engine_vex.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,17 @@
         if not (data is None or self.state.is_top(data)) or self.state._store_tops:
             if data is None:
                 # make sure it's a top
                 data = self.state.top(size * self.arch.byte_width)
             self.state.store_register(stmt.offset, size, data)
             self.state.add_replacement(self._codeloc(block_only=False), VEXReg(stmt.offset, size), data)
 
+    def _handle_PutI(self, stmt):
+        self._expr(stmt.data)
+
     def _store_data(self, addr, data, size, endness):
         # pylint: disable=unused-argument,no-self-use
         if isinstance(addr, claripy.ast.Base):
             sp_offset = self.extract_offset_to_sp(addr)
             if sp_offset is not None:
                 # Local variables
                 self.state.store_local_variable(sp_offset, size, data, endness)
@@ -256,14 +259,17 @@
     # Expression handlers
     #
 
     def _handle_Get(self, expr):
         size = expr.result_size(self.tyenv) // self.arch.byte_width
         return self.state.load_register(expr.offset, size)
 
+    def _handle_GetI(self, expr):
+        return self.state.top(expr.result_size(self.tyenv))
+
     def _handle_Load(self, expr):
         addr = self._expr(expr.addr)
         if addr is None or type(addr) in (Top, Bottom):
             return None
         size = expr.result_size(self.tyenv) // self.arch.byte_width
         return self._load_data(addr, size, expr.endness)
 
@@ -274,14 +280,21 @@
         if not self.state.do_binops:
             return self.state.top(expr.result_size(self.tyenv))
 
         r = super()._handle_Binop(expr)
         # print(expr.op, r)
         return r
 
+    def _handle_Triop(self, expr: pyvex.IRExpr.Triop):
+        if not self.state.do_binops:
+            return self.state.top(expr.result_size(self.tyenv))
+
+        r = super()._handle_Triop(expr)
+        return r
+
     def _handle_Conversion(self, expr):
         expr_ = self._expr(expr.args[0])
         to_size = expr.result_size(self.tyenv)
         if expr_ is None:
             return self._top(to_size)
         if self._is_top(expr_):
             return self._top(to_size).annotate(*expr_.annotations)
@@ -307,7 +320,9 @@
                 if isinstance(anno, RegisterComparisonAnnotation):
                     if anno.cmp_op == "eq":
                         v = (anno.offset, anno.size, anno.value)
                         if v not in self.state.block_initial_reg_values[self.block.addr, dst.concrete_value]:
                             self.state.block_initial_reg_values[self.block.addr, dst.concrete_value].append(v)
 
         super()._handle_Exit(stmt)
+
+    _handle_CmpF = _handle_CmpEQ
```

### Comparing `angr-9.2.97/angr/analyses/propagator/outdated_definition_walker.py` & `angr-9.2.98/angr/analyses/propagator/outdated_definition_walker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/propagator/propagator.py` & `angr-9.2.98/angr/analyses/propagator/propagator.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/propagator/values.py` & `angr-9.2.98/angr/analyses/propagator/values.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/propagator/vex_vars.py` & `angr-9.2.98/angr/analyses/propagator/vex_vars.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/proximity_graph.py` & `angr-9.2.98/angr/analyses/proximity_graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/reaching_definitions/__init__.py` & `angr-9.2.98/angr/analyses/reaching_definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/reaching_definitions/call_trace.py` & `angr-9.2.98/angr/analyses/reaching_definitions/call_trace.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/reaching_definitions/dep_graph.py` & `angr-9.2.98/angr/analyses/reaching_definitions/dep_graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/reaching_definitions/engine_ail.py` & `angr-9.2.98/angr/analyses/reaching_definitions/engine_ail.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/reaching_definitions/engine_vex.py` & `angr-9.2.98/angr/analyses/reaching_definitions/engine_vex.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,14 +172,17 @@
                     if stack_offset is not None:
                         self.state.add_stack_use(stack_offset, 1)
 
         if self.state.exit_observed and reg_offset == self.arch.sp_offset:
             return
         self.state.kill_and_add_definition(reg, data)
 
+    def _handle_PutI(self, stmt):
+        pass
+
     # e.g. STle(t6) = t21, t6 and/or t21 might include multiple values
     def _handle_Store(self, stmt):
         addr = self._expr(stmt.addr)
         size = stmt.data.result_size(self.tyenv) // 8
         data = self._expr(stmt.data)
 
         if addr.count() == 1:
@@ -400,14 +403,17 @@
                 for v in vs:
                     current_defs |= self.state.extract_defs(v)
 
         self.state.add_register_use_by_defs(current_defs)
 
         return values
 
+    def _handle_GetI(self, expr: pyvex.IRExpr.GetI) -> MultiValues:
+        return MultiValues(self.state.top(expr.result_size(self.tyenv)))
+
     # e.g. t27 = LDle:I64(t9), t9 might include multiple values
     # caution: Is also called from StoreG
     def _handle_Load(self, expr) -> MultiValues:
         addr = self._expr(expr.addr)
         bits = expr.result_size(self.tyenv)
         size = bits // self.arch.byte_width
```

### Comparing `angr-9.2.97/angr/analyses/reaching_definitions/function_handler.py` & `angr-9.2.98/angr/analyses/reaching_definitions/function_handler.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/reaching_definitions/heap_allocator.py` & `angr-9.2.98/angr/analyses/reaching_definitions/heap_allocator.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/reaching_definitions/rd_initializer.py` & `angr-9.2.98/angr/analyses/reaching_definitions/rd_initializer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/reaching_definitions/rd_state.py` & `angr-9.2.98/angr/analyses/reaching_definitions/rd_state.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/reaching_definitions/reaching_definitions.py` & `angr-9.2.98/angr/analyses/reaching_definitions/reaching_definitions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/reaching_definitions/subject.py` & `angr-9.2.98/angr/analyses/reaching_definitions/subject.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/reassembler.py` & `angr-9.2.98/angr/analyses/reassembler.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/soot_class_hierarchy.py` & `angr-9.2.98/angr/analyses/soot_class_hierarchy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/stack_pointer_tracker.py` & `angr-9.2.98/angr/analyses/stack_pointer_tracker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/static_hooker.py` & `angr-9.2.98/angr/analyses/static_hooker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/typehoon/dfa.py` & `angr-9.2.98/angr/analyses/typehoon/dfa.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/typehoon/lifter.py` & `angr-9.2.98/angr/analyses/typehoon/lifter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/typehoon/simple_solver.py` & `angr-9.2.98/angr/analyses/typehoon/simple_solver.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/typehoon/translator.py` & `angr-9.2.98/angr/analyses/typehoon/translator.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/typehoon/typeconsts.py` & `angr-9.2.98/angr/analyses/typehoon/typeconsts.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/typehoon/typehoon.py` & `angr-9.2.98/angr/analyses/typehoon/typehoon.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/typehoon/typevars.py` & `angr-9.2.98/angr/analyses/typehoon/typevars.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/variable_recovery/annotations.py` & `angr-9.2.98/angr/analyses/variable_recovery/annotations.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/variable_recovery/engine_ail.py` & `angr-9.2.98/angr/analyses/variable_recovery/engine_ail.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/variable_recovery/engine_base.py` & `angr-9.2.98/angr/analyses/variable_recovery/engine_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/variable_recovery/engine_vex.py` & `angr-9.2.98/angr/analyses/variable_recovery/engine_vex.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,17 @@
         r = self._expr(stmt.data)
         size = stmt.data.result_size(self.tyenv) // 8
 
         if offset == self.arch.ip_offset:
             return
         self._assign_to_register(offset, r, size)
 
+    def _handle_PutI(self, stmt):
+        pass
+
     def _handle_Store(self, stmt):
         addr_r = self._expr(stmt.addr)
         size = stmt.data.result_size(self.tyenv) // 8
         r = self._expr(stmt.data)
 
         self._store(addr_r, r, size, stmt=stmt)
 
@@ -155,14 +158,17 @@
             reg_offset,
             reg_size,
             expr=expr,
             force_variable_size=force_variable_size,
             create_variable=self.stmt_idx not in self.reg_read_stmts_to_ignore,
         )
 
+    def _handle_GetI(self, expr: pyvex.IRExpr.GetI):
+        return RichR(self.state.top(expr.result_size(self.tyenv)))
+
     def _handle_Load(self, expr: pyvex.IRExpr.Load) -> RichR:
         addr = self._expr(expr.addr)
         size = expr.result_size(self.tyenv) // 8
 
         return self._load(addr, size)
 
     def _handle_CCall(self, expr):  # pylint:disable=useless-return
```

### Comparing `angr-9.2.97/angr/analyses/variable_recovery/irsb_scanner.py` & `angr-9.2.98/angr/analyses/variable_recovery/irsb_scanner.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,20 @@
         #
         # we will not create a variable for the register read in the first instruction (read from r9) in this case.
         self.tmp_with_reg_as_value: Dict[int, int] = {}
         self.reg_with_reg_as_value: Dict[int, int] = {}
         self.reg_read_stmt_id: Dict[int, int] = {}
         self.reg_read_stmts_to_ignore: Set[int] = set()
 
+    def _top(self, size: int):
+        return None
+
+    def _is_top(self, expr) -> bool:
+        return True
+
     def _process_Stmt(self, whitelist=None):
         self.tmps_with_64bit_regs = set()
         self.tmps_assignment_stmtidx = {}
         self.tmps_converted_to_32bit = set()
 
         super()._process_Stmt(whitelist=whitelist)
 
@@ -51,14 +57,17 @@
                 # we are overwriting an existing register with a value from another register, before this register is
                 # ever used...
                 # in this case, we should ignore the previous register read
                 old_reg_offset = self.reg_with_reg_as_value[stmt.offset]
                 self.reg_read_stmts_to_ignore.add(self.reg_read_stmt_id[old_reg_offset])
             self.reg_with_reg_as_value[stmt.offset] = self.tmp_with_reg_as_value[stmt.data.tmp]
 
+    def _handle_PutI(self, stmt):
+        pass
+
     def _handle_Load(self, expr):
         pass
 
     def _handle_Store(self, stmt):
         pass
 
     def _handle_LoadG(self, stmt):
@@ -81,14 +90,17 @@
         super()._handle_WrTmp(stmt)
 
     def _handle_Get(self, expr):
         self.reg_read_stmt_id[expr.offset] = self.stmt_idx
         if expr.offset in self.reg_with_reg_as_value:
             del self.reg_with_reg_as_value[expr.offset]
 
+    def _handle_GetI(self, expr):
+        pass
+
     def _handle_RdTmp(self, expr):
         if expr.tmp in self.tmps_converted_to_32bit:
             self.tmps_converted_to_32bit.remove(expr.tmp)
 
     def _handle_Conversion(self, expr: pyvex.IRExpr.Unop):
         if expr.op == "Iop_64to32" and isinstance(expr.args[0], pyvex.IRExpr.RdTmp):
             # special handling for t11 = GET:I64(rdi); t4 = 64to32(t11) style of code in x86-64 (and other 64-bit
```

### Comparing `angr-9.2.97/angr/analyses/variable_recovery/variable_recovery.py` & `angr-9.2.98/angr/analyses/variable_recovery/variable_recovery.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/variable_recovery/variable_recovery_base.py` & `angr-9.2.98/angr/analyses/variable_recovery/variable_recovery_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/variable_recovery/variable_recovery_fast.py` & `angr-9.2.98/angr/analyses/variable_recovery/variable_recovery_fast.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/veritesting.py` & `angr-9.2.98/angr/analyses/veritesting.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/vfg.py` & `angr-9.2.98/angr/analyses/vfg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/vsa_ddg.py` & `angr-9.2.98/angr/analyses/vsa_ddg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/vtable.py` & `angr-9.2.98/angr/analyses/vtable.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/analyses/xrefs.py` & `angr-9.2.98/angr/analyses/xrefs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/angrdb/db.py` & `angr-9.2.98/angr/angrdb/db.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/angrdb/models.py` & `angr-9.2.98/angr/angrdb/models.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/angrdb/serializers/cfg_model.py` & `angr-9.2.98/angr/angrdb/serializers/cfg_model.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/angrdb/serializers/comments.py` & `angr-9.2.98/angr/angrdb/serializers/comments.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/angrdb/serializers/funcs.py` & `angr-9.2.98/angr/angrdb/serializers/funcs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/angrdb/serializers/kb.py` & `angr-9.2.98/angr/angrdb/serializers/kb.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/angrdb/serializers/labels.py` & `angr-9.2.98/angr/angrdb/serializers/labels.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/angrdb/serializers/loader.py` & `angr-9.2.98/angr/angrdb/serializers/loader.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/angrdb/serializers/structured_code.py` & `angr-9.2.98/angr/angrdb/serializers/structured_code.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/angrdb/serializers/variables.py` & `angr-9.2.98/angr/angrdb/serializers/variables.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/angrdb/serializers/xrefs.py` & `angr-9.2.98/angr/angrdb/serializers/xrefs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/annocfg.py` & `angr-9.2.98/angr/annocfg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/blade.py` & `angr-9.2.98/angr/blade.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/block.py` & `angr-9.2.98/angr/block.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/callable.py` & `angr-9.2.98/angr/callable.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/calling_conventions.py` & `angr-9.2.98/angr/calling_conventions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/code_location.py` & `angr-9.2.98/angr/code_location.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/codenode.py` & `angr-9.2.98/angr/codenode.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/concretization_strategies/__init__.py` & `angr-9.2.98/angr/concretization_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/concretization_strategies/any_named.py` & `angr-9.2.98/angr/concretization_strategies/any_named.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/concretization_strategies/controlled_data.py` & `angr-9.2.98/angr/concretization_strategies/controlled_data.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/concretization_strategies/eval.py` & `angr-9.2.98/angr/concretization_strategies/eval.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/concretization_strategies/logging.py` & `angr-9.2.98/angr/concretization_strategies/logging.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/concretization_strategies/max.py` & `angr-9.2.98/angr/concretization_strategies/max.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/concretization_strategies/nonzero.py` & `angr-9.2.98/angr/concretization_strategies/nonzero.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/concretization_strategies/nonzero_range.py` & `angr-9.2.98/angr/concretization_strategies/nonzero_range.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/concretization_strategies/norepeats.py` & `angr-9.2.98/angr/concretization_strategies/norepeats.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/concretization_strategies/norepeats_range.py` & `angr-9.2.98/angr/concretization_strategies/norepeats_range.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/concretization_strategies/range.py` & `angr-9.2.98/angr/concretization_strategies/range.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/concretization_strategies/signed_add.py` & `angr-9.2.98/angr/concretization_strategies/signed_add.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/concretization_strategies/solutions.py` & `angr-9.2.98/angr/concretization_strategies/solutions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/concretization_strategies/unlimited_range.py` & `angr-9.2.98/angr/concretization_strategies/unlimited_range.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/distributed/server.py` & `angr-9.2.98/angr/distributed/server.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/distributed/worker.py` & `angr-9.2.98/angr/distributed/worker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/__init__.py` & `angr-9.2.98/angr/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/concrete.py` & `angr-9.2.98/angr/engines/concrete.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/engine.py` & `angr-9.2.98/angr/engines/engine.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/failure.py` & `angr-9.2.98/angr/engines/failure.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/hook.py` & `angr-9.2.98/angr/engines/hook.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/light/data.py` & `angr-9.2.98/angr/engines/light/data.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/light/engine.py` & `angr-9.2.98/angr/engines/light/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,18 +235,63 @@
         if hasattr(self, handler):
             return getattr(self, handler)(expr)
         elif self.l is not None:
             self.l.error("Unsupported expression type %s.", type(expr).__name__)
         return None
 
     def _handle_Triop(self, expr: pyvex.IRExpr.Triop):  # pylint: disable=useless-return
-        if self.l is not None:
+        handler = None
+        if expr.op.startswith("Iop_AddF"):
+            handler = "_handle_AddF"
+        elif expr.op.startswith("Iop_SubF"):
+            handler = "_handle_AddF"
+        elif expr.op.startswith("Iop_MulF"):
+            handler = "_handle_MulF"
+        elif expr.op.startswith("Iop_DivF"):
+            handler = "_handle_DivF"
+        elif expr.op.startswith("Iop_SinF"):
+            handler = "_handle_SinF"
+        elif expr.op.startswith("Iop_ScaleF"):
+            handler = "_handle_ScaleF"
+
+        if handler is not None and hasattr(self, handler):
+            return getattr(self, handler)(expr)
+
+        if once(expr.op) and self.l is not None:
             self.l.error("Unsupported Triop %s.", expr.op)
+
         return None
 
+    def _handle_AddF(self, expr):
+        return self._top(expr.result_size(self.tyenv))
+
+    def _handle_SubF(self, expr):
+        return self._top(expr.result_size(self.tyenv))
+
+    def _handle_MulF(self, expr):
+        return self._top(expr.result_size(self.tyenv))
+
+    def _handle_DivF(self, expr):
+        return self._top(expr.result_size(self.tyenv))
+
+    def _handle_NegF(self, expr):
+        return self._top(expr.result_size(self.tyenv))
+
+    def _handle_AbsF(self, expr):
+        return self._top(expr.result_size(self.tyenv))
+
+    def _handle_SinF(self, expr):
+        return self._top(expr.result_size(self.tyenv))
+
+    def _handle_CosF(self, expr):
+        return self._top(expr.result_size(self.tyenv))
+
+    def _handle_ScaleF(self, expr):
+        return self._top(expr.result_size(self.tyenv))
+
     def _handle_RdTmp(self, expr):
         tmp = expr.tmp
 
         if tmp in self.tmps:
             return self.tmps[tmp]
         return None
 
@@ -290,14 +335,18 @@
             handler = "_handle_Not1"
         elif expr.op.startswith("Iop_Not"):
             handler = "_handle_Not"
         elif expr.op.startswith("Iop_Clz"):
             handler = "_handle_Clz"
         elif expr.op.startswith("Iop_Ctz"):
             handler = "_handle_Ctz"
+        elif expr.op.startswith("Iop_NegF"):
+            handler = "_handle_NegF"
+        elif expr.op.startswith("Iop_AbsF"):
+            handler = "_handle_AbsF"
 
         if handler is not None and hasattr(self, handler):
             return getattr(self, handler)(expr)
         else:
             if self.l is not None:
                 self.l.error("Unsupported Unop %s.", expr.op)
             return None
@@ -357,14 +406,18 @@
             handler = "_handle_32HLto64"
         elif expr.op.startswith("Const"):
             handler = "_handle_Const"
         elif expr.op.startswith("Iop_16HLto32"):
             handler = "_handle_16HLto32"
         elif expr.op.startswith("Iop_ExpCmpNE64"):
             handler = "_handle_ExpCmpNE64"
+        elif expr.op.startswith("Iop_SinF"):
+            handler = "_handle_SinF"
+        elif expr.op.startswith("Iop_CosF"):
+            handler = "_handle_CosF"
 
         vector_size, vector_count = None, None
         if handler is not None:
             # vector information
             m = re.match(r"Iop_[^\d]+(\d+)U{0,1}x(\d+)", expr.op)
             if m is not None:
                 vector_size = int(m.group(1))
@@ -535,14 +588,18 @@
         expr_0, expr_1 = args
 
         if self._is_top(expr_0) or self._is_top(expr_1):
             return self._top(expr_0.size())
 
         return expr_0 * expr_1
 
+    def _handle_Mull(self, expr):
+        self._binop_get_args(expr)
+        return self._top(expr.result_size(self.tyenv))
+
     def _handle_DivMod(self, expr):
         args, r = self._binop_get_args(expr)
         if args is None:
             return r
         expr_0, expr_1 = args
 
         if self._is_top(expr_0) or self._is_top(expr_1):
@@ -934,64 +991,118 @@
             b = struct.pack("<f", arg)
             v = struct.unpack("<I", b)[0]
             return v
 
         return expr
 
     def _ail_handle_UnaryOp(self, expr):
-        handler_name = "_ail_handle_%s" % expr.op
+        handler_name = f"_handle_{expr.op}"
         try:
             handler = getattr(self, handler_name)
         except AttributeError:
-            if self.l is not None:
-                self.l.warning("Unsupported UnaryOp %s.", expr.op)
-            return None
+            handler_name = "_ail_handle_%s" % expr.op
+            try:
+                handler = getattr(self, handler_name)
+            except AttributeError:
+                if self.l is not None:
+                    self.l.warning("Unsupported UnaryOp %s.", expr.op)
+                return None
 
         return handler(expr)
 
     def _ail_handle_BinaryOp(self, expr):
-        handler_name = "_ail_handle_%s" % expr.op
+        handler_name = f"_handle_{expr.op}"
         try:
             handler = getattr(self, handler_name)
         except AttributeError:
-            if self.l is not None:
-                self.l.warning("Unsupported BinaryOp %s.", expr.op)
-            return None
+            handler_name = "_ail_handle_%s" % expr.op
+            try:
+                handler = getattr(self, handler_name)
+            except AttributeError:
+                if self.l is not None:
+                    self.l.warning("Unsupported BinaryOp %s.", expr.op)
+                return None
 
         return handler(expr)
 
     def _ail_handle_TernaryOp(self, expr):
-        handler_name = "_ail_handle_%s" % expr.op
+        handler_name = f"_handle_{expr.op}"
         try:
             handler = getattr(self, handler_name)
         except AttributeError:
-            if self.l is not None:
-                self.l.warning("Unsupported Ternary %s.", expr.op)
-            return None
+            handler_name = "_ail_handle_%s" % expr.op
+            try:
+                handler = getattr(self, handler_name)
+            except AttributeError:
+                if self.l is not None:
+                    self.l.warning("Unsupported Ternary %s.", expr.op)
+                return None
 
         return handler(expr)
 
     #
     # Binary operation handlers
     #
 
+    def _ail_handle_CmpEQ(self, expr):
+        arg0, arg1 = expr.operands
+
+        expr_0 = self._expr(arg0)
+        expr_1 = self._expr(arg1)
+        if expr_0 is None:
+            expr_0 = arg0
+        if expr_1 is None:
+            expr_1 = arg1
+
+        try:
+            if isinstance(expr_0, ailment.Expr.Const) and isinstance(expr_1, ailment.Expr.Const):
+                if expr_0.value == expr_1.value:
+                    return ailment.Expr.Const(None, None, 1, 1)
+                return ailment.Expr.Const(None, None, 0, 1)
+        except TypeError:
+            pass
+        return ailment.Expr.BinaryOp(expr.idx, "CmpEQ", [expr_0, expr_1], expr.signed, **expr.tags)
+
+    def _ail_handle_CmpNE(self, expr):
+        arg0, arg1 = expr.operands
+
+        expr_0 = self._expr(arg0)
+        expr_1 = self._expr(arg1)
+        if expr_0 is None:
+            expr_0 = arg0
+        if expr_1 is None:
+            expr_1 = arg1
+
+        try:
+            if isinstance(expr_0, ailment.Expr.Const) and isinstance(expr_1, ailment.Expr.Const):
+                if expr_0.value != expr_1.value:
+                    return ailment.Expr.Const(None, None, 1, 1)
+                return ailment.Expr.Const(None, None, 0, 1)
+        except TypeError:
+            pass
+        return ailment.Expr.BinaryOp(expr.idx, "CmpNE", [expr_0, expr_1], expr.signed, **expr.tags)
+
     def _ail_handle_CmpLT(self, expr):
         arg0, arg1 = expr.operands
 
         expr_0 = self._expr(arg0)
         expr_1 = self._expr(arg1)
         if expr_0 is None:
             expr_0 = arg0
         if expr_1 is None:
             expr_1 = arg1
 
         try:
-            return expr_0 <= expr_1
+            if isinstance(expr_0, ailment.Expr.Const) and isinstance(expr_1, ailment.Expr.Const):
+                if expr_0.value < expr_1.value:
+                    return ailment.Expr.Const(None, None, 1, 1)
+                return ailment.Expr.Const(None, None, 0, 1)
         except TypeError:
-            return ailment.Expr.BinaryOp(expr.idx, "CmpLT", [expr_0, expr_1], expr.signed, **expr.tags)
+            pass
+        return ailment.Expr.BinaryOp(expr.idx, "CmpLT", [expr_0, expr_1], expr.signed, **expr.tags)
 
     def _ail_handle_Add(self, expr):
         arg0, arg1 = expr.operands
 
         expr_0 = self._expr(arg0)
         expr_1 = self._expr(arg1)
         if expr_0 is None:
```

### Comparing `angr-9.2.97/angr/engines/pcode/behavior.py` & `angr-9.2.98/angr/engines/pcode/behavior.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/pcode/cc.py` & `angr-9.2.98/angr/engines/pcode/cc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/pcode/emulate.py` & `angr-9.2.98/angr/engines/pcode/emulate.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/pcode/engine.py` & `angr-9.2.98/angr/engines/pcode/engine.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/pcode/lifter.py` & `angr-9.2.98/angr/engines/pcode/lifter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/procedure.py` & `angr-9.2.98/angr/engines/procedure.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/engine.py` & `angr-9.2.98/angr/engines/soot/engine.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/expressions/__init__.py` & `angr-9.2.98/angr/engines/soot/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/expressions/arrayref.py` & `angr-9.2.98/angr/engines/soot/expressions/arrayref.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/expressions/binop.py` & `angr-9.2.98/angr/engines/soot/expressions/binop.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/expressions/cast.py` & `angr-9.2.98/angr/engines/soot/expressions/cast.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/expressions/condition.py` & `angr-9.2.98/angr/engines/soot/expressions/condition.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/expressions/constants.py` & `angr-9.2.98/angr/engines/soot/expressions/constants.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/expressions/invoke.py` & `angr-9.2.98/angr/engines/soot/expressions/invoke.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/expressions/new.py` & `angr-9.2.98/angr/engines/soot/expressions/new.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/expressions/newArray.py` & `angr-9.2.98/angr/engines/soot/expressions/newArray.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/expressions/newMultiArray.py` & `angr-9.2.98/angr/engines/soot/expressions/newMultiArray.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/expressions/phi.py` & `angr-9.2.98/angr/engines/soot/expressions/phi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/field_dispatcher.py` & `angr-9.2.98/angr/engines/soot/field_dispatcher.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/method_dispatcher.py` & `angr-9.2.98/angr/engines/soot/method_dispatcher.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/statements/__init__.py` & `angr-9.2.98/angr/engines/soot/statements/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/statements/assign.py` & `angr-9.2.98/angr/engines/soot/statements/assign.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/statements/base.py` & `angr-9.2.98/angr/engines/soot/statements/base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/statements/if_.py` & `angr-9.2.98/angr/engines/soot/statements/if_.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/statements/switch.py` & `angr-9.2.98/angr/engines/soot/statements/switch.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/values/__init__.py` & `angr-9.2.98/angr/engines/soot/values/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/values/arrayref.py` & `angr-9.2.98/angr/engines/soot/values/arrayref.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/values/instancefieldref.py` & `angr-9.2.98/angr/engines/soot/values/instancefieldref.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/values/staticfieldref.py` & `angr-9.2.98/angr/engines/soot/values/staticfieldref.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/values/strref.py` & `angr-9.2.98/angr/engines/soot/values/strref.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/soot/values/thisref.py` & `angr-9.2.98/angr/engines/soot/values/thisref.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/successors.py` & `angr-9.2.98/angr/engines/successors.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/syscall.py` & `angr-9.2.98/angr/engines/syscall.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/unicorn.py` & `angr-9.2.98/angr/engines/unicorn.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/vex/claripy/ccall.py` & `angr-9.2.98/angr/engines/vex/claripy/ccall.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/vex/claripy/datalayer.py` & `angr-9.2.98/angr/engines/vex/claripy/datalayer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/vex/claripy/irop.py` & `angr-9.2.98/angr/engines/vex/claripy/irop.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/vex/heavy/actions.py` & `angr-9.2.98/angr/engines/vex/heavy/actions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/vex/heavy/concretizers.py` & `angr-9.2.98/angr/engines/vex/heavy/concretizers.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/vex/heavy/dirty.py` & `angr-9.2.98/angr/engines/vex/heavy/dirty.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/vex/heavy/heavy.py` & `angr-9.2.98/angr/engines/vex/heavy/heavy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/vex/heavy/inspect.py` & `angr-9.2.98/angr/engines/vex/heavy/inspect.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/vex/heavy/resilience.py` & `angr-9.2.98/angr/engines/vex/heavy/resilience.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/vex/heavy/super_fastpath.py` & `angr-9.2.98/angr/engines/vex/heavy/super_fastpath.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/vex/lifter.py` & `angr-9.2.98/angr/engines/vex/lifter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/vex/light/light.py` & `angr-9.2.98/angr/engines/vex/light/light.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/vex/light/resilience.py` & `angr-9.2.98/angr/engines/vex/light/resilience.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/engines/vex/light/slicing.py` & `angr-9.2.98/angr/engines/vex/light/slicing.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/errors.py` & `angr-9.2.98/angr/errors.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/__init__.py` & `angr-9.2.98/angr/exploration_techniques/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/bucketizer.py` & `angr-9.2.98/angr/exploration_techniques/bucketizer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/common.py` & `angr-9.2.98/angr/exploration_techniques/common.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/dfs.py` & `angr-9.2.98/angr/exploration_techniques/dfs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/director.py` & `angr-9.2.98/angr/exploration_techniques/director.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/driller_core.py` & `angr-9.2.98/angr/exploration_techniques/driller_core.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/explorer.py` & `angr-9.2.98/angr/exploration_techniques/explorer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/lengthlimiter.py` & `angr-9.2.98/angr/exploration_techniques/lengthlimiter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/local_loop_seer.py` & `angr-9.2.98/angr/exploration_techniques/local_loop_seer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/loop_seer.py` & `angr-9.2.98/angr/exploration_techniques/loop_seer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/manual_mergepoint.py` & `angr-9.2.98/angr/exploration_techniques/manual_mergepoint.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/memory_watcher.py` & `angr-9.2.98/angr/exploration_techniques/memory_watcher.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/oppologist.py` & `angr-9.2.98/angr/exploration_techniques/oppologist.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/slicecutor.py` & `angr-9.2.98/angr/exploration_techniques/slicecutor.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/spiller.py` & `angr-9.2.98/angr/exploration_techniques/spiller.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/spiller_db.py` & `angr-9.2.98/angr/exploration_techniques/spiller_db.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/stochastic.py` & `angr-9.2.98/angr/exploration_techniques/stochastic.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/suggestions.py` & `angr-9.2.98/angr/exploration_techniques/suggestions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/symbion.py` & `angr-9.2.98/angr/exploration_techniques/symbion.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/tech_builder.py` & `angr-9.2.98/angr/exploration_techniques/tech_builder.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/threading.py` & `angr-9.2.98/angr/exploration_techniques/threading.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/timeout.py` & `angr-9.2.98/angr/exploration_techniques/timeout.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/tracer.py` & `angr-9.2.98/angr/exploration_techniques/tracer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/unique.py` & `angr-9.2.98/angr/exploration_techniques/unique.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/exploration_techniques/veritesting.py` & `angr-9.2.98/angr/exploration_techniques/veritesting.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/factory.py` & `angr-9.2.98/angr/factory.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/flirt/__init__.py` & `angr-9.2.98/angr/flirt/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/flirt/build_sig.py` & `angr-9.2.98/angr/flirt/build_sig.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/keyed_region.py` & `angr-9.2.98/angr/keyed_region.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_base/knowledge_base.py` & `angr-9.2.98/angr/knowledge_base/knowledge_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/__init__.py` & `angr-9.2.98/angr/knowledge_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/callsite_prototypes.py` & `angr-9.2.98/angr/knowledge_plugins/callsite_prototypes.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/cfg/cfg_manager.py` & `angr-9.2.98/angr/knowledge_plugins/cfg/cfg_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/cfg/cfg_model.py` & `angr-9.2.98/angr/knowledge_plugins/cfg/cfg_model.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/cfg/cfg_node.py` & `angr-9.2.98/angr/knowledge_plugins/cfg/cfg_node.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/cfg/indirect_jump.py` & `angr-9.2.98/angr/knowledge_plugins/cfg/indirect_jump.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/cfg/memory_data.py` & `angr-9.2.98/angr/knowledge_plugins/cfg/memory_data.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/custom_strings.py` & `angr-9.2.98/angr/knowledge_plugins/custom_strings.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/data.py` & `angr-9.2.98/angr/knowledge_plugins/data.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/debug_variables.py` & `angr-9.2.98/angr/knowledge_plugins/debug_variables.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/functions/function.py` & `angr-9.2.98/angr/knowledge_plugins/functions/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -1531,14 +1531,18 @@
             name_variants.append(self.name[2:])
         # special handling for libc
         if self.name.startswith("__libc_"):
             name_variants.append(self.name[7:])
 
         for library in libraries:
             for name in name_variants:
+                if isinstance(library, SimSyscallLibrary):
+                    # FIXME: we don't support getting declaration from a syscall library yet. we don't have the concept
+                    # of abi at this point.
+                    continue
                 if not library.has_prototype(name):
                     continue
 
                 proto = library.get_prototype(name)
                 if self.project is None:
                     # we need to get arch from self.project
                     l.warning(
```

### Comparing `angr-9.2.97/angr/knowledge_plugins/functions/function_manager.py` & `angr-9.2.98/angr/knowledge_plugins/functions/function_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/functions/function_parser.py` & `angr-9.2.98/angr/knowledge_plugins/functions/function_parser.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/functions/soot_function.py` & `angr-9.2.98/angr/knowledge_plugins/functions/soot_function.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/indirect_jumps.py` & `angr-9.2.98/angr/knowledge_plugins/indirect_jumps.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/key_definitions/atoms.py` & `angr-9.2.98/angr/knowledge_plugins/key_definitions/atoms.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/key_definitions/definition.py` & `angr-9.2.98/angr/knowledge_plugins/key_definitions/definition.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/key_definitions/environment.py` & `angr-9.2.98/angr/knowledge_plugins/key_definitions/environment.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/key_definitions/heap_address.py` & `angr-9.2.98/angr/knowledge_plugins/key_definitions/heap_address.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/key_definitions/key_definition_manager.py` & `angr-9.2.98/angr/knowledge_plugins/key_definitions/key_definition_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/key_definitions/live_definitions.py` & `angr-9.2.98/angr/knowledge_plugins/key_definitions/live_definitions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/key_definitions/liveness.py` & `angr-9.2.98/angr/knowledge_plugins/key_definitions/liveness.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/key_definitions/rd_model.py` & `angr-9.2.98/angr/knowledge_plugins/key_definitions/rd_model.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/key_definitions/tag.py` & `angr-9.2.98/angr/knowledge_plugins/key_definitions/tag.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/key_definitions/undefined.py` & `angr-9.2.98/angr/knowledge_plugins/key_definitions/undefined.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/key_definitions/unknown_size.py` & `angr-9.2.98/angr/knowledge_plugins/key_definitions/unknown_size.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/key_definitions/uses.py` & `angr-9.2.98/angr/knowledge_plugins/key_definitions/uses.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/labels.py` & `angr-9.2.98/angr/knowledge_plugins/labels.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/patches.py` & `angr-9.2.98/angr/knowledge_plugins/patches.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/plugin.py` & `angr-9.2.98/angr/knowledge_plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/propagations/prop_value.py` & `angr-9.2.98/angr/knowledge_plugins/propagations/prop_value.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/propagations/propagation_manager.py` & `angr-9.2.98/angr/knowledge_plugins/propagations/propagation_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/propagations/propagation_model.py` & `angr-9.2.98/angr/knowledge_plugins/propagations/propagation_model.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/propagations/states.py` & `angr-9.2.98/angr/knowledge_plugins/propagations/states.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/structured_code/manager.py` & `angr-9.2.98/angr/knowledge_plugins/structured_code/manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/sync/sync_controller.py` & `angr-9.2.98/angr/knowledge_plugins/sync/sync_controller.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/types.py` & `angr-9.2.98/angr/knowledge_plugins/types.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/variables/variable_access.py` & `angr-9.2.98/angr/knowledge_plugins/variables/variable_access.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/variables/variable_manager.py` & `angr-9.2.98/angr/knowledge_plugins/variables/variable_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/xrefs/xref.py` & `angr-9.2.98/angr/knowledge_plugins/xrefs/xref.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/knowledge_plugins/xrefs/xref_manager.py` & `angr-9.2.98/angr/knowledge_plugins/xrefs/xref_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/misc/ansi.py` & `angr-9.2.98/angr/misc/ansi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/misc/autoimport.py` & `angr-9.2.98/angr/misc/autoimport.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/misc/bug_report.py` & `angr-9.2.98/angr/misc/bug_report.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/misc/hookset.py` & `angr-9.2.98/angr/misc/hookset.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/misc/import_hooks.py` & `angr-9.2.98/angr/misc/import_hooks.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/misc/loggers.py` & `angr-9.2.98/angr/misc/loggers.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/misc/picklable_lock.py` & `angr-9.2.98/angr/misc/picklable_lock.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/misc/plugins.py` & `angr-9.2.98/angr/misc/plugins.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/misc/testing.py` & `angr-9.2.98/angr/misc/testing.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/misc/ux.py` & `angr-9.2.98/angr/misc/ux.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/misc/weakpatch.py` & `angr-9.2.98/angr/misc/weakpatch.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/cgc/allocate.py` & `angr-9.2.98/angr/procedures/cgc/allocate.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/cgc/deallocate.py` & `angr-9.2.98/angr/procedures/cgc/deallocate.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/cgc/fdwait.py` & `angr-9.2.98/angr/procedures/cgc/fdwait.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/cgc/random.py` & `angr-9.2.98/angr/procedures/cgc/random.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/cgc/receive.py` & `angr-9.2.98/angr/procedures/cgc/receive.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/cgc/transmit.py` & `angr-9.2.98/angr/procedures/cgc/transmit.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/__init__.py` & `angr-9.2.98/angr/procedures/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/glibc.py` & `angr-9.2.98/angr/procedures/definitions/glibc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/gnulib.py` & `angr-9.2.98/angr/procedures/definitions/gnulib.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/libstdcpp.py` & `angr-9.2.98/angr/procedures/definitions/libstdcpp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/linux_kernel.py` & `angr-9.2.98/angr/procedures/definitions/linux_kernel.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/msvcr.py` & `angr-9.2.98/angr/procedures/definitions/msvcr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/parse_syscalls_from_local_system.py` & `angr-9.2.98/angr/procedures/definitions/parse_syscalls_from_local_system.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/parse_win32json.py` & `angr-9.2.98/angr/procedures/definitions/parse_win32json.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/types_win32.py` & `angr-9.2.98/angr/procedures/definitions/types_win32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/wdk_api-ms-win-dx-d3dkmt-l1-1-4.py` & `angr-9.2.98/angr/procedures/definitions/wdk_api-ms-win-dx-d3dkmt-l1-1-4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/wdk_api-ms-win-dx-d3dkmt-l1-1-6.py` & `angr-9.2.98/angr/procedures/definitions/wdk_api-ms-win-dx-d3dkmt-l1-1-6.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/wdk_clfs.py` & `angr-9.2.98/angr/procedures/definitions/wdk_clfs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/wdk_fltmgr.py` & `angr-9.2.98/angr/procedures/definitions/wdk_fltmgr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/wdk_fwpkclnt.py` & `angr-9.2.98/angr/procedures/definitions/wdk_fwpkclnt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/wdk_fwpuclnt.py` & `angr-9.2.98/angr/procedures/definitions/wdk_fwpuclnt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/wdk_gdi32.py` & `angr-9.2.98/angr/procedures/definitions/wdk_gdi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/wdk_hal.py` & `angr-9.2.98/angr/procedures/definitions/wdk_hal.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/wdk_ksecdd.py` & `angr-9.2.98/angr/procedures/definitions/wdk_ksecdd.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/wdk_ndis.py` & `angr-9.2.98/angr/procedures/definitions/wdk_ndis.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/wdk_ntoskrnl.py` & `angr-9.2.98/angr/procedures/definitions/wdk_ntoskrnl.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/wdk_offreg.py` & `angr-9.2.98/angr/procedures/definitions/wdk_offreg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/wdk_pshed.py` & `angr-9.2.98/angr/procedures/definitions/wdk_pshed.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/wdk_secur32.py` & `angr-9.2.98/angr/procedures/definitions/wdk_secur32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/wdk_vhfum.py` & `angr-9.2.98/angr/procedures/definitions/wdk_vhfum.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_aclui.py` & `angr-9.2.98/angr/procedures/definitions/win32_aclui.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_activeds.py` & `angr-9.2.98/angr/procedures/definitions/win32_activeds.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_advapi32.py` & `angr-9.2.98/angr/procedures/definitions/win32_advapi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_advpack.py` & `angr-9.2.98/angr/procedures/definitions/win32_advpack.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_amsi.py` & `angr-9.2.98/angr/procedures/definitions/win32_amsi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-1.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-3.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-3.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-6.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-6.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-apiquery-l2-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-apiquery-l2-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-backgroundtask-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-backgroundtask-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-1.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-2.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-enclave-l1-1-1.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-enclave-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-errorhandling-l1-1-3.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-errorhandling-l1-1-3.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-1.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-file-fromapp-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-file-fromapp-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-handle-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-handle-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-ioring-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-ioring-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-marshal-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-marshal-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-3.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-3.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-4.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-5.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-5.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-6.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-6.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-7.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-7.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-8.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-8.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-path-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-path-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-1.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-1.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-2.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-slapi-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-slapi-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-state-helpers-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-state-helpers-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-synch-l1-2-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-synch-l1-2-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-3.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-3.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-4.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-6.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-6.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-util-l1-1-1.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-util-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-1.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-winrt-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-registration-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-winrt-registration-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-robuffer-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-winrt-robuffer-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-roparameterizediid-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-winrt-roparameterizediid-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-1.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-wow64-l1-1-1.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-core-wow64-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-1.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-dx-d3dkmt-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-dx-d3dkmt-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-deviceinformation-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-gaming-deviceinformation-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-expandedresources-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-gaming-expandedresources-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-1.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-2.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-3.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-3.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-4.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-mm-misc-l1-1-1.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-mm-misc-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-net-isolation-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-net-isolation-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-security-base-l1-2-2.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-security-base-l1-2-2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-1.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-3.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-3.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-4.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-5.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-5.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-1.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-2.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-shcore-stream-winrt-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-shcore-stream-winrt-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-wsl-api-l1-1-0.py` & `angr-9.2.98/angr/procedures/definitions/win32_api-ms-win-wsl-api-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_apphelp.py` & `angr-9.2.98/angr/procedures/definitions/win32_apphelp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_authz.py` & `angr-9.2.98/angr/procedures/definitions/win32_authz.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_avicap32.py` & `angr-9.2.98/angr/procedures/definitions/win32_avicap32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_avifil32.py` & `angr-9.2.98/angr/procedures/definitions/win32_avifil32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_avrt.py` & `angr-9.2.98/angr/procedures/definitions/win32_avrt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_bcp47mrm.py` & `angr-9.2.98/angr/procedures/definitions/win32_bcp47mrm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_bcrypt.py` & `angr-9.2.98/angr/procedures/definitions/win32_bcrypt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_bcryptprimitives.py` & `angr-9.2.98/angr/procedures/definitions/win32_bcryptprimitives.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_bluetoothapis.py` & `angr-9.2.98/angr/procedures/definitions/win32_bluetoothapis.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_bthprops.py` & `angr-9.2.98/angr/procedures/definitions/win32_bthprops.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_bthprops_cpl.py` & `angr-9.2.98/angr/procedures/definitions/win32_bthprops_cpl.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_cabinet.py` & `angr-9.2.98/angr/procedures/definitions/win32_cabinet.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_certadm.py` & `angr-9.2.98/angr/procedures/definitions/win32_certadm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_certpoleng.py` & `angr-9.2.98/angr/procedures/definitions/win32_certpoleng.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_cfgmgr32.py` & `angr-9.2.98/angr/procedures/definitions/win32_cfgmgr32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_chakra.py` & `angr-9.2.98/angr/procedures/definitions/win32_chakra.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_cldapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_cldapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_clfsw32.py` & `angr-9.2.98/angr/procedures/definitions/win32_clfsw32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_clusapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_clusapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_comctl32.py` & `angr-9.2.98/angr/procedures/definitions/win32_comctl32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_comdlg32.py` & `angr-9.2.98/angr/procedures/definitions/win32_comdlg32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_compstui.py` & `angr-9.2.98/angr/procedures/definitions/win32_compstui.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_computecore.py` & `angr-9.2.98/angr/procedures/definitions/win32_computecore.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_computenetwork.py` & `angr-9.2.98/angr/procedures/definitions/win32_computenetwork.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_computestorage.py` & `angr-9.2.98/angr/procedures/definitions/win32_computestorage.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_comsvcs.py` & `angr-9.2.98/angr/procedures/definitions/win32_comsvcs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_coremessaging.py` & `angr-9.2.98/angr/procedures/definitions/win32_coremessaging.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_credui.py` & `angr-9.2.98/angr/procedures/definitions/win32_credui.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_crypt32.py` & `angr-9.2.98/angr/procedures/definitions/win32_crypt32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_cryptnet.py` & `angr-9.2.98/angr/procedures/definitions/win32_cryptnet.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_cryptui.py` & `angr-9.2.98/angr/procedures/definitions/win32_cryptui.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_cryptxml.py` & `angr-9.2.98/angr/procedures/definitions/win32_cryptxml.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_cscapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_cscapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_d2d1.py` & `angr-9.2.98/angr/procedures/definitions/win32_d2d1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_d3d10.py` & `angr-9.2.98/angr/procedures/definitions/win32_d3d10.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_d3d10_1.py` & `angr-9.2.98/angr/procedures/definitions/win32_d3d10_1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_d3d11.py` & `angr-9.2.98/angr/procedures/definitions/win32_d3d11.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_d3d12.py` & `angr-9.2.98/angr/procedures/definitions/win32_d3d12.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_d3d9.py` & `angr-9.2.98/angr/procedures/definitions/win32_d3d9.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_d3dcompiler_47.py` & `angr-9.2.98/angr/procedures/definitions/win32_d3dcompiler_47.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_d3dcsx.py` & `angr-9.2.98/angr/procedures/definitions/win32_d3dcsx.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_davclnt.py` & `angr-9.2.98/angr/procedures/definitions/win32_davclnt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dbgeng.py` & `angr-9.2.98/angr/procedures/definitions/win32_dbgeng.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dbghelp.py` & `angr-9.2.98/angr/procedures/definitions/win32_dbghelp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dbgmodel.py` & `angr-9.2.98/angr/procedures/definitions/win32_dbgmodel.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dciman32.py` & `angr-9.2.98/angr/procedures/definitions/win32_dciman32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dcomp.py` & `angr-9.2.98/angr/procedures/definitions/win32_dcomp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_ddraw.py` & `angr-9.2.98/angr/procedures/definitions/win32_ddraw.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_deviceaccess.py` & `angr-9.2.98/angr/procedures/definitions/win32_deviceaccess.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dflayout.py` & `angr-9.2.98/angr/procedures/definitions/win32_dflayout.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dhcpcsvc.py` & `angr-9.2.98/angr/procedures/definitions/win32_dhcpcsvc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dhcpcsvc6.py` & `angr-9.2.98/angr/procedures/definitions/win32_dhcpcsvc6.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dhcpsapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_dhcpsapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_diagnosticdataquery.py` & `angr-9.2.98/angr/procedures/definitions/win32_diagnosticdataquery.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dinput8.py` & `angr-9.2.98/angr/procedures/definitions/win32_dinput8.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_directml.py` & `angr-9.2.98/angr/procedures/definitions/win32_directml.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dmprocessxmlfiltered.py` & `angr-9.2.98/angr/procedures/definitions/win32_dmprocessxmlfiltered.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dnsapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_dnsapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_drt.py` & `angr-9.2.98/angr/procedures/definitions/win32_drt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_drtprov.py` & `angr-9.2.98/angr/procedures/definitions/win32_drtprov.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_drttransport.py` & `angr-9.2.98/angr/procedures/definitions/win32_drttransport.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dsound.py` & `angr-9.2.98/angr/procedures/definitions/win32_dsound.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dsparse.py` & `angr-9.2.98/angr/procedures/definitions/win32_dsparse.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dsprop.py` & `angr-9.2.98/angr/procedures/definitions/win32_dsprop.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dssec.py` & `angr-9.2.98/angr/procedures/definitions/win32_dssec.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dsuiext.py` & `angr-9.2.98/angr/procedures/definitions/win32_dsuiext.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dwmapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_dwmapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dwrite.py` & `angr-9.2.98/angr/procedures/definitions/win32_dwrite.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dxcompiler.py` & `angr-9.2.98/angr/procedures/definitions/win32_dxcompiler.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dxcore.py` & `angr-9.2.98/angr/procedures/definitions/win32_dxcore.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dxgi.py` & `angr-9.2.98/angr/procedures/definitions/win32_dxgi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_dxva2.py` & `angr-9.2.98/angr/procedures/definitions/win32_dxva2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_eappcfg.py` & `angr-9.2.98/angr/procedures/definitions/win32_eappcfg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_eappprxy.py` & `angr-9.2.98/angr/procedures/definitions/win32_eappprxy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_efswrt.py` & `angr-9.2.98/angr/procedures/definitions/win32_efswrt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_elscore.py` & `angr-9.2.98/angr/procedures/definitions/win32_elscore.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_esent.py` & `angr-9.2.98/angr/procedures/definitions/win32_esent.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_evr.py` & `angr-9.2.98/angr/procedures/definitions/win32_evr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_faultrep.py` & `angr-9.2.98/angr/procedures/definitions/win32_faultrep.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_fhsvcctl.py` & `angr-9.2.98/angr/procedures/definitions/win32_fhsvcctl.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_firewallapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_firewallapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_fltlib.py` & `angr-9.2.98/angr/procedures/definitions/win32_fltlib.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_fontsub.py` & `angr-9.2.98/angr/procedures/definitions/win32_fontsub.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_forceinline.py` & `angr-9.2.98/angr/procedures/definitions/win32_forceinline.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_fwpuclnt.py` & `angr-9.2.98/angr/procedures/definitions/win32_fwpuclnt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_fxsutility.py` & `angr-9.2.98/angr/procedures/definitions/win32_fxsutility.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_gdi32.py` & `angr-9.2.98/angr/procedures/definitions/win32_gdi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_gdiplus.py` & `angr-9.2.98/angr/procedures/definitions/win32_gdiplus.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_glu32.py` & `angr-9.2.98/angr/procedures/definitions/win32_glu32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_gpedit.py` & `angr-9.2.98/angr/procedures/definitions/win32_gpedit.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_hhctrl_ocx.py` & `angr-9.2.98/angr/procedures/definitions/win32_hhctrl_ocx.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_hid.py` & `angr-9.2.98/angr/procedures/definitions/win32_hid.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_hlink.py` & `angr-9.2.98/angr/procedures/definitions/win32_hlink.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_hrtfapo.py` & `angr-9.2.98/angr/procedures/definitions/win32_hrtfapo.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_httpapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_httpapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_icm32.py` & `angr-9.2.98/angr/procedures/definitions/win32_icm32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_icmui.py` & `angr-9.2.98/angr/procedures/definitions/win32_icmui.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_icu.py` & `angr-9.2.98/angr/procedures/definitions/win32_icu.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_ieframe.py` & `angr-9.2.98/angr/procedures/definitions/win32_ieframe.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_imagehlp.py` & `angr-9.2.98/angr/procedures/definitions/win32_imagehlp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_imgutil.py` & `angr-9.2.98/angr/procedures/definitions/win32_imgutil.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_imm32.py` & `angr-9.2.98/angr/procedures/definitions/win32_imm32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_infocardapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_infocardapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_inkobjcore.py` & `angr-9.2.98/angr/procedures/definitions/win32_inkobjcore.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_iphlpapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_iphlpapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_iscsidsc.py` & `angr-9.2.98/angr/procedures/definitions/win32_iscsidsc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_isolatedwindowsenvironmentutils.py` & `angr-9.2.98/angr/procedures/definitions/win32_isolatedwindowsenvironmentutils.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_kernel32.py` & `angr-9.2.98/angr/procedures/definitions/win32_kernel32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_kernelbase.py` & `angr-9.2.98/angr/procedures/definitions/win32_kernelbase.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_keycredmgr.py` & `angr-9.2.98/angr/procedures/definitions/win32_keycredmgr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_ksproxy_ax.py` & `angr-9.2.98/angr/procedures/definitions/win32_ksproxy_ax.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_ksuser.py` & `angr-9.2.98/angr/procedures/definitions/win32_ksuser.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_ktmw32.py` & `angr-9.2.98/angr/procedures/definitions/win32_ktmw32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_licenseprotection.py` & `angr-9.2.98/angr/procedures/definitions/win32_licenseprotection.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_loadperf.py` & `angr-9.2.98/angr/procedures/definitions/win32_loadperf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_magnification.py` & `angr-9.2.98/angr/procedures/definitions/win32_magnification.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mapi32.py` & `angr-9.2.98/angr/procedures/definitions/win32_mapi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mdmlocalmanagement.py` & `angr-9.2.98/angr/procedures/definitions/win32_mdmlocalmanagement.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mdmregistration.py` & `angr-9.2.98/angr/procedures/definitions/win32_mdmregistration.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mf.py` & `angr-9.2.98/angr/procedures/definitions/win32_mf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mfcore.py` & `angr-9.2.98/angr/procedures/definitions/win32_mfcore.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mfplat.py` & `angr-9.2.98/angr/procedures/definitions/win32_mfplat.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mfplay.py` & `angr-9.2.98/angr/procedures/definitions/win32_mfplay.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mfreadwrite.py` & `angr-9.2.98/angr/procedures/definitions/win32_mfreadwrite.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mfsensorgroup.py` & `angr-9.2.98/angr/procedures/definitions/win32_mfsensorgroup.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mfsrcsnk.py` & `angr-9.2.98/angr/procedures/definitions/win32_mfsrcsnk.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mgmtapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_mgmtapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mi.py` & `angr-9.2.98/angr/procedures/definitions/win32_mi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mmdevapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_mmdevapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mpr.py` & `angr-9.2.98/angr/procedures/definitions/win32_mpr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mprapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_mprapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mqrt.py` & `angr-9.2.98/angr/procedures/definitions/win32_mqrt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mrmsupport.py` & `angr-9.2.98/angr/procedures/definitions/win32_mrmsupport.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_msacm32.py` & `angr-9.2.98/angr/procedures/definitions/win32_msacm32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_msajapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_msajapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mscms.py` & `angr-9.2.98/angr/procedures/definitions/win32_mscms.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mscoree.py` & `angr-9.2.98/angr/procedures/definitions/win32_mscoree.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_msctfmonitor.py` & `angr-9.2.98/angr/procedures/definitions/win32_msctfmonitor.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_msdelta.py` & `angr-9.2.98/angr/procedures/definitions/win32_msdelta.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_msdmo.py` & `angr-9.2.98/angr/procedures/definitions/win32_msdmo.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_msdrm.py` & `angr-9.2.98/angr/procedures/definitions/win32_msdrm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_msi.py` & `angr-9.2.98/angr/procedures/definitions/win32_msi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_msimg32.py` & `angr-9.2.98/angr/procedures/definitions/win32_msimg32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mspatcha.py` & `angr-9.2.98/angr/procedures/definitions/win32_mspatcha.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mspatchc.py` & `angr-9.2.98/angr/procedures/definitions/win32_mspatchc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_msports.py` & `angr-9.2.98/angr/procedures/definitions/win32_msports.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_msrating.py` & `angr-9.2.98/angr/procedures/definitions/win32_msrating.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mssign32.py` & `angr-9.2.98/angr/procedures/definitions/win32_mssign32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mstask.py` & `angr-9.2.98/angr/procedures/definitions/win32_mstask.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_msvfw32.py` & `angr-9.2.98/angr/procedures/definitions/win32_msvfw32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mswsock.py` & `angr-9.2.98/angr/procedures/definitions/win32_mswsock.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_mtxdm.py` & `angr-9.2.98/angr/procedures/definitions/win32_mtxdm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_ncrypt.py` & `angr-9.2.98/angr/procedures/definitions/win32_ncrypt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_ndfapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_ndfapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_netapi32.py` & `angr-9.2.98/angr/procedures/definitions/win32_netapi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_netsh.py` & `angr-9.2.98/angr/procedures/definitions/win32_netsh.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_netshell.py` & `angr-9.2.98/angr/procedures/definitions/win32_netshell.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_newdev.py` & `angr-9.2.98/angr/procedures/definitions/win32_newdev.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_ninput.py` & `angr-9.2.98/angr/procedures/definitions/win32_ninput.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_normaliz.py` & `angr-9.2.98/angr/procedures/definitions/win32_normaliz.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_ntdll.py` & `angr-9.2.98/angr/procedures/definitions/win32_ntdll.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_ntdllk.py` & `angr-9.2.98/angr/procedures/definitions/win32_ntdllk.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_ntdsapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_ntdsapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_ntlanman.py` & `angr-9.2.98/angr/procedures/definitions/win32_ntlanman.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_odbc32.py` & `angr-9.2.98/angr/procedures/definitions/win32_odbc32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_odbcbcp.py` & `angr-9.2.98/angr/procedures/definitions/win32_odbcbcp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_ole32.py` & `angr-9.2.98/angr/procedures/definitions/win32_ole32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_oleacc.py` & `angr-9.2.98/angr/procedures/definitions/win32_oleacc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_oleaut32.py` & `angr-9.2.98/angr/procedures/definitions/win32_oleaut32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_oledlg.py` & `angr-9.2.98/angr/procedures/definitions/win32_oledlg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_ondemandconnroutehelper.py` & `angr-9.2.98/angr/procedures/definitions/win32_ondemandconnroutehelper.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_opengl32.py` & `angr-9.2.98/angr/procedures/definitions/win32_opengl32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_opmxbox.py` & `angr-9.2.98/angr/procedures/definitions/win32_opmxbox.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_p2p.py` & `angr-9.2.98/angr/procedures/definitions/win32_p2p.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_p2pgraph.py` & `angr-9.2.98/angr/procedures/definitions/win32_p2pgraph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_pdh.py` & `angr-9.2.98/angr/procedures/definitions/win32_pdh.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_peerdist.py` & `angr-9.2.98/angr/procedures/definitions/win32_peerdist.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_powrprof.py` & `angr-9.2.98/angr/procedures/definitions/win32_powrprof.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_prntvpt.py` & `angr-9.2.98/angr/procedures/definitions/win32_prntvpt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_projectedfslib.py` & `angr-9.2.98/angr/procedures/definitions/win32_projectedfslib.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_propsys.py` & `angr-9.2.98/angr/procedures/definitions/win32_propsys.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_psapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_psapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_quartz.py` & `angr-9.2.98/angr/procedures/definitions/win32_quartz.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_query.py` & `angr-9.2.98/angr/procedures/definitions/win32_query.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_qwave.py` & `angr-9.2.98/angr/procedures/definitions/win32_qwave.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_rasapi32.py` & `angr-9.2.98/angr/procedures/definitions/win32_rasapi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_rasdlg.py` & `angr-9.2.98/angr/procedures/definitions/win32_rasdlg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_resutils.py` & `angr-9.2.98/angr/procedures/definitions/win32_resutils.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_rometadata.py` & `angr-9.2.98/angr/procedures/definitions/win32_rometadata.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_rpcns4.py` & `angr-9.2.98/angr/procedures/definitions/win32_rpcns4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_rpcproxy.py` & `angr-9.2.98/angr/procedures/definitions/win32_rpcproxy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_rpcrt4.py` & `angr-9.2.98/angr/procedures/definitions/win32_rpcrt4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_rstrtmgr.py` & `angr-9.2.98/angr/procedures/definitions/win32_rstrtmgr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_rtm.py` & `angr-9.2.98/angr/procedures/definitions/win32_rtm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_rtutils.py` & `angr-9.2.98/angr/procedures/definitions/win32_rtutils.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_rtworkq.py` & `angr-9.2.98/angr/procedures/definitions/win32_rtworkq.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_sas.py` & `angr-9.2.98/angr/procedures/definitions/win32_sas.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_scarddlg.py` & `angr-9.2.98/angr/procedures/definitions/win32_scarddlg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_schannel.py` & `angr-9.2.98/angr/procedures/definitions/win32_schannel.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_sechost.py` & `angr-9.2.98/angr/procedures/definitions/win32_sechost.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_secur32.py` & `angr-9.2.98/angr/procedures/definitions/win32_secur32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_sensapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_sensapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_sensorsutilsv2.py` & `angr-9.2.98/angr/procedures/definitions/win32_sensorsutilsv2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_setupapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_setupapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_sfc.py` & `angr-9.2.98/angr/procedures/definitions/win32_sfc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_shdocvw.py` & `angr-9.2.98/angr/procedures/definitions/win32_shdocvw.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_shell32.py` & `angr-9.2.98/angr/procedures/definitions/win32_shell32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_shlwapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_shlwapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_slc.py` & `angr-9.2.98/angr/procedures/definitions/win32_slc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_slcext.py` & `angr-9.2.98/angr/procedures/definitions/win32_slcext.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_slwga.py` & `angr-9.2.98/angr/procedures/definitions/win32_slwga.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_snmpapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_snmpapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_spoolss.py` & `angr-9.2.98/angr/procedures/definitions/win32_spoolss.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_srclient.py` & `angr-9.2.98/angr/procedures/definitions/win32_srclient.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_srpapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_srpapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_sspicli.py` & `angr-9.2.98/angr/procedures/definitions/win32_sspicli.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_sti.py` & `angr-9.2.98/angr/procedures/definitions/win32_sti.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_t2embed.py` & `angr-9.2.98/angr/procedures/definitions/win32_t2embed.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_tapi32.py` & `angr-9.2.98/angr/procedures/definitions/win32_tapi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_tbs.py` & `angr-9.2.98/angr/procedures/definitions/win32_tbs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_tdh.py` & `angr-9.2.98/angr/procedures/definitions/win32_tdh.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_tokenbinding.py` & `angr-9.2.98/angr/procedures/definitions/win32_tokenbinding.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_traffic.py` & `angr-9.2.98/angr/procedures/definitions/win32_traffic.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_txfw32.py` & `angr-9.2.98/angr/procedures/definitions/win32_txfw32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_ualapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_ualapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_uiautomationcore.py` & `angr-9.2.98/angr/procedures/definitions/win32_uiautomationcore.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_urlmon.py` & `angr-9.2.98/angr/procedures/definitions/win32_urlmon.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_user32.py` & `angr-9.2.98/angr/procedures/definitions/win32_user32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_userenv.py` & `angr-9.2.98/angr/procedures/definitions/win32_userenv.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_usp10.py` & `angr-9.2.98/angr/procedures/definitions/win32_usp10.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_uxtheme.py` & `angr-9.2.98/angr/procedures/definitions/win32_uxtheme.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_verifier.py` & `angr-9.2.98/angr/procedures/definitions/win32_verifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_version.py` & `angr-9.2.98/angr/procedures/definitions/win32_version.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_vertdll.py` & `angr-9.2.98/angr/procedures/definitions/win32_vertdll.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_virtdisk.py` & `angr-9.2.98/angr/procedures/definitions/win32_virtdisk.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_vmdevicehost.py` & `angr-9.2.98/angr/procedures/definitions/win32_vmdevicehost.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_vmsavedstatedumpprovider.py` & `angr-9.2.98/angr/procedures/definitions/win32_vmsavedstatedumpprovider.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_vssapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_vssapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wcmapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_wcmapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wdsbp.py` & `angr-9.2.98/angr/procedures/definitions/win32_wdsbp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wdsclientapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_wdsclientapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wdsmc.py` & `angr-9.2.98/angr/procedures/definitions/win32_wdsmc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wdspxe.py` & `angr-9.2.98/angr/procedures/definitions/win32_wdspxe.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wdstptc.py` & `angr-9.2.98/angr/procedures/definitions/win32_wdstptc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_webauthn.py` & `angr-9.2.98/angr/procedures/definitions/win32_webauthn.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_webservices.py` & `angr-9.2.98/angr/procedures/definitions/win32_webservices.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_websocket.py` & `angr-9.2.98/angr/procedures/definitions/win32_websocket.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wecapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_wecapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wer.py` & `angr-9.2.98/angr/procedures/definitions/win32_wer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wevtapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_wevtapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_winbio.py` & `angr-9.2.98/angr/procedures/definitions/win32_winbio.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_windows_ai_machinelearning.py` & `angr-9.2.98/angr/procedures/definitions/win32_windows_ai_machinelearning.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_windows_data_pdf.py` & `angr-9.2.98/angr/procedures/definitions/win32_windows_data_pdf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_windows_media_mediacontrol.py` & `angr-9.2.98/angr/procedures/definitions/win32_windows_media_mediacontrol.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_windows_networking.py` & `angr-9.2.98/angr/procedures/definitions/win32_windows_networking.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_windows_ui_xaml.py` & `angr-9.2.98/angr/procedures/definitions/win32_windows_ui_xaml.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_windowscodecs.py` & `angr-9.2.98/angr/procedures/definitions/win32_windowscodecs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_winfax.py` & `angr-9.2.98/angr/procedures/definitions/win32_winfax.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_winhttp.py` & `angr-9.2.98/angr/procedures/definitions/win32_winhttp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_winhvemulation.py` & `angr-9.2.98/angr/procedures/definitions/win32_winhvemulation.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_winhvplatform.py` & `angr-9.2.98/angr/procedures/definitions/win32_winhvplatform.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wininet.py` & `angr-9.2.98/angr/procedures/definitions/win32_wininet.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_winml.py` & `angr-9.2.98/angr/procedures/definitions/win32_winml.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_winmm.py` & `angr-9.2.98/angr/procedures/definitions/win32_winmm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_winscard.py` & `angr-9.2.98/angr/procedures/definitions/win32_winscard.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_winspool.py` & `angr-9.2.98/angr/procedures/definitions/win32_winspool.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_winspool_drv.py` & `angr-9.2.98/angr/procedures/definitions/win32_winspool_drv.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wintrust.py` & `angr-9.2.98/angr/procedures/definitions/win32_wintrust.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_winusb.py` & `angr-9.2.98/angr/procedures/definitions/win32_winusb.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wlanapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_wlanapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wlanui.py` & `angr-9.2.98/angr/procedures/definitions/win32_wlanui.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wldap32.py` & `angr-9.2.98/angr/procedures/definitions/win32_wldap32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wldp.py` & `angr-9.2.98/angr/procedures/definitions/win32_wldp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wmvcore.py` & `angr-9.2.98/angr/procedures/definitions/win32_wmvcore.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wnvapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_wnvapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wofutil.py` & `angr-9.2.98/angr/procedures/definitions/win32_wofutil.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_ws2_32.py` & `angr-9.2.98/angr/procedures/definitions/win32_ws2_32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wscapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_wscapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wsclient.py` & `angr-9.2.98/angr/procedures/definitions/win32_wsclient.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wsdapi.py` & `angr-9.2.98/angr/procedures/definitions/win32_wsdapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wsmsvc.py` & `angr-9.2.98/angr/procedures/definitions/win32_wsmsvc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wsnmp32.py` & `angr-9.2.98/angr/procedures/definitions/win32_wsnmp32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_wtsapi32.py` & `angr-9.2.98/angr/procedures/definitions/win32_wtsapi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_xaudio2_8.py` & `angr-9.2.98/angr/procedures/definitions/win32_xaudio2_8.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_xinput1_4.py` & `angr-9.2.98/angr/procedures/definitions/win32_xinput1_4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_xinputuap.py` & `angr-9.2.98/angr/procedures/definitions/win32_xinputuap.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_xmllite.py` & `angr-9.2.98/angr/procedures/definitions/win32_xmllite.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_xolehlp.py` & `angr-9.2.98/angr/procedures/definitions/win32_xolehlp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/definitions/win32_xpsprint.py` & `angr-9.2.98/angr/procedures/definitions/win32_xpsprint.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/glibc/__ctype_b_loc.py` & `angr-9.2.98/angr/procedures/glibc/__ctype_b_loc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/glibc/__ctype_tolower_loc.py` & `angr-9.2.98/angr/procedures/glibc/__ctype_tolower_loc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/glibc/__ctype_toupper_loc.py` & `angr-9.2.98/angr/procedures/glibc/__ctype_toupper_loc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/glibc/__libc_init.py` & `angr-9.2.98/angr/procedures/glibc/__libc_init.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/glibc/__libc_start_main.py` & `angr-9.2.98/angr/procedures/glibc/__libc_start_main.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/glibc/dynamic_loading.py` & `angr-9.2.98/angr/procedures/glibc/dynamic_loading.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java/__init__.py` & `angr-9.2.98/angr/procedures/java/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java/unconstrained.py` & `angr-9.2.98/angr/procedures/java/unconstrained.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java_io/write.py` & `angr-9.2.98/angr/procedures/java_io/write.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java_jni/__init__.py` & `angr-9.2.98/angr/procedures/java_jni/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java_jni/array_operations.py` & `angr-9.2.98/angr/procedures/java_jni/array_operations.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java_jni/class_and_interface_operations.py` & `angr-9.2.98/angr/procedures/java_jni/class_and_interface_operations.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java_jni/field_access.py` & `angr-9.2.98/angr/procedures/java_jni/field_access.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java_jni/global_and_local_refs.py` & `angr-9.2.98/angr/procedures/java_jni/global_and_local_refs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java_jni/method_calls.py` & `angr-9.2.98/angr/procedures/java_jni/method_calls.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java_jni/not_implemented.py` & `angr-9.2.98/angr/procedures/java_jni/not_implemented.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java_jni/object_operations.py` & `angr-9.2.98/angr/procedures/java_jni/object_operations.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java_jni/string_operations.py` & `angr-9.2.98/angr/procedures/java_jni/string_operations.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java_lang/character.py` & `angr-9.2.98/angr/procedures/java_lang/character.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java_lang/double.py` & `angr-9.2.98/angr/procedures/java_lang/double.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java_lang/integer.py` & `angr-9.2.98/angr/procedures/java_lang/integer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java_lang/string.py` & `angr-9.2.98/angr/procedures/java_lang/string.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java_lang/stringbuilder.py` & `angr-9.2.98/angr/procedures/java_lang/stringbuilder.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java_util/collection.py` & `angr-9.2.98/angr/procedures/java_util/collection.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java_util/iterator.py` & `angr-9.2.98/angr/procedures/java_util/iterator.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java_util/list.py` & `angr-9.2.98/angr/procedures/java_util/list.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java_util/map.py` & `angr-9.2.98/angr/procedures/java_util/map.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/java_util/scanner_nextline.py` & `angr-9.2.98/angr/procedures/java_util/scanner_nextline.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/error.py` & `angr-9.2.98/angr/procedures/libc/error.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/fclose.py` & `angr-9.2.98/angr/procedures/libc/fclose.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/feof.py` & `angr-9.2.98/angr/procedures/libc/feof.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/fgetc.py` & `angr-9.2.98/angr/procedures/libc/fgetc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/fgets.py` & `angr-9.2.98/angr/procedures/libc/fgets.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/fopen.py` & `angr-9.2.98/angr/procedures/libc/fopen.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/fprintf.py` & `angr-9.2.98/angr/procedures/libc/fprintf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/fputc.py` & `angr-9.2.98/angr/procedures/libc/fputc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/fputs.py` & `angr-9.2.98/angr/procedures/libc/fputs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/fread.py` & `angr-9.2.98/angr/procedures/libc/fread.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/fscanf.py` & `angr-9.2.98/angr/procedures/libc/fscanf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/fseek.py` & `angr-9.2.98/angr/procedures/libc/fseek.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/ftell.py` & `angr-9.2.98/angr/procedures/libc/ftell.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/getdelim.py` & `angr-9.2.98/angr/procedures/libc/getdelim.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/gets.py` & `angr-9.2.98/angr/procedures/libc/gets.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/memcmp.py` & `angr-9.2.98/angr/procedures/libc/memcmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/memcpy.py` & `angr-9.2.98/angr/procedures/libc/memcpy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/memset.py` & `angr-9.2.98/angr/procedures/libc/memset.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/printf.py` & `angr-9.2.98/angr/procedures/libc/printf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/scanf.py` & `angr-9.2.98/angr/procedures/libc/scanf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/snprintf.py` & `angr-9.2.98/angr/procedures/libc/snprintf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/sprintf.py` & `angr-9.2.98/angr/procedures/libc/sprintf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/strchr.py` & `angr-9.2.98/angr/procedures/libc/strchr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/strcmp.py` & `angr-9.2.98/angr/procedures/libc/strcmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/strlen.py` & `angr-9.2.98/angr/procedures/libc/strlen.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/strncmp.py` & `angr-9.2.98/angr/procedures/libc/strncmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/strncpy.py` & `angr-9.2.98/angr/procedures/libc/strncpy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/strstr.py` & `angr-9.2.98/angr/procedures/libc/strstr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/strtol.py` & `angr-9.2.98/angr/procedures/libc/strtol.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/tmpnam.py` & `angr-9.2.98/angr/procedures/libc/tmpnam.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/ungetc.py` & `angr-9.2.98/angr/procedures/libc/ungetc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/libc/wchar.py` & `angr-9.2.98/angr/procedures/libc/wchar.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_kernel/access.py` & `angr-9.2.98/angr/procedures/linux_kernel/access.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_kernel/arch_prctl.py` & `angr-9.2.98/angr/procedures/linux_kernel/arch_prctl.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_kernel/arm_user_helpers.py` & `angr-9.2.98/angr/procedures/linux_kernel/arm_user_helpers.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_kernel/cwd.py` & `angr-9.2.98/angr/procedures/linux_kernel/cwd.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_kernel/fstat.py` & `angr-9.2.98/angr/procedures/linux_kernel/fstat.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_kernel/fstat64.py` & `angr-9.2.98/angr/procedures/linux_kernel/fstat64.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_kernel/futex.py` & `angr-9.2.98/angr/procedures/linux_kernel/futex.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_kernel/getrlimit.py` & `angr-9.2.98/angr/procedures/linux_kernel/getrlimit.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_kernel/iovec.py` & `angr-9.2.98/angr/procedures/linux_kernel/iovec.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_kernel/lseek.py` & `angr-9.2.98/angr/procedures/linux_kernel/lseek.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_kernel/mprotect.py` & `angr-9.2.98/angr/procedures/linux_kernel/mprotect.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_kernel/openat.py` & `angr-9.2.98/angr/procedures/linux_kernel/openat.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_kernel/sigaction.py` & `angr-9.2.98/angr/procedures/linux_kernel/sigaction.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_kernel/sigprocmask.py` & `angr-9.2.98/angr/procedures/linux_kernel/sigprocmask.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_kernel/stat.py` & `angr-9.2.98/angr/procedures/linux_kernel/stat.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_kernel/sysinfo.py` & `angr-9.2.98/angr/procedures/linux_kernel/sysinfo.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_kernel/time.py` & `angr-9.2.98/angr/procedures/linux_kernel/time.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_kernel/uid.py` & `angr-9.2.98/angr/procedures/linux_kernel/uid.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_kernel/uname.py` & `angr-9.2.98/angr/procedures/linux_kernel/uname.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_kernel/unlink.py` & `angr-9.2.98/angr/procedures/linux_kernel/unlink.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_loader/sim_loader.py` & `angr-9.2.98/angr/procedures/linux_loader/sim_loader.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/linux_loader/tls.py` & `angr-9.2.98/angr/procedures/linux_loader/tls.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/msvcr/__getmainargs.py` & `angr-9.2.98/angr/procedures/msvcr/__getmainargs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/msvcr/_initterm.py` & `angr-9.2.98/angr/procedures/msvcr/_initterm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/msvcr/fmode.py` & `angr-9.2.98/angr/procedures/msvcr/fmode.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/ntdll/exceptions.py` & `angr-9.2.98/angr/procedures/ntdll/exceptions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/posix/accept.py` & `angr-9.2.98/angr/procedures/posix/accept.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/posix/chroot.py` & `angr-9.2.98/angr/procedures/posix/chroot.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/posix/dup.py` & `angr-9.2.98/angr/procedures/posix/dup.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/posix/fdopen.py` & `angr-9.2.98/angr/procedures/posix/fdopen.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/posix/getenv.py` & `angr-9.2.98/angr/procedures/posix/getenv.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/posix/gethostbyname.py` & `angr-9.2.98/angr/procedures/posix/gethostbyname.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/posix/inet_ntoa.py` & `angr-9.2.98/angr/procedures/posix/inet_ntoa.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/posix/mmap.py` & `angr-9.2.98/angr/procedures/posix/mmap.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/posix/open.py` & `angr-9.2.98/angr/procedures/posix/open.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/posix/poll.py` & `angr-9.2.98/angr/procedures/posix/poll.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/posix/pread64.py` & `angr-9.2.98/angr/procedures/posix/pread64.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/posix/pthread.py` & `angr-9.2.98/angr/procedures/posix/pthread.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/posix/pwrite64.py` & `angr-9.2.98/angr/procedures/posix/pwrite64.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/posix/readdir.py` & `angr-9.2.98/angr/procedures/posix/readdir.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/posix/select.py` & `angr-9.2.98/angr/procedures/posix/select.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/posix/send.py` & `angr-9.2.98/angr/procedures/posix/send.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/posix/sigaction.py` & `angr-9.2.98/angr/procedures/posix/sigaction.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/posix/sim_time.py` & `angr-9.2.98/angr/procedures/posix/sim_time.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/posix/socket.py` & `angr-9.2.98/angr/procedures/posix/socket.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/posix/strcasecmp.py` & `angr-9.2.98/angr/procedures/posix/strcasecmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/posix/strtok_r.py` & `angr-9.2.98/angr/procedures/posix/strtok_r.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/procedure_dict.py` & `angr-9.2.98/angr/procedures/procedure_dict.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/stubs/ReturnUnconstrained.py` & `angr-9.2.98/angr/procedures/stubs/ReturnUnconstrained.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/stubs/UserHook.py` & `angr-9.2.98/angr/procedures/stubs/UserHook.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/stubs/crazy_scanf.py` & `angr-9.2.98/angr/procedures/stubs/crazy_scanf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/stubs/format_parser.py` & `angr-9.2.98/angr/procedures/stubs/format_parser.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/stubs/syscall_stub.py` & `angr-9.2.98/angr/procedures/stubs/syscall_stub.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/tracer/receive.py` & `angr-9.2.98/angr/procedures/tracer/receive.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/tracer/transmit.py` & `angr-9.2.98/angr/procedures/tracer/transmit.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/win32/GetLastInputInfo.py` & `angr-9.2.98/angr/procedures/win32/GetLastInputInfo.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/win32/GetModuleHandle.py` & `angr-9.2.98/angr/procedures/win32/GetModuleHandle.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/win32/GetProcessAffinityMask.py` & `angr-9.2.98/angr/procedures/win32/GetProcessAffinityMask.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/win32/InterlockedExchange.py` & `angr-9.2.98/angr/procedures/win32/InterlockedExchange.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/win32/VirtualAlloc.py` & `angr-9.2.98/angr/procedures/win32/VirtualAlloc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/win32/VirtualProtect.py` & `angr-9.2.98/angr/procedures/win32/VirtualProtect.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/win32/dynamic_loading.py` & `angr-9.2.98/angr/procedures/win32/dynamic_loading.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/win32/file_handles.py` & `angr-9.2.98/angr/procedures/win32/file_handles.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/win32/heap.py` & `angr-9.2.98/angr/procedures/win32/heap.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/win32/is_bad_ptr.py` & `angr-9.2.98/angr/procedures/win32/is_bad_ptr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/win32/local_storage.py` & `angr-9.2.98/angr/procedures/win32/local_storage.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/win32/sim_time.py` & `angr-9.2.98/angr/procedures/win32/sim_time.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/win32/system_paths.py` & `angr-9.2.98/angr/procedures/win32/system_paths.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/procedures/win_user32/messagebox.py` & `angr-9.2.98/angr/procedures/win_user32/messagebox.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/project.py` & `angr-9.2.98/angr/project.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/protos/cfg_pb2.py` & `angr-9.2.98/angr/protos/cfg_pb2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/protos/function_pb2.py` & `angr-9.2.98/angr/protos/function_pb2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/protos/primitives_pb2.py` & `angr-9.2.98/angr/protos/primitives_pb2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/protos/variables_pb2.py` & `angr-9.2.98/angr/protos/variables_pb2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/protos/xrefs_pb2.py` & `angr-9.2.98/angr/protos/xrefs_pb2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/serializable.py` & `angr-9.2.98/angr/serializable.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/service.py` & `angr-9.2.98/angr/service.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/sim_manager.py` & `angr-9.2.98/angr/sim_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/sim_options.py` & `angr-9.2.98/angr/sim_options.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/sim_procedure.py` & `angr-9.2.98/angr/sim_procedure.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/sim_state.py` & `angr-9.2.98/angr/sim_state.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/sim_state_options.py` & `angr-9.2.98/angr/sim_state_options.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/sim_type.py` & `angr-9.2.98/angr/sim_type.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/sim_variable.py` & `angr-9.2.98/angr/sim_variable.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/simos/__init__.py` & `angr-9.2.98/angr/simos/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/simos/cgc.py` & `angr-9.2.98/angr/simos/cgc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/simos/javavm.py` & `angr-9.2.98/angr/simos/javavm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/simos/linux.py` & `angr-9.2.98/angr/simos/linux.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/simos/simos.py` & `angr-9.2.98/angr/simos/simos.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/simos/snimmuc_nxp.py` & `angr-9.2.98/angr/simos/snimmuc_nxp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/simos/userland.py` & `angr-9.2.98/angr/simos/userland.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/simos/windows.py` & `angr-9.2.98/angr/simos/windows.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/slicer.py` & `angr-9.2.98/angr/slicer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_hierarchy.py` & `angr-9.2.98/angr/state_hierarchy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/__init__.py` & `angr-9.2.98/angr/state_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/callstack.py` & `angr-9.2.98/angr/state_plugins/callstack.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/cgc.py` & `angr-9.2.98/angr/state_plugins/cgc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/concrete.py` & `angr-9.2.98/angr/state_plugins/concrete.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/debug_variables.py` & `angr-9.2.98/angr/state_plugins/debug_variables.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/filesystem.py` & `angr-9.2.98/angr/state_plugins/filesystem.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/gdb.py` & `angr-9.2.98/angr/state_plugins/gdb.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/globals.py` & `angr-9.2.98/angr/state_plugins/globals.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/heap/heap_base.py` & `angr-9.2.98/angr/state_plugins/heap/heap_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/heap/heap_brk.py` & `angr-9.2.98/angr/state_plugins/heap/heap_brk.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/heap/heap_freelist.py` & `angr-9.2.98/angr/state_plugins/heap/heap_freelist.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/heap/heap_libc.py` & `angr-9.2.98/angr/state_plugins/heap/heap_libc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/heap/heap_ptmalloc.py` & `angr-9.2.98/angr/state_plugins/heap/heap_ptmalloc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/heap/utils.py` & `angr-9.2.98/angr/state_plugins/heap/utils.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/history.py` & `angr-9.2.98/angr/state_plugins/history.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/inspect.py` & `angr-9.2.98/angr/state_plugins/inspect.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/javavm_classloader.py` & `angr-9.2.98/angr/state_plugins/javavm_classloader.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/jni_references.py` & `angr-9.2.98/angr/state_plugins/jni_references.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/libc.py` & `angr-9.2.98/angr/state_plugins/libc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/light_registers.py` & `angr-9.2.98/angr/state_plugins/light_registers.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/log.py` & `angr-9.2.98/angr/state_plugins/log.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/loop_data.py` & `angr-9.2.98/angr/state_plugins/loop_data.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/plugin.py` & `angr-9.2.98/angr/state_plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/posix.py` & `angr-9.2.98/angr/state_plugins/posix.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/preconstrainer.py` & `angr-9.2.98/angr/state_plugins/preconstrainer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/scratch.py` & `angr-9.2.98/angr/state_plugins/scratch.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/sim_action.py` & `angr-9.2.98/angr/state_plugins/sim_action.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/sim_action_object.py` & `angr-9.2.98/angr/state_plugins/sim_action_object.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/sim_event.py` & `angr-9.2.98/angr/state_plugins/sim_event.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/solver.py` & `angr-9.2.98/angr/state_plugins/solver.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/symbolizer.py` & `angr-9.2.98/angr/state_plugins/symbolizer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/trace_additions.py` & `angr-9.2.98/angr/state_plugins/trace_additions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/uc_manager.py` & `angr-9.2.98/angr/state_plugins/uc_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/unicorn_engine.py` & `angr-9.2.98/angr/state_plugins/unicorn_engine.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/state_plugins/view.py` & `angr-9.2.98/angr/state_plugins/view.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/file.py` & `angr-9.2.98/angr/storage/file.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/__init__.py` & `angr-9.2.98/angr/storage/memory_mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/__init__.pyi` & `angr-9.2.98/angr/storage/memory_mixins/__init__.pyi`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/actions_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/actions_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/address_concretization_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/address_concretization_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/bvv_conversion_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/bvv_conversion_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/clouseau_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/clouseau_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/conditional_store_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/conditional_store_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/convenient_mappings_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/convenient_mappings_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/default_filler_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/default_filler_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/hex_dumper_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/hex_dumper_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/javavm_memory/javavm_memory_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/javavm_memory/javavm_memory_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/keyvalue_memory/keyvalue_memory_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/keyvalue_memory/keyvalue_memory_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/label_merger_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/label_merger_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/multi_value_merger_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/multi_value_merger_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/name_resolution_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/name_resolution_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/paged_memory/page_backer_mixins.py` & `angr-9.2.98/angr/storage/memory_mixins/paged_memory/page_backer_mixins.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/paged_memory/paged_memory_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/paged_memory/paged_memory_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/paged_memory/paged_memory_multivalue_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/paged_memory/paged_memory_multivalue_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/__init__.py` & `angr-9.2.98/angr/storage/memory_mixins/paged_memory/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/cooperation.py` & `angr-9.2.98/angr/storage/memory_mixins/paged_memory/pages/cooperation.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/history_tracking_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/paged_memory/pages/history_tracking_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/ispo_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/paged_memory/pages/ispo_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/list_page.py` & `angr-9.2.98/angr/storage/memory_mixins/paged_memory/pages/list_page.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # pylint:disable=abstract-method,arguments-differ
 import logging
 from typing import Optional, List, Set, Tuple
 
+import claripy
+
 from angr.utils.dynamic_dictlist import DynamicDictList
 from angr.storage.memory_object import SimMemoryObject, SimLabeledMemoryObject
 from . import PageBase
 from .cooperation import MemoryObjectMixin
 
 
 l = logging.getLogger(name=__name__)
@@ -188,17 +190,22 @@
                     new_mo = SimMemoryObject(merged_val, mo_base, endness=the_endness)
                 self.store(b, new_mo, size=size, cooperate=True)
                 # merged_objects.add(new_object)
                 # merged_objects.update(mos)
                 merged_offsets.add(b)
 
             else:
-                # get the size that we can merge easily. This is the minimum of
-                # the size of all memory objects and unallocated spaces.
-                min_size = min([mo.length - (b + page_addr - mo.base) for mo, _ in memory_objects])
+                # get the size that we can merge easily. This is the minimum of the size of all memory objects and
+                # unallocated spaces.
+                min_size = None
+                mask = (1 << memory.state.arch.bits) - 1
+                for mo, _ in memory_objects:
+                    mo_size = mo.length - ((b + page_addr - mo.base) & mask)
+                    if min_size is None or mo_size < min_size:
+                        min_size = mo_size
                 for um, _ in unconstrained_in:
                     for i in range(0, min_size):
                         if um._contains(b + i, page_addr):
                             min_size = i
                             break
                 merged_to = b + min_size
                 l.info("... determined minimum size of %d", min_size)
@@ -259,23 +266,31 @@
             o_contains = other._contains(c, page_addr)
             if not s_contains and o_contains:
                 differences.add(c)
             elif s_contains and not o_contains:
                 differences.add(c)
             else:
                 if self.content[c] is None:
+                    if self.sinkhole is None:
+                        v = claripy.BVV(0, 8)
+                    else:
+                        v = (self.sinkhole.bytes_at(page_addr + c, 1),)
                     self.content[c] = SimMemoryObject(
-                        self.sinkhole.bytes_at(page_addr + c, 1),
+                        v,
                         page_addr + c,
                         byte_width=byte_width,
                         endness="Iend_BE",
                     )
                 if other.content[c] is None:
+                    if other.sinkhole is None:
+                        v = claripy.BVV(0, 8)
+                    else:
+                        v = (other.sinkhole.bytes_at(page_addr + c, 1),)
                     other.content[c] = SimMemoryObject(
-                        other.sinkhole.bytes_at(page_addr + c, 1),
+                        v,
                         page_addr + c,
                         byte_width=byte_width,
                         endness="Iend_BE",
                     )
                 if s_contains and self.content[c] != other.content[c]:
                     same = None
                     if self._mo_cmp is not None:
```

### Comparing `angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/multi_values.py` & `angr-9.2.98/angr/storage/memory_mixins/paged_memory/pages/multi_values.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/mv_list_page.py` & `angr-9.2.98/angr/storage/memory_mixins/paged_memory/pages/mv_list_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,17 +235,18 @@
 
                 merged_offsets.add(b)
 
             else:
                 # get the size that we can merge easily. This is the minimum of the size of all memory objects and
                 # unallocated spaces.
                 min_size = len(self.content) - b
+                mask = (1 << memory.state.arch.bits) - 1
                 for mo_set in mo_sets:
                     for mo in mo_set:
-                        min_size = min(min_size, mo.length - (b + page_addr - mo.base))
+                        min_size = min(min_size, mo.length - ((b + page_addr - mo.base) & mask))
                 for um, _ in unconstrained_in:
                     for i in range(0, min_size):
                         if um._contains(b + i, page_addr):
                             min_size = i
                             break
                 merged_to = b + min_size
                 l.info("... determined minimum size of %d", min_size)
```

### Comparing `angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/permissions_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/paged_memory/pages/permissions_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/refcount_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/paged_memory/pages/refcount_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/ultra_page.py` & `angr-9.2.98/angr/storage/memory_mixins/paged_memory/pages/ultra_page.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/paged_memory/privileged_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/paged_memory/privileged_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/paged_memory/stack_allocation_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/paged_memory/stack_allocation_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/regioned_memory/abstract_address_descriptor.py` & `angr-9.2.98/angr/storage/memory_mixins/regioned_memory/abstract_address_descriptor.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/regioned_memory/abstract_merger_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/regioned_memory/abstract_merger_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/regioned_memory/region_data.py` & `angr-9.2.98/angr/storage/memory_mixins/regioned_memory/region_data.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/regioned_memory/region_meta_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/regioned_memory/region_meta_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/regioned_memory/regioned_address_concretization_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/regioned_memory/regioned_address_concretization_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/regioned_memory/regioned_memory_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/regioned_memory/regioned_memory_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/regioned_memory/static_find_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/regioned_memory/static_find_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/simple_interface_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/simple_interface_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,16 @@
             size=tsize,
             endness=self._translate_endness(endness),
             condition=self._translate_cond(condition),
             **kwargs,
         )
 
     def _translate_addr(self, a):
+        if isinstance(a, int):
+            return a
         if isinstance(a, claripy.ast.Base) and not a.singlevalued:
             raise SimMemoryError("address not supported")
         return self.state.solver.eval(a)
 
     def _translate_data(self, d, size):
         if type(d) in (bytes, bytearray):
             return self.state.solver.BVV(d)
@@ -39,14 +41,16 @@
             return self.state.solver.BVV(d, size * self.state.arch.byte_width)
         elif isinstance(d, claripy.ast.Base):
             return d
         else:
             raise SimMemoryError("data not supported")
 
     def _translate_size(self, s, data):
+        if isinstance(s, int):
+            return s
         if isinstance(s, claripy.ast.Base) and not s.singlevalued:
             raise SimMemoryError("size not supported")
         if s is None:
             if isinstance(data, claripy.ast.BV):
                 return len(data) // self.state.arch.byte_width
             elif isinstance(data, (bytes, bytearray)):
                 return len(data)
```

### Comparing `angr-9.2.97/angr/storage/memory_mixins/size_resolution_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/size_resolution_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/slotted_memory.py` & `angr-9.2.98/angr/storage/memory_mixins/slotted_memory.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/smart_find_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/smart_find_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/top_merger_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/top_merger_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/underconstrained_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/underconstrained_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_mixins/unwrapper_mixin.py` & `angr-9.2.98/angr/storage/memory_mixins/unwrapper_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/memory_object.py` & `angr-9.2.98/angr/storage/memory_object.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/storage/pcap.py` & `angr-9.2.98/angr/storage/pcap.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/tablespecs.py` & `angr-9.2.98/angr/tablespecs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/utils/__init__.py` & `angr-9.2.98/angr/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/utils/algo.py` & `angr-9.2.98/angr/utils/algo.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/utils/cowdict.py` & `angr-9.2.98/angr/utils/cowdict.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/utils/dynamic_dictlist.py` & `angr-9.2.98/angr/utils/dynamic_dictlist.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/utils/enums_conv.py` & `angr-9.2.98/angr/utils/enums_conv.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/utils/formatting.py` & `angr-9.2.98/angr/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/utils/funcid.py` & `angr-9.2.98/angr/utils/funcid.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/utils/graph.py` & `angr-9.2.98/angr/utils/graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/utils/library.py` & `angr-9.2.98/angr/utils/library.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/utils/loader.py` & `angr-9.2.98/angr/utils/loader.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/utils/mp.py` & `angr-9.2.98/angr/utils/mp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/utils/segment_list.py` & `angr-9.2.98/angr/utils/segment_list.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/utils/timing.py` & `angr-9.2.98/angr/utils/timing.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr/vaults.py` & `angr-9.2.98/angr/vaults.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/angr.egg-info/PKG-INFO` & `angr-9.2.98/angr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angr
-Version: 9.2.97
+Version: 9.2.98
 Summary: A multi-architecture binary analysis toolkit, with the ability to perform dynamic symbolic execution and various static analyses on binaries
 Home-page: https://github.com/angr/angr
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -13,31 +13,31 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: CppHeaderParser
 Requires-Dist: GitPython
-Requires-Dist: ailment==9.2.97
-Requires-Dist: archinfo==9.2.97
+Requires-Dist: ailment==9.2.98
+Requires-Dist: archinfo==9.2.98
 Requires-Dist: cachetools
 Requires-Dist: capstone==5.0.0.post1
 Requires-Dist: cffi>=1.14.0
-Requires-Dist: claripy==9.2.97
-Requires-Dist: cle==9.2.97
+Requires-Dist: claripy==9.2.98
+Requires-Dist: cle==9.2.98
 Requires-Dist: dpkt
 Requires-Dist: itanium-demangler
 Requires-Dist: mulpyplexer
 Requires-Dist: nampa
 Requires-Dist: networkx!=2.8.1,>=2.0
 Requires-Dist: protobuf>=3.19.0
 Requires-Dist: psutil
 Requires-Dist: pycparser>=2.18
 Requires-Dist: pyformlang
-Requires-Dist: pyvex==9.2.97
+Requires-Dist: pyvex==9.2.98
 Requires-Dist: rich>=13.1.0
 Requires-Dist: rpyc
 Requires-Dist: sortedcontainers
 Requires-Dist: sympy
 Requires-Dist: unicorn==2.0.1.post1
 Requires-Dist: unique-log-filter
 Requires-Dist: colorama; platform_system == "Windows"
```

### Comparing `angr-9.2.97/angr.egg-info/SOURCES.txt` & `angr-9.2.98/angr.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -134,14 +134,15 @@
 angr/analyses/decompiler/optimization_passes/code_motion.py
 angr/analyses/decompiler/optimization_passes/const_derefs.py
 angr/analyses/decompiler/optimization_passes/cross_jump_reverter.py
 angr/analyses/decompiler/optimization_passes/div_simplifier.py
 angr/analyses/decompiler/optimization_passes/engine_base.py
 angr/analyses/decompiler/optimization_passes/expr_op_swapper.py
 angr/analyses/decompiler/optimization_passes/flip_boolean_cmp.py
+angr/analyses/decompiler/optimization_passes/inlined_string_transformation_simplifier.py
 angr/analyses/decompiler/optimization_passes/ite_expr_converter.py
 angr/analyses/decompiler/optimization_passes/ite_region_converter.py
 angr/analyses/decompiler/optimization_passes/lowered_switch_simplifier.py
 angr/analyses/decompiler/optimization_passes/mod_simplifier.py
 angr/analyses/decompiler/optimization_passes/multi_simplifier.py
 angr/analyses/decompiler/optimization_passes/optimization_pass.py
 angr/analyses/decompiler/optimization_passes/register_save_area_simplifier.py
@@ -173,14 +174,15 @@
 angr/analyses/decompiler/peephole_optimizations/constant_derefs.py
 angr/analyses/decompiler/peephole_optimizations/conv_a_sub0_shr_and.py
 angr/analyses/decompiler/peephole_optimizations/conv_shl_shr.py
 angr/analyses/decompiler/peephole_optimizations/eager_eval.py
 angr/analyses/decompiler/peephole_optimizations/extended_byte_and_mask.py
 angr/analyses/decompiler/peephole_optimizations/inlined_strcpy.py
 angr/analyses/decompiler/peephole_optimizations/inlined_strcpy_consolidation.py
+angr/analyses/decompiler/peephole_optimizations/inlined_wstrcpy.py
 angr/analyses/decompiler/peephole_optimizations/invert_negated_logical_conjuction_disjunction.py
 angr/analyses/decompiler/peephole_optimizations/one_sub_bool.py
 angr/analyses/decompiler/peephole_optimizations/remove_cascading_conversions.py
 angr/analyses/decompiler/peephole_optimizations/remove_empty_if_body.py
 angr/analyses/decompiler/peephole_optimizations/remove_noop_conversions.py
 angr/analyses/decompiler/peephole_optimizations/remove_redundant_bitmasks.py
 angr/analyses/decompiler/peephole_optimizations/remove_redundant_conversions.py
```

### Comparing `angr-9.2.97/angr.egg-info/requires.txt` & `angr-9.2.98/angr.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 CppHeaderParser
 GitPython
-ailment==9.2.97
-archinfo==9.2.97
+ailment==9.2.98
+archinfo==9.2.98
 cachetools
 capstone==5.0.0.post1
 cffi>=1.14.0
-claripy==9.2.97
-cle==9.2.97
+claripy==9.2.98
+cle==9.2.98
 dpkt
 itanium-demangler
 mulpyplexer
 nampa
 networkx!=2.8.1,>=2.0
 protobuf>=3.19.0
 psutil
 pycparser>=2.18
 pyformlang
-pyvex==9.2.97
+pyvex==9.2.98
 rich>=13.1.0
 rpyc
 sortedcontainers
 sympy
 unicorn==2.0.1.post1
 unique-log-filter
```

### Comparing `angr-9.2.97/native/Makefile` & `angr-9.2.98/native/Makefile`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/native/angr_native.def` & `angr-9.2.98/native/angr_native.def`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/native/log.c` & `angr-9.2.98/native/log.c`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/native/log.h` & `angr-9.2.98/native/log.h`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/native/sim_unicorn.cpp` & `angr-9.2.98/native/sim_unicorn.cpp`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/native/sim_unicorn.hpp` & `angr-9.2.98/native/sim_unicorn.hpp`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/pyproject.toml` & `angr-9.2.98/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=59", "wheel", "pyvex==9.2.97", "unicorn==2.0.1.post1"]
+requires = ["setuptools>=59", "wheel", "pyvex==9.2.98", "unicorn==2.0.1.post1"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
 target-version = ['py38']
 force-exclude = '''
 /(
```

### Comparing `angr-9.2.97/setup.cfg` & `angr-9.2.98/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -18,31 +18,31 @@
 	Programming Language :: Python :: 3.12
 
 [options]
 packages = find:
 install_requires = 
 	CppHeaderParser
 	GitPython
-	ailment==9.2.97
-	archinfo==9.2.97
+	ailment==9.2.98
+	archinfo==9.2.98
 	cachetools
 	capstone==5.0.0.post1
 	cffi>=1.14.0
-	claripy==9.2.97
-	cle==9.2.97
+	claripy==9.2.98
+	cle==9.2.98
 	dpkt
 	itanium-demangler
 	mulpyplexer
 	nampa
 	networkx!=2.8.1,>=2.0
 	protobuf>=3.19.0
 	psutil
 	pycparser>=2.18
 	pyformlang
-	pyvex==9.2.97
+	pyvex==9.2.98
 	rich>=13.1.0
 	rpyc
 	sortedcontainers
 	sympy
 	unicorn==2.0.1.post1
 	unique-log-filter
 	colorama;platform_system=='Windows'
```

### Comparing `angr-9.2.97/setup.py` & `angr-9.2.98/setup.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/tests/test_calling_conventions.py` & `angr-9.2.98/tests/test_calling_conventions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.97/tests/test_types.py` & `angr-9.2.98/tests/test_types.py`

 * *Files identical despite different names*


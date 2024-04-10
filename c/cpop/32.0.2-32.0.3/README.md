# Comparing `tmp/cpop-32.0.2.tar.gz` & `tmp/cpop-32.0.3.tar.gz`

## Comparing `cpop-32.0.2.tar` & `cpop-32.0.3.tar`

### file list

```diff
@@ -1,173 +1,174 @@
--rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 cpop-32.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     8448 2020-02-02 00:00:00.000000 cpop-32.0.2/src/cpop/contract.pyx
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 cpop-32.0.2/src/cpop/data.pyx
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/config.yaml
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/dirs.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/exc.py
--rw-r--r--   0        0        0    24935 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/hub.py
--rw-r--r--   0        0        0    11370 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/loader.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/ref.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/scanner.py
--rw-r--r--   0        0        0     7642 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/verify.py
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/log/async.py
--rw-r--r--   0        0        0     9498 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/mods/config.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/mods/contract.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/mods/dyne.py
--rw-r--r--   0        0        0     6941 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/mods/sub.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/mods/task.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cpop-32.0.2/src/pop/mods/test.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/conftest.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/alias/init.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/cmods/ctest.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/cmods/contracts/ctest.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/contracts/ctx.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/contracts/ctx_args.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/contracts/ctx_update.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/contracts/many.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/contracts/priv.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/contracts/test.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/contracts/testing.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/coro/test.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/coro/contracts/test.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/csigs/sigs.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/csigs/contracts/sigs.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/external_module/api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/__init__.py
--rw-r--r--   0        0        0     7459 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_basic.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_bench.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_cli.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_contract_ctx.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_coro.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_cpop.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_fail.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_no_raise_on_pre_failure.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_raise_on_pre_failure.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_serial.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/func/test_sub.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contract_ordering/single_module/thing.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contract_ordering/single_module/contracts/default.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contract_ordering/single_module/contracts/dunder.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contract_ordering/single_module/contracts/init.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contract_ordering/single_module/contracts/thing.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contracted/test_contracted_access.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contracted/mods/contracted_access.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/contracted/mods/contracts/contracted_access.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/recursive_contract/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/recursive_contract/test_sub.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/bad.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/falias_dict.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/falias_func.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/foo.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/fork.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/many.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/priv.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/proc.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/test.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/testing.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/vbad.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/virt.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/vtrue.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/bad_import/bad_import.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/contract_ctx/ctx.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/contract_ctx/ctx_args.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/contract_ctx/ctx_update.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/contract_sig/fail_sigs.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/contract_sig/pass_sigs.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/contract_sig/contracts/init.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/coro/coro.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/iter/bar.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/iter/foo.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/iter/init.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/nest/basic.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/same_vname/will_load.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/same_vname/will_not_load.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/subinit/init.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/mods/subinit/subinit.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/regression/contract_masking/test_contract_masking.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/regression/contract_masking/test_duplicate_contracts.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/regression/contract_masking/contract1/init.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/regression/contract_masking/contract2/init.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/regression/contract_masking/sub/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/sdirs/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/sdirs/l11/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/sdirs/l11/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/sdirs/l12/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/sdirs/l12/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/sdirs/l13/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/sdirs/l13/l2/test.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/README.rst
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/cn/config.yaml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/cn/contract/test.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/cn/contract/contracts/test.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/config.yaml
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/init.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/clash.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/dup1.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/dup2.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/float.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/init.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/invalid.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/neg.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/neg_last.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/pos.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/pos_first.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/pos_first_tie.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/unordered_1.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/unordered_2.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/verify_fail.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/verify_pass.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/verify_raise.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/contracts/zero.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/nest/init.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/recursive_contracts/clash.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/recursive_contracts/init.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/recursive_contracts/unordered_3.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/co1/contract_ordering/recursive_contracts/unordered_4.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/config/config.yaml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn1/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn1/dn1/nest/dn1.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn1/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn2/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn2/dn1/nest/dn2.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn2/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn3/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn3/dn1/nest/dn3.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn3/dn1/nest/over.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn3/dn1/nest/next/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dn3/dn1/nest/next/last/test.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne1/config.yaml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne1/dyne1/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne1/dyne1/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne1/nest/dyne/nest.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne2/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne2/dyne2/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne2/dyne2/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne2/nest/dyne/nest.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne3/config.yaml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne3/dyne3/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne3/dyne3/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne3/nest/dyne/nest.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne4/config.yaml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne4/dyne4/nest/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/dyne4/dyne4/nest/subvert.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/fork/config.yaml
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/fork/fork/rsub.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/fork/fork/nest/init.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/v1/config.yaml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/tpath/v1/v1/load.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/unit/__init__.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/unit/test_contract.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 cpop-32.0.2/tests/unit/test_sigs.py
--rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-32.0.2/.gitignore
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 cpop-32.0.2/README.rst
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 cpop-32.0.2/pyproject.toml
--rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 cpop-32.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 cpop-32.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     8448 2020-02-02 00:00:00.000000 cpop-32.0.3/src/cpop/contract.pyx
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 cpop-32.0.3/src/cpop/data.pyx
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/config.yaml
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/dirs.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/exc.py
+-rw-r--r--   0        0        0    24876 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/hub.py
+-rw-r--r--   0        0        0    11428 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/loader.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/ref.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/scanner.py
+-rw-r--r--   0        0        0     7642 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/verify.py
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/log/async.py
+-rw-r--r--   0        0        0     9482 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/mods/config.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/mods/contract.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/mods/dyne.py
+-rw-r--r--   0        0        0     6941 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/mods/sub.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/mods/task.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/mods/test.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/conftest.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/alias/init.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/cmods/ctest.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/cmods/contracts/ctest.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/contracts/ctx.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/contracts/ctx_args.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/contracts/ctx_update.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/contracts/many.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/contracts/priv.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/contracts/test.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/contracts/testing.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/coro/test.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/coro/contracts/test.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/csigs/sigs.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/csigs/contracts/sigs.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/external_module/api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/__init__.py
+-rw-r--r--   0        0        0     7459 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_basic.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_bench.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_cli.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_contract_ctx.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_coro.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_cpop.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_fail.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_hub.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_no_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_serial.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_sub.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contract_ordering/single_module/thing.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contract_ordering/single_module/contracts/default.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contract_ordering/single_module/contracts/dunder.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contract_ordering/single_module/contracts/init.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contract_ordering/single_module/contracts/thing.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contracted/test_contracted_access.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contracted/mods/contracted_access.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contracted/mods/contracts/contracted_access.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/recursive_contract/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/recursive_contract/test_sub.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/bad.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/falias_dict.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/falias_func.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/foo.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/fork.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/many.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/priv.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/proc.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/test.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/testing.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/vbad.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/virt.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/vtrue.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/bad_import/bad_import.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/contract_ctx/ctx.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/contract_ctx/ctx_args.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/contract_ctx/ctx_update.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/contract_sig/fail_sigs.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/contract_sig/pass_sigs.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/contract_sig/contracts/init.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/coro/coro.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/iter/bar.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/iter/foo.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/iter/init.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/nest/basic.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/same_vname/will_load.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/same_vname/will_not_load.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/subinit/init.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/subinit/subinit.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/regression/contract_masking/test_contract_masking.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/regression/contract_masking/test_duplicate_contracts.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/regression/contract_masking/contract1/init.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/regression/contract_masking/contract2/init.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/regression/contract_masking/sub/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/sdirs/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/sdirs/l11/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/sdirs/l11/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/sdirs/l12/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/sdirs/l12/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/sdirs/l13/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/sdirs/l13/l2/test.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/README.rst
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/cn/config.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/cn/contract/test.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/cn/contract/contracts/test.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/config.yaml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/init.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/clash.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/dup1.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/dup2.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/float.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/init.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/invalid.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/neg.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/neg_last.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/pos.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/pos_first.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/pos_first_tie.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/unordered_1.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/unordered_2.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/verify_fail.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/verify_pass.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/verify_raise.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/zero.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/nest/init.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/recursive_contracts/clash.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/recursive_contracts/init.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/recursive_contracts/unordered_3.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/recursive_contracts/unordered_4.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/config/config.yaml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn1/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn1/dn1/nest/dn1.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn1/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn2/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn2/dn1/nest/dn2.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn2/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn3/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn3/dn1/nest/dn3.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn3/dn1/nest/over.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn3/dn1/nest/next/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn3/dn1/nest/next/last/test.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne1/config.yaml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne1/dyne1/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne1/dyne1/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne1/nest/dyne/nest.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne2/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne2/dyne2/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne2/dyne2/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne2/nest/dyne/nest.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne3/config.yaml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne3/dyne3/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne3/dyne3/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne3/nest/dyne/nest.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne4/config.yaml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne4/dyne4/nest/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne4/dyne4/nest/subvert.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/fork/config.yaml
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/fork/fork/rsub.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/fork/fork/nest/init.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/v1/config.yaml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/v1/v1/load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/unit/__init__.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/unit/test_contract.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/unit/test_sigs.py
+-rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-32.0.3/.gitignore
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 cpop-32.0.3/README.rst
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 cpop-32.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 cpop-32.0.3/PKG-INFO
```

### Comparing `cpop-32.0.2/.pre-commit-config.yaml` & `cpop-32.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/src/cpop/contract.pyx` & `cpop-32.0.3/src/cpop/contract.pyx`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/src/cpop/data.pyx` & `cpop-32.0.3/src/cpop/data.pyx`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/src/pop/config.yaml` & `cpop-32.0.3/src/pop/config.yaml`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/src/pop/dirs.py` & `cpop-32.0.3/src/pop/dirs.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/src/pop/exc.py` & `cpop-32.0.3/src/pop/exc.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/src/pop/hub.py` & `cpop-32.0.3/src/pop/hub.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,15 +345,15 @@
         }
         subs = {}
         sub_alias = {}
         imports = {}
         loaded = {}
         # tracks what has been setattr-ed on this sub for performance; if something needs to be
         # *removed*, we can delattr everything in _cached, it will be re-set on the next call.
-        super().__init__([loaded, subs, sub_alias, imports])
+        super().__init__([loaded, imports, subs, sub_alias])
         self._subs = subs
         self._sub_alias = sub_alias
         self._imports = imports
         self._loaded = loaded
         self._reload_mods = {}
         self._alias = []
         self._loaded_all = False
@@ -537,17 +537,14 @@
             return pop.ref.last(self._hub, item)
 
         try:
             return self[item]
         except KeyError:
             raise AttributeError(f"'{self._subname}' has no attribute '{item}'")
 
-    def __iter__(self):
-        return iter(self._loaded)
-
     async def _sub_init(self):
         """
         Run load init.py for the sub, running '__init__' function if present
         """
         await self._find_mod("init", match_only=True)
 
     def _process_load_error(
```

### Comparing `cpop-32.0.2/src/pop/loader.py` & `cpop-32.0.3/src/pop/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,7 +334,10 @@
     def __getstate__(self):
         return {
             "vars": {k: v for k, v in self._vars.items() if isinstance(v, BASE_TYPES)}
         }
 
     def __setstate__(self, state: dict[str, any]):
         self._vars.update(state["vars"])
+
+    def __iter__(self):
+        return iter(self._attrs)
```

### Comparing `cpop-32.0.2/src/pop/scanner.py` & `cpop-32.0.3/src/pop/scanner.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/src/pop/verify.py` & `cpop-32.0.3/src/pop/verify.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/src/pop/log/async.py` & `cpop-32.0.3/src/pop/log/async.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/src/pop/mods/config.py` & `cpop-32.0.3/src/pop/mods/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import cpop.data
 
 
 async def load(
-    hub: "pop.hub.Hub",
+    hub,
     cli: str = None,
     cli_config: dict[str, object] = None,
     config: dict[str, object] = None,
     subcommands: dict[str, object] = None,
     global_clis: list[str] = None,
     parser_args: tuple = None,
 ):
@@ -266,8 +266,7 @@
                     # only update absolute paths for keys
                     #  ending in _dir, _path or _file
                     if path.is_absolute():
                         # remove the root from the path, then join it to the main root
                         OPT[namespace][key] = root_dir.joinpath(*path.parts[1:])
             except TypeError:
                 continue
-
```

### Comparing `cpop-32.0.2/src/pop/mods/contract.py` & `cpop-32.0.3/src/pop/mods/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/src/pop/mods/sub.py` & `cpop-32.0.3/src/pop/mods/sub.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/src/pop/mods/task.py` & `cpop-32.0.3/src/pop/mods/task.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/src/pop/mods/test.py` & `cpop-32.0.3/src/pop/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/conftest.py` & `cpop-32.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/contracts/ctx.py` & `cpop-32.0.3/tests/contracts/ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/contracts/many.py` & `cpop-32.0.3/tests/contracts/many.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/contracts/test.py` & `cpop-32.0.3/tests/contracts/test.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/func/test_basic.py` & `cpop-32.0.3/tests/func/test_basic.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/func/test_contract_ctx.py` & `cpop-32.0.3/tests/func/test_contract_ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/func/test_fail.py` & `cpop-32.0.3/tests/func/test_fail.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/func/test_no_raise_on_pre_failure.py` & `cpop-32.0.3/tests/func/test_no_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/func/test_raise_on_pre_failure.py` & `cpop-32.0.3/tests/func/test_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/integration/contract_ordering/single_module/contracts/default.py` & `cpop-32.0.3/tests/integration/contract_ordering/single_module/contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/integration/contract_ordering/single_module/contracts/dunder.py` & `cpop-32.0.3/tests/integration/contract_ordering/single_module/contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/integration/contract_ordering/single_module/contracts/init.py` & `cpop-32.0.3/tests/integration/contract_ordering/single_module/contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/integration/contract_ordering/single_module/contracts/thing.py` & `cpop-32.0.3/tests/integration/contract_ordering/single_module/contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/default.py` & `cpop-32.0.3/tests/integration/contract_ordering/single_module/recursive_contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py` & `cpop-32.0.3/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/init.py` & `cpop-32.0.3/tests/integration/contract_ordering/single_module/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py` & `cpop-32.0.3/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py` & `cpop-32.0.3/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py` & `cpop-32.0.3/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/mods/proc.py` & `cpop-32.0.3/tests/mods/proc.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/mods/test.py` & `cpop-32.0.3/tests/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/regression/contract_masking/test_contract_masking.py` & `cpop-32.0.3/tests/regression/contract_masking/test_contract_masking.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/regression/contract_masking/test_duplicate_contracts.py` & `cpop-32.0.3/tests/regression/contract_masking/test_duplicate_contracts.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/tpath/cn/contract/test.py` & `cpop-32.0.3/tests/tpath/cn/contract/test.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/tpath/co1/contract_ordering/init.py` & `cpop-32.0.3/tests/tpath/co1/contract_ordering/init.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/tpath/co1/contract_ordering/nest/init.py` & `cpop-32.0.3/tests/tpath/co1/contract_ordering/nest/init.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/unit/test_contract.py` & `cpop-32.0.3/tests/unit/test_contract.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/tests/unit/test_sigs.py` & `cpop-32.0.3/tests/unit/test_sigs.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/.gitignore` & `cpop-32.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/README.rst` & `cpop-32.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `cpop-32.0.2/pyproject.toml` & `cpop-32.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-cython"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cpop"
-version = "32.0.2"
+version = "32.0.3"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch45@gmail.com"},
 ]
 classifiers = [
```

### Comparing `cpop-32.0.2/PKG-INFO` & `cpop-32.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 32.0.2
+Version: 32.0.3
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch45@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


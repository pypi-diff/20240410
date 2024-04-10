# Comparing `tmp/in_toto-2.2.0.tar.gz` & `tmp/in_toto-2.3.0.tar.gz`

## Comparing `in_toto-2.2.0.tar` & `in_toto-2.3.0.tar`

### file list

```diff
@@ -1,134 +1,134 @@
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 in_toto-2.2.0/.coveragerc
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 in_toto-2.2.0/requirements-build.txt
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 in_toto-2.2.0/requirements-dev.txt
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 in_toto-2.2.0/requirements-docs.txt
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 in_toto-2.2.0/requirements-lint.txt
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 in_toto-2.2.0/requirements-pinned.txt
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 in_toto-2.2.0/requirements-test.txt
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 in_toto-2.2.0/requirements.txt
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 in_toto-2.2.0/tox.ini
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/__init__.py
--rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/common_args.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/exceptions.py
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/formats.py
--rwxr-xr-x   0        0        0     2594 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/in_toto_match_products.py
--rwxr-xr-x   0        0        0     3843 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/in_toto_mock.py
--rw-r--r--   0        0        0    10192 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/in_toto_record.py
--rwxr-xr-x   0        0        0    10440 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/in_toto_run.py
--rw-r--r--   0        0        0    13185 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/in_toto_sign.py
--rwxr-xr-x   0        0        0     9203 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/in_toto_verify.py
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/log.py
--rw-r--r--   0        0        0    10775 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/rulelib.py
--rw-r--r--   0        0        0    40377 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/runlib.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/settings.py
--rw-r--r--   0        0        0    55831 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/verifylib.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/models/__init__.py
--rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/models/_signer.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/models/common.py
--rw-r--r--   0        0        0    23587 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/models/layout.py
--rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/models/link.py
--rw-r--r--   0        0        0    14687 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/models/metadata.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/resolver/__init__.py
--rw-r--r--   0        0        0    12090 2020-02-02 00:00:00.000000 in_toto-2.2.0/in_toto/resolver/_resolver.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/__init__.py
--rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/common.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/runtests.py
--rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/test_common_args.py
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/test_directory_resolver.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/test_in_toto_match_products.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/test_in_toto_mock.py
--rw-r--r--   0        0        0    19098 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/test_in_toto_record.py
--rwxr-xr-x   0        0        0    19109 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/test_in_toto_run.py
--rw-r--r--   0        0        0    15648 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/test_in_toto_sign.py
--rwxr-xr-x   0        0        0    19690 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/test_in_toto_verify.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/test_log.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/test_ostree_resolver.py
--rw-r--r--   0        0        0     7922 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/test_param_substitution.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/test_resolver.py
--rw-r--r--   0        0        0    13445 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/test_rulelib.py
--rwxr-xr-x   0        0        0    52785 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/test_runlib.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/test_settings.py
--rw-r--r--   0        0        0    69106 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/test_verifylib.py
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/demo_dsse_files/demo.layout.template
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/demo_dsse_files/package.2f89b927.link
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/demo_dsse_files/write-code.776a00e2.link
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/demo_files/alice
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/demo_files/alice.pub
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/demo_files/bob
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/demo_files/bob.pub
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/demo_files/carl
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/demo_files/carl.pub
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/demo_files/danny
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/demo_files/danny.pub
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/demo_files/demo.layout.template
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/demo_files/foo.tar.gz
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/demo_files/package.2f89b927.link
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/demo_files/write-code.776a00e2.link
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/demo_files_gpg/demo.layout.template
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/demo_files_gpg/foo.tar.gz
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/demo_files_gpg/package.7b3abb26.link
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/demo_files_gpg/write-code.8288ef56.link
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/gpg_keyrings/dsa/pubring.gpg
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/gpg_keyrings/dsa/random_seed
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/gpg_keyrings/dsa/secring.gpg
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/gpg_keyrings/dsa/trustdb.gpg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/gpg_keyrings/rsa/7B3ABB26B97B655AB9296BD15B0BD02E1C768C43.ssh
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/gpg_keyrings/rsa/8288EF560ED3795F9DF2C0DB56193089B285DA58.ssh
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/gpg_keyrings/rsa/8465A1E2E0FB2B40ADB2478E18FB3F537E0C8A17.ssh
--rw-r--r--   0        0        0    17740 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/gpg_keyrings/rsa/pubring.gpg
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/gpg_keyrings/rsa/random_seed
--rw-r--r--   0        0        0    27893 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/gpg_keyrings/rsa/secring.gpg
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/gpg_keyrings/rsa/trustdb.gpg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/models/__init__.py
--rwxr-xr-x   0        0        0      714 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/models/test_common.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/models/test_envelope.py
--rwxr-xr-x   0        0        0     1967 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/models/test_inspection.py
--rwxr-xr-x   0        0        0    14784 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/models/test_layout.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/models/test_link.py
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/models/test_metadata.py
--rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/models/test_signer.py
--rwxr-xr-x   0        0        0     2864 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/models/test_step.py
--rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/models/test_supply_chain_item.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/pems/ecdsa_private_encrypted.pem
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/pems/ecdsa_private_unencrypted.pem
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/pems/ecdsa_public.pem
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/pems/ed25519_private_encrypted.pem
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/pems/ed25519_private_unencrypted.pem
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/pems/ed25519_public.pem
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/pems/rsa_private_encrypted.pem
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/pems/rsa_private_unencrypted.pem
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/pems/rsa_public.pem
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/rc_test/.in_totorc
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/colliding_dir_resolver/subdir/0.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/dir_resolver/README.md
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/dir_resolver/subdir/0.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/dir_resolver/subdir/1.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/dir_resolver/subdir/Y.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/dir_resolver/subdir/Z.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/dir_resolver/subdir/a.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/dir_resolver/subdir/b.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/ostree_repo/config
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/ostree_repo/objects/04/d3e76d327333f3a5fcfb2fd067b90cc36a906d23db28adb3819e02e99f0f6a.dirtree
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/ostree_repo/objects/17/57d5e638ba33b5b43bee22ad24f8eecd14487965c076225664e64787a772c4.file
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/ostree_repo/objects/46/33304404a9fb8b9c98145aa85851d285b491e3b77e9cef663392857c4b1000.file
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/ostree_repo/objects/57/3c8b6ed22f77d085206364b0fca4334ab88c429a4e3d335f9b863ca421adc6.dirtree
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/ostree_repo/objects/6d/f05c195832bd23b044a3fdd76b3a30011c762dea6c271133cb20f7309abcb5.dirtree
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/ostree_repo/objects/6e/340b9cffb37a989ca544e6bb780a2c78901d3fb33738768511a30617afa01d.dirtree
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/ostree_repo/objects/77/3e0833bada391e17908ef72be2f3bab9662b6223b5cd6064af8ce7753368d1.dirtree
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/ostree_repo/objects/85/b69cc1ae509c55992d4eb47572cebb0fcfdf640aa2cdc0ad4b517cb6cf8b5d.dirtree
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/ostree_repo/objects/a6/1f97fffc19dbe77a59de47641b16a03a6a835cbe3d7f8a86f4fbb85342b551.file
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/ostree_repo/objects/cd/1875c7cb1d1c169f4ae48baee61c00d1be51efe0f0c2777759644e3a62012f.dirmeta
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/ostree_repo/objects/cf/3e103a6aed64aec261e2161d1026aa26349d422d238b1ad9e2e2a7eeed8591.commit
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/ostree_repo/objects/e3/777ae4075244944a952fa9705d5b26fa24cf5a841e7ce278f390ee3fc1928b.dirtree
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/ostree_repo/objects/f3/43cfdc0f6c428bdb30fc0dbf6c230972564153579b68e5fe5261444cf65abe.file
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/ostree_repo/objects/f7/d5cf77d40b20cbf35b0de40a6bc693d13afeac5c1e07b63f71754e0d6704a2.dirtree
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/resolver/ostree_repo/refs/heads/test-branch
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/scripts/expr
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/scripts/tar
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 in_toto-2.2.0/tests/scripts/touch
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 in_toto-2.2.0/.gitignore
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 in_toto-2.2.0/LICENSE
--rw-r--r--   0        0        0    10242 2020-02-02 00:00:00.000000 in_toto-2.2.0/README.md
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 in_toto-2.2.0/pyproject.toml
--rw-r--r--   0        0        0    11777 2020-02-02 00:00:00.000000 in_toto-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 in_toto-2.3.0/.coveragerc
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 in_toto-2.3.0/requirements-build.txt
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 in_toto-2.3.0/requirements-dev.txt
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 in_toto-2.3.0/requirements-docs.txt
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 in_toto-2.3.0/requirements-lint.txt
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 in_toto-2.3.0/requirements-pinned.txt
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 in_toto-2.3.0/requirements-test.txt
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 in_toto-2.3.0/requirements.txt
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 in_toto-2.3.0/tox.ini
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/__init__.py
+-rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/common_args.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/exceptions.py
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/formats.py
+-rwxr-xr-x   0        0        0     2594 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/in_toto_match_products.py
+-rwxr-xr-x   0        0        0     3843 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/in_toto_mock.py
+-rw-r--r--   0        0        0    10192 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/in_toto_record.py
+-rwxr-xr-x   0        0        0    10440 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/in_toto_run.py
+-rw-r--r--   0        0        0    13185 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/in_toto_sign.py
+-rwxr-xr-x   0        0        0     9784 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/in_toto_verify.py
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/log.py
+-rw-r--r--   0        0        0    10775 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/rulelib.py
+-rw-r--r--   0        0        0    40377 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/runlib.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/settings.py
+-rw-r--r--   0        0        0    56646 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/verifylib.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/models/__init__.py
+-rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/models/_signer.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/models/common.py
+-rw-r--r--   0        0        0    23587 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/models/layout.py
+-rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/models/link.py
+-rw-r--r--   0        0        0    14687 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/models/metadata.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/resolver/__init__.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/resolver/_resolver.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/common.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/runtests.py
+-rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_common_args.py
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_directory_resolver.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_in_toto_match_products.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_in_toto_mock.py
+-rw-r--r--   0        0        0    19098 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_in_toto_record.py
+-rwxr-xr-x   0        0        0    19109 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_in_toto_run.py
+-rw-r--r--   0        0        0    15648 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_in_toto_sign.py
+-rwxr-xr-x   0        0        0    19690 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_in_toto_verify.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_log.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_ostree_resolver.py
+-rw-r--r--   0        0        0     7922 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_param_substitution.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_resolver.py
+-rw-r--r--   0        0        0    13445 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_rulelib.py
+-rwxr-xr-x   0        0        0    52785 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_runlib.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_settings.py
+-rw-r--r--   0        0        0    69111 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_verifylib.py
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_dsse_files/demo.layout.template
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_dsse_files/package.2f89b927.link
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_dsse_files/write-code.776a00e2.link
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/alice
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/alice.pub
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/bob
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/bob.pub
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/carl
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/carl.pub
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/danny
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/danny.pub
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/demo.layout.template
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/foo.tar.gz
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/package.2f89b927.link
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/write-code.776a00e2.link
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files_gpg/demo.layout.template
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files_gpg/foo.tar.gz
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files_gpg/package.7b3abb26.link
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files_gpg/write-code.8288ef56.link
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/dsa/pubring.gpg
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/dsa/random_seed
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/dsa/secring.gpg
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/dsa/trustdb.gpg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/rsa/7B3ABB26B97B655AB9296BD15B0BD02E1C768C43.ssh
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/rsa/8288EF560ED3795F9DF2C0DB56193089B285DA58.ssh
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/rsa/8465A1E2E0FB2B40ADB2478E18FB3F537E0C8A17.ssh
+-rw-r--r--   0        0        0    17740 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/rsa/pubring.gpg
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/rsa/random_seed
+-rw-r--r--   0        0        0    27893 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/rsa/secring.gpg
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/rsa/trustdb.gpg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/models/__init__.py
+-rwxr-xr-x   0        0        0      714 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/models/test_common.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/models/test_envelope.py
+-rwxr-xr-x   0        0        0     1967 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/models/test_inspection.py
+-rwxr-xr-x   0        0        0    14784 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/models/test_layout.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/models/test_link.py
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/models/test_metadata.py
+-rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/models/test_signer.py
+-rwxr-xr-x   0        0        0     2864 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/models/test_step.py
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/models/test_supply_chain_item.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/pems/ecdsa_private_encrypted.pem
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/pems/ecdsa_private_unencrypted.pem
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/pems/ecdsa_public.pem
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/pems/ed25519_private_encrypted.pem
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/pems/ed25519_private_unencrypted.pem
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/pems/ed25519_public.pem
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/pems/rsa_private_encrypted.pem
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/pems/rsa_private_unencrypted.pem
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/pems/rsa_public.pem
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/rc_test/.in_totorc
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/colliding_dir_resolver/subdir/0.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/dir_resolver/README.md
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/dir_resolver/subdir/0.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/dir_resolver/subdir/1.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/dir_resolver/subdir/Y.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/dir_resolver/subdir/Z.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/dir_resolver/subdir/a.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/dir_resolver/subdir/b.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/config
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/04/d3e76d327333f3a5fcfb2fd067b90cc36a906d23db28adb3819e02e99f0f6a.dirtree
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/17/57d5e638ba33b5b43bee22ad24f8eecd14487965c076225664e64787a772c4.file
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/46/33304404a9fb8b9c98145aa85851d285b491e3b77e9cef663392857c4b1000.file
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/57/3c8b6ed22f77d085206364b0fca4334ab88c429a4e3d335f9b863ca421adc6.dirtree
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/6d/f05c195832bd23b044a3fdd76b3a30011c762dea6c271133cb20f7309abcb5.dirtree
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/6e/340b9cffb37a989ca544e6bb780a2c78901d3fb33738768511a30617afa01d.dirtree
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/77/3e0833bada391e17908ef72be2f3bab9662b6223b5cd6064af8ce7753368d1.dirtree
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/85/b69cc1ae509c55992d4eb47572cebb0fcfdf640aa2cdc0ad4b517cb6cf8b5d.dirtree
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/a6/1f97fffc19dbe77a59de47641b16a03a6a835cbe3d7f8a86f4fbb85342b551.file
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/cd/1875c7cb1d1c169f4ae48baee61c00d1be51efe0f0c2777759644e3a62012f.dirmeta
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/cf/3e103a6aed64aec261e2161d1026aa26349d422d238b1ad9e2e2a7eeed8591.commit
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/e3/777ae4075244944a952fa9705d5b26fa24cf5a841e7ce278f390ee3fc1928b.dirtree
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/f3/43cfdc0f6c428bdb30fc0dbf6c230972564153579b68e5fe5261444cf65abe.file
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/f7/d5cf77d40b20cbf35b0de40a6bc693d13afeac5c1e07b63f71754e0d6704a2.dirtree
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/refs/heads/test-branch
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/scripts/expr
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/scripts/tar
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/scripts/touch
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 in_toto-2.3.0/.gitignore
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 in_toto-2.3.0/LICENSE
+-rw-r--r--   0        0        0    10242 2020-02-02 00:00:00.000000 in_toto-2.3.0/README.md
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 in_toto-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0    11777 2020-02-02 00:00:00.000000 in_toto-2.3.0/PKG-INFO
```

### Comparing `in_toto-2.2.0/requirements-pinned.txt` & `in_toto-2.3.0/requirements-pinned.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --output-file=requirements-pinned.txt requirements.txt
 #
-attrs==23.1.0
+attrs==23.2.0
     # via -r requirements.txt
 cffi==1.16.0
     # via
     #   cryptography
     #   pynacl
-cryptography==41.0.7
+cryptography==42.0.5
     # via securesystemslib
 iso8601==2.1.0
     # via -r requirements.txt
 pathspec==0.12.1
     # via -r requirements.txt
-pycparser==2.21
+pycparser==2.22
     # via cffi
 pynacl==1.5.0
     # via securesystemslib
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via -r requirements.txt
 securesystemslib[crypto,pynacl]==0.31.0
     # via -r requirements.txt
 six==1.16.0
     # via python-dateutil
```

### Comparing `in_toto-2.2.0/tox.ini` & `in_toto-2.3.0/tox.ini`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/in_toto/common_args.py` & `in_toto-2.3.0/in_toto/common_args.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/in_toto/exceptions.py` & `in_toto-2.3.0/in_toto/exceptions.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/in_toto/formats.py` & `in_toto-2.3.0/in_toto/formats.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/in_toto/in_toto_match_products.py` & `in_toto-2.3.0/in_toto/in_toto_match_products.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/in_toto/in_toto_mock.py` & `in_toto-2.3.0/in_toto/in_toto_mock.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/in_toto/in_toto_record.py` & `in_toto-2.3.0/in_toto/in_toto_record.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/in_toto/in_toto_run.py` & `in_toto-2.3.0/in_toto/in_toto_run.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/in_toto/in_toto_sign.py` & `in_toto-2.3.0/in_toto/in_toto_sign.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/in_toto/in_toto_verify.py` & `in_toto-2.3.0/in_toto/in_toto_verify.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     VERBOSE_ARGS,
     VERBOSE_KWARGS,
     sort_action_groups,
     title_case_action_groups,
 )
 from in_toto.models._signer import load_public_key_from_file
 from in_toto.models.metadata import Metadata
+from in_toto.settings import LINK_CMD_EXEC_TIMEOUT
 
 # Command line interfaces should use in_toto base logger (c.f. in_toto.log)
 LOG = logging.getLogger("in_toto")
 
 
 def create_parser():
     """Create and return configured ArgumentParser instance."""
@@ -213,14 +214,27 @@
             "path to directory from which link metadata files for steps defined"
             " in the root layout should be loaded. If not passed, links are"
             " loaded from the current working directory."
         ),
     )
 
     parser.add_argument(*GPG_HOME_ARGS, **GPG_HOME_KWARGS)
+    parser.add_argument(
+        "--inspection-timeout",
+        dest="inspect_timeout",
+        type=int,
+        default=LINK_CMD_EXEC_TIMEOUT,
+        help=(
+            "integer that represents the max timeout in seconds for the "
+            "   in-toto-verify command for inspect subprocess."
+            "   Default is '{timeout}' seconds.".format(
+                timeout=LINK_CMD_EXEC_TIMEOUT
+            )
+        ),
+    )
 
     verbosity_args = parser.add_mutually_exclusive_group(required=False)
     verbosity_args.add_argument(*VERBOSE_ARGS, **VERBOSE_KWARGS)
     verbosity_args.add_argument(*QUIET_ARGS, **QUIET_KWARGS)
 
     parser.add_argument(
         "--version",
@@ -275,15 +289,20 @@
             )
 
         if args.verification_keys:
             for path in args.verification_keys:
                 key = load_public_key_from_file(path)
                 layout_key_dict[key["keyid"]] = key
 
-        verifylib.in_toto_verify(layout, layout_key_dict, args.link_dir)
+        verifylib.in_toto_verify(
+            layout,
+            layout_key_dict,
+            args.link_dir,
+            inspect_timeout=args.inspect_timeout,
+        )
 
     except Exception as e:  # pylint: disable=broad-exception-caught
         LOG.error("(in-toto-verify) %s: %s", type(e).__name__, e)
         sys.exit(1)
 
     sys.exit(0)
```

### Comparing `in_toto-2.2.0/in_toto/log.py` & `in_toto-2.3.0/in_toto/log.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/in_toto/rulelib.py` & `in_toto-2.3.0/in_toto/rulelib.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/in_toto/runlib.py` & `in_toto-2.3.0/in_toto/runlib.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/in_toto/settings.py` & `in_toto-2.3.0/in_toto/settings.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/in_toto/verifylib.py` & `in_toto-2.3.0/in_toto/verifylib.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,19 @@
             )
 
         steps_metadata[step.name] = links_per_step
 
     return steps_metadata
 
 
-def run_all_inspections(layout, persist_inspection_links):
+def run_all_inspections(
+    layout,
+    persist_inspection_links,
+    timeout=in_toto.settings.LINK_CMD_EXEC_TIMEOUT,
+):
     """
     <Purpose>
       Extracts all inspections from a passed Layout's inspect field and
       iteratively runs each command defined in the Inspection's `run` field using
       `runlib.in_toto_run`, which returns a Link object.
 
       If a link command returns non-zero the verification is aborted.
@@ -190,14 +194,18 @@
       layout:
               A Layout object which is used to extract the Inspections.
 
       persist_inspection_links:
               A boolean indicating whether link metadata files for inspection
               are written to cwd.
 
+      timeout:
+              Integer that is the amount of seconds that the inspection run will
+              fail after.
+
     <Exceptions>
       Calls function that raises BadReturnValueError if an inspection returned
       non-int or non-zero.
 
     <Returns>
       A dictionary of metadata about the executed inspections, e.g.:
 
@@ -220,15 +228,19 @@
 
         # FIXME: What should we record as material/product?
         # Is the current directory a sensible default? In general?
         # If so, we should probably make it a default in run_link
         # We could use artifact rule paths.
         material_list = product_list = ["."]
         link = in_toto.runlib.in_toto_run(
-            inspection.name, material_list, product_list, inspection.run
+            inspection.name,
+            material_list,
+            product_list,
+            inspection.run,
+            timeout=timeout,
         )
 
         _raise_on_bad_retval(
             link.signed.byproducts.get("return-value"), inspection.run
         )
 
         inspection_links_dict[inspection.name] = link.signed
@@ -1325,15 +1337,17 @@
         # take one exemplary link (e.g. the first in the step_link_dict)
         # form the reduced_chain_link_dict to return
         reduced_chain_link_dict[step_name] = list(key_link_dict.values())[0]
 
     return reduced_chain_link_dict
 
 
-def verify_sublayouts(layout, steps_metadata, superlayout_link_dir_path):
+def verify_sublayouts(
+    layout, steps_metadata, superlayout_link_dir_path, inspect_timeout
+):
     """
     <Purpose>
       Extracts link or layout object for each step in steps_metadata. Checks if
       any step has been delegated by the functionary, recurses into the
       delegation, and replaces the layout object with an equivalent link object.
       Returns the extracted link objects in a dict called chain_link_dict.
 
@@ -1354,14 +1368,18 @@
 
       superlayout_link_dir_path:
               A path to a directory, where links of the superlayout are loaded
               from. Links of the sublayout are expected to be in a subdirectory
               relative to this path, with a name in the format
               in_toto.models.layout.SUBLAYOUT_LINK_DIR_FORMAT.
 
+      inspect_timeout:
+              Integer value that is the number of seconds to pass to the run
+              command to timeout the subprocess within.
+
     <Exceptions>
       raises an Exception if verification of the delegated step fails.
 
     <Side Effects>
       None.
 
     <Returns>
@@ -1408,14 +1426,15 @@
                 # Make a recursive call to in_toto_verify with the
                 # layout and the extracted key object
                 summary_link = in_toto_verify(
                     metadata,
                     layout_key_dict,
                     link_dir_path=sublayout_link_dir_path,
                     step_name=step_name,
+                    inspect_timeout=inspect_timeout,
                 )
 
                 # Replace the layout object with the link object returned
                 # by in-toto-verify
                 payload = summary_link
 
             key_link_dict[keyid] = payload
@@ -1483,14 +1502,15 @@
 def in_toto_verify(
     metadata,
     layout_key_dict,
     link_dir_path=".",
     substitution_parameters=None,
     step_name="",
     persist_inspection_links=True,
+    inspect_timeout=in_toto.settings.LINK_CMD_EXEC_TIMEOUT,
 ):
     """Performs complete in-toto supply chain verification for a final product.
 
     The verification procedure consists of the following activities, performed in
     the given order:
 
     1.  Verify layout signatures
@@ -1537,14 +1557,18 @@
 
       step_name (optional): A name assigned to the returned link. This is mostly
           useful during recursive sublayout verification.
 
       persist_inspection_links (optional): A boolean that determines whether or
           not link metadata files for inspection are written to cwd.
 
+      inspect_timeout (optional): An integer value that defaults to
+          in_toto.settings.LINK_CMD_EXEC_TIMEOUT in seconds which ends up timing
+          out the run command subprocess if it runs over.
+
     Raises:
       securesystemslib.exceptions.FormatError: Passed parameters are malformed.
 
       SignatureVerificationError: No layout verification key is passed, or any of
           the passed keys fails to verify a signature.
 
       LayoutExpiredError: The layout is expired.
@@ -1594,15 +1618,17 @@
     LOG.info("Reading link metadata files...")
     steps_metadata = load_links_for_layout(layout, link_dir_path)
 
     LOG.info("Verifying link metadata signatures...")
     steps_metadata = verify_link_signature_thresholds(layout, steps_metadata)
 
     LOG.info("Verifying sublayouts...")
-    chain_link_dict = verify_sublayouts(layout, steps_metadata, link_dir_path)
+    chain_link_dict = verify_sublayouts(
+        layout, steps_metadata, link_dir_path, inspect_timeout
+    )
 
     LOG.info("Verifying alignment of reported commands...")
     verify_all_steps_command_alignment(layout, chain_link_dict)
 
     LOG.info("Verifying threshold constraints...")
     verify_threshold_constraints(layout, chain_link_dict)
     reduced_chain_link_dict = reduce_chain_links(chain_link_dict)
@@ -1610,15 +1636,17 @@
     # NOTE: Processing step rules before executing inspections guarantees that
     # inspection commands don't run on compromised target files, however, this
     # also precludes step match rules from referencing inspection artifacts.
     LOG.info("Verifying Step rules...")
     verify_all_item_rules(layout.steps, reduced_chain_link_dict)
 
     LOG.info("Executing Inspection commands...")
-    inspection_link_dict = run_all_inspections(layout, persist_inspection_links)
+    inspection_link_dict = run_all_inspections(
+        layout, persist_inspection_links, inspect_timeout
+    )
 
     LOG.info("Verifying Inspection rules...")
     # Artifact rules for inspections can reference links that correspond to
     # Steps or Inspections, hence the concatenation of both collections of links
     combined_links = reduced_chain_link_dict.copy()
     combined_links.update(inspection_link_dict)
     verify_all_item_rules(layout.inspect, combined_links)
```

### Comparing `in_toto-2.2.0/in_toto/models/_signer.py` & `in_toto-2.3.0/in_toto/models/_signer.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/in_toto/models/common.py` & `in_toto-2.3.0/in_toto/models/common.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/in_toto/models/layout.py` & `in_toto-2.3.0/in_toto/models/layout.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/in_toto/models/link.py` & `in_toto-2.3.0/in_toto/models/link.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/in_toto/models/metadata.py` & `in_toto-2.3.0/in_toto/models/metadata.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/in_toto/resolver/__init__.py` & `in_toto-2.3.0/in_toto/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/in_toto/resolver/_resolver.py` & `in_toto-2.3.0/in_toto/resolver/_resolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Resolver interface and implementations for files, OSTree, and directory
 artifacts."""
+
 import locale
 import logging
 import os
 from abc import ABCMeta, abstractmethod
 from functools import cmp_to_key
 from itertools import combinations
 from os.path import exists, isdir, isfile, join, normpath
```

### Comparing `in_toto-2.2.0/tests/__init__.py` & `in_toto-2.3.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/common.py` & `in_toto-2.3.0/tests/common.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/runtests.py` & `in_toto-2.3.0/tests/runtests.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/test_common_args.py` & `in_toto-2.3.0/tests/test_common_args.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/test_directory_resolver.py` & `in_toto-2.3.0/tests/test_directory_resolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test cases for DirectoryResolver."""
+
 #!/usr/bin/env python
 # coding=utf-8
 
 # Copyright New York University and the in-toto contributors
 # SPDX-License-Identifier: Apache-2.0
```

### Comparing `in_toto-2.2.0/tests/test_in_toto_match_products.py` & `in_toto-2.3.0/tests/test_in_toto_match_products.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/test_in_toto_mock.py` & `in_toto-2.3.0/tests/test_in_toto_mock.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/test_in_toto_record.py` & `in_toto-2.3.0/tests/test_in_toto_record.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/test_in_toto_run.py` & `in_toto-2.3.0/tests/test_in_toto_run.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/test_in_toto_sign.py` & `in_toto-2.3.0/tests/test_in_toto_sign.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/test_in_toto_verify.py` & `in_toto-2.3.0/tests/test_in_toto_verify.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/test_log.py` & `in_toto-2.3.0/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/test_ostree_resolver.py` & `in_toto-2.3.0/tests/test_ostree_resolver.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/test_param_substitution.py` & `in_toto-2.3.0/tests/test_param_substitution.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/test_resolver.py` & `in_toto-2.3.0/tests/test_resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test cases for resolver.py."""
+
 from pathlib import Path
 from unittest import TestCase, main
 
 from in_toto.resolver import RESOLVER_FOR_URI_SCHEME, FileResolver, Resolver
 from tests.common import TmpDirMixin
```

### Comparing `in_toto-2.2.0/tests/test_rulelib.py` & `in_toto-2.3.0/tests/test_rulelib.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/test_runlib.py` & `in_toto-2.3.0/tests/test_runlib.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/test_settings.py` & `in_toto-2.3.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/test_verifylib.py` & `in_toto-2.3.0/tests/test_verifylib.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,15 +430,15 @@
         test_cases = [
             # Foo required, pass
             ["foo", {"foo"}, False],
             # Foo is required, but only bar there, blow up
             ["foo", {"bar"}, True],
             # A pattern is passed, which should be interpreted *literally*
             ["*", {"*"}, False],
-            ["*", {"foo"}, True]
+            ["*", {"foo"}, True],
             #
         ]
 
         for i, test_data in enumerate(test_cases):
             pattern, queue, should_raise = test_data
 
             msg = "test {}: {}".format(i, dict(zip(test_data_keys, test_data)))
@@ -1574,15 +1574,15 @@
 
     @classmethod
     def tearDownClass(cls):
         cls.tear_down_test_dir()
 
     def test_verify_demo_as_sublayout(self):
         """Test super layout's passing sublayout verification."""
-        verify_sublayouts(self.super_layout, self.super_layout_links, ".")
+        verify_sublayouts(self.super_layout, self.super_layout_links, ".", 10)
 
 
 class TestInTotoVerifyMultiLevelSublayouts(unittest.TestCase, TmpDirMixin):
     """Test verifylib.in_toto_verify with multiple levels of sublayouts."""
 
     def test_verify_multi_level_sublayout(self):
         # Create and change into temporary directory
```

### Comparing `in_toto-2.2.0/tests/demo_dsse_files/demo.layout.template` & `in_toto-2.3.0/tests/demo_dsse_files/demo.layout.template`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/demo_dsse_files/package.2f89b927.link` & `in_toto-2.3.0/tests/demo_dsse_files/package.2f89b927.link`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/demo_dsse_files/write-code.776a00e2.link` & `in_toto-2.3.0/tests/demo_dsse_files/write-code.776a00e2.link`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/demo_files/alice` & `in_toto-2.3.0/tests/demo_files/alice`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/demo_files/alice.pub` & `in_toto-2.3.0/tests/demo_files/alice.pub`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/demo_files/bob` & `in_toto-2.3.0/tests/demo_files/bob`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/demo_files/bob.pub` & `in_toto-2.3.0/tests/demo_files/bob.pub`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/demo_files/carl` & `in_toto-2.3.0/tests/demo_files/carl`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/demo_files/carl.pub` & `in_toto-2.3.0/tests/demo_files/carl.pub`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/demo_files/demo.layout.template` & `in_toto-2.3.0/tests/demo_files/demo.layout.template`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/demo_files/package.2f89b927.link` & `in_toto-2.3.0/tests/demo_files/package.2f89b927.link`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/demo_files/write-code.776a00e2.link` & `in_toto-2.3.0/tests/demo_files/write-code.776a00e2.link`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/demo_files_gpg/demo.layout.template` & `in_toto-2.3.0/tests/demo_files_gpg/demo.layout.template`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/demo_files_gpg/package.7b3abb26.link` & `in_toto-2.3.0/tests/demo_files_gpg/package.7b3abb26.link`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/demo_files_gpg/write-code.8288ef56.link` & `in_toto-2.3.0/tests/demo_files_gpg/write-code.8288ef56.link`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh` & `in_toto-2.3.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/gpg_keyrings/dsa/pubring.gpg` & `in_toto-2.3.0/tests/gpg_keyrings/dsa/pubring.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/gpg_keyrings/dsa/random_seed` & `in_toto-2.3.0/tests/gpg_keyrings/dsa/random_seed`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/gpg_keyrings/dsa/secring.gpg` & `in_toto-2.3.0/tests/gpg_keyrings/dsa/secring.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/gpg_keyrings/dsa/trustdb.gpg` & `in_toto-2.3.0/tests/gpg_keyrings/dsa/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/gpg_keyrings/rsa/pubring.gpg` & `in_toto-2.3.0/tests/gpg_keyrings/rsa/pubring.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/gpg_keyrings/rsa/random_seed` & `in_toto-2.3.0/tests/gpg_keyrings/rsa/random_seed`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/gpg_keyrings/rsa/secring.gpg` & `in_toto-2.3.0/tests/gpg_keyrings/rsa/secring.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/gpg_keyrings/rsa/trustdb.gpg` & `in_toto-2.3.0/tests/gpg_keyrings/rsa/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/models/test_common.py` & `in_toto-2.3.0/tests/models/test_common.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/models/test_envelope.py` & `in_toto-2.3.0/tests/models/test_envelope.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/models/test_inspection.py` & `in_toto-2.3.0/tests/models/test_inspection.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/models/test_layout.py` & `in_toto-2.3.0/tests/models/test_layout.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/models/test_link.py` & `in_toto-2.3.0/tests/models/test_link.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/models/test_metadata.py` & `in_toto-2.3.0/tests/models/test_metadata.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/models/test_signer.py` & `in_toto-2.3.0/tests/models/test_signer.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/models/test_step.py` & `in_toto-2.3.0/tests/models/test_step.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/models/test_supply_chain_item.py` & `in_toto-2.3.0/tests/models/test_supply_chain_item.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/pems/rsa_private_encrypted.pem` & `in_toto-2.3.0/tests/pems/rsa_private_encrypted.pem`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/pems/rsa_private_unencrypted.pem` & `in_toto-2.3.0/tests/pems/rsa_private_unencrypted.pem`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/scripts/expr` & `in_toto-2.3.0/tests/scripts/expr`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/scripts/tar` & `in_toto-2.3.0/tests/scripts/tar`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/tests/scripts/touch` & `in_toto-2.3.0/tests/scripts/touch`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/.gitignore` & `in_toto-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/LICENSE` & `in_toto-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/README.md` & `in_toto-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `in_toto-2.2.0/pyproject.toml` & `in_toto-2.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "Topic :: Software Development",
 ]
 dependencies = [
     "attrs",
     "iso8601",
     "pathspec",
     "python-dateutil",
-    "securesystemslib[crypto]>=0.31.0",
+    "securesystemslib[crypto]~=0.31.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 # Install pynacl as optional dependency to use with securesystemslib, as a
 # workaround for `"ssl-pynacl": ["securesystemslib[pynacl]>=0.11.3"]`,
 # which currently is not supported in "extra_require" (see pypa/pip#4957).
```

### Comparing `in_toto-2.2.0/PKG-INFO` & `in_toto-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: in-toto
-Version: 2.2.0
+Version: 2.3.0
 Summary: A framework to define and secure the integrity of software supply chains
 Project-URL: Bug Reports, https://github.com/in-toto/in-toto/issues
 Project-URL: Homepage, https://in-toto.io
 Project-URL: Source, https://github.com/in-toto/in-toto
 Author-email: "New York University: Secure Systems Lab" <in-toto-dev@googlegroups.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -26,15 +26,15 @@
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development
 Requires-Python: ~=3.8
 Requires-Dist: attrs
 Requires-Dist: iso8601
 Requires-Dist: pathspec
 Requires-Dist: python-dateutil
-Requires-Dist: securesystemslib[crypto]>=0.31.0
+Requires-Dist: securesystemslib[crypto]~=0.31.0
 Provides-Extra: pynacl
 Requires-Dist: pynacl>1.2.0; extra == 'pynacl'
 Description-Content-Type: text/markdown
 
 # in-toto ![Build](https://github.com/in-toto/in-toto/workflows/Run%20in-toto%20tests%20and%20linter/badge.svg) [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/1523/badge)](https://bestpractices.coreinfrastructure.org/projects/1523) [![Documentation Status](https://readthedocs.org/projects/in-toto/badge/?version=latest)](https://in-toto.readthedocs.io/en/latest/?badge=latest)
 
 in-toto provides a framework to protect the integrity of the software supply chain. It does so by verifying that each task in the chain is carried out as planned, by authorized personnel only, and that the product is not tampered with in transit.
```


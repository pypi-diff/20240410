# Comparing `tmp/dipdup-7.5.3.tar.gz` & `tmp/dipdup-7.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dipdup-7.5.3.tar", last modified: Wed Mar 27 23:47:39 2024, max compression
+gzip compressed data, was "dipdup-7.5.4.tar", last modified: Tue Apr  9 23:15:02 2024, max compression
```

## Comparing `dipdup-7.5.3.tar` & `dipdup-7.5.4.tar`

### file list

```diff
@@ -1,1354 +1,1354 @@
--rw-r--r--   0        0        0     1067 2024-03-27 23:40:26.474306 dipdup-7.5.3/LICENSE
--rw-r--r--   0        0        0     2581 2024-03-27 23:40:26.474306 dipdup-7.5.3/README.md
--rw-r--r--   0        0        0     5101 2024-03-27 23:47:39.573316 dipdup-7.5.3/pyproject.toml
--rw-r--r--   0        0        0      267 2024-03-27 23:40:26.486306 dipdup-7.5.3/src/demo_auction/.dockerignore
--rw-r--r--   0        0        0      363 2024-03-27 23:40:26.486306 dipdup-7.5.3/src/demo_auction/.gitignore
--rw-r--r--   0        0        0       35 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_auction/.ruff_cache/.gitignore
--rw-r--r--   0        0        0      154 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_auction/.ruff_cache/0.3.4/13321372466980456068
--rw-r--r--   0        0        0      269 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_auction/.ruff_cache/0.3.4/14680930435403884952
--rw-r--r--   0        0        0      368 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_auction/.ruff_cache/0.3.4/16683249404466238974
--rw-r--r--   0        0        0      338 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_auction/.ruff_cache/0.3.4/5238306502958837480
--rw-r--r--   0        0        0      291 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_auction/.ruff_cache/0.3.4/8995236205513772283
--rw-r--r--   0        0        0       43 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_auction/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      936 2024-03-27 23:40:26.486306 dipdup-7.5.3/src/demo_auction/Makefile
--rw-r--r--   0        0        0      910 2024-03-27 23:40:26.486306 dipdup-7.5.3/src/demo_auction/README.md
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.486306 dipdup-7.5.3/src/demo_auction/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.486306 dipdup-7.5.3/src/demo_auction/abi/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.486306 dipdup-7.5.3/src/demo_auction/configs/.keep
--rw-r--r--   0        0        0      523 2024-03-27 23:40:26.486306 dipdup-7.5.3/src/demo_auction/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0       73 2024-03-27 23:40:26.486306 dipdup-7.5.3/src/demo_auction/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      548 2024-03-27 23:40:26.486306 dipdup-7.5.3/src/demo_auction/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      559 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/configs/replay.yaml
--rw-r--r--   0        0        0      431 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/deploy/.env.default
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/deploy/.keep
--rw-r--r--   0        0        0      218 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/deploy/Dockerfile
--rw-r--r--   0        0        0      363 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2675 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1261 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/deploy/compose.yaml
--rw-r--r--   0        0        0      242 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/deploy/sqlite.env.default
--rw-r--r--   0        0        0      456 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/deploy/swarm.env.default
--rw-r--r--   0        0        0     1077 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/dipdup.yaml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/graphql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/handlers/.keep
--rw-r--r--   0        0        0      913 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/handlers/on_bid.py
--rw-r--r--   0        0        0     1619 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/handlers/on_create_auction.py
--rw-r--r--   0        0        0      712 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/handlers/on_withdraw.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/hasura/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/hooks/.keep
--rw-r--r--   0        0        0      378 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/models/.keep
--rw-r--r--   0        0        0     1445 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/py.typed
--rw-r--r--   0        0        0     1499 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/sql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/types/.keep
--rw-r--r--   0        0        0      177 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/types/tzcolors_auction/tezos_parameters/bid.py
--rw-r--r--   0        0        0      381 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/types/tzcolors_auction/tezos_parameters/create_auction.py
--rw-r--r--   0        0        0      187 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/types/tzcolors_auction/tezos_parameters/withdraw.py
--rw-r--r--   0        0        0      499 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_auction/types/tzcolors_auction/tezos_storage.py
--rw-r--r--   0        0        0      268 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/.dockerignore
--rw-r--r--   0        0        0      364 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/.gitignore
--rw-r--r--   0        0        0       35 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_big_maps/.ruff_cache/.gitignore
--rw-r--r--   0        0        0      343 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_big_maps/.ruff_cache/0.3.4/18223003769808588768
--rw-r--r--   0        0        0      394 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_big_maps/.ruff_cache/0.3.4/777497163175248698
--rw-r--r--   0        0        0      339 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_big_maps/.ruff_cache/0.3.4/8818109360184037567
--rw-r--r--   0        0        0      219 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_big_maps/.ruff_cache/0.3.4/9845733184017015521
--rw-r--r--   0        0        0       43 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_big_maps/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      937 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/Makefile
--rw-r--r--   0        0        0      911 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/README.md
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/abi/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/configs/.keep
--rw-r--r--   0        0        0      523 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0       74 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      550 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      561 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/configs/replay.yaml
--rw-r--r--   0        0        0      431 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/deploy/.env.default
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/deploy/.keep
--rw-r--r--   0        0        0      220 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/deploy/Dockerfile
--rw-r--r--   0        0        0      365 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2677 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1262 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/deploy/compose.yaml
--rw-r--r--   0        0        0      243 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/deploy/sqlite.env.default
--rw-r--r--   0        0        0      458 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/deploy/swarm.env.default
--rw-r--r--   0        0        0      725 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/dipdup.yaml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/graphql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/handlers/.keep
--rw-r--r--   0        0        0      846 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/handlers/on_update_expiry_map.py
--rw-r--r--   0        0        0     1690 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/handlers/on_update_records.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/hasura/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/hooks/.keep
--rw-r--r--   0        0        0      378 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/models/.keep
--rw-r--r--   0        0        0      667 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/py.typed
--rw-r--r--   0        0        0     1500 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/sql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/types/.keep
--rw-r--r--   0        0        0      199 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/types/name_registry/tezos_big_maps/store_expiry_map_key.py
--rw-r--r--   0        0        0      203 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/types/name_registry/tezos_big_maps/store_expiry_map_value.py
--rw-r--r--   0        0        0      194 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/types/name_registry/tezos_big_maps/store_records_key.py
--rw-r--r--   0        0        0      427 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_big_maps/types/name_registry/tezos_big_maps/store_records_value.py
--rw-r--r--   0        0        0      265 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/.dockerignore
--rw-r--r--   0        0        0      361 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/.gitignore
--rw-r--r--   0        0        0       35 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_blank/.ruff_cache/.gitignore
--rw-r--r--   0        0        0      354 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_blank/.ruff_cache/0.3.4/5560044885556879355
--rw-r--r--   0        0        0      336 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_blank/.ruff_cache/0.3.4/7542205611444200449
--rw-r--r--   0        0        0       43 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_blank/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      934 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/Makefile
--rw-r--r--   0        0        0      912 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/README.md
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/abi/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/configs/.keep
--rw-r--r--   0        0        0      523 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0       71 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      544 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      559 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/configs/replay.yaml
--rw-r--r--   0        0        0      402 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/deploy/.env.default
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/deploy/.keep
--rw-r--r--   0        0        0      214 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/deploy/Dockerfile
--rw-r--r--   0        0        0      359 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2671 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1259 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/deploy/compose.yaml
--rw-r--r--   0        0        0      211 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/deploy/sqlite.env.default
--rw-r--r--   0        0        0      423 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/deploy/swarm.env.default
--rw-r--r--   0        0        0       37 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/dipdup.yaml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/graphql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.490306 dipdup-7.5.3/src/demo_blank/handlers/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_blank/hasura/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_blank/hooks/.keep
--rw-r--r--   0        0        0      378 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_blank/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_blank/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_blank/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_blank/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_blank/models/.keep
--rw-r--r--   0        0        0     1241 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_blank/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_blank/py.typed
--rw-r--r--   0        0        0     1501 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_blank/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_blank/sql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_blank/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_blank/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_blank/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_blank/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_blank/types/.keep
--rw-r--r--   0        0        0      263 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/.dockerignore
--rw-r--r--   0        0        0      359 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/.gitignore
--rw-r--r--   0        0        0       35 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_dao/.ruff_cache/.gitignore
--rw-r--r--   0        0        0      334 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_dao/.ruff_cache/0.3.4/12864778552688321726
--rw-r--r--   0        0        0      153 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_dao/.ruff_cache/0.3.4/2866025793036437098
--rw-r--r--   0        0        0      328 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_dao/.ruff_cache/0.3.4/5039692335175112662
--rw-r--r--   0        0        0      142 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_dao/.ruff_cache/0.3.4/7017744597325188444
--rw-r--r--   0        0        0      201 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_dao/.ruff_cache/0.3.4/8261465866126735821
--rw-r--r--   0        0        0       43 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_dao/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      932 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/Makefile
--rw-r--r--   0        0        0      907 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/README.md
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/abi/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/configs/.keep
--rw-r--r--   0        0        0      523 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0       69 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      540 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      552 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/configs/replay.yaml
--rw-r--r--   0        0        0      431 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/deploy/.env.default
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/deploy/.keep
--rw-r--r--   0        0        0      210 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/deploy/Dockerfile
--rw-r--r--   0        0        0      355 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2667 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1257 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/deploy/compose.yaml
--rw-r--r--   0        0        0      238 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/deploy/sqlite.env.default
--rw-r--r--   0        0        0      448 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/deploy/swarm.env.default
--rw-r--r--   0        0        0      643 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/dipdup.yaml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/graphql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/handlers/.keep
--rw-r--r--   0        0        0      408 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/handlers/on_origination.py
--rw-r--r--   0        0        0      506 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/handlers/on_propose.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/hasura/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/hooks/.keep
--rw-r--r--   0        0        0      378 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/models/.keep
--rw-r--r--   0        0        0      782 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/py.typed
--rw-r--r--   0        0        0     1496 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/sql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/types/.keep
--rw-r--r--   0        0        0      360 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/types/registry/tezos_parameters/propose.py
--rw-r--r--   0        0        0     2475 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dao/types/registry/tezos_storage.py
--rw-r--r--   0        0        0      263 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/.dockerignore
--rw-r--r--   0        0        0      359 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/.gitignore
--rw-r--r--   0        0        0       35 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_dex/.ruff_cache/.gitignore
--rw-r--r--   0        0        0      334 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_dex/.ruff_cache/0.3.4/12720300385992220224
--rw-r--r--   0        0        0      155 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_dex/.ruff_cache/0.3.4/1283190351464374579
--rw-r--r--   0        0        0      144 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_dex/.ruff_cache/0.3.4/13791459030855475338
--rw-r--r--   0        0        0      356 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_dex/.ruff_cache/0.3.4/13835389426450357211
--rw-r--r--   0        0        0      512 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_dex/.ruff_cache/0.3.4/14735723557445667823
--rw-r--r--   0        0        0      156 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_dex/.ruff_cache/0.3.4/16702393409896512014
--rw-r--r--   0        0        0      513 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_dex/.ruff_cache/0.3.4/4129881479918551501
--rw-r--r--   0        0        0     1110 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_dex/.ruff_cache/0.3.4/467002119024090504
--rw-r--r--   0        0        0      144 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_dex/.ruff_cache/0.3.4/8389263870688788824
--rw-r--r--   0        0        0      143 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_dex/.ruff_cache/0.3.4/9806112482546647631
--rw-r--r--   0        0        0      143 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_dex/.ruff_cache/0.3.4/9852384314064524541
--rw-r--r--   0        0        0       43 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_dex/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      932 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/Makefile
--rw-r--r--   0        0        0      918 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/README.md
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/abi/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/configs/.keep
--rw-r--r--   0        0        0      523 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0       69 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      540 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      563 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/configs/replay.yaml
--rw-r--r--   0        0        0      402 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/deploy/.env.default
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/deploy/.keep
--rw-r--r--   0        0        0      210 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/deploy/Dockerfile
--rw-r--r--   0        0        0      355 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2667 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1257 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/deploy/compose.yaml
--rw-r--r--   0        0        0      209 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/deploy/sqlite.env.default
--rw-r--r--   0        0        0      419 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/deploy/swarm.env.default
--rw-r--r--   0        0        0     4845 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/dipdup.yaml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/graphql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/handlers/.keep
--rw-r--r--   0        0        0     1829 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/handlers/on_fa12_divest_liquidity.py
--rw-r--r--   0        0        0     1737 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/handlers/on_fa12_invest_liquidity.py
--rw-r--r--   0        0        0      579 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/handlers/on_fa12_origination.py
--rw-r--r--   0        0        0     1610 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/handlers/on_fa12_tez_to_token.py
--rw-r--r--   0        0        0     1676 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/handlers/on_fa12_token_to_tez.py
--rw-r--r--   0        0        0     1022 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/handlers/on_fa12_transfer.py
--rw-r--r--   0        0        0      931 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/handlers/on_fa12_withdraw_profit.py
--rw-r--r--   0        0        0     1855 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/handlers/on_fa2_divest_liquidity.py
--rw-r--r--   0        0        0     1763 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/handlers/on_fa2_invest_liquidity.py
--rw-r--r--   0        0        0      573 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/handlers/on_fa2_origination.py
--rw-r--r--   0        0        0     1604 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/handlers/on_fa2_tez_to_token.py
--rw-r--r--   0        0        0     1642 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/handlers/on_fa2_token_to_tez.py
--rw-r--r--   0        0        0     1143 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/handlers/on_fa2_transfer.py
--rw-r--r--   0        0        0      927 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/handlers/on_fa2_withdraw_profit.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/hasura/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/hooks/.keep
--rw-r--r--   0        0        0      378 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/models/.keep
--rw-r--r--   0        0        0      916 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/py.typed
--rw-r--r--   0        0        0     1507 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.494306 dipdup-7.5.3/src/demo_dex/sql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/types/.keep
--rw-r--r--   0        0        0      340 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/types/fa12_token/tezos_parameters/transfer.py
--rw-r--r--   0        0        0      714 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/types/fa12_token/tezos_storage.py
--rw-r--r--   0        0        0      479 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/types/fa2_token/tezos_parameters/transfer.py
--rw-r--r--   0        0        0     1045 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/types/fa2_token/tezos_storage.py
--rw-r--r--   0        0        0      311 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/types/quipu_fa12/tezos_parameters/divest_liquidity.py
--rw-r--r--   0        0        0      201 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/types/quipu_fa12/tezos_parameters/invest_liquidity.py
--rw-r--r--   0        0        0      297 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/types/quipu_fa12/tezos_parameters/tez_to_token_payment.py
--rw-r--r--   0        0        0      313 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/types/quipu_fa12/tezos_parameters/token_to_tez_payment.py
--rw-r--r--   0        0        0      340 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/types/quipu_fa12/tezos_parameters/transfer.py
--rw-r--r--   0        0        0      199 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/types/quipu_fa12/tezos_parameters/withdraw_profit.py
--rw-r--r--   0        0        0     1393 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/types/quipu_fa12/tezos_storage.py
--rw-r--r--   0        0        0      311 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/types/quipu_fa2/tezos_parameters/divest_liquidity.py
--rw-r--r--   0        0        0      201 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/types/quipu_fa2/tezos_parameters/invest_liquidity.py
--rw-r--r--   0        0        0      297 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/types/quipu_fa2/tezos_parameters/tez_to_token_payment.py
--rw-r--r--   0        0        0      313 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/types/quipu_fa2/tezos_parameters/token_to_tez_payment.py
--rw-r--r--   0        0        0      479 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/types/quipu_fa2/tezos_parameters/transfer.py
--rw-r--r--   0        0        0      199 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/types/quipu_fa2/tezos_parameters/withdraw_profit.py
--rw-r--r--   0        0        0     1405 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_dex/types/quipu_fa2/tezos_storage.py
--rw-r--r--   0        0        0      267 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/.dockerignore
--rw-r--r--   0        0        0      363 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/.gitignore
--rw-r--r--   0        0        0       35 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_domains/.ruff_cache/.gitignore
--rw-r--r--   0        0        0      340 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_domains/.ruff_cache/0.3.4/11062311691735906861
--rw-r--r--   0        0        0      393 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_domains/.ruff_cache/0.3.4/11633625913283519006
--rw-r--r--   0        0        0      218 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_domains/.ruff_cache/0.3.4/2203309634464738842
--rw-r--r--   0        0        0      408 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_domains/.ruff_cache/0.3.4/8625775505454680759
--rw-r--r--   0        0        0       43 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_domains/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      936 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/Makefile
--rw-r--r--   0        0        0      919 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/README.md
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/abi/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/configs/.keep
--rw-r--r--   0        0        0      523 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0       73 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      548 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      568 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/configs/replay.yaml
--rw-r--r--   0        0        0      431 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/deploy/.env.default
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/deploy/.keep
--rw-r--r--   0        0        0      218 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/deploy/Dockerfile
--rw-r--r--   0        0        0      363 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2675 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1261 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/deploy/compose.yaml
--rw-r--r--   0        0        0      242 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/deploy/sqlite.env.default
--rw-r--r--   0        0        0      456 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/deploy/swarm.env.default
--rw-r--r--   0        0        0      893 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/dipdup.yaml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/graphql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/handlers/.keep
--rw-r--r--   0        0        0     1938 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/handlers/on_update_expiry_map.py
--rw-r--r--   0        0        0     3286 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/handlers/on_update_records.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/hasura/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/hooks/.keep
--rw-r--r--   0        0        0      959 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/hooks/check_expiration.py
--rw-r--r--   0        0        0      378 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/models/.keep
--rw-r--r--   0        0        0      972 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/py.typed
--rw-r--r--   0        0        0     1508 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/sql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/types/.keep
--rw-r--r--   0        0        0      199 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/types/name_registry/tezos_big_maps/store_expiry_map_key.py
--rw-r--r--   0        0        0      203 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/types/name_registry/tezos_big_maps/store_expiry_map_value.py
--rw-r--r--   0        0        0      194 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/types/name_registry/tezos_big_maps/store_records_key.py
--rw-r--r--   0        0        0      427 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_domains/types/name_registry/tezos_big_maps/store_records_value.py
--rw-r--r--   0        0        0      269 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/.dockerignore
--rw-r--r--   0        0        0      365 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/.gitignore
--rw-r--r--   0        0        0       35 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_etherlink/.ruff_cache/.gitignore
--rw-r--r--   0        0        0      366 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_etherlink/.ruff_cache/0.3.4/10092114008825007150
--rw-r--r--   0        0        0      153 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_etherlink/.ruff_cache/0.3.4/10339687797233811857
--rw-r--r--   0        0        0      340 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_etherlink/.ruff_cache/0.3.4/12356644429613338918
--rw-r--r--   0        0        0      157 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_etherlink/.ruff_cache/0.3.4/13962181083648045861
--rw-r--r--   0        0        0      148 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_etherlink/.ruff_cache/0.3.4/18147846495933148634
--rw-r--r--   0        0        0      164 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_etherlink/.ruff_cache/0.3.4/6214507364006453834
--rw-r--r--   0        0        0      221 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_etherlink/.ruff_cache/0.3.4/6582630073886514365
--rw-r--r--   0        0        0      146 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_etherlink/.ruff_cache/0.3.4/8271038388090321411
--rw-r--r--   0        0        0      204 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_etherlink/.ruff_cache/0.3.4/9438807181160902768
--rw-r--r--   0        0        0       43 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_etherlink/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      938 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/Makefile
--rw-r--r--   0        0        0      921 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/README.md
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/abi/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/configs/.keep
--rw-r--r--   0        0        0      523 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0       75 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      552 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      572 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/configs/replay.yaml
--rw-r--r--   0        0        0      442 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/deploy/.env.default
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/deploy/.keep
--rw-r--r--   0        0        0      222 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/deploy/Dockerfile
--rw-r--r--   0        0        0      367 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2679 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1263 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/deploy/compose.yaml
--rw-r--r--   0        0        0      255 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/deploy/sqlite.env.default
--rw-r--r--   0        0        0      471 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/deploy/swarm.env.default
--rw-r--r--   0        0        0     1343 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/dipdup.yaml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/graphql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/handlers/.keep
--rw-r--r--   0        0        0      874 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/handlers/on_deposit.py
--rw-r--r--   0        0        0      583 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/handlers/on_withdraw.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/hasura/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/hooks/.keep
--rw-r--r--   0        0        0      378 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/models/.keep
--rw-r--r--   0        0        0     1241 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/py.typed
--rw-r--r--   0        0        0     1510 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.498306 dipdup-7.5.3/src/demo_etherlink/sql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_etherlink/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_etherlink/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_etherlink/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_etherlink/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_etherlink/types/.keep
--rw-r--r--   0        0        0      894 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_etherlink/types/rollup/tezos_parameters/default.py
--rw-r--r--   0        0        0      189 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_etherlink/types/rollup/tezos_storage.py
--rw-r--r--   0        0        0      398 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_etherlink/types/ticket_helper/tezos_parameters/default.py
--rw-r--r--   0        0        0      744 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_etherlink/types/ticket_helper/tezos_storage.py
--rw-r--r--   0        0        0      185 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_etherlink/types/ticketer/tezos_parameters/deposit.py
--rw-r--r--   0        0        0      512 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_etherlink/types/ticketer/tezos_parameters/withdraw.py
--rw-r--r--   0        0        0      712 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_etherlink/types/ticketer/tezos_storage.py
--rw-r--r--   0        0        0      266 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/.dockerignore
--rw-r--r--   0        0        0      362 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/.gitignore
--rw-r--r--   0        0        0       35 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_events/.ruff_cache/.gitignore
--rw-r--r--   0        0        0      357 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_events/.ruff_cache/0.3.4/14955908790401476896
--rw-r--r--   0        0        0      274 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_events/.ruff_cache/0.3.4/5970380176296333037
--rw-r--r--   0        0        0      337 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_events/.ruff_cache/0.3.4/6057790105724240668
--rw-r--r--   0        0        0      214 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_events/.ruff_cache/0.3.4/6814525569214726022
--rw-r--r--   0        0        0       43 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_events/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      935 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/Makefile
--rw-r--r--   0        0        0      909 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/README.md
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/abi/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/configs/.keep
--rw-r--r--   0        0        0      523 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0       72 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      546 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      557 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/configs/replay.yaml
--rw-r--r--   0        0        0      402 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/deploy/.env.default
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/deploy/.keep
--rw-r--r--   0        0        0      216 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/deploy/Dockerfile
--rw-r--r--   0        0        0      361 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2673 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1260 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/deploy/compose.yaml
--rw-r--r--   0        0        0      212 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/deploy/sqlite.env.default
--rw-r--r--   0        0        0      425 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/deploy/swarm.env.default
--rw-r--r--   0        0        0      534 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/dipdup.yaml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/graphql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/handlers/.keep
--rw-r--r--   0        0        0      311 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/handlers/on_move_event.py
--rw-r--r--   0        0        0      237 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/handlers/on_other_event.py
--rw-r--r--   0        0        0      311 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/handlers/on_roll_event.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/hasura/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/hooks/.keep
--rw-r--r--   0        0        0      378 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/models/.keep
--rw-r--r--   0        0        0     1241 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/py.typed
--rw-r--r--   0        0        0     1498 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/sql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/types/.keep
--rw-r--r--   0        0        0      317 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/types/events_contract/tezos_events/move.py
--rw-r--r--   0        0        0      266 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_events/types/events_contract/tezos_events/roll.py
--rw-r--r--   0        0        0      270 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/.dockerignore
--rw-r--r--   0        0        0      366 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/.gitignore
--rw-r--r--   0        0        0       35 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_evm_events/.ruff_cache/.gitignore
--rw-r--r--   0        0        0      341 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_evm_events/.ruff_cache/0.3.4/10786704751147363155
--rw-r--r--   0        0        0      141 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_evm_events/.ruff_cache/0.3.4/6587051254022175351
--rw-r--r--   0        0        0      355 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_evm_events/.ruff_cache/0.3.4/68027748452251478
--rw-r--r--   0        0        0      155 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_evm_events/.ruff_cache/0.3.4/8734188227036928974
--rw-r--r--   0        0        0       43 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_evm_events/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      939 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/Makefile
--rw-r--r--   0        0        0      927 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/README.md
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/abi/.keep
--rw-r--r--   0        0        0    11460 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/abi/eth_usdt/abi.json
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/configs/.keep
--rw-r--r--   0        0        0      523 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0       76 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      554 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      579 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/configs/replay.yaml
--rw-r--r--   0        0        0      644 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/deploy/.env.default
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/deploy/.keep
--rw-r--r--   0        0        0      224 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/deploy/Dockerfile
--rw-r--r--   0        0        0      369 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2681 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1264 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/deploy/compose.yaml
--rw-r--r--   0        0        0      458 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/deploy/sqlite.env.default
--rw-r--r--   0        0        0      675 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/deploy/swarm.env.default
--rw-r--r--   0        0        0      811 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/dipdup.yaml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/graphql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/handlers/.keep
--rw-r--r--   0        0        0     1291 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/handlers/on_transfer.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/hasura/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/hooks/.keep
--rw-r--r--   0        0        0      378 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/models/.keep
--rw-r--r--   0        0        0      469 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/py.typed
--rw-r--r--   0        0        0     1516 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/sql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.502306 dipdup-7.5.3/src/demo_evm_events/types/.keep
--rw-r--r--   0        0        0      331 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_events/types/eth_usdt/evm_events/transfer.py
--rw-r--r--   0        0        0      276 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/.dockerignore
--rw-r--r--   0        0        0      372 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/.gitignore
--rw-r--r--   0        0        0       35 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_evm_transactions/.ruff_cache/.gitignore
--rw-r--r--   0        0        0      347 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_evm_transactions/.ruff_cache/0.3.4/10331561065334203895
--rw-r--r--   0        0        0      373 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_evm_transactions/.ruff_cache/0.3.4/15674958585356899910
--rw-r--r--   0        0        0      147 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_evm_transactions/.ruff_cache/0.3.4/16247831392390980520
--rw-r--r--   0        0        0      162 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_evm_transactions/.ruff_cache/0.3.4/9790295155389652707
--rw-r--r--   0        0        0       43 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_evm_transactions/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      945 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/Makefile
--rw-r--r--   0        0        0      935 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/README.md
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/abi/.keep
--rw-r--r--   0        0        0    11460 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/abi/eth_usdt/abi.json
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/configs/.keep
--rw-r--r--   0        0        0      523 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0       82 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      566 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      593 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/configs/replay.yaml
--rw-r--r--   0        0        0      644 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/deploy/.env.default
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/deploy/.keep
--rw-r--r--   0        0        0      236 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/deploy/Dockerfile
--rw-r--r--   0        0        0      381 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2693 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1270 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/deploy/compose.yaml
--rw-r--r--   0        0        0      464 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/deploy/sqlite.env.default
--rw-r--r--   0        0        0      687 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/deploy/swarm.env.default
--rw-r--r--   0        0        0      850 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/dipdup.yaml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/graphql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/handlers/.keep
--rw-r--r--   0        0        0     1345 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/handlers/on_transfer.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/hasura/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/hooks/.keep
--rw-r--r--   0        0        0      378 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/models/.keep
--rw-r--r--   0        0        0      469 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/py.typed
--rw-r--r--   0        0        0     1524 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/sql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/types/.keep
--rw-r--r--   0        0        0      262 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_evm_transactions/types/eth_usdt/evm_methods/transfer.py
--rw-r--r--   0        0        0      269 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/.dockerignore
--rw-r--r--   0        0        0      365 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/.gitignore
--rw-r--r--   0        0        0       35 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_factories/.ruff_cache/.gitignore
--rw-r--r--   0        0        0      346 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_factories/.ruff_cache/0.3.4/10307510839735857496
--rw-r--r--   0        0        0      147 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_factories/.ruff_cache/0.3.4/10782288783242833089
--rw-r--r--   0        0        0      340 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_factories/.ruff_cache/0.3.4/17639899329758428436
--rw-r--r--   0        0        0      157 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_factories/.ruff_cache/0.3.4/8246141455296590254
--rw-r--r--   0        0        0      216 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_factories/.ruff_cache/0.3.4/8501597654723000256
--rw-r--r--   0        0        0      145 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_factories/.ruff_cache/0.3.4/9575138874823045403
--rw-r--r--   0        0        0       43 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_factories/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      938 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/Makefile
--rw-r--r--   0        0        0      924 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/README.md
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/abi/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/configs/.keep
--rw-r--r--   0        0        0      523 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0       75 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      552 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      575 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/configs/replay.yaml
--rw-r--r--   0        0        0      431 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/deploy/.env.default
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/deploy/.keep
--rw-r--r--   0        0        0      222 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/deploy/Dockerfile
--rw-r--r--   0        0        0      367 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2679 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1263 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/deploy/compose.yaml
--rw-r--r--   0        0        0      244 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/deploy/sqlite.env.default
--rw-r--r--   0        0        0      460 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/deploy/swarm.env.default
--rw-r--r--   0        0        0     1090 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/dipdup.yaml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/graphql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/handlers/.keep
--rw-r--r--   0        0        0     1082 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/handlers/on_factory_origination.py
--rw-r--r--   0        0        0      658 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/handlers/on_transfer.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/hasura/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/hooks/.keep
--rw-r--r--   0        0        0      378 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/models/.keep
--rw-r--r--   0        0        0      208 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/py.typed
--rw-r--r--   0        0        0     1513 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/sql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/types/.keep
--rw-r--r--   0        0        0     1355 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/types/factory/tezos_storage.py
--rw-r--r--   0        0        0      479 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/types/token/tezos_parameters/transfer.py
--rw-r--r--   0        0        0     1128 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_factories/types/token/tezos_storage.py
--rw-r--r--   0        0        0      264 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_head/.dockerignore
--rw-r--r--   0        0        0      360 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_head/.gitignore
--rw-r--r--   0        0        0       35 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_head/.ruff_cache/.gitignore
--rw-r--r--   0        0        0      139 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_head/.ruff_cache/0.3.4/10069098666661965578
--rw-r--r--   0        0        0      351 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_head/.ruff_cache/0.3.4/16898887970286933302
--rw-r--r--   0        0        0      335 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_head/.ruff_cache/0.3.4/2682715868652859621
--rw-r--r--   0        0        0       43 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_head/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      933 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_head/Makefile
--rw-r--r--   0        0        0      927 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_head/README.md
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_head/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_head/abi/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_head/configs/.keep
--rw-r--r--   0        0        0      523 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_head/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0       70 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_head/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      542 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_head/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      573 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_head/configs/replay.yaml
--rw-r--r--   0        0        0      431 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_head/deploy/.env.default
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_head/deploy/.keep
--rw-r--r--   0        0        0      212 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_head/deploy/Dockerfile
--rw-r--r--   0        0        0      357 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_head/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2669 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_head/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1258 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_head/deploy/compose.yaml
--rw-r--r--   0        0        0      239 2024-03-27 23:40:26.506306 dipdup-7.5.3/src/demo_head/deploy/sqlite.env.default
--rw-r--r--   0        0        0      450 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_head/deploy/swarm.env.default
--rw-r--r--   0        0        0      240 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_head/dipdup.yaml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_head/graphql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_head/handlers/.keep
--rw-r--r--   0        0        0      237 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_head/handlers/on_mainnet_head.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_head/hasura/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_head/hooks/.keep
--rw-r--r--   0        0        0      378 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_head/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_head/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_head/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_head/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_head/models/.keep
--rw-r--r--   0        0        0     1241 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_head/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_head/py.typed
--rw-r--r--   0        0        0     1516 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_head/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_head/sql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_head/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_head/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_head/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_head/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_head/types/.keep
--rw-r--r--   0        0        0      275 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/.dockerignore
--rw-r--r--   0        0        0      371 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/.gitignore
--rw-r--r--   0        0        0       35 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_nft_marketplace/.ruff_cache/.gitignore
--rw-r--r--   0        0        0      354 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_nft_marketplace/.ruff_cache/0.3.4/13540575866931156275
--rw-r--r--   0        0        0      335 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_nft_marketplace/.ruff_cache/0.3.4/16196868449162888949
--rw-r--r--   0        0        0      346 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_nft_marketplace/.ruff_cache/0.3.4/281375156109423751
--rw-r--r--   0        0        0      164 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_nft_marketplace/.ruff_cache/0.3.4/3451910247393675105
--rw-r--r--   0        0        0      156 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_nft_marketplace/.ruff_cache/0.3.4/4196954571566648963
--rw-r--r--   0        0        0      156 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_nft_marketplace/.ruff_cache/0.3.4/5484731337912520482
--rw-r--r--   0        0        0      392 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_nft_marketplace/.ruff_cache/0.3.4/7440941421425896923
--rw-r--r--   0        0        0       43 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_nft_marketplace/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      944 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/Makefile
--rw-r--r--   0        0        0      921 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/README.md
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/abi/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/configs/.keep
--rw-r--r--   0        0        0      523 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0       81 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      564 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      578 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/configs/replay.yaml
--rw-r--r--   0        0        0      527 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/deploy/.env.default
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/deploy/.keep
--rw-r--r--   0        0        0      234 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/deploy/Dockerfile
--rw-r--r--   0        0        0      379 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2691 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1269 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/deploy/compose.yaml
--rw-r--r--   0        0        0      346 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/deploy/sqlite.env.default
--rw-r--r--   0        0        0      568 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/deploy/swarm.env.default
--rw-r--r--   0        0        0     1199 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/dipdup.yaml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/graphql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/handlers/.keep
--rw-r--r--   0        0        0      605 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/handlers/on_cancel_swap.py
--rw-r--r--   0        0        0     1037 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/handlers/on_collect.py
--rw-r--r--   0        0        0      977 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/handlers/on_mint.py
--rw-r--r--   0        0        0      885 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/handlers/on_swap.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/hasura/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/hooks/.keep
--rw-r--r--   0        0        0      378 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/models/.keep
--rw-r--r--   0        0        0     1306 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/py.typed
--rw-r--r--   0        0        0     1510 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/sql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/types/.keep
--rw-r--r--   0        0        0      192 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/cancel_swap.py
--rw-r--r--   0        0        0      281 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/collect.py
--rw-r--r--   0        0        0      317 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/mint_objkt.py
--rw-r--r--   0        0        0      299 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/swap.py
--rw-r--r--   0        0        0      752 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/types/hen_minter/tezos_storage.py
--rw-r--r--   0        0        0      318 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/types/hen_objkts/tezos_parameters/mint.py
--rw-r--r--   0        0        0     1046 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_nft_marketplace/types/hen_objkts/tezos_storage.py
--rw-r--r--   0        0        0      263 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/.dockerignore
--rw-r--r--   0        0        0      359 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/.gitignore
--rw-r--r--   0        0        0       35 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_raw/.ruff_cache/.gitignore
--rw-r--r--   0        0        0      386 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_raw/.ruff_cache/0.3.4/12331798895854021952
--rw-r--r--   0        0        0      135 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_raw/.ruff_cache/0.3.4/14693484283308087925
--rw-r--r--   0        0        0      334 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_raw/.ruff_cache/0.3.4/2166531889291963779
--rw-r--r--   0        0        0       43 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_raw/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      932 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/Makefile
--rw-r--r--   0        0        0      939 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/README.md
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/abi/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/configs/.keep
--rw-r--r--   0        0        0      523 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0       69 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      540 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      584 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/configs/replay.yaml
--rw-r--r--   0        0        0      431 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/deploy/.env.default
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/deploy/.keep
--rw-r--r--   0        0        0      210 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/deploy/Dockerfile
--rw-r--r--   0        0        0      355 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2667 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1257 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/deploy/compose.yaml
--rw-r--r--   0        0        0      238 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/deploy/sqlite.env.default
--rw-r--r--   0        0        0      448 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/deploy/swarm.env.default
--rw-r--r--   0        0        0      411 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/dipdup.yaml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/graphql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/handlers/.keep
--rw-r--r--   0        0        0      350 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/handlers/on_operation.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/hasura/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/hooks/.keep
--rw-r--r--   0        0        0      378 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/models/.keep
--rw-r--r--   0        0        0      245 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/py.typed
--rw-r--r--   0        0        0     1528 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/sql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.510306 dipdup-7.5.3/src/demo_raw/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_raw/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_raw/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_raw/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_raw/types/.keep
--rw-r--r--   0        0        0      265 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/.dockerignore
--rw-r--r--   0        0        0      361 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/.gitignore
--rw-r--r--   0        0        0       35 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_token/.ruff_cache/.gitignore
--rw-r--r--   0        0        0      336 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_token/.ruff_cache/0.3.4/10422505560343211401
--rw-r--r--   0        0        0      268 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_token/.ruff_cache/0.3.4/15231586338726134695
--rw-r--r--   0        0        0      334 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_token/.ruff_cache/0.3.4/15351618443697016585
--rw-r--r--   0        0        0      141 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_token/.ruff_cache/0.3.4/17556758471474737634
--rw-r--r--   0        0        0      211 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_token/.ruff_cache/0.3.4/694067902165491097
--rw-r--r--   0        0        0       43 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_token/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      934 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/Makefile
--rw-r--r--   0        0        0      913 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/README.md
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/abi/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/configs/.keep
--rw-r--r--   0        0        0      523 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0       71 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      544 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      560 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/configs/replay.yaml
--rw-r--r--   0        0        0      402 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/deploy/.env.default
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/deploy/.keep
--rw-r--r--   0        0        0      214 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/deploy/Dockerfile
--rw-r--r--   0        0        0      359 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2671 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1259 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/deploy/compose.yaml
--rw-r--r--   0        0        0      211 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/deploy/sqlite.env.default
--rw-r--r--   0        0        0      423 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/deploy/swarm.env.default
--rw-r--r--   0        0        0      730 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/dipdup.yaml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/graphql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/handlers/.keep
--rw-r--r--   0        0        0      436 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/handlers/on_balance_update.py
--rw-r--r--   0        0        0      630 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/handlers/on_mint.py
--rw-r--r--   0        0        0      928 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/handlers/on_transfer.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/hasura/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/hooks/.keep
--rw-r--r--   0        0        0      378 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/models/.keep
--rw-r--r--   0        0        0      370 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/py.typed
--rw-r--r--   0        0        0     1502 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/sql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/types/.keep
--rw-r--r--   0        0        0      263 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/types/tzbtc/tezos_parameters/mint.py
--rw-r--r--   0        0        0      340 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/types/tzbtc/tezos_parameters/transfer.py
--rw-r--r--   0        0        0      373 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token/types/tzbtc/tezos_storage.py
--rw-r--r--   0        0        0      274 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/.dockerignore
--rw-r--r--   0        0        0      370 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/.gitignore
--rw-r--r--   0        0        0       35 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_token_balances/.ruff_cache/.gitignore
--rw-r--r--   0        0        0      151 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_token_balances/.ruff_cache/0.3.4/535662070015189733
--rw-r--r--   0        0        0      361 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_token_balances/.ruff_cache/0.3.4/6395880071000187438
--rw-r--r--   0        0        0      345 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_token_balances/.ruff_cache/0.3.4/7294843446271708814
--rw-r--r--   0        0        0       43 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_token_balances/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      943 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/Makefile
--rw-r--r--   0        0        0      911 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/README.md
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/abi/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/configs/.keep
--rw-r--r--   0        0        0      523 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0       80 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      562 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      567 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/configs/replay.yaml
--rw-r--r--   0        0        0      402 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/deploy/.env.default
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/deploy/.keep
--rw-r--r--   0        0        0      232 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/deploy/Dockerfile
--rw-r--r--   0        0        0      377 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2689 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1268 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/deploy/compose.yaml
--rw-r--r--   0        0        0      220 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/deploy/sqlite.env.default
--rw-r--r--   0        0        0      441 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/deploy/swarm.env.default
--rw-r--r--   0        0        0      407 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/dipdup.yaml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/graphql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/handlers/.keep
--rw-r--r--   0        0        0      472 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/handlers/on_balance_update.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/hasura/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/hooks/.keep
--rw-r--r--   0        0        0      378 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/models/.keep
--rw-r--r--   0        0        0      198 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/py.typed
--rw-r--r--   0        0        0     1500 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/sql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_balances/types/.keep
--rw-r--r--   0        0        0      275 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_transfers/.dockerignore
--rw-r--r--   0        0        0      371 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_transfers/.gitignore
--rw-r--r--   0        0        0       35 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_token_transfers/.ruff_cache/.gitignore
--rw-r--r--   0        0        0      364 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_token_transfers/.ruff_cache/0.3.4/16290975948393778209
--rw-r--r--   0        0        0      223 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_token_transfers/.ruff_cache/0.3.4/654664746373936869
--rw-r--r--   0        0        0      346 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_token_transfers/.ruff_cache/0.3.4/7975283872622358495
--rw-r--r--   0        0        0       43 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_token_transfers/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      944 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_transfers/Makefile
--rw-r--r--   0        0        0      913 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_transfers/README.md
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_transfers/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_transfers/abi/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_transfers/configs/.keep
--rw-r--r--   0        0        0      523 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_transfers/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0       81 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_transfers/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      564 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_transfers/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      570 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_transfers/configs/replay.yaml
--rw-r--r--   0        0        0      402 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_transfers/deploy/.env.default
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_transfers/deploy/.keep
--rw-r--r--   0        0        0      234 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_transfers/deploy/Dockerfile
--rw-r--r--   0        0        0      379 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_transfers/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2691 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_transfers/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1269 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_transfers/deploy/compose.yaml
--rw-r--r--   0        0        0      221 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_transfers/deploy/sqlite.env.default
--rw-r--r--   0        0        0      443 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_transfers/deploy/swarm.env.default
--rw-r--r--   0        0        0      409 2024-03-27 23:40:26.514306 dipdup-7.5.3/src/demo_token_transfers/dipdup.yaml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_token_transfers/graphql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_token_transfers/handlers/.keep
--rw-r--r--   0        0        0      545 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_token_transfers/handlers/on_balance_update.py
--rw-r--r--   0        0        0      836 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_token_transfers/handlers/on_token_transfer.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_token_transfers/hasura/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_token_transfers/hooks/.keep
--rw-r--r--   0        0        0      378 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_token_transfers/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_token_transfers/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_token_transfers/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_token_transfers/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_token_transfers/models/.keep
--rw-r--r--   0        0        0      370 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_token_transfers/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_token_transfers/py.typed
--rw-r--r--   0        0        0     1502 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_token_transfers/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_token_transfers/sql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_token_transfers/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_token_transfers/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_token_transfers/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_token_transfers/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_token_transfers/types/.keep
--rw-r--r--   0        0        0      267 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/.dockerignore
--rw-r--r--   0        0        0      363 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/.gitignore
--rw-r--r--   0        0        0       35 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_uniswap/.ruff_cache/.gitignore
--rw-r--r--   0        0        0      375 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_uniswap/.ruff_cache/0.3.4/13812209342053110860
--rw-r--r--   0        0        0      357 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_uniswap/.ruff_cache/0.3.4/1403170075816339954
--rw-r--r--   0        0        0      444 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_uniswap/.ruff_cache/0.3.4/18437025411164132658
--rw-r--r--   0        0        0      338 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_uniswap/.ruff_cache/0.3.4/3813010953694990537
--rw-r--r--   0        0        0      147 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_uniswap/.ruff_cache/0.3.4/5235765555903392059
--rw-r--r--   0        0        0     2471 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_uniswap/.ruff_cache/0.3.4/5362454613440678388
--rw-r--r--   0        0        0      365 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_uniswap/.ruff_cache/0.3.4/8803315520534010762
--rw-r--r--   0        0        0      155 2024-03-27 23:41:15.430652 dipdup-7.5.3/src/demo_uniswap/.ruff_cache/0.3.4/9726195062970630113
--rw-r--r--   0        0        0       43 2024-03-27 23:41:15.386652 dipdup-7.5.3/src/demo_uniswap/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      936 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/Makefile
--rw-r--r--   0        0        0      946 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/README.md
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/abi/.keep
--rw-r--r--   0        0        0     3684 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/abi/erc20/ERC20.json
--rw-r--r--   0        0        0      268 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/abi/erc20/ERC20NameBytes.json
--rw-r--r--   0        0        0      270 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/abi/erc20/ERC20SymbolBytes.json
--rw-r--r--   0        0        0     4418 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/abi/factory/abi.json
--rw-r--r--   0        0        0    19609 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/abi/pool/abi.json
--rw-r--r--   0        0        0    24313 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/abi/position_manager/abi.json
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/configs/.keep
--rw-r--r--   0        0        0      523 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0       73 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      548 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      615 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/configs/replay.yaml
--rw-r--r--   0        0        0      644 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/deploy/.env.default
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/deploy/.keep
--rw-r--r--   0        0        0      218 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/deploy/Dockerfile
--rw-r--r--   0        0        0      363 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2695 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1281 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/deploy/compose.yaml
--rw-r--r--   0        0        0      455 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/deploy/sqlite.env.default
--rw-r--r--   0        0        0      669 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/deploy/swarm.env.default
--rw-r--r--   0        0        0     2039 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/dipdup.yaml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/graphql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/handlers/.keep
--rw-r--r--   0        0        0     2668 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/handlers/factory/pool_created.py
--rw-r--r--   0        0        0      531 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/handlers/pool/burn.py
--rw-r--r--   0        0        0      291 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/handlers/pool/flash.py
--rw-r--r--   0        0        0      871 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/handlers/pool/initialize.py
--rw-r--r--   0        0        0     1329 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/handlers/pool/mint.py
--rw-r--r--   0        0        0     6569 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/handlers/pool/swap.py
--rw-r--r--   0        0        0     1249 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/handlers/position_manager/collect.py
--rw-r--r--   0        0        0     1383 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/handlers/position_manager/decrease_liquidity.py
--rw-r--r--   0        0        0     1471 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/handlers/position_manager/increase_liquidity.py
--rw-r--r--   0        0        0     1367 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/handlers/position_manager/transfer.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/hasura/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/hooks/.keep
--rw-r--r--   0        0        0      378 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/models/.keep
--rw-r--r--   0        0        0    19956 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/models/__init__.py
--rw-r--r--   0        0        0      373 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/models/abi.py
--rw-r--r--   0        0        0     4207 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/models/pool.py
--rw-r--r--   0        0        0     2831 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/models/position.py
--rw-r--r--   0        0        0     1452 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/models/repo.py
--rw-r--r--   0        0        0      577 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/models/tick.py
--rw-r--r--   0        0        0     7140 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/models/token.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/py.typed
--rw-r--r--   0        0        0     1535 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/sql/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/sql/on_reindex/.keep
--rw-r--r--   0        0        0      225 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/sql/on_reindex/00_prepare_db.sql
--rw-r--r--   0        0        0      792 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/sql/on_reindex/20_create_ca_quotes_1m.sql
--rw-r--r--   0        0        0      788 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/sql/on_reindex/21_create_ca_quotes_1h.sql
--rw-r--r--   0        0        0      787 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/sql/on_reindex/22_create_ca_quotes_1d.sql
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/types/.keep
--rw-r--r--   0        0        0      321 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/types/factory/evm_events/pool_created.py
--rw-r--r--   0        0        0      330 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/types/pool/evm_events/burn.py
--rw-r--r--   0        0        0      339 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/types/pool/evm_events/collect.py
--rw-r--r--   0        0        0      328 2024-03-27 23:40:26.518306 dipdup-7.5.3/src/demo_uniswap/types/pool/evm_events/flash.py
--rw-r--r--   0        0        0      275 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/demo_uniswap/types/pool/evm_events/initialize.py
--rw-r--r--   0        0        0      346 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/demo_uniswap/types/pool/evm_events/mint.py
--rw-r--r--   0        0        0      351 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/demo_uniswap/types/pool/evm_events/swap.py
--rw-r--r--   0        0        0      303 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/demo_uniswap/types/position_manager/evm_events/collect.py
--rw-r--r--   0        0        0      323 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/demo_uniswap/types/position_manager/evm_events/decrease_liquidity.py
--rw-r--r--   0        0        0      323 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/demo_uniswap/types/position_manager/evm_events/increase_liquidity.py
--rw-r--r--   0        0        0      333 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/demo_uniswap/types/position_manager/evm_events/transfer.py
--rw-r--r--   0        0        0      180 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/__init__.py
--rw-r--r--   0        0        0      105 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/__main__.py
--rw-r--r--   0        0        0     1989 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/api.py
--rw-r--r--   0        0        0    25974 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/cli.py
--rw-r--r--   0        0        0     7935 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/codegen/__init__.py
--rw-r--r--   0        0        0     9399 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/codegen/evm_subsquid.py
--rw-r--r--   0        0        0    19380 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/codegen/tezos_tzkt.py
--rw-r--r--   0        0        0    43903 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/config/__init__.py
--rw-r--r--   0        0        0      597 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/config/abi_etherscan.py
--rw-r--r--   0        0        0      690 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/config/coinbase.py
--rw-r--r--   0        0        0     1451 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/config/evm.py
--rw-r--r--   0        0        0     1307 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/config/evm_node.py
--rw-r--r--   0        0        0     1698 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/config/evm_subsquid.py
--rw-r--r--   0        0        0     2747 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/config/evm_subsquid_events.py
--rw-r--r--   0        0        0      804 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/config/evm_subsquid_traces.py
--rw-r--r--   0        0        0     3311 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/config/evm_subsquid_transactions.py
--rw-r--r--   0        0        0      446 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/config/http.py
--rw-r--r--   0        0        0      519 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/config/ipfs.py
--rw-r--r--   0        0        0     2009 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/config/tezos.py
--rw-r--r--   0        0        0     2290 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/config/tezos_tzkt.py
--rw-r--r--   0        0        0     3828 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/config/tezos_tzkt_big_maps.py
--rw-r--r--   0        0        0     3144 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/config/tezos_tzkt_events.py
--rw-r--r--   0        0        0     1524 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/config/tezos_tzkt_head.py
--rw-r--r--   0        0        0    14829 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/config/tezos_tzkt_operations.py
--rw-r--r--   0        0        0     2706 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/config/tezos_tzkt_token_balances.py
--rw-r--r--   0        0        0     3180 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/config/tezos_tzkt_token_transfers.py
--rw-r--r--   0        0        0      745 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/config/tzip_metadata.py
--rw-r--r--   0        0        0    30143 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/context.py
--rw-r--r--   0        0        0    15587 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/database.py
--rw-r--r--   0        0        0     5524 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/datasources/__init__.py
--rw-r--r--   0        0        0     1680 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/datasources/abi_etherscan.py
--rw-r--r--   0        0        0     2251 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/datasources/coinbase.py
--rw-r--r--   0        0        0    16246 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/datasources/evm_node.py
--rw-r--r--   0        0        0     8233 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/datasources/evm_subsquid.py
--rw-r--r--   0        0        0      399 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/datasources/http.py
--rw-r--r--   0        0        0      524 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/datasources/ipfs.py
--rw-r--r--   0        0        0    48706 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/datasources/tezos_tzkt.py
--rw-r--r--   0        0        0     1545 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/datasources/tzip_metadata.py
--rw-r--r--   0        0        0    34239 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/dipdup.py
--rw-r--r--   0        0        0     3175 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/env.py
--rw-r--r--   0        0        0     8666 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/exceptions.py
--rw-r--r--   0        0        0     4447 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/fetcher.py
--rw-r--r--   0        0        0     6780 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/fields.py
--rw-r--r--   0        0        0    26459 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/hasura.py
--rw-r--r--   0        0        0    10860 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/http.py
--rw-r--r--   0        0        0    10261 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/index.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/indexes/__init__.py
--rw-r--r--   0        0        0     2827 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/indexes/evm_node.py
--rw-r--r--   0        0        0     5726 2024-03-27 23:40:26.522306 dipdup-7.5.3/src/dipdup/indexes/evm_subsquid.py
--rw-r--r--   0        0        0     3664 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/evm_subsquid_events/fetcher.py
--rw-r--r--   0        0        0     4780 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/evm_subsquid_events/index.py
--rw-r--r--   0        0        0     3741 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/evm_subsquid_events/matcher.py
--rw-r--r--   0        0        0      266 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/evm_subsquid_traces/fetcher.py
--rw-r--r--   0        0        0      560 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/evm_subsquid_traces/index.py
--rw-r--r--   0        0        0        4 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/evm_subsquid_traces/matcher.py
--rw-r--r--   0        0        0     3444 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/evm_subsquid_transactions/fetcher.py
--rw-r--r--   0        0        0     3802 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/evm_subsquid_transactions/index.py
--rw-r--r--   0        0        0     3967 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/evm_subsquid_transactions/matcher.py
--rw-r--r--   0        0        0      497 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_big_maps/__init__.py
--rw-r--r--   0        0        0     3160 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_big_maps/fetcher.py
--rw-r--r--   0        0        0     5061 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_big_maps/index.py
--rw-r--r--   0        0        0     2659 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_big_maps/matcher.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_events/__init__.py
--rw-r--r--   0        0        0     1363 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_events/fetcher.py
--rw-r--r--   0        0        0     3446 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_events/index.py
--rw-r--r--   0        0        0     3781 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_events/matcher.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_head/__init__.py
--rw-r--r--   0        0        0     2679 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_head/index.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_operations/__init__.py
--rw-r--r--   0        0        0    23285 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_operations/fetcher.py
--rw-r--r--   0        0        0    13692 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_operations/index.py
--rw-r--r--   0        0        0    10443 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_operations/matcher.py
--rw-r--r--   0        0        0     7554 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_operations/parser.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_token_balances/__init__.py
--rw-r--r--   0        0        0     2753 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_token_balances/index.py
--rw-r--r--   0        0        0     1545 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_token_balances/matcher.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_token_transfers/__init__.py
--rw-r--r--   0        0        0     1576 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_token_transfers/fetcher.py
--rw-r--r--   0        0        0     3209 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_token_transfers/index.py
--rw-r--r--   0        0        0     1817 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_token_transfers/matcher.py
--rwxr-xr-x   0        0        0     9239 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/install.py
--rw-r--r--   0        0        0    22316 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/models/__init__.py
--rw-r--r--   0        0        0     1240 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/models/coinbase.py
--rw-r--r--   0        0        0     6463 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/models/evm_node.py
--rw-r--r--   0        0        0     8462 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/models/evm_subsquid.py
--rw-r--r--   0        0        0    24947 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/models/tezos_tzkt.py
--rw-r--r--   0        0        0      407 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/models/tzip_metadata.py
--rw-r--r--   0        0        0     7216 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/package.py
--rw-r--r--   0        0        0     6265 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/performance.py
--rw-r--r--   0        0        0    10232 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/project.py
--rw-r--r--   0        0        0      277 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/base/.dockerignore.j2
--rw-r--r--   0        0        0      372 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/base/.gitignore.j2
--rw-r--r--   0        0        0      945 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/base/Makefile.j2
--rw-r--r--   0        0        0     1061 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/base/README.md.j2
--rw-r--r--   0        0        0      524 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/base/configs/dipdup.compose.yaml.j2
--rw-r--r--   0        0        0       82 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/base/configs/dipdup.sqlite.yaml.j2
--rw-r--r--   0        0        0      567 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/base/configs/dipdup.swarm.yaml.j2
--rw-r--r--   0        0        0      291 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/base/deploy/Dockerfile.j2
--rw-r--r--   0        0        0      382 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/base/deploy/compose.sqlite.yaml.j2
--rw-r--r--   0        0        0     2744 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/base/deploy/compose.swarm.yaml.j2
--rw-r--r--   0        0        0     1294 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/base/deploy/compose.yaml.j2
--rw-r--r--   0        0        0     2849 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/base/pyproject.toml.j2
--rw-r--r--   0        0        0     1087 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/demo_auction/dipdup.yaml.j2
--rw-r--r--   0        0        0      935 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/demo_auction/handlers/on_bid.py.j2
--rw-r--r--   0        0        0     1641 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/demo_auction/handlers/on_create_auction.py.j2
--rw-r--r--   0        0        0      734 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/demo_auction/handlers/on_withdraw.py.j2
--rw-r--r--   0        0        0     1447 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/demo_auction/models/__init__.py.j2
--rw-r--r--   0        0        0      116 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/demo_auction/replay.yaml
--rw-r--r--   0        0        0      734 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/demo_big_maps/dipdup.yaml.j2
--rw-r--r--   0        0        0      865 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/demo_big_maps/handlers/on_update_expiry_map.py.j2
--rw-r--r--   0        0        0     1709 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/demo_big_maps/handlers/on_update_records.py.j2
--rw-r--r--   0        0        0      669 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/demo_big_maps/models/__init__.py.j2
--rw-r--r--   0        0        0      118 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/demo_big_maps/replay.yaml
--rw-r--r--   0        0        0       49 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/demo_blank/dipdup.yaml.j2
--rw-r--r--   0        0        0      116 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/demo_blank/replay.yaml
--rw-r--r--   0        0        0      657 2024-03-27 23:40:26.526306 dipdup-7.5.3/src/dipdup/projects/demo_dao/dipdup.yaml.j2
--rw-r--r--   0        0        0      431 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_dao/handlers/on_origination.py.j2
--rw-r--r--   0        0        0      540 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_dao/handlers/on_propose.py.j2
--rw-r--r--   0        0        0      784 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_dao/models/__init__.py.j2
--rw-r--r--   0        0        0      109 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_dao/replay.yaml
--rw-r--r--   0        0        0     4859 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_dex/dipdup.yaml.j2
--rw-r--r--   0        0        0     1885 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa12_divest_liquidity.py.j2
--rw-r--r--   0        0        0     1793 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa12_invest_liquidity.py.j2
--rw-r--r--   0        0        0      602 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa12_origination.py.j2
--rw-r--r--   0        0        0     1666 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa12_tez_to_token.py.j2
--rw-r--r--   0        0        0     1732 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa12_token_to_tez.py.j2
--rw-r--r--   0        0        0     1056 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa12_transfer.py.j2
--rw-r--r--   0        0        0      993 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa12_withdraw_profit.py.j2
--rw-r--r--   0        0        0     1911 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa2_divest_liquidity.py.j2
--rw-r--r--   0        0        0     1819 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa2_invest_liquidity.py.j2
--rw-r--r--   0        0        0      596 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa2_origination.py.j2
--rw-r--r--   0        0        0     1660 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa2_tez_to_token.py.j2
--rw-r--r--   0        0        0     1698 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa2_token_to_tez.py.j2
--rw-r--r--   0        0        0     1177 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa2_transfer.py.j2
--rw-r--r--   0        0        0      989 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa2_withdraw_profit.py.j2
--rw-r--r--   0        0        0      918 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_dex/models/__init__.py.j2
--rw-r--r--   0        0        0      120 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_dex/replay.yaml
--rw-r--r--   0        0        0      903 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_domains/dipdup.yaml.j2
--rw-r--r--   0        0        0     1967 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_domains/handlers/on_update_expiry_map.py.j2
--rw-r--r--   0        0        0     3314 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_domains/handlers/on_update_records.py.j2
--rw-r--r--   0        0        0      968 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_domains/hooks/check_expiration.py.j2
--rw-r--r--   0        0        0      972 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_domains/models/__init__.py.j2
--rw-r--r--   0        0        0      125 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_domains/replay.yaml
--rw-r--r--   0        0        0     1343 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_etherlink/dipdup.yaml.j2
--rw-r--r--   0        0        0      129 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_etherlink/replay.yaml
--rw-r--r--   0        0        0      545 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_events/dipdup.yaml.j2
--rw-r--r--   0        0        0      114 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_events/replay.yaml
--rw-r--r--   0        0        0      818 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_evm_events/dipdup.yaml.j2
--rw-r--r--   0        0        0     1305 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_evm_events/handlers/on_transfer.py.j2
--rw-r--r--   0        0        0      470 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_evm_events/models/__init__.py.j2
--rw-r--r--   0        0        0      136 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_evm_events/replay.yaml
--rw-r--r--   0        0        0      851 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_evm_transactions/dipdup.yaml.j2
--rw-r--r--   0        0        0     1346 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_evm_transactions/handlers/on_transfer.py.j2
--rw-r--r--   0        0        0      470 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_evm_transactions/models/__init__.py.j2
--rw-r--r--   0        0        0      150 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_evm_transactions/replay.yaml
--rw-r--r--   0        0        0     1098 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_factories/dipdup.yaml.j2
--rw-r--r--   0        0        0     1082 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_factories/handlers/on_factory_origination.py.j2
--rw-r--r--   0        0        0      681 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_factories/handlers/on_transfer.py.j2
--rw-r--r--   0        0        0      214 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_factories/models/__init__.py.j2
--rw-r--r--   0        0        0      132 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_factories/replay.yaml
--rw-r--r--   0        0        0      253 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_head/dipdup.yaml.j2
--rw-r--r--   0        0        0      130 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_head/replay.yaml
--rw-r--r--   0        0        0     1201 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_nft_marketplace/dipdup.yaml.j2
--rw-r--r--   0        0        0      603 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_nft_marketplace/handlers/on_cancel_swap.py.j2
--rw-r--r--   0        0        0     1035 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_nft_marketplace/handlers/on_collect.py.j2
--rw-r--r--   0        0        0      973 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_nft_marketplace/handlers/on_mint.py.j2
--rw-r--r--   0        0        0      883 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_nft_marketplace/handlers/on_swap.py.j2
--rw-r--r--   0        0        0     1309 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_nft_marketplace/models/__init__.py.j2
--rw-r--r--   0        0        0      135 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_nft_marketplace/replay.yaml
--rw-r--r--   0        0        0      425 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_raw/dipdup.yaml.j2
--rw-r--r--   0        0        0      364 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_raw/handlers/on_operation.py.j2
--rw-r--r--   0        0        0      247 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_raw/models/__init__.py.j2
--rw-r--r--   0        0        0      141 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_raw/replay.yaml
--rw-r--r--   0        0        0      742 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_token/dipdup.yaml.j2
--rw-r--r--   0        0        0      448 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_token/handlers/on_balance_update.py.j2
--rw-r--r--   0        0        0      664 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_token/handlers/on_mint.py.j2
--rw-r--r--   0        0        0      962 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_token/handlers/on_transfer.py.j2
--rw-r--r--   0        0        0      372 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_token/models/__init__.py.j2
--rw-r--r--   0        0        0      117 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_token/replay.yaml
--rw-r--r--   0        0        0      410 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_token_balances/dipdup.yaml.j2
--rw-r--r--   0        0        0      473 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_token_balances/handlers/on_balance_update.py.j2
--rw-r--r--   0        0        0      200 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_token_balances/models/__init__.py.j2
--rw-r--r--   0        0        0      124 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_token_balances/replay.yaml
--rw-r--r--   0        0        0      411 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_token_transfers/dipdup.yaml.j2
--rw-r--r--   0        0        0      545 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_token_transfers/handlers/on_balance_update.py.j2
--rw-r--r--   0        0        0      836 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_token_transfers/handlers/on_token_transfer.py.j2
--rw-r--r--   0        0        0      372 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_token_transfers/models/__init__.py.j2
--rw-r--r--   0        0        0      127 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_token_transfers/replay.yaml
--rw-r--r--   0        0        0     3685 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/abi/erc20/ERC20.json.j2
--rw-r--r--   0        0        0      269 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/abi/erc20/ERC20NameBytes.json.j2
--rw-r--r--   0        0        0      271 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/abi/erc20/ERC20SymbolBytes.json.j2
--rw-r--r--   0        0        0     2049 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/dipdup.yaml.j2
--rw-r--r--   0        0        0     2711 2024-03-27 23:40:26.530306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/handlers/factory/pool_created.py.j2
--rw-r--r--   0        0        0      567 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/handlers/pool/burn.py.j2
--rw-r--r--   0        0        0      309 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/handlers/pool/flash.py.j2
--rw-r--r--   0        0        0      898 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/handlers/pool/initialize.py.j2
--rw-r--r--   0        0        0     1375 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/handlers/pool/mint.py.j2
--rw-r--r--   0        0        0     6641 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/handlers/pool/swap.py.j2
--rw-r--r--   0        0        0     1286 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/handlers/position_manager/collect.py.j2
--rw-r--r--   0        0        0     1420 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/handlers/position_manager/decrease_liquidity.py.j2
--rw-r--r--   0        0        0     1508 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/handlers/position_manager/increase_liquidity.py.j2
--rw-r--r--   0        0        0     1405 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/handlers/position_manager/transfer.py.j2
--rw-r--r--   0        0        0    19957 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/models/__init__.py.j2
--rw-r--r--   0        0        0      373 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/models/abi.py.j2
--rw-r--r--   0        0        0     4269 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/models/pool.py.j2
--rw-r--r--   0        0        0     2849 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/models/position.py.j2
--rw-r--r--   0        0        0     1461 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/models/repo.py.j2
--rw-r--r--   0        0        0      586 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/models/tick.py.j2
--rw-r--r--   0        0        0     7167 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/models/token.py.j2
--rw-r--r--   0        0        0      250 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/replay.yaml
--rw-r--r--   0        0        0      226 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/sql/on_reindex/00_prepare_db.sql.j2
--rw-r--r--   0        0        0      793 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/sql/on_reindex/20_create_ca_quotes_1m.sql.j2
--rw-r--r--   0        0        0      789 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/sql/on_reindex/21_create_ca_quotes_1h.sql.j2
--rw-r--r--   0        0        0      788 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/projects/demo_uniswap/sql/on_reindex/22_create_ca_quotes_1d.sql.j2
--rw-r--r--   0        0        0     4126 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/prometheus.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/py.typed
--rw-r--r--   0        0        0     1774 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/pysignalr.py
--rw-r--r--   0        0        0     2147 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/report.py
--rw-r--r--   0        0        0     4938 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/scheduler.py
--rw-r--r--   0        0        0     4598 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/sentry.py
--rw-r--r--   0        0        0      272 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/sql/dipdup_approve.sql
--rw-r--r--   0        0        0      199 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/sql/dipdup_head_status.sql
--rw-r--r--   0        0        0     1904 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/sql/dipdup_wipe.sql
--rw-r--r--   0        0        0     2077 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/subscriptions.py
--rw-r--r--   0        0        0     2227 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/sys.py
--rw-r--r--   0        0        0      227 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/templates/callback.py.j2
--rw-r--r--   0        0        0     1241 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/templates/models.py
--rw-r--r--   0        0        0      276 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/templates/replay.yaml.j2
--rw-r--r--   0        0        0     6532 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/test.py
--rw-r--r--   0        0        0     3017 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/transactions.py
--rw-r--r--   0        0        0     7610 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/utils.py
--rw-r--r--   0        0        0     5466 2024-03-27 23:40:26.534306 dipdup-7.5.3/src/dipdup/yaml.py
--rw-r--r--   0        0        0      864 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/__init__.py
--rw-r--r--   0        0        0      496 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/asdf.yml
--rw-r--r--   0        0        0     1222 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/demo_auction.yml
--rw-r--r--   0        0        0      780 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/demo_big_maps.yml
--rw-r--r--   0        0        0      747 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/demo_dao.yml
--rw-r--r--   0        0        0     5012 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/demo_dex.yml
--rw-r--r--   0        0        0      943 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/demo_domains.yml
--rw-r--r--   0        0        0     1392 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/demo_etherlink.yaml
--rw-r--r--   0        0        0      583 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/demo_events.yml
--rw-r--r--   0        0        0      824 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/demo_evm_events.yml
--rw-r--r--   0        0        0      844 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/demo_evm_events_node.yml
--rw-r--r--   0        0        0      877 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/demo_evm_transactions.yml
--rw-r--r--   0        0        0      897 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/demo_evm_transactions_node.yml
--rw-r--r--   0        0        0     1144 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/demo_factories.yml
--rw-r--r--   0        0        0     1316 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/demo_nft_marketplace.yml
--rw-r--r--   0        0        0      590 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/demo_raw.yml
--rw-r--r--   0        0        0      711 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/demo_token.yml
--rw-r--r--   0        0        0      456 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/demo_token_balances.yml
--rw-r--r--   0        0        0      527 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/demo_token_transfers.yml
--rw-r--r--   0        0        0      527 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/demo_token_transfers_2.yml
--rw-r--r--   0        0        0      527 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/demo_token_transfers_3.yml
--rw-r--r--   0        0        0      814 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/demo_token_transfers_4.yml
--rw-r--r--   0        0        0     1252 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/dipdup.yml
--rw-r--r--   0        0        0      521 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/hen_subjkt.yml
--rw-r--r--   0        0        0      496 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/hjkl.yml
--rw-r--r--   0        0        0      546 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/kolibri_ovens.yml
--rw-r--r--   0        0        0      684 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/operation_filters.yml
--rw-r--r--   0        0        0      496 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/qwer.yml
--rw-r--r--   0        0        0      496 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/rewq.yml
--rw-r--r--   0        0        0       98 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/test_postgres.yaml
--rw-r--r--   0        0        0      151 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/test_postgres_immune.yaml
--rw-r--r--   0        0        0       44 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/test_sqlite.yaml
--rw-r--r--   0        0        0      128 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/test_sqlite_immune.yaml
--rw-r--r--   0        0        0      534 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/yupana.yml
--rw-r--r--   0        0        0      496 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/configs/zxcv.yml
--rw-r--r--   0        0        0     1311 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/profile_abi_decoding.py
--rw-r--r--   0        0        0    29145 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/replays/0535b2dcc93076e6026fa48cc501adaed47b7b060e6483d8312f40c184d7287d
--rw-r--r--   0        0        0      305 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/replays/0b7d26b8f2813d12a80b9e96cc6f0bb186bf9ac5c5b0c0b3bb2cc8d750126843
--rw-r--r--   0        0        0      959 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/replays/0eaaba2830dbdd3a80286fbc367084bce6e55c678e21da178a7eb16beef6c997
--rw-r--r--   0        0        0    25834 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/replays/1228b36594bb93d619170ad49373f1ceec52d10faafdd727b37f3cdeffd663db
--rw-r--r--   0        0        0    13886 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/replays/13afdf001ce3d6a0219c0f7f6d372d9b645770e5f4304576f7f7a37b45af96fc
--rw-r--r--   0        0        0      403 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/replays/1430e37dce64ecb83499da8feaa3c0906e4fdf5d0a3c3570174645e97ba54bc4
--rw-r--r--   0        0        0      295 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/replays/185f6628ac43f6ca728c5b79b7b81a3c3671efce7f14030a06a27e90cf641dea
--rw-r--r--   0        0        0        2 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/replays/1c717490846300e1639e96a0c1438b6dd2abd6de013c5edec49042fa364c06e6
--rw-r--r--   0        0        0     1871 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/replays/27373c23411bf37b605c8d0ead9a0e6c6c1f1718ce7863b095b759811e44e155
--rw-r--r--   0        0        0     1824 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/replays/2a45ec6372b45e46199a6af24272cb93586777a0522cd1203b3eeef213ce4583
--rw-r--r--   0        0        0    54602 2024-03-27 23:40:26.534306 dipdup-7.5.3/tests/replays/383899084f79460e96fd311bb64e4925738c486b39d6281539456c5fcac41620
--rw-r--r--   0        0        0   234676 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/388fe9107380b6dd1e9ce3a87c23abd56ad39dfb6cb8a5a27b959e5b0434633b
--rw-r--r--   0        0        0      642 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/39b8664d1bca5d374ff905c8a3a396b53d19ee469dc37545a8ca6b080bd0e9e0
--rw-r--r--   0        0        0     1200 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/3a2bd8b6b72bf18152d2550c106789fa9b8abc98ea9d759a6597b7ebfbab0fc2
--rw-r--r--   0        0        0    34389 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/3f5927db41422038d8e2cc203ef56a769c66b25835cdee42b17bc61e600be550
--rw-r--r--   0        0        0      804 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/43cb0ab415d8b8b3f7addc3e82ea27d93b2c66ff55c117e1e0c7c64a0fcfc3f2
--rw-r--r--   0        0        0   109726 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/4a57776d93475adfd9c49b6c3295a7cedfc23b73733a1fb5f0c985ee039dc5dc
--rw-r--r--   0        0        0     1160 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/4aa7f9b0657be0c44baf2caed8c7cb08d02097a4095cf6417f78cba3a25e8423
--rw-r--r--   0        0        0       67 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/4fbdb4667971fab446a5ac5937a7c8cc6ef5813ff00af24b6fd1b1a0427bedbb
--rw-r--r--   0        0        0   192680 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/5483a0e11009e0f186bf70c214e2597d267a75a1e19152a9e7ed1ec257ce88ca
--rw-r--r--   0        0        0    40432 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/587613799ebfae42b1884016d1a44a452d68e70e3ed80641d90b8e7657ba8ee5
--rw-r--r--   0        0        0       32 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/5b004196490632859ec1b019d640f6bbb93fc86a433c8969e10f36f51ac2c78d
--rw-r--r--   0        0        0    40439 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/5b99bc4beb6a9a33f7d2f118426458e4c788e0ab6d9e51949d3ccbf8b4003fc1
--rw-r--r--   0        0        0    33335 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/607ecfd3653eda82aac502ac370c6ad7144d30c1e3c525ed520d44f9edf5b7e9
--rw-r--r--   0        0        0       67 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/60f48c13c47a1347786a6dcf6f741874e7b30b587d148faa67d15067bb3871de
--rw-r--r--   0        0        0        2 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/694f9dfac7db616fa52c4d35bca1036b6521d285ed1873028303b83822b5980b
--rw-r--r--   0        0        0      132 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/6d0c5443d41a15551acb41adc10d36d4895f5786d6922a878b5c5414610e0ebc
--rw-r--r--   0        0        0      754 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/6d76a3c3f427ff534c551de1793cb1d1dfbd22ccad97f5917a9f9b201a3f9804
--rw-r--r--   0        0        0     1781 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/6fa41b68da742cc7cf8a0d68baef77ce8b2e9abf765767318d7ff4cf453ded4c
--rw-r--r--   0        0        0      451 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/739d17c86095aac3da3508a16dc1c9ae9459ea86eeb09f62aaefc32de2997918
--rw-r--r--   0        0        0        2 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/759b79ec12b1305d9fa8e1a5218e62bb3d3ad913580e19914d30d8aa09920ae4
--rw-r--r--   0        0        0    50588 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/7b6cf9b8c69712bf26ed09059352ec740606969bf20eab0dedda870273f4fde9
--rw-r--r--   0        0        0      807 2024-03-27 23:40:26.538307 dipdup-7.5.3/tests/replays/803e05a8d0bb9e7cfb49530271d43ea62111b6419e7cded2d221f7e0e0c92ece
--rw-r--r--   0        0        0   203748 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/8060a1f95213d470ee947a12242ef76cb7fb0c05bbaecc385eb6ec4a20d694c4
--rw-r--r--   0        0        0      395 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/8335acc6585656ec3a4301cd8b089401f2dc2c7d758b381c96c730e610b67f7b
--rw-r--r--   0        0        0     1151 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/93516225810a23a6799f2f9a1dee055ca79a66ee2b8d0f32be820c9c385e936b
--rw-r--r--   0        0        0      877 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/9e6e907842da2cd494c558ea5ecc211fd12e56bfc547450978fb7dfe03853e58
--rw-r--r--   0        0        0    22801 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/a3ce91a1b0d505cc221f0e201781466ba1e2d6dc7b624b9bc75a03ce3dbb0f92
--rw-r--r--   0        0        0      767 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/aa8fe6037996b296bf9a3011e45cd9ecb92fb728592a843f91b03b2848cb1fb1
--rw-r--r--   0        0        0     1931 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/acaa57345850f3b76471a7b3a8fb76b7f83e824f1520a2e0ee8ec93cdd6cb1c3
--rw-r--r--   0        0        0     1882 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/acc952ba1905717315212f952ed689d7b8f683165b31c0a7a25199aed9fda27f
--rw-r--r--   0        0        0       67 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/af37212b31e932f269c42c7f34ad8f3849bd8aed244652c41b9327c508985ce5
--rw-r--r--   0        0        0     1200 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/b3af887f7ad8172af75b94a09bedfb9ae1e14f8819a36d6ce9f709721068263b
--rw-r--r--   0        0        0    34407 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/b89b0ea704071e273d3c74a4dbb7b4f6c6fd9ea1848c69b452dce4f04872d3b5
--rw-r--r--   0        0        0     2271 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/bec4433b4206f00c2310a7961cff7f539434b9161b45673793aa5a3b50234313
--rw-r--r--   0        0        0      403 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/bed2329e63d559db2fb81c69606e715d1f90aaacab6ae45b33516e7828841a3c
--rw-r--r--   0        0        0    89684 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/c1c3eef91f7149d7aa2da072f71598f3ad5e29250cfa441bb6d4411acd70d657
--rw-r--r--   0        0        0    25834 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/cc5d3d4a58d5cb6bc7270d38c797b7740b79f913590ef0164abd50e58fba9405
--rw-r--r--   0        0        0     1157 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/d0a594d14bcb3fbf916092ec6707dfd3c9f48f53f0a1ad40a32023e7a87f8ef5
--rw-r--r--   0        0        0     6669 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/d62748a927a09395579b5790c8f871cc8653081cf4475abc93173989f950b92b
--rw-r--r--   0        0        0    27896 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/d94397f6ecec8ce25f87177fe410f6498d7d30a04360506c0cd300d291c167e7
--rw-r--r--   0        0        0      132 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/db797e6bf4c1b9c3237af5dec694fb1b6d21418a5a2f7947eb7f54d4e9201baf
--rw-r--r--   0        0        0    20467 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/dca9cf4f9f27623f10975d369444899458ab9ea85c22af2da6ce6ce8c09c2b58
--rw-r--r--   0        0        0      767 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/dd5d267c6e8e943a637ede23d708587123b9184560358d294be7fbed0d4b587a
--rw-r--r--   0        0        0   209761 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/e10e6552f0dce5124e0d72b74c508541a8098c407c9a3b0d2e10a7408b4d7cfe
--rw-r--r--   0        0        0    17502 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/e4a563a0b19379a44e9d2dc398131e9fd30d6039ff4ffacf1252db0bf8b433aa
--rw-r--r--   0        0        0       67 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/e82ba90c8570b92c0b1fc360b853aca3f1d7de457aacb9f6f19fa3e43879a8b3
--rw-r--r--   0        0        0      132 2024-03-27 23:40:26.542307 dipdup-7.5.3/tests/replays/e9fa56a94eb559c550dfbca4b27ef350a0b4a787afbe60205482a38223dcea04
--rw-r--r--   0        0        0   713738 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/replays/eb8b6b33cb2e165d1a3a73c09938d3083671a82ad73d4c0cff1fb2a5e5715f76
--rw-r--r--   0        0        0    27505 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/replays/eb8e2c3ce2fe7792d2c8e81c61d37821275b64021343103b0c955042ae802189
--rw-r--r--   0        0        0    17245 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/replays/f3d608f99e6b92e28a064bb9c10c3c605c9c817383c1eebcc68f663d1d23d650
--rw-r--r--   0        0        0   211527 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/replays/f7d244938de3e3d153e4ef8172cab0f1e896b801904a54ac034d3d14352ee64a
--rw-r--r--   0        0        0    27847 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/replays/f9fa1571c3d850f4a19c286205291893d184a9d124390d0358034a8b8366556d
--rw-r--r--   0        0        0   118246 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/replays/fe80425d17f2467fccc527a99b5a11da144f63f9a3cab83989be0f8fed737264
--rw-r--r--   0        0        0      996 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/replays/ff51b3535acc2972090ecd5db3af8f827464c9d92f1aa661630976e5b4ed4cbe
--rw-r--r--   0        0        0     4599 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/responses/asdf.json
--rw-r--r--   0        0        0     6704 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/responses/ftzfun.json
--rw-r--r--   0        0        0     3445 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/responses/hen_subjkt.json
--rw-r--r--   0        0        0     5210 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/responses/hjkl.json
--rw-r--r--   0        0        0     2097 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/responses/kolibri_ovens.json
--rw-r--r--   0        0        0    11186 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/responses/ooQuCAKBHkmWy2VciDAV9c6CFTywuMLupLzVoKDwS1xvR4EdRng.json
--rw-r--r--   0        0        0     1811 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/responses/origination_amount.json
--rw-r--r--   0        0        0     4256 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/responses/qwer.json
--rw-r--r--   0        0        0     5307 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/responses/rewq.json
--rw-r--r--   0        0        0    38178 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/responses/yupana.json
--rw-r--r--   0        0        0     5909 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/responses/zxcv.json
--rw-r--r--   0        0        0     1077 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/schemas/asdf/storage.json
--rw-r--r--   0        0        0     2116 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/schemas/hen_subjkt/storage.json
--rw-r--r--   0        0        0     1638 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/schemas/hjkl/storage.json
--rw-r--r--   0        0        0      800 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/schemas/kolibri_ovens/storage.json
--rw-r--r--   0        0        0     1005 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/schemas/qwer/storage.json
--rw-r--r--   0        0        0     2212 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/schemas/rewq/storage.json
--rw-r--r--   0        0        0    12561 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/schemas/yupana/storage.json
--rw-r--r--   0        0        0     2660 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/schemas/zxcv/storage.json
--rw-r--r--   0        0        0     3767 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/test_config/test_callbacks.py
--rw-r--r--   0        0        0     4642 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/test_config/test_config.py
--rw-r--r--   0        0        0     4138 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/test_config/test_custom_config.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/test_datasources/__init__.py
--rw-r--r--   0        0        0      814 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/test_datasources/test_ipfs.py
--rw-r--r--   0        0        0      795 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/test_datasources/test_metadata.py
--rw-r--r--   0        0        0     8320 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/test_datasources/test_tzkt.py
--rw-r--r--   0        0        0     1215 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/test_datasources/test_tzkt_blocks.py
--rw-r--r--   0        0        0     1971 2024-03-27 23:40:26.546306 dipdup-7.5.3/tests/test_datasources/test_tzkt_buffer.py
--rw-r--r--   0        0        0     1425 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/test_datasources/test_tzkt_quotes.py
--rw-r--r--   0        0        0     8973 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/test_demos.py
--rw-r--r--   0        0        0     2872 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/test_dipdup.py
--rw-r--r--   0        0        0     3094 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/test_hasura.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/test_http.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/test_index/__init__.py
--rw-r--r--   0        0        0     7393 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/test_index/test_tzkt_operations.py
--rw-r--r--   0        0        0     5409 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/test_introspection.py
--rw-r--r--   0        0        0    11401 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/test_models.py
--rw-r--r--   0        0        0    13543 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/test_rollback.py
--rw-r--r--   0        0        0     6692 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/test_schema.py
--rw-r--r--   0        0        0     3620 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/test_utils.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/asdf/__init__.py
--rw-r--r--   0        0        0      455 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/asdf/storage.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/bazaar/__init__.py
--rw-r--r--   0        0        0      539 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/bazaar/storage.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/ftzfun/__init__.py
--rw-r--r--   0        0        0      881 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/ftzfun/storage.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/hen_subjkt/__init__.py
--rw-r--r--   0        0        0      558 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/hen_subjkt/storage.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/hjkl/__init__.py
--rw-r--r--   0        0        0      564 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/hjkl/storage.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/kolibri_ovens/__init__.py
--rw-r--r--   0        0        0      200 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/kolibri_ovens/set_delegate.py
--rw-r--r--   0        0        0      392 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/kolibri_ovens/storage.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/listofmaps/__init__.py
--rw-r--r--   0        0        0      104 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/listofmaps/storage.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/qwer/__init__.py
--rw-r--r--   0        0        0      452 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/qwer/storage.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/rewq/__init__.py
--rw-r--r--   0        0        0      770 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/rewq/storage.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/tezotop/__init__.py
--rw-r--r--   0        0        0      660 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/tezotop/storage.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/yupana/__init__.py
--rw-r--r--   0        0        0     2635 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/yupana/storage.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/zxcv/__init__.py
--rw-r--r--   0        0        0      981 2024-03-27 23:40:26.550307 dipdup-7.5.3/tests/types/zxcv/storage.py
--rw-r--r--   0        0        0     4732 1970-01-01 00:00:00.000000 dipdup-7.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-09 23:07:36.399830 dipdup-7.5.4/LICENSE
+-rw-r--r--   0        0        0     2581 2024-04-09 23:07:36.399830 dipdup-7.5.4/README.md
+-rw-r--r--   0        0        0     5101 2024-04-09 23:15:02.174955 dipdup-7.5.4/pyproject.toml
+-rw-r--r--   0        0        0      267 2024-04-09 23:07:36.411831 dipdup-7.5.4/src/demo_auction/.dockerignore
+-rw-r--r--   0        0        0      363 2024-04-09 23:07:36.411831 dipdup-7.5.4/src/demo_auction/.gitignore
+-rw-r--r--   0        0        0       35 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_auction/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      291 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_auction/.ruff_cache/0.3.5/15635057057909269342
+-rw-r--r--   0        0        0      338 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_auction/.ruff_cache/0.3.5/16470011701158794569
+-rw-r--r--   0        0        0      368 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_auction/.ruff_cache/0.3.5/17658190832657717516
+-rw-r--r--   0        0        0      154 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_auction/.ruff_cache/0.3.5/3661566128250832699
+-rw-r--r--   0        0        0      269 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_auction/.ruff_cache/0.3.5/5982868015305951553
+-rw-r--r--   0        0        0       43 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_auction/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      936 2024-04-09 23:07:36.411831 dipdup-7.5.4/src/demo_auction/Makefile
+-rw-r--r--   0        0        0      910 2024-04-09 23:07:36.411831 dipdup-7.5.4/src/demo_auction/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.411831 dipdup-7.5.4/src/demo_auction/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.411831 dipdup-7.5.4/src/demo_auction/abi/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.411831 dipdup-7.5.4/src/demo_auction/configs/.keep
+-rw-r--r--   0        0        0      523 2024-04-09 23:07:36.411831 dipdup-7.5.4/src/demo_auction/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0       73 2024-04-09 23:07:36.411831 dipdup-7.5.4/src/demo_auction/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      548 2024-04-09 23:07:36.411831 dipdup-7.5.4/src/demo_auction/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      559 2024-04-09 23:07:36.411831 dipdup-7.5.4/src/demo_auction/configs/replay.yaml
+-rw-r--r--   0        0        0      431 2024-04-09 23:07:36.411831 dipdup-7.5.4/src/demo_auction/deploy/.env.default
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.411831 dipdup-7.5.4/src/demo_auction/deploy/.keep
+-rw-r--r--   0        0        0      218 2024-04-09 23:07:36.411831 dipdup-7.5.4/src/demo_auction/deploy/Dockerfile
+-rw-r--r--   0        0        0      363 2024-04-09 23:07:36.411831 dipdup-7.5.4/src/demo_auction/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2675 2024-04-09 23:07:36.411831 dipdup-7.5.4/src/demo_auction/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1261 2024-04-09 23:07:36.411831 dipdup-7.5.4/src/demo_auction/deploy/compose.yaml
+-rw-r--r--   0        0        0      242 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      456 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/deploy/swarm.env.default
+-rw-r--r--   0        0        0     1077 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/dipdup.yaml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/graphql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/handlers/.keep
+-rw-r--r--   0        0        0      913 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/handlers/on_bid.py
+-rw-r--r--   0        0        0     1619 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/handlers/on_create_auction.py
+-rw-r--r--   0        0        0      712 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/handlers/on_withdraw.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/hasura/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/hooks/.keep
+-rw-r--r--   0        0        0      378 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/models/.keep
+-rw-r--r--   0        0        0     1445 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/py.typed
+-rw-r--r--   0        0        0     1499 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/sql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/types/.keep
+-rw-r--r--   0        0        0      177 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/types/tzcolors_auction/tezos_parameters/bid.py
+-rw-r--r--   0        0        0      381 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/types/tzcolors_auction/tezos_parameters/create_auction.py
+-rw-r--r--   0        0        0      187 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/types/tzcolors_auction/tezos_parameters/withdraw.py
+-rw-r--r--   0        0        0      499 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_auction/types/tzcolors_auction/tezos_storage.py
+-rw-r--r--   0        0        0      268 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/.dockerignore
+-rw-r--r--   0        0        0      364 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/.gitignore
+-rw-r--r--   0        0        0       35 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_big_maps/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      219 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_big_maps/.ruff_cache/0.3.5/13744238530215110863
+-rw-r--r--   0        0        0      394 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_big_maps/.ruff_cache/0.3.5/17373131790238605435
+-rw-r--r--   0        0        0      339 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_big_maps/.ruff_cache/0.3.5/2955696403654854472
+-rw-r--r--   0        0        0      343 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_big_maps/.ruff_cache/0.3.5/9433195061015572675
+-rw-r--r--   0        0        0       43 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_big_maps/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      937 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/Makefile
+-rw-r--r--   0        0        0      911 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/abi/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/configs/.keep
+-rw-r--r--   0        0        0      523 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0       74 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      550 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      561 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/configs/replay.yaml
+-rw-r--r--   0        0        0      431 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/deploy/.env.default
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/deploy/.keep
+-rw-r--r--   0        0        0      220 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/deploy/Dockerfile
+-rw-r--r--   0        0        0      365 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2677 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1262 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/deploy/compose.yaml
+-rw-r--r--   0        0        0      243 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      458 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/deploy/swarm.env.default
+-rw-r--r--   0        0        0      725 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/dipdup.yaml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/graphql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/handlers/.keep
+-rw-r--r--   0        0        0      846 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/handlers/on_update_expiry_map.py
+-rw-r--r--   0        0        0     1690 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/handlers/on_update_records.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/hasura/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/hooks/.keep
+-rw-r--r--   0        0        0      378 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/models/.keep
+-rw-r--r--   0        0        0      667 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/py.typed
+-rw-r--r--   0        0        0     1500 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/sql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/types/.keep
+-rw-r--r--   0        0        0      199 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/types/name_registry/tezos_big_maps/store_expiry_map_key.py
+-rw-r--r--   0        0        0      203 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/types/name_registry/tezos_big_maps/store_expiry_map_value.py
+-rw-r--r--   0        0        0      194 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/types/name_registry/tezos_big_maps/store_records_key.py
+-rw-r--r--   0        0        0      427 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_big_maps/types/name_registry/tezos_big_maps/store_records_value.py
+-rw-r--r--   0        0        0      265 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/.dockerignore
+-rw-r--r--   0        0        0      361 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/.gitignore
+-rw-r--r--   0        0        0       35 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_blank/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      336 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_blank/.ruff_cache/0.3.5/12172753112764134098
+-rw-r--r--   0        0        0      354 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_blank/.ruff_cache/0.3.5/7064015182751687391
+-rw-r--r--   0        0        0       43 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_blank/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      934 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/Makefile
+-rw-r--r--   0        0        0      912 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/abi/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/configs/.keep
+-rw-r--r--   0        0        0      523 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0       71 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      544 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      559 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/configs/replay.yaml
+-rw-r--r--   0        0        0      402 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/deploy/.env.default
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/deploy/.keep
+-rw-r--r--   0        0        0      214 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/deploy/Dockerfile
+-rw-r--r--   0        0        0      359 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2671 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1259 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/deploy/compose.yaml
+-rw-r--r--   0        0        0      211 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      423 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/deploy/swarm.env.default
+-rw-r--r--   0        0        0       37 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/dipdup.yaml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/graphql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/handlers/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/hasura/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/hooks/.keep
+-rw-r--r--   0        0        0      378 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.415830 dipdup-7.5.4/src/demo_blank/models/.keep
+-rw-r--r--   0        0        0     1241 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_blank/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_blank/py.typed
+-rw-r--r--   0        0        0     1501 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_blank/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_blank/sql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_blank/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_blank/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_blank/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_blank/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_blank/types/.keep
+-rw-r--r--   0        0        0      263 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/.dockerignore
+-rw-r--r--   0        0        0      359 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/.gitignore
+-rw-r--r--   0        0        0       35 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_dao/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      153 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_dao/.ruff_cache/0.3.5/14008987445524047848
+-rw-r--r--   0        0        0      201 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_dao/.ruff_cache/0.3.5/2146085926717066313
+-rw-r--r--   0        0        0      334 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_dao/.ruff_cache/0.3.5/3667366973558527546
+-rw-r--r--   0        0        0      328 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_dao/.ruff_cache/0.3.5/4827808853738895797
+-rw-r--r--   0        0        0      142 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_dao/.ruff_cache/0.3.5/7256014187454356602
+-rw-r--r--   0        0        0       43 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_dao/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      932 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/Makefile
+-rw-r--r--   0        0        0      907 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/abi/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/configs/.keep
+-rw-r--r--   0        0        0      523 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0       69 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      540 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      552 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/configs/replay.yaml
+-rw-r--r--   0        0        0      431 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/deploy/.env.default
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/deploy/.keep
+-rw-r--r--   0        0        0      210 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/deploy/Dockerfile
+-rw-r--r--   0        0        0      355 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2667 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1257 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/deploy/compose.yaml
+-rw-r--r--   0        0        0      238 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      448 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/deploy/swarm.env.default
+-rw-r--r--   0        0        0      643 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/dipdup.yaml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/graphql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/handlers/.keep
+-rw-r--r--   0        0        0      408 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/handlers/on_origination.py
+-rw-r--r--   0        0        0      506 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/handlers/on_propose.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/hasura/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/hooks/.keep
+-rw-r--r--   0        0        0      378 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/models/.keep
+-rw-r--r--   0        0        0      782 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/py.typed
+-rw-r--r--   0        0        0     1496 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/sql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/types/.keep
+-rw-r--r--   0        0        0      360 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/types/registry/tezos_parameters/propose.py
+-rw-r--r--   0        0        0     2475 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dao/types/registry/tezos_storage.py
+-rw-r--r--   0        0        0      263 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/.dockerignore
+-rw-r--r--   0        0        0      359 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/.gitignore
+-rw-r--r--   0        0        0       35 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_dex/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      334 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_dex/.ruff_cache/0.3.5/10154177989203775933
+-rw-r--r--   0        0        0      356 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_dex/.ruff_cache/0.3.5/11231591400380693096
+-rw-r--r--   0        0        0      513 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_dex/.ruff_cache/0.3.5/11744045978700083414
+-rw-r--r--   0        0        0      143 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_dex/.ruff_cache/0.3.5/14829319066810751712
+-rw-r--r--   0        0        0      144 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_dex/.ruff_cache/0.3.5/14967953906436846482
+-rw-r--r--   0        0        0     1110 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_dex/.ruff_cache/0.3.5/15668834222879262927
+-rw-r--r--   0        0        0      156 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_dex/.ruff_cache/0.3.5/16477189981468498568
+-rw-r--r--   0        0        0      155 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_dex/.ruff_cache/0.3.5/17951098284708353564
+-rw-r--r--   0        0        0      144 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_dex/.ruff_cache/0.3.5/3636242551805637072
+-rw-r--r--   0        0        0      143 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_dex/.ruff_cache/0.3.5/779905150700776090
+-rw-r--r--   0        0        0      512 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_dex/.ruff_cache/0.3.5/8239091470560594148
+-rw-r--r--   0        0        0       43 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_dex/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      932 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/Makefile
+-rw-r--r--   0        0        0      918 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/abi/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/configs/.keep
+-rw-r--r--   0        0        0      523 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0       69 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      540 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      563 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/configs/replay.yaml
+-rw-r--r--   0        0        0      402 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/deploy/.env.default
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/deploy/.keep
+-rw-r--r--   0        0        0      210 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/deploy/Dockerfile
+-rw-r--r--   0        0        0      355 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2667 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1257 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/deploy/compose.yaml
+-rw-r--r--   0        0        0      209 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      419 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/deploy/swarm.env.default
+-rw-r--r--   0        0        0     4845 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/dipdup.yaml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/graphql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/handlers/.keep
+-rw-r--r--   0        0        0     1829 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/handlers/on_fa12_divest_liquidity.py
+-rw-r--r--   0        0        0     1737 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/handlers/on_fa12_invest_liquidity.py
+-rw-r--r--   0        0        0      579 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/handlers/on_fa12_origination.py
+-rw-r--r--   0        0        0     1610 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/handlers/on_fa12_tez_to_token.py
+-rw-r--r--   0        0        0     1676 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/handlers/on_fa12_token_to_tez.py
+-rw-r--r--   0        0        0     1022 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/handlers/on_fa12_transfer.py
+-rw-r--r--   0        0        0      931 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/handlers/on_fa12_withdraw_profit.py
+-rw-r--r--   0        0        0     1855 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/handlers/on_fa2_divest_liquidity.py
+-rw-r--r--   0        0        0     1763 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/handlers/on_fa2_invest_liquidity.py
+-rw-r--r--   0        0        0      573 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/handlers/on_fa2_origination.py
+-rw-r--r--   0        0        0     1604 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/handlers/on_fa2_tez_to_token.py
+-rw-r--r--   0        0        0     1642 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/handlers/on_fa2_token_to_tez.py
+-rw-r--r--   0        0        0     1143 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/handlers/on_fa2_transfer.py
+-rw-r--r--   0        0        0      927 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/handlers/on_fa2_withdraw_profit.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/hasura/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/hooks/.keep
+-rw-r--r--   0        0        0      378 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/models/.keep
+-rw-r--r--   0        0        0      916 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/py.typed
+-rw-r--r--   0        0        0     1507 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/sql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/types/.keep
+-rw-r--r--   0        0        0      340 2024-04-09 23:07:36.419830 dipdup-7.5.4/src/demo_dex/types/fa12_token/tezos_parameters/transfer.py
+-rw-r--r--   0        0        0      714 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_dex/types/fa12_token/tezos_storage.py
+-rw-r--r--   0        0        0      479 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_dex/types/fa2_token/tezos_parameters/transfer.py
+-rw-r--r--   0        0        0     1045 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_dex/types/fa2_token/tezos_storage.py
+-rw-r--r--   0        0        0      311 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_dex/types/quipu_fa12/tezos_parameters/divest_liquidity.py
+-rw-r--r--   0        0        0      201 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_dex/types/quipu_fa12/tezos_parameters/invest_liquidity.py
+-rw-r--r--   0        0        0      297 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_dex/types/quipu_fa12/tezos_parameters/tez_to_token_payment.py
+-rw-r--r--   0        0        0      313 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_dex/types/quipu_fa12/tezos_parameters/token_to_tez_payment.py
+-rw-r--r--   0        0        0      340 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_dex/types/quipu_fa12/tezos_parameters/transfer.py
+-rw-r--r--   0        0        0      199 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_dex/types/quipu_fa12/tezos_parameters/withdraw_profit.py
+-rw-r--r--   0        0        0     1393 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_dex/types/quipu_fa12/tezos_storage.py
+-rw-r--r--   0        0        0      311 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_dex/types/quipu_fa2/tezos_parameters/divest_liquidity.py
+-rw-r--r--   0        0        0      201 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_dex/types/quipu_fa2/tezos_parameters/invest_liquidity.py
+-rw-r--r--   0        0        0      297 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_dex/types/quipu_fa2/tezos_parameters/tez_to_token_payment.py
+-rw-r--r--   0        0        0      313 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_dex/types/quipu_fa2/tezos_parameters/token_to_tez_payment.py
+-rw-r--r--   0        0        0      479 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_dex/types/quipu_fa2/tezos_parameters/transfer.py
+-rw-r--r--   0        0        0      199 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_dex/types/quipu_fa2/tezos_parameters/withdraw_profit.py
+-rw-r--r--   0        0        0     1405 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_dex/types/quipu_fa2/tezos_storage.py
+-rw-r--r--   0        0        0      267 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/.dockerignore
+-rw-r--r--   0        0        0      363 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/.gitignore
+-rw-r--r--   0        0        0       35 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_domains/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      340 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_domains/.ruff_cache/0.3.5/1653114590814564457
+-rw-r--r--   0        0        0      218 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_domains/.ruff_cache/0.3.5/16606089096731248748
+-rw-r--r--   0        0        0      393 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_domains/.ruff_cache/0.3.5/16807837529979951790
+-rw-r--r--   0        0        0      408 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_domains/.ruff_cache/0.3.5/17347659879741306166
+-rw-r--r--   0        0        0       43 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_domains/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      936 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/Makefile
+-rw-r--r--   0        0        0      919 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/abi/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/configs/.keep
+-rw-r--r--   0        0        0      523 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0       73 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      548 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      568 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/configs/replay.yaml
+-rw-r--r--   0        0        0      431 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/deploy/.env.default
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/deploy/.keep
+-rw-r--r--   0        0        0      218 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/deploy/Dockerfile
+-rw-r--r--   0        0        0      363 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2675 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1261 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/deploy/compose.yaml
+-rw-r--r--   0        0        0      242 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      456 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/deploy/swarm.env.default
+-rw-r--r--   0        0        0      893 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/dipdup.yaml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/graphql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/handlers/.keep
+-rw-r--r--   0        0        0     1938 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/handlers/on_update_expiry_map.py
+-rw-r--r--   0        0        0     3286 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/handlers/on_update_records.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/hasura/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/hooks/.keep
+-rw-r--r--   0        0        0      959 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/hooks/check_expiration.py
+-rw-r--r--   0        0        0      378 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/models/.keep
+-rw-r--r--   0        0        0      972 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/py.typed
+-rw-r--r--   0        0        0     1508 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/sql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/types/.keep
+-rw-r--r--   0        0        0      199 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/types/name_registry/tezos_big_maps/store_expiry_map_key.py
+-rw-r--r--   0        0        0      203 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/types/name_registry/tezos_big_maps/store_expiry_map_value.py
+-rw-r--r--   0        0        0      194 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/types/name_registry/tezos_big_maps/store_records_key.py
+-rw-r--r--   0        0        0      427 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_domains/types/name_registry/tezos_big_maps/store_records_value.py
+-rw-r--r--   0        0        0      269 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/.dockerignore
+-rw-r--r--   0        0        0      365 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/.gitignore
+-rw-r--r--   0        0        0       35 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_etherlink/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      146 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_etherlink/.ruff_cache/0.3.5/10680875162971713114
+-rw-r--r--   0        0        0      148 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_etherlink/.ruff_cache/0.3.5/14733888254605228641
+-rw-r--r--   0        0        0      366 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_etherlink/.ruff_cache/0.3.5/15696295736644807429
+-rw-r--r--   0        0        0      204 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_etherlink/.ruff_cache/0.3.5/16350567609703314250
+-rw-r--r--   0        0        0      153 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_etherlink/.ruff_cache/0.3.5/17373343747385769313
+-rw-r--r--   0        0        0      221 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_etherlink/.ruff_cache/0.3.5/4991091694669649063
+-rw-r--r--   0        0        0      164 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_etherlink/.ruff_cache/0.3.5/5886189957198173541
+-rw-r--r--   0        0        0      340 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_etherlink/.ruff_cache/0.3.5/6362157745979274215
+-rw-r--r--   0        0        0      157 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_etherlink/.ruff_cache/0.3.5/77679207932664451
+-rw-r--r--   0        0        0       43 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_etherlink/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      938 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/Makefile
+-rw-r--r--   0        0        0      921 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/abi/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/configs/.keep
+-rw-r--r--   0        0        0      523 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0       75 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      552 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      572 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/configs/replay.yaml
+-rw-r--r--   0        0        0      442 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/deploy/.env.default
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/deploy/.keep
+-rw-r--r--   0        0        0      222 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/deploy/Dockerfile
+-rw-r--r--   0        0        0      367 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2679 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1263 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/deploy/compose.yaml
+-rw-r--r--   0        0        0      255 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      471 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/deploy/swarm.env.default
+-rw-r--r--   0        0        0     1343 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/dipdup.yaml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/graphql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/handlers/.keep
+-rw-r--r--   0        0        0      874 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/handlers/on_deposit.py
+-rw-r--r--   0        0        0      583 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/handlers/on_withdraw.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/hasura/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/hooks/.keep
+-rw-r--r--   0        0        0      378 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/models/.keep
+-rw-r--r--   0        0        0     1241 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/py.typed
+-rw-r--r--   0        0        0     1510 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/sql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/types/.keep
+-rw-r--r--   0        0        0      894 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/types/rollup/tezos_parameters/default.py
+-rw-r--r--   0        0        0      189 2024-04-09 23:07:36.423831 dipdup-7.5.4/src/demo_etherlink/types/rollup/tezos_storage.py
+-rw-r--r--   0        0        0      398 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_etherlink/types/ticket_helper/tezos_parameters/default.py
+-rw-r--r--   0        0        0      744 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_etherlink/types/ticket_helper/tezos_storage.py
+-rw-r--r--   0        0        0      185 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_etherlink/types/ticketer/tezos_parameters/deposit.py
+-rw-r--r--   0        0        0      512 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_etherlink/types/ticketer/tezos_parameters/withdraw.py
+-rw-r--r--   0        0        0      712 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_etherlink/types/ticketer/tezos_storage.py
+-rw-r--r--   0        0        0      266 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/.dockerignore
+-rw-r--r--   0        0        0      362 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/.gitignore
+-rw-r--r--   0        0        0       35 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_events/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      337 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_events/.ruff_cache/0.3.5/17522230860281686467
+-rw-r--r--   0        0        0      274 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_events/.ruff_cache/0.3.5/18079411417655400768
+-rw-r--r--   0        0        0      214 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_events/.ruff_cache/0.3.5/4579253872783291273
+-rw-r--r--   0        0        0      357 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_events/.ruff_cache/0.3.5/6223243106641055953
+-rw-r--r--   0        0        0       43 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_events/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      935 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/Makefile
+-rw-r--r--   0        0        0      909 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/abi/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/configs/.keep
+-rw-r--r--   0        0        0      523 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0       72 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      546 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      557 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/configs/replay.yaml
+-rw-r--r--   0        0        0      402 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/deploy/.env.default
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/deploy/.keep
+-rw-r--r--   0        0        0      216 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/deploy/Dockerfile
+-rw-r--r--   0        0        0      361 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2673 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1260 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/deploy/compose.yaml
+-rw-r--r--   0        0        0      212 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      425 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/deploy/swarm.env.default
+-rw-r--r--   0        0        0      534 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/dipdup.yaml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/graphql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/handlers/.keep
+-rw-r--r--   0        0        0      311 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/handlers/on_move_event.py
+-rw-r--r--   0        0        0      237 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/handlers/on_other_event.py
+-rw-r--r--   0        0        0      311 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/handlers/on_roll_event.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/hasura/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/hooks/.keep
+-rw-r--r--   0        0        0      378 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/models/.keep
+-rw-r--r--   0        0        0     1241 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/py.typed
+-rw-r--r--   0        0        0     1498 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/sql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/types/.keep
+-rw-r--r--   0        0        0      317 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/types/events_contract/tezos_events/move.py
+-rw-r--r--   0        0        0      266 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_events/types/events_contract/tezos_events/roll.py
+-rw-r--r--   0        0        0      270 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/.dockerignore
+-rw-r--r--   0        0        0      366 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/.gitignore
+-rw-r--r--   0        0        0       35 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_evm_events/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      341 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_evm_events/.ruff_cache/0.3.5/12359413407323508229
+-rw-r--r--   0        0        0      141 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_evm_events/.ruff_cache/0.3.5/12709813665789233726
+-rw-r--r--   0        0        0      155 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_evm_events/.ruff_cache/0.3.5/3388611015623138532
+-rw-r--r--   0        0        0      355 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_evm_events/.ruff_cache/0.3.5/9173012470832326414
+-rw-r--r--   0        0        0       43 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_evm_events/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      939 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/Makefile
+-rw-r--r--   0        0        0      927 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/abi/.keep
+-rw-r--r--   0        0        0    11460 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/abi/eth_usdt/abi.json
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/configs/.keep
+-rw-r--r--   0        0        0      523 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0       76 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      554 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      579 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/configs/replay.yaml
+-rw-r--r--   0        0        0      644 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/deploy/.env.default
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/deploy/.keep
+-rw-r--r--   0        0        0      224 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/deploy/Dockerfile
+-rw-r--r--   0        0        0      369 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2681 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1264 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/deploy/compose.yaml
+-rw-r--r--   0        0        0      458 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      675 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/deploy/swarm.env.default
+-rw-r--r--   0        0        0      811 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/dipdup.yaml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/graphql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/handlers/.keep
+-rw-r--r--   0        0        0     1291 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/handlers/on_transfer.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/hasura/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/hooks/.keep
+-rw-r--r--   0        0        0      378 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/models/.keep
+-rw-r--r--   0        0        0      469 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/py.typed
+-rw-r--r--   0        0        0     1516 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/sql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/types/.keep
+-rw-r--r--   0        0        0      331 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_events/types/eth_usdt/evm_events/transfer.py
+-rw-r--r--   0        0        0      276 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_transactions/.dockerignore
+-rw-r--r--   0        0        0      372 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_transactions/.gitignore
+-rw-r--r--   0        0        0       35 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_evm_transactions/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      347 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_evm_transactions/.ruff_cache/0.3.5/10214084676533312387
+-rw-r--r--   0        0        0      162 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_evm_transactions/.ruff_cache/0.3.5/11025955361010972789
+-rw-r--r--   0        0        0      147 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_evm_transactions/.ruff_cache/0.3.5/4447239632156981289
+-rw-r--r--   0        0        0      373 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_evm_transactions/.ruff_cache/0.3.5/8784263686743080453
+-rw-r--r--   0        0        0       43 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_evm_transactions/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      945 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_transactions/Makefile
+-rw-r--r--   0        0        0      935 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_transactions/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_transactions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_transactions/abi/.keep
+-rw-r--r--   0        0        0    11460 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_transactions/abi/eth_usdt/abi.json
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_transactions/configs/.keep
+-rw-r--r--   0        0        0      523 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_transactions/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0       82 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_transactions/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      566 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_transactions/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      593 2024-04-09 23:07:36.427831 dipdup-7.5.4/src/demo_evm_transactions/configs/replay.yaml
+-rw-r--r--   0        0        0      644 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/deploy/.env.default
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/deploy/.keep
+-rw-r--r--   0        0        0      236 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/deploy/Dockerfile
+-rw-r--r--   0        0        0      381 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2693 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1270 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/deploy/compose.yaml
+-rw-r--r--   0        0        0      464 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      687 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/deploy/swarm.env.default
+-rw-r--r--   0        0        0      850 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/dipdup.yaml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/graphql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/handlers/.keep
+-rw-r--r--   0        0        0     1345 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/handlers/on_transfer.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/hasura/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/hooks/.keep
+-rw-r--r--   0        0        0      378 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/models/.keep
+-rw-r--r--   0        0        0      469 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/py.typed
+-rw-r--r--   0        0        0     1524 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/sql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/types/.keep
+-rw-r--r--   0        0        0      262 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_evm_transactions/types/eth_usdt/evm_methods/transfer.py
+-rw-r--r--   0        0        0      269 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/.dockerignore
+-rw-r--r--   0        0        0      365 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/.gitignore
+-rw-r--r--   0        0        0       35 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_factories/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      340 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_factories/.ruff_cache/0.3.5/10233029633647880206
+-rw-r--r--   0        0        0      346 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_factories/.ruff_cache/0.3.5/13737547531499678185
+-rw-r--r--   0        0        0      157 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_factories/.ruff_cache/0.3.5/15342930602428448495
+-rw-r--r--   0        0        0      216 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_factories/.ruff_cache/0.3.5/1630500539198869605
+-rw-r--r--   0        0        0      147 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_factories/.ruff_cache/0.3.5/4826931972718837623
+-rw-r--r--   0        0        0      145 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_factories/.ruff_cache/0.3.5/8761498347916604964
+-rw-r--r--   0        0        0       43 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_factories/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      938 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/Makefile
+-rw-r--r--   0        0        0      924 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/abi/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/configs/.keep
+-rw-r--r--   0        0        0      523 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0       75 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      552 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      575 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/configs/replay.yaml
+-rw-r--r--   0        0        0      431 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/deploy/.env.default
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/deploy/.keep
+-rw-r--r--   0        0        0      222 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/deploy/Dockerfile
+-rw-r--r--   0        0        0      367 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2679 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1263 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/deploy/compose.yaml
+-rw-r--r--   0        0        0      244 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      460 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/deploy/swarm.env.default
+-rw-r--r--   0        0        0     1090 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/dipdup.yaml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/graphql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/handlers/.keep
+-rw-r--r--   0        0        0     1082 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/handlers/on_factory_origination.py
+-rw-r--r--   0        0        0      658 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/handlers/on_transfer.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/hasura/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/hooks/.keep
+-rw-r--r--   0        0        0      378 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/models/.keep
+-rw-r--r--   0        0        0      208 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/py.typed
+-rw-r--r--   0        0        0     1513 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/sql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/types/.keep
+-rw-r--r--   0        0        0     1355 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/types/factory/tezos_storage.py
+-rw-r--r--   0        0        0      479 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/types/token/tezos_parameters/transfer.py
+-rw-r--r--   0        0        0     1128 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_factories/types/token/tezos_storage.py
+-rw-r--r--   0        0        0      264 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/.dockerignore
+-rw-r--r--   0        0        0      360 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/.gitignore
+-rw-r--r--   0        0        0       35 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_head/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      335 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_head/.ruff_cache/0.3.5/15227884898265811517
+-rw-r--r--   0        0        0      351 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_head/.ruff_cache/0.3.5/4633362819611091641
+-rw-r--r--   0        0        0      139 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_head/.ruff_cache/0.3.5/9051252982318253170
+-rw-r--r--   0        0        0       43 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_head/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      933 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/Makefile
+-rw-r--r--   0        0        0      927 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/abi/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/configs/.keep
+-rw-r--r--   0        0        0      523 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0       70 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      542 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      573 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/configs/replay.yaml
+-rw-r--r--   0        0        0      431 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/deploy/.env.default
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/deploy/.keep
+-rw-r--r--   0        0        0      212 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/deploy/Dockerfile
+-rw-r--r--   0        0        0      357 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2669 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1258 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/deploy/compose.yaml
+-rw-r--r--   0        0        0      239 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      450 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/deploy/swarm.env.default
+-rw-r--r--   0        0        0      240 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/dipdup.yaml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/graphql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/handlers/.keep
+-rw-r--r--   0        0        0      237 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/handlers/on_mainnet_head.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/hasura/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/hooks/.keep
+-rw-r--r--   0        0        0      378 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/models/.keep
+-rw-r--r--   0        0        0     1241 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/py.typed
+-rw-r--r--   0        0        0     1516 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.431831 dipdup-7.5.4/src/demo_head/sql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_head/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_head/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_head/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_head/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_head/types/.keep
+-rw-r--r--   0        0        0      275 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/.dockerignore
+-rw-r--r--   0        0        0      371 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/.gitignore
+-rw-r--r--   0        0        0       35 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_nft_marketplace/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      156 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_nft_marketplace/.ruff_cache/0.3.5/12829316766635429555
+-rw-r--r--   0        0        0      354 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_nft_marketplace/.ruff_cache/0.3.5/16523667269463482759
+-rw-r--r--   0        0        0      156 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_nft_marketplace/.ruff_cache/0.3.5/1657943231965107365
+-rw-r--r--   0        0        0      392 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_nft_marketplace/.ruff_cache/0.3.5/17775571669347730701
+-rw-r--r--   0        0        0      335 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_nft_marketplace/.ruff_cache/0.3.5/3914317717543688300
+-rw-r--r--   0        0        0      164 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_nft_marketplace/.ruff_cache/0.3.5/4286445595740083944
+-rw-r--r--   0        0        0      346 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_nft_marketplace/.ruff_cache/0.3.5/6687226130600904613
+-rw-r--r--   0        0        0       43 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_nft_marketplace/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      944 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/Makefile
+-rw-r--r--   0        0        0      921 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/abi/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/configs/.keep
+-rw-r--r--   0        0        0      523 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0       81 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      564 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      578 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/configs/replay.yaml
+-rw-r--r--   0        0        0      527 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/deploy/.env.default
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/deploy/.keep
+-rw-r--r--   0        0        0      234 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/deploy/Dockerfile
+-rw-r--r--   0        0        0      379 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2691 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1269 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/deploy/compose.yaml
+-rw-r--r--   0        0        0      346 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      568 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/deploy/swarm.env.default
+-rw-r--r--   0        0        0     1199 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/dipdup.yaml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/graphql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/handlers/.keep
+-rw-r--r--   0        0        0      605 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/handlers/on_cancel_swap.py
+-rw-r--r--   0        0        0     1037 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/handlers/on_collect.py
+-rw-r--r--   0        0        0      977 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/handlers/on_mint.py
+-rw-r--r--   0        0        0      885 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/handlers/on_swap.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/hasura/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/hooks/.keep
+-rw-r--r--   0        0        0      378 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/models/.keep
+-rw-r--r--   0        0        0     1306 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/py.typed
+-rw-r--r--   0        0        0     1510 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/sql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/types/.keep
+-rw-r--r--   0        0        0      192 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/cancel_swap.py
+-rw-r--r--   0        0        0      281 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/collect.py
+-rw-r--r--   0        0        0      317 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/mint_objkt.py
+-rw-r--r--   0        0        0      299 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/swap.py
+-rw-r--r--   0        0        0      752 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/types/hen_minter/tezos_storage.py
+-rw-r--r--   0        0        0      318 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/types/hen_objkts/tezos_parameters/mint.py
+-rw-r--r--   0        0        0     1046 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_nft_marketplace/types/hen_objkts/tezos_storage.py
+-rw-r--r--   0        0        0      263 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/.dockerignore
+-rw-r--r--   0        0        0      359 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/.gitignore
+-rw-r--r--   0        0        0       35 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_raw/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      386 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_raw/.ruff_cache/0.3.5/13422843267514079142
+-rw-r--r--   0        0        0      135 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_raw/.ruff_cache/0.3.5/4945642387082377418
+-rw-r--r--   0        0        0      334 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_raw/.ruff_cache/0.3.5/5420026911396989035
+-rw-r--r--   0        0        0       43 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_raw/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      932 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/Makefile
+-rw-r--r--   0        0        0      939 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/abi/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/configs/.keep
+-rw-r--r--   0        0        0      523 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0       69 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      540 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      584 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/configs/replay.yaml
+-rw-r--r--   0        0        0      431 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/deploy/.env.default
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/deploy/.keep
+-rw-r--r--   0        0        0      210 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/deploy/Dockerfile
+-rw-r--r--   0        0        0      355 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2667 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1257 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/deploy/compose.yaml
+-rw-r--r--   0        0        0      238 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      448 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/deploy/swarm.env.default
+-rw-r--r--   0        0        0      411 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/dipdup.yaml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/graphql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/handlers/.keep
+-rw-r--r--   0        0        0      350 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/handlers/on_operation.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/hasura/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/hooks/.keep
+-rw-r--r--   0        0        0      378 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/models/.keep
+-rw-r--r--   0        0        0      245 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/py.typed
+-rw-r--r--   0        0        0     1528 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/sql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_raw/types/.keep
+-rw-r--r--   0        0        0      265 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_token/.dockerignore
+-rw-r--r--   0        0        0      361 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_token/.gitignore
+-rw-r--r--   0        0        0       35 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_token/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      336 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_token/.ruff_cache/0.3.5/13449091145025056738
+-rw-r--r--   0        0        0      211 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_token/.ruff_cache/0.3.5/14962660535470023419
+-rw-r--r--   0        0        0      268 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_token/.ruff_cache/0.3.5/15801236650718996476
+-rw-r--r--   0        0        0      141 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_token/.ruff_cache/0.3.5/18041563092892658553
+-rw-r--r--   0        0        0      334 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_token/.ruff_cache/0.3.5/8788930368301803615
+-rw-r--r--   0        0        0       43 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_token/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      934 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_token/Makefile
+-rw-r--r--   0        0        0      913 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_token/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_token/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_token/abi/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_token/configs/.keep
+-rw-r--r--   0        0        0      523 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_token/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0       71 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_token/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      544 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_token/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      560 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_token/configs/replay.yaml
+-rw-r--r--   0        0        0      402 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_token/deploy/.env.default
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.435831 dipdup-7.5.4/src/demo_token/deploy/.keep
+-rw-r--r--   0        0        0      214 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/deploy/Dockerfile
+-rw-r--r--   0        0        0      359 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2671 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1259 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/deploy/compose.yaml
+-rw-r--r--   0        0        0      211 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      423 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/deploy/swarm.env.default
+-rw-r--r--   0        0        0      730 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/dipdup.yaml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/graphql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/handlers/.keep
+-rw-r--r--   0        0        0      436 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/handlers/on_balance_update.py
+-rw-r--r--   0        0        0      630 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/handlers/on_mint.py
+-rw-r--r--   0        0        0      928 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/handlers/on_transfer.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/hasura/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/hooks/.keep
+-rw-r--r--   0        0        0      378 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/models/.keep
+-rw-r--r--   0        0        0      370 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/py.typed
+-rw-r--r--   0        0        0     1502 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/sql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/types/.keep
+-rw-r--r--   0        0        0      263 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/types/tzbtc/tezos_parameters/mint.py
+-rw-r--r--   0        0        0      340 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/types/tzbtc/tezos_parameters/transfer.py
+-rw-r--r--   0        0        0      373 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token/types/tzbtc/tezos_storage.py
+-rw-r--r--   0        0        0      274 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/.dockerignore
+-rw-r--r--   0        0        0      370 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/.gitignore
+-rw-r--r--   0        0        0       35 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_token_balances/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      361 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_token_balances/.ruff_cache/0.3.5/12311832164475855171
+-rw-r--r--   0        0        0      345 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_token_balances/.ruff_cache/0.3.5/5209994484446011581
+-rw-r--r--   0        0        0      151 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_token_balances/.ruff_cache/0.3.5/9107185036162072710
+-rw-r--r--   0        0        0       43 2024-04-09 23:08:35.676277 dipdup-7.5.4/src/demo_token_balances/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      943 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/Makefile
+-rw-r--r--   0        0        0      911 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/abi/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/configs/.keep
+-rw-r--r--   0        0        0      523 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0       80 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      562 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      567 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/configs/replay.yaml
+-rw-r--r--   0        0        0      402 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/deploy/.env.default
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/deploy/.keep
+-rw-r--r--   0        0        0      232 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/deploy/Dockerfile
+-rw-r--r--   0        0        0      377 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2689 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1268 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/deploy/compose.yaml
+-rw-r--r--   0        0        0      220 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      441 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/deploy/swarm.env.default
+-rw-r--r--   0        0        0      407 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/dipdup.yaml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/graphql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/handlers/.keep
+-rw-r--r--   0        0        0      472 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/handlers/on_balance_update.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/hasura/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/hooks/.keep
+-rw-r--r--   0        0        0      378 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/models/.keep
+-rw-r--r--   0        0        0      198 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/py.typed
+-rw-r--r--   0        0        0     1500 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/sql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_balances/types/.keep
+-rw-r--r--   0        0        0      275 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/.dockerignore
+-rw-r--r--   0        0        0      371 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/.gitignore
+-rw-r--r--   0        0        0       35 2024-04-09 23:08:35.680278 dipdup-7.5.4/src/demo_token_transfers/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      364 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_token_transfers/.ruff_cache/0.3.5/10175264658608344443
+-rw-r--r--   0        0        0      223 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_token_transfers/.ruff_cache/0.3.5/13076229559559773055
+-rw-r--r--   0        0        0      346 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_token_transfers/.ruff_cache/0.3.5/17353147022194868752
+-rw-r--r--   0        0        0       43 2024-04-09 23:08:35.680278 dipdup-7.5.4/src/demo_token_transfers/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      944 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/Makefile
+-rw-r--r--   0        0        0      913 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/abi/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/configs/.keep
+-rw-r--r--   0        0        0      523 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0       81 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      564 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      570 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/configs/replay.yaml
+-rw-r--r--   0        0        0      402 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/deploy/.env.default
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/deploy/.keep
+-rw-r--r--   0        0        0      234 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/deploy/Dockerfile
+-rw-r--r--   0        0        0      379 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2691 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1269 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/deploy/compose.yaml
+-rw-r--r--   0        0        0      221 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      443 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/deploy/swarm.env.default
+-rw-r--r--   0        0        0      409 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/dipdup.yaml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/graphql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/handlers/.keep
+-rw-r--r--   0        0        0      545 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/handlers/on_balance_update.py
+-rw-r--r--   0        0        0      836 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/handlers/on_token_transfer.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/hasura/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/hooks/.keep
+-rw-r--r--   0        0        0      378 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/models/.keep
+-rw-r--r--   0        0        0      370 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/py.typed
+-rw-r--r--   0        0        0     1502 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/sql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.439831 dipdup-7.5.4/src/demo_token_transfers/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_token_transfers/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_token_transfers/types/.keep
+-rw-r--r--   0        0        0      267 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/.dockerignore
+-rw-r--r--   0        0        0      363 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/.gitignore
+-rw-r--r--   0        0        0       35 2024-04-09 23:08:35.680278 dipdup-7.5.4/src/demo_uniswap/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      357 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_uniswap/.ruff_cache/0.3.5/16152085020556079584
+-rw-r--r--   0        0        0      147 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_uniswap/.ruff_cache/0.3.5/17660790964988697818
+-rw-r--r--   0        0        0      444 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_uniswap/.ruff_cache/0.3.5/2170990585853492345
+-rw-r--r--   0        0        0      155 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_uniswap/.ruff_cache/0.3.5/3477470057356153740
+-rw-r--r--   0        0        0      375 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_uniswap/.ruff_cache/0.3.5/3758205171147508537
+-rw-r--r--   0        0        0      365 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_uniswap/.ruff_cache/0.3.5/6172317202976927728
+-rw-r--r--   0        0        0     2471 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_uniswap/.ruff_cache/0.3.5/7681863458869765244
+-rw-r--r--   0        0        0      338 2024-04-09 23:08:35.724278 dipdup-7.5.4/src/demo_uniswap/.ruff_cache/0.3.5/8650910402495689490
+-rw-r--r--   0        0        0       43 2024-04-09 23:08:35.680278 dipdup-7.5.4/src/demo_uniswap/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      936 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/Makefile
+-rw-r--r--   0        0        0      946 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/abi/.keep
+-rw-r--r--   0        0        0     3684 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/abi/erc20/ERC20.json
+-rw-r--r--   0        0        0      268 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/abi/erc20/ERC20NameBytes.json
+-rw-r--r--   0        0        0      270 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/abi/erc20/ERC20SymbolBytes.json
+-rw-r--r--   0        0        0     4418 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/abi/factory/abi.json
+-rw-r--r--   0        0        0    19609 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/abi/pool/abi.json
+-rw-r--r--   0        0        0    24313 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/abi/position_manager/abi.json
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/configs/.keep
+-rw-r--r--   0        0        0      523 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0       73 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      548 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      615 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/configs/replay.yaml
+-rw-r--r--   0        0        0      644 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/deploy/.env.default
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/deploy/.keep
+-rw-r--r--   0        0        0      218 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/deploy/Dockerfile
+-rw-r--r--   0        0        0      363 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2695 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1281 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/deploy/compose.yaml
+-rw-r--r--   0        0        0      455 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      669 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/deploy/swarm.env.default
+-rw-r--r--   0        0        0     2039 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/dipdup.yaml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/graphql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/handlers/.keep
+-rw-r--r--   0        0        0     2668 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/handlers/factory/pool_created.py
+-rw-r--r--   0        0        0      531 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/handlers/pool/burn.py
+-rw-r--r--   0        0        0      291 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/handlers/pool/flash.py
+-rw-r--r--   0        0        0      871 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/handlers/pool/initialize.py
+-rw-r--r--   0        0        0     1329 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/handlers/pool/mint.py
+-rw-r--r--   0        0        0     6569 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/handlers/pool/swap.py
+-rw-r--r--   0        0        0     1249 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/handlers/position_manager/collect.py
+-rw-r--r--   0        0        0     1383 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/handlers/position_manager/decrease_liquidity.py
+-rw-r--r--   0        0        0     1471 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/handlers/position_manager/increase_liquidity.py
+-rw-r--r--   0        0        0     1367 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/handlers/position_manager/transfer.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/hasura/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/hooks/.keep
+-rw-r--r--   0        0        0      378 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/models/.keep
+-rw-r--r--   0        0        0    19956 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/models/__init__.py
+-rw-r--r--   0        0        0      373 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/models/abi.py
+-rw-r--r--   0        0        0     4207 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/models/pool.py
+-rw-r--r--   0        0        0     2831 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/models/position.py
+-rw-r--r--   0        0        0     1452 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/models/repo.py
+-rw-r--r--   0        0        0      577 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/models/tick.py
+-rw-r--r--   0        0        0     7140 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/models/token.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/py.typed
+-rw-r--r--   0        0        0     1535 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/sql/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/sql/on_reindex/.keep
+-rw-r--r--   0        0        0      225 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/sql/on_reindex/00_prepare_db.sql
+-rw-r--r--   0        0        0      792 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/sql/on_reindex/20_create_ca_quotes_1m.sql
+-rw-r--r--   0        0        0      788 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/sql/on_reindex/21_create_ca_quotes_1h.sql
+-rw-r--r--   0        0        0      787 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/sql/on_reindex/22_create_ca_quotes_1d.sql
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/types/.keep
+-rw-r--r--   0        0        0      321 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/types/factory/evm_events/pool_created.py
+-rw-r--r--   0        0        0      330 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/types/pool/evm_events/burn.py
+-rw-r--r--   0        0        0      339 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/types/pool/evm_events/collect.py
+-rw-r--r--   0        0        0      328 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/types/pool/evm_events/flash.py
+-rw-r--r--   0        0        0      275 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/types/pool/evm_events/initialize.py
+-rw-r--r--   0        0        0      346 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/types/pool/evm_events/mint.py
+-rw-r--r--   0        0        0      351 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/types/pool/evm_events/swap.py
+-rw-r--r--   0        0        0      303 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/types/position_manager/evm_events/collect.py
+-rw-r--r--   0        0        0      323 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/types/position_manager/evm_events/decrease_liquidity.py
+-rw-r--r--   0        0        0      323 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/types/position_manager/evm_events/increase_liquidity.py
+-rw-r--r--   0        0        0      333 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/demo_uniswap/types/position_manager/evm_events/transfer.py
+-rw-r--r--   0        0        0      180 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/dipdup/__init__.py
+-rw-r--r--   0        0        0      105 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/dipdup/__main__.py
+-rw-r--r--   0        0        0     1989 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/dipdup/api.py
+-rw-r--r--   0        0        0    25974 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/dipdup/cli.py
+-rw-r--r--   0        0        0     7935 2024-04-09 23:07:36.443831 dipdup-7.5.4/src/dipdup/codegen/__init__.py
+-rw-r--r--   0        0        0     9399 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/codegen/evm_subsquid.py
+-rw-r--r--   0        0        0    19380 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/codegen/tezos_tzkt.py
+-rw-r--r--   0        0        0    45163 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/config/__init__.py
+-rw-r--r--   0        0        0      709 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/config/abi_etherscan.py
+-rw-r--r--   0        0        0      802 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/config/coinbase.py
+-rw-r--r--   0        0        0     1555 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/config/evm.py
+-rw-r--r--   0        0        0     1354 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/config/evm_node.py
+-rw-r--r--   0        0        0     1863 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/config/evm_subsquid.py
+-rw-r--r--   0        0        0     2912 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/config/evm_subsquid_events.py
+-rw-r--r--   0        0        0      969 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/config/evm_subsquid_traces.py
+-rw-r--r--   0        0        0     3569 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/config/evm_subsquid_transactions.py
+-rw-r--r--   0        0        0      558 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/config/http.py
+-rw-r--r--   0        0        0      631 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/config/ipfs.py
+-rw-r--r--   0        0        0     2121 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/config/tezos.py
+-rw-r--r--   0        0        0     2455 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/config/tezos_tzkt.py
+-rw-r--r--   0        0        0     3993 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/config/tezos_tzkt_big_maps.py
+-rw-r--r--   0        0        0     3362 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/config/tezos_tzkt_events.py
+-rw-r--r--   0        0        0     1689 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/config/tezos_tzkt_head.py
+-rw-r--r--   0        0        0    15312 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/config/tezos_tzkt_operations.py
+-rw-r--r--   0        0        0     2871 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/config/tezos_tzkt_token_balances.py
+-rw-r--r--   0        0        0     3293 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/config/tezos_tzkt_token_transfers.py
+-rw-r--r--   0        0        0      857 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/config/tzip_metadata.py
+-rw-r--r--   0        0        0    30143 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/context.py
+-rw-r--r--   0        0        0    15587 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/database.py
+-rw-r--r--   0        0        0     5524 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/datasources/__init__.py
+-rw-r--r--   0        0        0     1680 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/datasources/abi_etherscan.py
+-rw-r--r--   0        0        0     2251 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/datasources/coinbase.py
+-rw-r--r--   0        0        0    16246 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/datasources/evm_node.py
+-rw-r--r--   0        0        0     8233 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/datasources/evm_subsquid.py
+-rw-r--r--   0        0        0      399 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/datasources/http.py
+-rw-r--r--   0        0        0      524 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/datasources/ipfs.py
+-rw-r--r--   0        0        0    48706 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/datasources/tezos_tzkt.py
+-rw-r--r--   0        0        0     1545 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/datasources/tzip_metadata.py
+-rw-r--r--   0        0        0    34239 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/dipdup.py
+-rw-r--r--   0        0        0     3175 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/env.py
+-rw-r--r--   0        0        0     8666 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/exceptions.py
+-rw-r--r--   0        0        0     4447 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/fetcher.py
+-rw-r--r--   0        0        0     6780 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/fields.py
+-rw-r--r--   0        0        0    26459 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/hasura.py
+-rw-r--r--   0        0        0    10860 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/http.py
+-rw-r--r--   0        0        0    10261 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/index.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/indexes/__init__.py
+-rw-r--r--   0        0        0     2827 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/indexes/evm_node.py
+-rw-r--r--   0        0        0     5726 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/indexes/evm_subsquid.py
+-rw-r--r--   0        0        0     3664 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/indexes/evm_subsquid_events/fetcher.py
+-rw-r--r--   0        0        0     4780 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/indexes/evm_subsquid_events/index.py
+-rw-r--r--   0        0        0     3741 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/indexes/evm_subsquid_events/matcher.py
+-rw-r--r--   0        0        0      266 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/indexes/evm_subsquid_traces/fetcher.py
+-rw-r--r--   0        0        0      560 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/indexes/evm_subsquid_traces/index.py
+-rw-r--r--   0        0        0        4 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/indexes/evm_subsquid_traces/matcher.py
+-rw-r--r--   0        0        0     3444 2024-04-09 23:07:36.447831 dipdup-7.5.4/src/dipdup/indexes/evm_subsquid_transactions/fetcher.py
+-rw-r--r--   0        0        0     3802 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/evm_subsquid_transactions/index.py
+-rw-r--r--   0        0        0     3967 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/evm_subsquid_transactions/matcher.py
+-rw-r--r--   0        0        0      497 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_big_maps/__init__.py
+-rw-r--r--   0        0        0     3160 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_big_maps/fetcher.py
+-rw-r--r--   0        0        0     5061 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_big_maps/index.py
+-rw-r--r--   0        0        0     2659 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_big_maps/matcher.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_events/__init__.py
+-rw-r--r--   0        0        0     1363 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_events/fetcher.py
+-rw-r--r--   0        0        0     3446 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_events/index.py
+-rw-r--r--   0        0        0     3781 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_events/matcher.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_head/__init__.py
+-rw-r--r--   0        0        0     2679 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_head/index.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_operations/__init__.py
+-rw-r--r--   0        0        0    23285 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_operations/fetcher.py
+-rw-r--r--   0        0        0    13692 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_operations/index.py
+-rw-r--r--   0        0        0    10443 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_operations/matcher.py
+-rw-r--r--   0        0        0     7554 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_operations/parser.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_token_balances/__init__.py
+-rw-r--r--   0        0        0     2753 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_token_balances/index.py
+-rw-r--r--   0        0        0     1545 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_token_balances/matcher.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_token_transfers/__init__.py
+-rw-r--r--   0        0        0     1576 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_token_transfers/fetcher.py
+-rw-r--r--   0        0        0     3209 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_token_transfers/index.py
+-rw-r--r--   0        0        0     1817 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_token_transfers/matcher.py
+-rwxr-xr-x   0        0        0     9239 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/install.py
+-rw-r--r--   0        0        0    22316 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/models/__init__.py
+-rw-r--r--   0        0        0     1240 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/models/coinbase.py
+-rw-r--r--   0        0        0     6463 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/models/evm_node.py
+-rw-r--r--   0        0        0     8462 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/models/evm_subsquid.py
+-rw-r--r--   0        0        0    24947 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/models/tezos_tzkt.py
+-rw-r--r--   0        0        0      407 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/models/tzip_metadata.py
+-rw-r--r--   0        0        0     7216 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/package.py
+-rw-r--r--   0        0        0     6265 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/performance.py
+-rw-r--r--   0        0        0    10232 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/project.py
+-rw-r--r--   0        0        0      277 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/base/.dockerignore.j2
+-rw-r--r--   0        0        0      372 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/base/.gitignore.j2
+-rw-r--r--   0        0        0      945 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/base/Makefile.j2
+-rw-r--r--   0        0        0     1061 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/base/README.md.j2
+-rw-r--r--   0        0        0      524 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/base/configs/dipdup.compose.yaml.j2
+-rw-r--r--   0        0        0       82 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/base/configs/dipdup.sqlite.yaml.j2
+-rw-r--r--   0        0        0      567 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/base/configs/dipdup.swarm.yaml.j2
+-rw-r--r--   0        0        0      291 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/base/deploy/Dockerfile.j2
+-rw-r--r--   0        0        0      382 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/base/deploy/compose.sqlite.yaml.j2
+-rw-r--r--   0        0        0     2744 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/base/deploy/compose.swarm.yaml.j2
+-rw-r--r--   0        0        0     1294 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/base/deploy/compose.yaml.j2
+-rw-r--r--   0        0        0     2849 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/base/pyproject.toml.j2
+-rw-r--r--   0        0        0     1087 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_auction/dipdup.yaml.j2
+-rw-r--r--   0        0        0      935 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_auction/handlers/on_bid.py.j2
+-rw-r--r--   0        0        0     1641 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_auction/handlers/on_create_auction.py.j2
+-rw-r--r--   0        0        0      734 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_auction/handlers/on_withdraw.py.j2
+-rw-r--r--   0        0        0     1447 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_auction/models/__init__.py.j2
+-rw-r--r--   0        0        0      116 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_auction/replay.yaml
+-rw-r--r--   0        0        0      734 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_big_maps/dipdup.yaml.j2
+-rw-r--r--   0        0        0      865 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_big_maps/handlers/on_update_expiry_map.py.j2
+-rw-r--r--   0        0        0     1709 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_big_maps/handlers/on_update_records.py.j2
+-rw-r--r--   0        0        0      669 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_big_maps/models/__init__.py.j2
+-rw-r--r--   0        0        0      118 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_big_maps/replay.yaml
+-rw-r--r--   0        0        0       49 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_blank/dipdup.yaml.j2
+-rw-r--r--   0        0        0      116 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_blank/replay.yaml
+-rw-r--r--   0        0        0      657 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_dao/dipdup.yaml.j2
+-rw-r--r--   0        0        0      431 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_dao/handlers/on_origination.py.j2
+-rw-r--r--   0        0        0      540 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_dao/handlers/on_propose.py.j2
+-rw-r--r--   0        0        0      784 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_dao/models/__init__.py.j2
+-rw-r--r--   0        0        0      109 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_dao/replay.yaml
+-rw-r--r--   0        0        0     4859 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_dex/dipdup.yaml.j2
+-rw-r--r--   0        0        0     1885 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa12_divest_liquidity.py.j2
+-rw-r--r--   0        0        0     1793 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa12_invest_liquidity.py.j2
+-rw-r--r--   0        0        0      602 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa12_origination.py.j2
+-rw-r--r--   0        0        0     1666 2024-04-09 23:07:36.451831 dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa12_tez_to_token.py.j2
+-rw-r--r--   0        0        0     1732 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa12_token_to_tez.py.j2
+-rw-r--r--   0        0        0     1056 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa12_transfer.py.j2
+-rw-r--r--   0        0        0      993 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa12_withdraw_profit.py.j2
+-rw-r--r--   0        0        0     1911 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa2_divest_liquidity.py.j2
+-rw-r--r--   0        0        0     1819 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa2_invest_liquidity.py.j2
+-rw-r--r--   0        0        0      596 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa2_origination.py.j2
+-rw-r--r--   0        0        0     1660 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa2_tez_to_token.py.j2
+-rw-r--r--   0        0        0     1698 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa2_token_to_tez.py.j2
+-rw-r--r--   0        0        0     1177 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa2_transfer.py.j2
+-rw-r--r--   0        0        0      989 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa2_withdraw_profit.py.j2
+-rw-r--r--   0        0        0      918 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_dex/models/__init__.py.j2
+-rw-r--r--   0        0        0      120 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_dex/replay.yaml
+-rw-r--r--   0        0        0      903 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_domains/dipdup.yaml.j2
+-rw-r--r--   0        0        0     1967 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_domains/handlers/on_update_expiry_map.py.j2
+-rw-r--r--   0        0        0     3314 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_domains/handlers/on_update_records.py.j2
+-rw-r--r--   0        0        0      968 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_domains/hooks/check_expiration.py.j2
+-rw-r--r--   0        0        0      972 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_domains/models/__init__.py.j2
+-rw-r--r--   0        0        0      125 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_domains/replay.yaml
+-rw-r--r--   0        0        0     1343 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_etherlink/dipdup.yaml.j2
+-rw-r--r--   0        0        0      129 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_etherlink/replay.yaml
+-rw-r--r--   0        0        0      545 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_events/dipdup.yaml.j2
+-rw-r--r--   0        0        0      114 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_events/replay.yaml
+-rw-r--r--   0        0        0      818 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_evm_events/dipdup.yaml.j2
+-rw-r--r--   0        0        0     1305 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_evm_events/handlers/on_transfer.py.j2
+-rw-r--r--   0        0        0      470 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_evm_events/models/__init__.py.j2
+-rw-r--r--   0        0        0      136 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_evm_events/replay.yaml
+-rw-r--r--   0        0        0      851 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_evm_transactions/dipdup.yaml.j2
+-rw-r--r--   0        0        0     1346 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_evm_transactions/handlers/on_transfer.py.j2
+-rw-r--r--   0        0        0      470 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_evm_transactions/models/__init__.py.j2
+-rw-r--r--   0        0        0      150 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_evm_transactions/replay.yaml
+-rw-r--r--   0        0        0     1098 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_factories/dipdup.yaml.j2
+-rw-r--r--   0        0        0     1082 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_factories/handlers/on_factory_origination.py.j2
+-rw-r--r--   0        0        0      681 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_factories/handlers/on_transfer.py.j2
+-rw-r--r--   0        0        0      214 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_factories/models/__init__.py.j2
+-rw-r--r--   0        0        0      132 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_factories/replay.yaml
+-rw-r--r--   0        0        0      253 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_head/dipdup.yaml.j2
+-rw-r--r--   0        0        0      130 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_head/replay.yaml
+-rw-r--r--   0        0        0     1201 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_nft_marketplace/dipdup.yaml.j2
+-rw-r--r--   0        0        0      603 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_nft_marketplace/handlers/on_cancel_swap.py.j2
+-rw-r--r--   0        0        0     1035 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_nft_marketplace/handlers/on_collect.py.j2
+-rw-r--r--   0        0        0      973 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_nft_marketplace/handlers/on_mint.py.j2
+-rw-r--r--   0        0        0      883 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_nft_marketplace/handlers/on_swap.py.j2
+-rw-r--r--   0        0        0     1309 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_nft_marketplace/models/__init__.py.j2
+-rw-r--r--   0        0        0      135 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_nft_marketplace/replay.yaml
+-rw-r--r--   0        0        0      425 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_raw/dipdup.yaml.j2
+-rw-r--r--   0        0        0      364 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_raw/handlers/on_operation.py.j2
+-rw-r--r--   0        0        0      247 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_raw/models/__init__.py.j2
+-rw-r--r--   0        0        0      141 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_raw/replay.yaml
+-rw-r--r--   0        0        0      742 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_token/dipdup.yaml.j2
+-rw-r--r--   0        0        0      448 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_token/handlers/on_balance_update.py.j2
+-rw-r--r--   0        0        0      664 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_token/handlers/on_mint.py.j2
+-rw-r--r--   0        0        0      962 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_token/handlers/on_transfer.py.j2
+-rw-r--r--   0        0        0      372 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_token/models/__init__.py.j2
+-rw-r--r--   0        0        0      117 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_token/replay.yaml
+-rw-r--r--   0        0        0      410 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_token_balances/dipdup.yaml.j2
+-rw-r--r--   0        0        0      473 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_token_balances/handlers/on_balance_update.py.j2
+-rw-r--r--   0        0        0      200 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_token_balances/models/__init__.py.j2
+-rw-r--r--   0        0        0      124 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_token_balances/replay.yaml
+-rw-r--r--   0        0        0      411 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_token_transfers/dipdup.yaml.j2
+-rw-r--r--   0        0        0      545 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_token_transfers/handlers/on_balance_update.py.j2
+-rw-r--r--   0        0        0      836 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_token_transfers/handlers/on_token_transfer.py.j2
+-rw-r--r--   0        0        0      372 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_token_transfers/models/__init__.py.j2
+-rw-r--r--   0        0        0      127 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_token_transfers/replay.yaml
+-rw-r--r--   0        0        0     3685 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/abi/erc20/ERC20.json.j2
+-rw-r--r--   0        0        0      269 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/abi/erc20/ERC20NameBytes.json.j2
+-rw-r--r--   0        0        0      271 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/abi/erc20/ERC20SymbolBytes.json.j2
+-rw-r--r--   0        0        0     2049 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/dipdup.yaml.j2
+-rw-r--r--   0        0        0     2711 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/handlers/factory/pool_created.py.j2
+-rw-r--r--   0        0        0      567 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/handlers/pool/burn.py.j2
+-rw-r--r--   0        0        0      309 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/handlers/pool/flash.py.j2
+-rw-r--r--   0        0        0      898 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/handlers/pool/initialize.py.j2
+-rw-r--r--   0        0        0     1375 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/handlers/pool/mint.py.j2
+-rw-r--r--   0        0        0     6641 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/handlers/pool/swap.py.j2
+-rw-r--r--   0        0        0     1286 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/handlers/position_manager/collect.py.j2
+-rw-r--r--   0        0        0     1420 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/handlers/position_manager/decrease_liquidity.py.j2
+-rw-r--r--   0        0        0     1508 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/handlers/position_manager/increase_liquidity.py.j2
+-rw-r--r--   0        0        0     1405 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/handlers/position_manager/transfer.py.j2
+-rw-r--r--   0        0        0    19957 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/models/__init__.py.j2
+-rw-r--r--   0        0        0      373 2024-04-09 23:07:36.455831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/models/abi.py.j2
+-rw-r--r--   0        0        0     4269 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/models/pool.py.j2
+-rw-r--r--   0        0        0     2849 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/models/position.py.j2
+-rw-r--r--   0        0        0     1461 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/models/repo.py.j2
+-rw-r--r--   0        0        0      586 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/models/tick.py.j2
+-rw-r--r--   0        0        0     7167 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/models/token.py.j2
+-rw-r--r--   0        0        0      250 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/replay.yaml
+-rw-r--r--   0        0        0      226 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/sql/on_reindex/00_prepare_db.sql.j2
+-rw-r--r--   0        0        0      793 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/sql/on_reindex/20_create_ca_quotes_1m.sql.j2
+-rw-r--r--   0        0        0      789 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/sql/on_reindex/21_create_ca_quotes_1h.sql.j2
+-rw-r--r--   0        0        0      788 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/projects/demo_uniswap/sql/on_reindex/22_create_ca_quotes_1d.sql.j2
+-rw-r--r--   0        0        0     4126 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/prometheus.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/py.typed
+-rw-r--r--   0        0        0     1774 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/pysignalr.py
+-rw-r--r--   0        0        0     2147 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/report.py
+-rw-r--r--   0        0        0     4938 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/scheduler.py
+-rw-r--r--   0        0        0     4598 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/sentry.py
+-rw-r--r--   0        0        0      272 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/sql/dipdup_approve.sql
+-rw-r--r--   0        0        0      199 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/sql/dipdup_head_status.sql
+-rw-r--r--   0        0        0     1904 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/sql/dipdup_wipe.sql
+-rw-r--r--   0        0        0     2077 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/subscriptions.py
+-rw-r--r--   0        0        0     2227 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/sys.py
+-rw-r--r--   0        0        0      227 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/templates/callback.py.j2
+-rw-r--r--   0        0        0     1241 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/templates/models.py
+-rw-r--r--   0        0        0      276 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/templates/replay.yaml.j2
+-rw-r--r--   0        0        0     6532 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/test.py
+-rw-r--r--   0        0        0     3017 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/transactions.py
+-rw-r--r--   0        0        0     7610 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/utils.py
+-rw-r--r--   0        0        0     5500 2024-04-09 23:07:36.459831 dipdup-7.5.4/src/dipdup/yaml.py
+-rw-r--r--   0        0        0      864 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/__init__.py
+-rw-r--r--   0        0        0      496 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/asdf.yml
+-rw-r--r--   0        0        0     1222 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/demo_auction.yml
+-rw-r--r--   0        0        0      780 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/demo_big_maps.yml
+-rw-r--r--   0        0        0      747 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/demo_dao.yml
+-rw-r--r--   0        0        0     5012 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/demo_dex.yml
+-rw-r--r--   0        0        0      943 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/demo_domains.yml
+-rw-r--r--   0        0        0     1392 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/demo_etherlink.yaml
+-rw-r--r--   0        0        0      583 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/demo_events.yml
+-rw-r--r--   0        0        0      824 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/demo_evm_events.yml
+-rw-r--r--   0        0        0      844 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/demo_evm_events_node.yml
+-rw-r--r--   0        0        0      877 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/demo_evm_transactions.yml
+-rw-r--r--   0        0        0      897 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/demo_evm_transactions_node.yml
+-rw-r--r--   0        0        0     1144 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/demo_factories.yml
+-rw-r--r--   0        0        0     1316 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/demo_nft_marketplace.yml
+-rw-r--r--   0        0        0      590 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/demo_raw.yml
+-rw-r--r--   0        0        0      711 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/demo_token.yml
+-rw-r--r--   0        0        0      456 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/demo_token_balances.yml
+-rw-r--r--   0        0        0      527 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/demo_token_transfers.yml
+-rw-r--r--   0        0        0      527 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/demo_token_transfers_2.yml
+-rw-r--r--   0        0        0      527 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/demo_token_transfers_3.yml
+-rw-r--r--   0        0        0      814 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/demo_token_transfers_4.yml
+-rw-r--r--   0        0        0     1252 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/dipdup.yml
+-rw-r--r--   0        0        0      521 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/hen_subjkt.yml
+-rw-r--r--   0        0        0      496 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/hjkl.yml
+-rw-r--r--   0        0        0      546 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/kolibri_ovens.yml
+-rw-r--r--   0        0        0      684 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/operation_filters.yml
+-rw-r--r--   0        0        0      496 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/qwer.yml
+-rw-r--r--   0        0        0      496 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/rewq.yml
+-rw-r--r--   0        0        0       98 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/test_postgres.yaml
+-rw-r--r--   0        0        0      151 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/test_postgres_immune.yaml
+-rw-r--r--   0        0        0       44 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/test_sqlite.yaml
+-rw-r--r--   0        0        0      128 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/test_sqlite_immune.yaml
+-rw-r--r--   0        0        0      534 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/yupana.yml
+-rw-r--r--   0        0        0      496 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/configs/zxcv.yml
+-rw-r--r--   0        0        0     1311 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/profile_abi_decoding.py
+-rw-r--r--   0        0        0    29145 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/replays/0535b2dcc93076e6026fa48cc501adaed47b7b060e6483d8312f40c184d7287d
+-rw-r--r--   0        0        0      305 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/replays/0b7d26b8f2813d12a80b9e96cc6f0bb186bf9ac5c5b0c0b3bb2cc8d750126843
+-rw-r--r--   0        0        0      959 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/replays/0eaaba2830dbdd3a80286fbc367084bce6e55c678e21da178a7eb16beef6c997
+-rw-r--r--   0        0        0    25834 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/replays/1228b36594bb93d619170ad49373f1ceec52d10faafdd727b37f3cdeffd663db
+-rw-r--r--   0        0        0    13886 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/replays/13afdf001ce3d6a0219c0f7f6d372d9b645770e5f4304576f7f7a37b45af96fc
+-rw-r--r--   0        0        0      403 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/replays/1430e37dce64ecb83499da8feaa3c0906e4fdf5d0a3c3570174645e97ba54bc4
+-rw-r--r--   0        0        0      295 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/replays/185f6628ac43f6ca728c5b79b7b81a3c3671efce7f14030a06a27e90cf641dea
+-rw-r--r--   0        0        0        2 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/replays/1c717490846300e1639e96a0c1438b6dd2abd6de013c5edec49042fa364c06e6
+-rw-r--r--   0        0        0     1871 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/replays/27373c23411bf37b605c8d0ead9a0e6c6c1f1718ce7863b095b759811e44e155
+-rw-r--r--   0        0        0     1824 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/replays/2a45ec6372b45e46199a6af24272cb93586777a0522cd1203b3eeef213ce4583
+-rw-r--r--   0        0        0    54602 2024-04-09 23:07:36.459831 dipdup-7.5.4/tests/replays/383899084f79460e96fd311bb64e4925738c486b39d6281539456c5fcac41620
+-rw-r--r--   0        0        0   234676 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/388fe9107380b6dd1e9ce3a87c23abd56ad39dfb6cb8a5a27b959e5b0434633b
+-rw-r--r--   0        0        0      642 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/39b8664d1bca5d374ff905c8a3a396b53d19ee469dc37545a8ca6b080bd0e9e0
+-rw-r--r--   0        0        0     1200 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/3a2bd8b6b72bf18152d2550c106789fa9b8abc98ea9d759a6597b7ebfbab0fc2
+-rw-r--r--   0        0        0    34389 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/3f5927db41422038d8e2cc203ef56a769c66b25835cdee42b17bc61e600be550
+-rw-r--r--   0        0        0      804 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/43cb0ab415d8b8b3f7addc3e82ea27d93b2c66ff55c117e1e0c7c64a0fcfc3f2
+-rw-r--r--   0        0        0   109726 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/4a57776d93475adfd9c49b6c3295a7cedfc23b73733a1fb5f0c985ee039dc5dc
+-rw-r--r--   0        0        0     1160 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/4aa7f9b0657be0c44baf2caed8c7cb08d02097a4095cf6417f78cba3a25e8423
+-rw-r--r--   0        0        0       67 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/4fbdb4667971fab446a5ac5937a7c8cc6ef5813ff00af24b6fd1b1a0427bedbb
+-rw-r--r--   0        0        0   192680 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/5483a0e11009e0f186bf70c214e2597d267a75a1e19152a9e7ed1ec257ce88ca
+-rw-r--r--   0        0        0    40432 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/587613799ebfae42b1884016d1a44a452d68e70e3ed80641d90b8e7657ba8ee5
+-rw-r--r--   0        0        0       32 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/5b004196490632859ec1b019d640f6bbb93fc86a433c8969e10f36f51ac2c78d
+-rw-r--r--   0        0        0    40439 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/5b99bc4beb6a9a33f7d2f118426458e4c788e0ab6d9e51949d3ccbf8b4003fc1
+-rw-r--r--   0        0        0    33335 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/607ecfd3653eda82aac502ac370c6ad7144d30c1e3c525ed520d44f9edf5b7e9
+-rw-r--r--   0        0        0       67 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/60f48c13c47a1347786a6dcf6f741874e7b30b587d148faa67d15067bb3871de
+-rw-r--r--   0        0        0        2 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/694f9dfac7db616fa52c4d35bca1036b6521d285ed1873028303b83822b5980b
+-rw-r--r--   0        0        0      132 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/6d0c5443d41a15551acb41adc10d36d4895f5786d6922a878b5c5414610e0ebc
+-rw-r--r--   0        0        0      754 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/6d76a3c3f427ff534c551de1793cb1d1dfbd22ccad97f5917a9f9b201a3f9804
+-rw-r--r--   0        0        0     1781 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/6fa41b68da742cc7cf8a0d68baef77ce8b2e9abf765767318d7ff4cf453ded4c
+-rw-r--r--   0        0        0      451 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/739d17c86095aac3da3508a16dc1c9ae9459ea86eeb09f62aaefc32de2997918
+-rw-r--r--   0        0        0        2 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/759b79ec12b1305d9fa8e1a5218e62bb3d3ad913580e19914d30d8aa09920ae4
+-rw-r--r--   0        0        0    50588 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/7b6cf9b8c69712bf26ed09059352ec740606969bf20eab0dedda870273f4fde9
+-rw-r--r--   0        0        0      807 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/803e05a8d0bb9e7cfb49530271d43ea62111b6419e7cded2d221f7e0e0c92ece
+-rw-r--r--   0        0        0   203748 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/8060a1f95213d470ee947a12242ef76cb7fb0c05bbaecc385eb6ec4a20d694c4
+-rw-r--r--   0        0        0      395 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/8335acc6585656ec3a4301cd8b089401f2dc2c7d758b381c96c730e610b67f7b
+-rw-r--r--   0        0        0     1151 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/93516225810a23a6799f2f9a1dee055ca79a66ee2b8d0f32be820c9c385e936b
+-rw-r--r--   0        0        0      877 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/9e6e907842da2cd494c558ea5ecc211fd12e56bfc547450978fb7dfe03853e58
+-rw-r--r--   0        0        0    22801 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/a3ce91a1b0d505cc221f0e201781466ba1e2d6dc7b624b9bc75a03ce3dbb0f92
+-rw-r--r--   0        0        0      767 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/aa8fe6037996b296bf9a3011e45cd9ecb92fb728592a843f91b03b2848cb1fb1
+-rw-r--r--   0        0        0     1931 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/acaa57345850f3b76471a7b3a8fb76b7f83e824f1520a2e0ee8ec93cdd6cb1c3
+-rw-r--r--   0        0        0     1882 2024-04-09 23:07:36.463831 dipdup-7.5.4/tests/replays/acc952ba1905717315212f952ed689d7b8f683165b31c0a7a25199aed9fda27f
+-rw-r--r--   0        0        0       67 2024-04-09 23:07:36.467831 dipdup-7.5.4/tests/replays/af37212b31e932f269c42c7f34ad8f3849bd8aed244652c41b9327c508985ce5
+-rw-r--r--   0        0        0     1200 2024-04-09 23:07:36.467831 dipdup-7.5.4/tests/replays/b3af887f7ad8172af75b94a09bedfb9ae1e14f8819a36d6ce9f709721068263b
+-rw-r--r--   0        0        0    34407 2024-04-09 23:07:36.467831 dipdup-7.5.4/tests/replays/b89b0ea704071e273d3c74a4dbb7b4f6c6fd9ea1848c69b452dce4f04872d3b5
+-rw-r--r--   0        0        0     2271 2024-04-09 23:07:36.467831 dipdup-7.5.4/tests/replays/bec4433b4206f00c2310a7961cff7f539434b9161b45673793aa5a3b50234313
+-rw-r--r--   0        0        0      403 2024-04-09 23:07:36.467831 dipdup-7.5.4/tests/replays/bed2329e63d559db2fb81c69606e715d1f90aaacab6ae45b33516e7828841a3c
+-rw-r--r--   0        0        0    89684 2024-04-09 23:07:36.467831 dipdup-7.5.4/tests/replays/c1c3eef91f7149d7aa2da072f71598f3ad5e29250cfa441bb6d4411acd70d657
+-rw-r--r--   0        0        0    25834 2024-04-09 23:07:36.467831 dipdup-7.5.4/tests/replays/cc5d3d4a58d5cb6bc7270d38c797b7740b79f913590ef0164abd50e58fba9405
+-rw-r--r--   0        0        0     1157 2024-04-09 23:07:36.467831 dipdup-7.5.4/tests/replays/d0a594d14bcb3fbf916092ec6707dfd3c9f48f53f0a1ad40a32023e7a87f8ef5
+-rw-r--r--   0        0        0     6669 2024-04-09 23:07:36.467831 dipdup-7.5.4/tests/replays/d62748a927a09395579b5790c8f871cc8653081cf4475abc93173989f950b92b
+-rw-r--r--   0        0        0    27896 2024-04-09 23:07:36.467831 dipdup-7.5.4/tests/replays/d94397f6ecec8ce25f87177fe410f6498d7d30a04360506c0cd300d291c167e7
+-rw-r--r--   0        0        0      132 2024-04-09 23:07:36.467831 dipdup-7.5.4/tests/replays/db797e6bf4c1b9c3237af5dec694fb1b6d21418a5a2f7947eb7f54d4e9201baf
+-rw-r--r--   0        0        0    20467 2024-04-09 23:07:36.467831 dipdup-7.5.4/tests/replays/dca9cf4f9f27623f10975d369444899458ab9ea85c22af2da6ce6ce8c09c2b58
+-rw-r--r--   0        0        0      767 2024-04-09 23:07:36.467831 dipdup-7.5.4/tests/replays/dd5d267c6e8e943a637ede23d708587123b9184560358d294be7fbed0d4b587a
+-rw-r--r--   0        0        0   209761 2024-04-09 23:07:36.467831 dipdup-7.5.4/tests/replays/e10e6552f0dce5124e0d72b74c508541a8098c407c9a3b0d2e10a7408b4d7cfe
+-rw-r--r--   0        0        0    17502 2024-04-09 23:07:36.467831 dipdup-7.5.4/tests/replays/e4a563a0b19379a44e9d2dc398131e9fd30d6039ff4ffacf1252db0bf8b433aa
+-rw-r--r--   0        0        0       67 2024-04-09 23:07:36.467831 dipdup-7.5.4/tests/replays/e82ba90c8570b92c0b1fc360b853aca3f1d7de457aacb9f6f19fa3e43879a8b3
+-rw-r--r--   0        0        0      132 2024-04-09 23:07:36.467831 dipdup-7.5.4/tests/replays/e9fa56a94eb559c550dfbca4b27ef350a0b4a787afbe60205482a38223dcea04
+-rw-r--r--   0        0        0   713738 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/replays/eb8b6b33cb2e165d1a3a73c09938d3083671a82ad73d4c0cff1fb2a5e5715f76
+-rw-r--r--   0        0        0    27505 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/replays/eb8e2c3ce2fe7792d2c8e81c61d37821275b64021343103b0c955042ae802189
+-rw-r--r--   0        0        0    17245 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/replays/f3d608f99e6b92e28a064bb9c10c3c605c9c817383c1eebcc68f663d1d23d650
+-rw-r--r--   0        0        0   211527 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/replays/f7d244938de3e3d153e4ef8172cab0f1e896b801904a54ac034d3d14352ee64a
+-rw-r--r--   0        0        0    27847 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/replays/f9fa1571c3d850f4a19c286205291893d184a9d124390d0358034a8b8366556d
+-rw-r--r--   0        0        0   118246 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/replays/fe80425d17f2467fccc527a99b5a11da144f63f9a3cab83989be0f8fed737264
+-rw-r--r--   0        0        0      996 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/replays/ff51b3535acc2972090ecd5db3af8f827464c9d92f1aa661630976e5b4ed4cbe
+-rw-r--r--   0        0        0     4599 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/responses/asdf.json
+-rw-r--r--   0        0        0     6704 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/responses/ftzfun.json
+-rw-r--r--   0        0        0     3445 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/responses/hen_subjkt.json
+-rw-r--r--   0        0        0     5210 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/responses/hjkl.json
+-rw-r--r--   0        0        0     2097 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/responses/kolibri_ovens.json
+-rw-r--r--   0        0        0    11186 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/responses/ooQuCAKBHkmWy2VciDAV9c6CFTywuMLupLzVoKDwS1xvR4EdRng.json
+-rw-r--r--   0        0        0     1811 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/responses/origination_amount.json
+-rw-r--r--   0        0        0     4256 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/responses/qwer.json
+-rw-r--r--   0        0        0     5307 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/responses/rewq.json
+-rw-r--r--   0        0        0    38178 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/responses/yupana.json
+-rw-r--r--   0        0        0     5909 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/responses/zxcv.json
+-rw-r--r--   0        0        0     1077 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/schemas/asdf/storage.json
+-rw-r--r--   0        0        0     2116 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/schemas/hen_subjkt/storage.json
+-rw-r--r--   0        0        0     1638 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/schemas/hjkl/storage.json
+-rw-r--r--   0        0        0      800 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/schemas/kolibri_ovens/storage.json
+-rw-r--r--   0        0        0     1005 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/schemas/qwer/storage.json
+-rw-r--r--   0        0        0     2212 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/schemas/rewq/storage.json
+-rw-r--r--   0        0        0    12561 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/schemas/yupana/storage.json
+-rw-r--r--   0        0        0     2660 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/schemas/zxcv/storage.json
+-rw-r--r--   0        0        0     3767 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/test_config/test_callbacks.py
+-rw-r--r--   0        0        0     5583 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/test_config/test_config.py
+-rw-r--r--   0        0        0     4138 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/test_config/test_custom_config.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/test_datasources/__init__.py
+-rw-r--r--   0        0        0      814 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/test_datasources/test_ipfs.py
+-rw-r--r--   0        0        0      795 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/test_datasources/test_metadata.py
+-rw-r--r--   0        0        0     8320 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/test_datasources/test_tzkt.py
+-rw-r--r--   0        0        0     1215 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/test_datasources/test_tzkt_blocks.py
+-rw-r--r--   0        0        0     1971 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/test_datasources/test_tzkt_buffer.py
+-rw-r--r--   0        0        0     1425 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/test_datasources/test_tzkt_quotes.py
+-rw-r--r--   0        0        0     9022 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/test_demos.py
+-rw-r--r--   0        0        0     2872 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/test_dipdup.py
+-rw-r--r--   0        0        0     3108 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/test_hasura.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/test_http.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.471831 dipdup-7.5.4/tests/test_index/__init__.py
+-rw-r--r--   0        0        0     7461 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/test_index/test_tzkt_operations.py
+-rw-r--r--   0        0        0     5409 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/test_introspection.py
+-rw-r--r--   0        0        0    11401 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/test_models.py
+-rw-r--r--   0        0        0    13543 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/test_rollback.py
+-rw-r--r--   0        0        0     6692 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/test_schema.py
+-rw-r--r--   0        0        0     3620 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/asdf/__init__.py
+-rw-r--r--   0        0        0      455 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/asdf/storage.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/bazaar/__init__.py
+-rw-r--r--   0        0        0      539 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/bazaar/storage.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/ftzfun/__init__.py
+-rw-r--r--   0        0        0      881 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/ftzfun/storage.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/hen_subjkt/__init__.py
+-rw-r--r--   0        0        0      558 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/hen_subjkt/storage.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/hjkl/__init__.py
+-rw-r--r--   0        0        0      564 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/hjkl/storage.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/kolibri_ovens/__init__.py
+-rw-r--r--   0        0        0      200 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/kolibri_ovens/set_delegate.py
+-rw-r--r--   0        0        0      392 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/kolibri_ovens/storage.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/listofmaps/__init__.py
+-rw-r--r--   0        0        0      104 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/listofmaps/storage.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/qwer/__init__.py
+-rw-r--r--   0        0        0      452 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/qwer/storage.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/rewq/__init__.py
+-rw-r--r--   0        0        0      770 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/rewq/storage.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/tezotop/__init__.py
+-rw-r--r--   0        0        0      660 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/tezotop/storage.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/yupana/__init__.py
+-rw-r--r--   0        0        0     2635 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/yupana/storage.py
+-rw-r--r--   0        0        0        0 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/zxcv/__init__.py
+-rw-r--r--   0        0        0      981 2024-04-09 23:07:36.475831 dipdup-7.5.4/tests/types/zxcv/storage.py
+-rw-r--r--   0        0        0     4732 1970-01-01 00:00:00.000000 dipdup-7.5.4/PKG-INFO
```

### Comparing `dipdup-7.5.3/LICENSE` & `dipdup-7.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/README.md` & `dipdup-7.5.4/README.md`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/pyproject.toml` & `dipdup-7.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "dipdup"
 description = "Modular framework for creating selective indexers and featureful backends for dapps"
-version = "7.5.3"
+version = "7.5.4"
 authors = [
     { name = "Lev Gorodetskii", email = "dipdup@drsr.io" },
     { name = "Vladimir Bobrikov", email = "vladimir_bobrikov@pm.me" },
     { name = "Michael Zaikin", email = "mz@baking-bad.org" },
 ]
 maintainers = [
     { name = "Lev Gorodetskii", email = "dipdup@drsr.io" },
```

### Comparing `dipdup-7.5.3/src/demo_auction/Makefile` & `dipdup-7.5.4/src/demo_auction/Makefile`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_auction/README.md` & `dipdup-7.5.4/src/demo_auction/README.md`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_auction/configs/dipdup.compose.yaml` & `dipdup-7.5.4/src/demo_auction/configs/dipdup.compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_auction/configs/dipdup.swarm.yaml` & `dipdup-7.5.4/src/demo_auction/configs/dipdup.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_auction/configs/replay.yaml` & `dipdup-7.5.4/src/demo_auction/configs/replay.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_auction/deploy/compose.swarm.yaml` & `dipdup-7.5.4/src/demo_auction/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_auction/deploy/compose.yaml` & `dipdup-7.5.4/src/demo_auction/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_auction/dipdup.yaml` & `dipdup-7.5.4/src/demo_auction/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_auction/handlers/on_bid.py` & `dipdup-7.5.4/src/demo_auction/handlers/on_bid.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_auction/handlers/on_create_auction.py` & `dipdup-7.5.4/src/demo_auction/handlers/on_create_auction.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_auction/handlers/on_withdraw.py` & `dipdup-7.5.4/src/demo_auction/handlers/on_withdraw.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_auction/models/__init__.py` & `dipdup-7.5.4/src/demo_auction/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_auction/pyproject.toml` & `dipdup-7.5.4/src/demo_auction/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by DipDup 7.5.3+editable
+# Generated by DipDup 7.5.4+editable
 [project]
 name = "demo_auction"
 version = "0.0.1"
 description = "NFT marketplace (TzColors)"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" },
```

### Comparing `dipdup-7.5.3/src/demo_big_maps/Makefile` & `dipdup-7.5.4/src/demo_big_maps/Makefile`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_big_maps/README.md` & `dipdup-7.5.4/src/demo_big_maps/README.md`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_big_maps/configs/dipdup.compose.yaml` & `dipdup-7.5.4/src/demo_big_maps/configs/dipdup.compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_big_maps/configs/dipdup.swarm.yaml` & `dipdup-7.5.4/src/demo_big_maps/configs/dipdup.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_big_maps/configs/replay.yaml` & `dipdup-7.5.4/src/demo_big_maps/configs/replay.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_big_maps/deploy/compose.swarm.yaml` & `dipdup-7.5.4/src/demo_big_maps/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_big_maps/deploy/compose.yaml` & `dipdup-7.5.4/src/demo_big_maps/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_big_maps/dipdup.yaml` & `dipdup-7.5.4/src/demo_big_maps/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_big_maps/handlers/on_update_expiry_map.py` & `dipdup-7.5.4/src/demo_big_maps/handlers/on_update_expiry_map.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_big_maps/handlers/on_update_records.py` & `dipdup-7.5.4/src/demo_big_maps/handlers/on_update_records.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_big_maps/models/__init__.py` & `dipdup-7.5.4/src/demo_big_maps/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_big_maps/pyproject.toml` & `dipdup-7.5.4/src/demo_big_maps/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by DipDup 7.5.3+editable
+# Generated by DipDup 7.5.4+editable
 [project]
 name = "demo_big_maps"
 version = "0.0.1"
 description = "Indexing specific big maps"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" },
```

### Comparing `dipdup-7.5.3/src/demo_blank/Makefile` & `dipdup-7.5.4/src/demo_blank/Makefile`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_blank/README.md` & `dipdup-7.5.4/src/demo_blank/README.md`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_blank/configs/dipdup.compose.yaml` & `dipdup-7.5.4/src/demo_blank/configs/dipdup.compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_blank/configs/dipdup.swarm.yaml` & `dipdup-7.5.4/src/demo_blank/configs/dipdup.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_blank/configs/replay.yaml` & `dipdup-7.5.4/src/demo_blank/configs/replay.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_blank/deploy/compose.swarm.yaml` & `dipdup-7.5.4/src/demo_blank/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_blank/deploy/compose.yaml` & `dipdup-7.5.4/src/demo_blank/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_blank/models/__init__.py` & `dipdup-7.5.4/src/demo_blank/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_blank/pyproject.toml` & `dipdup-7.5.4/src/demo_blank/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by DipDup 7.5.3+editable
+# Generated by DipDup 7.5.4+editable
 [project]
 name = "demo_blank"
 version = "0.0.1"
 description = "Empty config for a fresh start"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" },
```

### Comparing `dipdup-7.5.3/src/demo_dao/Makefile` & `dipdup-7.5.4/src/demo_dao/Makefile`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dao/README.md` & `dipdup-7.5.4/src/demo_dao/README.md`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dao/configs/dipdup.compose.yaml` & `dipdup-7.5.4/src/demo_dao/configs/dipdup.compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dao/configs/dipdup.swarm.yaml` & `dipdup-7.5.4/src/demo_dao/configs/dipdup.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dao/configs/replay.yaml` & `dipdup-7.5.4/src/demo_dao/configs/replay.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dao/deploy/compose.swarm.yaml` & `dipdup-7.5.4/src/demo_dao/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dao/deploy/compose.yaml` & `dipdup-7.5.4/src/demo_dao/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dao/dipdup.yaml` & `dipdup-7.5.4/src/demo_dao/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dao/models/__init__.py` & `dipdup-7.5.4/src/demo_dao/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dao/pyproject.toml` & `dipdup-7.5.4/src/demo_dex/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Generated by DipDup 7.5.3+editable
+# Generated by DipDup 7.5.4+editable
 [project]
-name = "demo_dao"
+name = "demo_dex"
 version = "0.0.1"
-description = "DAO registry (Homebase DAO)"
+description = "DEX balances and liquidity (Quipuswap)"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
```

### Comparing `dipdup-7.5.3/src/demo_dao/types/registry/tezos_storage.py` & `dipdup-7.5.4/src/demo_dao/types/registry/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/.ruff_cache/0.3.4/467002119024090504` & `dipdup-7.5.4/src/demo_dex/.ruff_cache/0.3.5/15668834222879262927`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 00000000: 3500 0000 0000 0000 2f68 6f6d 652f 7275  5......./home/ru
 00000010: 6e6e 6572 2f77 6f72 6b2f 6469 7064 7570  nner/work/dipdup
 00000020: 2f64 6970 6475 702f 7372 632f 6465 6d6f  /dipdup/src/demo
 00000030: 5f64 6578 2f68 616e 646c 6572 730e 0000  _dex/handlers...
-00000040: 0000 0000 001a 0000 0000 0000 006f 6e5f  .............on_
-00000050: 6661 3132 5f77 6974 6864 7261 775f 7072  fa12_withdraw_pr
-00000060: 6f66 6974 2e70 7996 1bc0 c4e1 5d58 fbfe  ofit.py.....]X..
-00000070: 0e4a 828e 0100 0001 0000 0000 0000 0000  .J..............
+00000040: 0000 0000 001b 0000 0000 0000 006f 6e5f  .............on_
+00000050: 6661 3132 5f69 6e76 6573 745f 6c69 7175  fa12_invest_liqu
+00000060: 6964 6974 792e 7079 85f2 e844 24ac a2f2  idity.py...D$...
+00000070: e3d3 1ec5 8e01 0000 0100 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000090: 0000 1500 0000 0000 0000 6f6e 5f66 6132  ..........on_fa2
-000000a0: 5f6f 7269 6769 6e61 7469 6f6e 2e70 7996  _origination.py.
-000000b0: 1bc0 c4e1 5d58 fbfe 0e4a 828e 0100 0001  ....]X...J......
-000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000d0: 0000 0000 0000 0000 0000 1600 0000 0000  ................
-000000e0: 0000 6f6e 5f66 6132 5f74 6f6b 656e 5f74  ..on_fa2_token_t
-000000f0: 6f5f 7465 7a2e 7079 961b c0c4 e15d 58fb  o_tez.py.....]X.
-00000100: fe0e 4a82 8e01 0000 0100 0000 0000 0000  ..J.............
+00000090: 0000 0015 0000 0000 0000 006f 6e5f 6661  ...........on_fa
+000000a0: 325f 6f72 6967 696e 6174 696f 6e2e 7079  2_origination.py
+000000b0: 85f2 e844 24ac a2f2 e3d3 1ec5 8e01 0000  ...D$...........
+000000c0: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+000000d0: 0000 0000 0000 0000 0000 0016 0000 0000  ................
+000000e0: 0000 006f 6e5f 6661 325f 746f 6b65 6e5f  ...on_fa2_token_
+000000f0: 746f 5f74 657a 2e70 7985 f2e8 4424 aca2  to_tez.py...D$..
+00000100: f2e3 d31e c58e 0100 0001 0000 0000 0000  ................
 00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000120: 0000 0013 0000 0000 0000 006f 6e5f 6661  ...........on_fa
-00000130: 3132 5f74 7261 6e73 6665 722e 7079 961b  12_transfer.py..
-00000140: c0c4 e15d 58fb fe0e 4a82 8e01 0000 0100  ...]X...J.......
+00000120: 0000 0000 1300 0000 0000 0000 6f6e 5f66  ............on_f
+00000130: 6131 325f 7472 616e 7366 6572 2e70 7985  a12_transfer.py.
+00000140: f2e8 4424 aca2 f2e3 d31e c58e 0100 0001  ..D$............
 00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000160: 0000 0000 0000 0000 001b 0000 0000 0000  ................
-00000170: 006f 6e5f 6661 3132 5f64 6976 6573 745f  .on_fa12_divest_
-00000180: 6c69 7175 6964 6974 792e 7079 961b c0c4  liquidity.py....
-00000190: e15d 58fb fe0e 4a82 8e01 0000 0100 0000  .]X...J.........
+00000160: 0000 0000 0000 0000 0000 1b00 0000 0000  ................
+00000170: 0000 6f6e 5f66 6131 325f 6469 7665 7374  ..on_fa12_divest
+00000180: 5f6c 6971 7569 6469 7479 2e70 7985 f2e8  _liquidity.py...
+00000190: 4424 aca2 f2e3 d31e c58e 0100 0001 0000  D$..............
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001b0: 0000 0000 0000 0017 0000 0000 0000 006f  ...............o
-000001c0: 6e5f 6661 3132 5f74 657a 5f74 6f5f 746f  n_fa12_tez_to_to
-000001d0: 6b65 6e2e 7079 961b c0c4 e15d 58fb fe0e  ken.py.....]X...
-000001e0: 4a82 8e01 0000 0100 0000 0000 0000 0000  J...............
+000001b0: 0000 0000 0000 0000 1700 0000 0000 0000  ................
+000001c0: 6f6e 5f66 6131 325f 7465 7a5f 746f 5f74  on_fa12_tez_to_t
+000001d0: 6f6b 656e 2e70 7985 f2e8 4424 aca2 f2e3  oken.py...D$....
+000001e0: d31e c58e 0100 0001 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0016 0000 0000 0000 006f 6e5f 6661 3132  .........on_fa12
-00000210: 5f6f 7269 6769 6e61 7469 6f6e 2e70 7996  _origination.py.
-00000220: 1bc0 c4e1 5d58 fbfe 0e4a 828e 0100 0001  ....]X...J......
-00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000240: 0000 0000 0000 0000 0000 1600 0000 0000  ................
-00000250: 0000 6f6e 5f66 6132 5f74 657a 5f74 6f5f  ..on_fa2_tez_to_
-00000260: 746f 6b65 6e2e 7079 961b c0c4 e15d 58fb  token.py.....]X.
-00000270: fe0e 4a82 8e01 0000 0100 0000 0000 0000  ..J.............
+00000200: 0000 1600 0000 0000 0000 6f6e 5f66 6131  ..........on_fa1
+00000210: 325f 6f72 6967 696e 6174 696f 6e2e 7079  2_origination.py
+00000220: 85f2 e844 24ac a2f2 e3d3 1ec5 8e01 0000  ...D$...........
+00000230: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+00000240: 0000 0000 0000 0000 0000 0016 0000 0000  ................
+00000250: 0000 006f 6e5f 6661 325f 7465 7a5f 746f  ...on_fa2_tez_to
+00000260: 5f74 6f6b 656e 2e70 7985 f2e8 4424 aca2  _token.py...D$..
+00000270: f2e3 d31e c58e 0100 0001 0000 0000 0000  ................
 00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000290: 0000 001a 0000 0000 0000 006f 6e5f 6661  ...........on_fa
-000002a0: 325f 6469 7665 7374 5f6c 6971 7569 6469  2_divest_liquidi
-000002b0: 7479 2e70 7996 1bc0 c4e1 5d58 fbfe 0e4a  ty.py.....]X...J
-000002c0: 828e 0100 0001 0000 0000 0000 0000 0000  ................
+00000290: 0000 0000 1a00 0000 0000 0000 6f6e 5f66  ............on_f
+000002a0: 6132 5f64 6976 6573 745f 6c69 7175 6964  a2_divest_liquid
+000002b0: 6974 792e 7079 85f2 e844 24ac a2f2 e3d3  ity.py...D$.....
+000002c0: 1ec5 8e01 0000 0100 0000 0000 0000 0000  ................
 000002d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002e0: 1200 0000 0000 0000 6f6e 5f66 6132 5f74  ........on_fa2_t
-000002f0: 7261 6e73 6665 722e 7079 961b c0c4 e15d  ransfer.py.....]
-00000300: 58fb fe0e 4a82 8e01 0000 0100 0000 0000  X...J...........
+000002e0: 0012 0000 0000 0000 006f 6e5f 6661 325f  .........on_fa2_
+000002f0: 7472 616e 7366 6572 2e70 7985 f2e8 4424  transfer.py...D$
+00000300: aca2 f2e3 d31e c58e 0100 0001 0000 0000  ................
 00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000320: 0000 0000 0019 0000 0000 0000 006f 6e5f  .............on_
-00000330: 6661 325f 7769 7468 6472 6177 5f70 726f  fa2_withdraw_pro
-00000340: 6669 742e 7079 961b c0c4 e15d 58fb fe0e  fit.py.....]X...
-00000350: 4a82 8e01 0000 0100 0000 0000 0000 0000  J...............
+00000320: 0000 0000 0000 1900 0000 0000 0000 6f6e  ..............on
+00000330: 5f66 6132 5f77 6974 6864 7261 775f 7072  _fa2_withdraw_pr
+00000340: 6f66 6974 2e70 7985 f2e8 4424 aca2 f2e3  ofit.py...D$....
+00000350: d31e c58e 0100 0001 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000370: 001a 0000 0000 0000 006f 6e5f 6661 325f  .........on_fa2_
-00000380: 696e 7665 7374 5f6c 6971 7569 6469 7479  invest_liquidity
-00000390: 2e70 7996 1bc0 c4e1 5d58 fbfe 0e4a 828e  .py.....]X...J..
-000003a0: 0100 0001 0000 0000 0000 0000 0000 0000  ................
-000003b0: 0000 0000 0000 0000 0000 0000 0000 1700  ................
-000003c0: 0000 0000 0000 6f6e 5f66 6131 325f 746f  ......on_fa12_to
-000003d0: 6b65 6e5f 746f 5f74 657a 2e70 7996 1bc0  ken_to_tez.py...
-000003e0: c4e1 5d58 fbfe 0e4a 828e 0100 0001 0000  ..]X...J........
+00000370: 0000 1a00 0000 0000 0000 6f6e 5f66 6131  ..........on_fa1
+00000380: 325f 7769 7468 6472 6177 5f70 726f 6669  2_withdraw_profi
+00000390: 742e 7079 85f2 e844 24ac a2f2 e3d3 1ec5  t.py...D$.......
+000003a0: 8e01 0000 0100 0000 0000 0000 0000 0000  ................
+000003b0: 0000 0000 0000 0000 0000 0000 0000 0017  ................
+000003c0: 0000 0000 0000 006f 6e5f 6661 3132 5f74  .......on_fa12_t
+000003d0: 6f6b 656e 5f74 6f5f 7465 7a2e 7079 85f2  oken_to_tez.py..
+000003e0: e844 24ac a2f2 e3d3 1ec5 8e01 0000 0100  .D$.............
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000400: 0000 0000 0000 0000 1b00 0000 0000 0000  ................
-00000410: 6f6e 5f66 6131 325f 696e 7665 7374 5f6c  on_fa12_invest_l
-00000420: 6971 7569 6469 7479 2e70 7996 1bc0 c4e1  iquidity.py.....
-00000430: 5d58 fbfe 0e4a 828e 0100 0001 0000 0000  ]X...J..........
+00000400: 0000 0000 0000 0000 001a 0000 0000 0000  ................
+00000410: 006f 6e5f 6661 325f 696e 7665 7374 5f6c  .on_fa2_invest_l
+00000420: 6971 7569 6469 7479 2e70 7985 f2e8 4424  iquidity.py...D$
+00000430: aca2 f2e3 d31e c58e 0100 0001 0000 0000  ................
 00000440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000450: 0000 0000 0000                           ......
```

### Comparing `dipdup-7.5.3/src/demo_dex/Makefile` & `dipdup-7.5.4/src/demo_dex/Makefile`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/README.md` & `dipdup-7.5.4/src/demo_dex/README.md`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/configs/dipdup.compose.yaml` & `dipdup-7.5.4/src/demo_dex/configs/dipdup.compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/configs/dipdup.swarm.yaml` & `dipdup-7.5.4/src/demo_dex/configs/dipdup.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/configs/replay.yaml` & `dipdup-7.5.4/src/demo_dex/configs/replay.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/deploy/compose.swarm.yaml` & `dipdup-7.5.4/src/demo_dex/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/deploy/compose.yaml` & `dipdup-7.5.4/src/demo_dex/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/dipdup.yaml` & `dipdup-7.5.4/src/demo_dex/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/handlers/on_fa12_divest_liquidity.py` & `dipdup-7.5.4/src/demo_dex/handlers/on_fa12_divest_liquidity.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/handlers/on_fa12_invest_liquidity.py` & `dipdup-7.5.4/src/demo_dex/handlers/on_fa12_invest_liquidity.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/handlers/on_fa12_origination.py` & `dipdup-7.5.4/src/demo_dex/handlers/on_fa12_origination.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/handlers/on_fa12_tez_to_token.py` & `dipdup-7.5.4/src/demo_dex/handlers/on_fa12_tez_to_token.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/handlers/on_fa12_token_to_tez.py` & `dipdup-7.5.4/src/demo_dex/handlers/on_fa12_token_to_tez.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/handlers/on_fa12_transfer.py` & `dipdup-7.5.4/src/demo_dex/handlers/on_fa12_transfer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/handlers/on_fa12_withdraw_profit.py` & `dipdup-7.5.4/src/demo_dex/handlers/on_fa12_withdraw_profit.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/handlers/on_fa2_divest_liquidity.py` & `dipdup-7.5.4/src/demo_dex/handlers/on_fa2_divest_liquidity.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/handlers/on_fa2_invest_liquidity.py` & `dipdup-7.5.4/src/demo_dex/handlers/on_fa2_invest_liquidity.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/handlers/on_fa2_origination.py` & `dipdup-7.5.4/src/demo_dex/handlers/on_fa2_origination.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/handlers/on_fa2_tez_to_token.py` & `dipdup-7.5.4/src/demo_dex/handlers/on_fa2_tez_to_token.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/handlers/on_fa2_token_to_tez.py` & `dipdup-7.5.4/src/demo_dex/handlers/on_fa2_token_to_tez.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/handlers/on_fa2_transfer.py` & `dipdup-7.5.4/src/demo_dex/handlers/on_fa2_transfer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/handlers/on_fa2_withdraw_profit.py` & `dipdup-7.5.4/src/demo_dex/handlers/on_fa2_withdraw_profit.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/models/__init__.py` & `dipdup-7.5.4/src/demo_dex/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/pyproject.toml` & `dipdup-7.5.4/src/demo_nft_marketplace/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Generated by DipDup 7.5.3+editable
+# Generated by DipDup 7.5.4+editable
 [project]
-name = "demo_dex"
+name = "demo_nft_marketplace"
 version = "0.0.1"
-description = "DEX balances and liquidity (Quipuswap)"
+description = "NFT marketplace (hic at nunc)"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
```

### Comparing `dipdup-7.5.3/src/demo_dex/types/fa12_token/tezos_storage.py` & `dipdup-7.5.4/src/demo_dex/types/fa12_token/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/types/fa2_token/tezos_storage.py` & `dipdup-7.5.4/src/demo_dex/types/fa2_token/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/types/quipu_fa12/tezos_storage.py` & `dipdup-7.5.4/src/demo_dex/types/quipu_fa12/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_dex/types/quipu_fa2/tezos_storage.py` & `dipdup-7.5.4/src/demo_dex/types/quipu_fa2/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_domains/Makefile` & `dipdup-7.5.4/src/demo_domains/Makefile`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_domains/README.md` & `dipdup-7.5.4/src/demo_domains/README.md`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_domains/configs/dipdup.compose.yaml` & `dipdup-7.5.4/src/demo_domains/configs/dipdup.compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_domains/configs/dipdup.swarm.yaml` & `dipdup-7.5.4/src/demo_domains/configs/dipdup.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_domains/configs/replay.yaml` & `dipdup-7.5.4/src/demo_domains/configs/replay.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_domains/deploy/compose.swarm.yaml` & `dipdup-7.5.4/src/demo_domains/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_domains/deploy/compose.yaml` & `dipdup-7.5.4/src/demo_domains/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_domains/dipdup.yaml` & `dipdup-7.5.4/src/demo_domains/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_domains/handlers/on_update_expiry_map.py` & `dipdup-7.5.4/src/demo_domains/handlers/on_update_expiry_map.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_domains/handlers/on_update_records.py` & `dipdup-7.5.4/src/demo_domains/handlers/on_update_records.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_domains/hooks/check_expiration.py` & `dipdup-7.5.4/src/demo_domains/hooks/check_expiration.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_domains/models/__init__.py` & `dipdup-7.5.4/src/demo_domains/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_domains/pyproject.toml` & `dipdup-7.5.4/src/demo_domains/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by DipDup 7.5.3+editable
+# Generated by DipDup 7.5.4+editable
 [project]
 name = "demo_domains"
 version = "0.0.1"
 description = "Domain name service (Tezos Domains)"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" },
```

### Comparing `dipdup-7.5.3/src/demo_etherlink/Makefile` & `dipdup-7.5.4/src/demo_etherlink/Makefile`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_etherlink/README.md` & `dipdup-7.5.4/src/demo_etherlink/README.md`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_etherlink/configs/dipdup.compose.yaml` & `dipdup-7.5.4/src/demo_etherlink/configs/dipdup.compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_etherlink/configs/dipdup.swarm.yaml` & `dipdup-7.5.4/src/demo_etherlink/configs/dipdup.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_etherlink/configs/replay.yaml` & `dipdup-7.5.4/src/demo_etherlink/configs/replay.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_etherlink/deploy/compose.swarm.yaml` & `dipdup-7.5.4/src/demo_etherlink/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_etherlink/deploy/compose.yaml` & `dipdup-7.5.4/src/demo_etherlink/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_etherlink/dipdup.yaml` & `dipdup-7.5.4/src/demo_etherlink/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_etherlink/handlers/on_deposit.py` & `dipdup-7.5.4/src/demo_etherlink/handlers/on_deposit.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_etherlink/handlers/on_withdraw.py` & `dipdup-7.5.4/src/demo_etherlink/handlers/on_withdraw.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_etherlink/models/__init__.py` & `dipdup-7.5.4/src/demo_etherlink/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_etherlink/pyproject.toml` & `dipdup-7.5.4/src/demo_token/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Generated by DipDup 7.5.3+editable
+# Generated by DipDup 7.5.4+editable
 [project]
-name = "demo_etherlink"
+name = "demo_token"
 version = "0.0.1"
-description = "Etherlink smart rollup transactions"
+description = "FA1.2 token contract operations"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
```

### Comparing `dipdup-7.5.3/src/demo_etherlink/types/rollup/tezos_parameters/default.py` & `dipdup-7.5.4/src/demo_etherlink/types/rollup/tezos_parameters/default.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_etherlink/types/ticket_helper/tezos_storage.py` & `dipdup-7.5.4/src/demo_etherlink/types/ticket_helper/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_etherlink/types/ticketer/tezos_parameters/withdraw.py` & `dipdup-7.5.4/src/demo_etherlink/types/ticketer/tezos_parameters/withdraw.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_etherlink/types/ticketer/tezos_storage.py` & `dipdup-7.5.4/src/demo_etherlink/types/ticketer/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_events/Makefile` & `dipdup-7.5.4/src/demo_events/Makefile`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_events/README.md` & `dipdup-7.5.4/src/demo_events/README.md`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_events/configs/dipdup.compose.yaml` & `dipdup-7.5.4/src/demo_events/configs/dipdup.compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_events/configs/dipdup.swarm.yaml` & `dipdup-7.5.4/src/demo_events/configs/dipdup.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_events/configs/replay.yaml` & `dipdup-7.5.4/src/demo_events/configs/replay.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_events/deploy/compose.swarm.yaml` & `dipdup-7.5.4/src/demo_events/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_events/deploy/compose.yaml` & `dipdup-7.5.4/src/demo_events/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_events/dipdup.yaml` & `dipdup-7.5.4/src/demo_events/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_events/models/__init__.py` & `dipdup-7.5.4/src/demo_events/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_events/pyproject.toml` & `dipdup-7.5.4/src/demo_events/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by DipDup 7.5.3+editable
+# Generated by DipDup 7.5.4+editable
 [project]
 name = "demo_events"
 version = "0.0.1"
 description = "Processing contract events"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" },
```

### Comparing `dipdup-7.5.3/src/demo_evm_events/Makefile` & `dipdup-7.5.4/src/demo_evm_events/Makefile`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_events/README.md` & `dipdup-7.5.4/src/demo_evm_events/README.md`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_events/abi/eth_usdt/abi.json` & `dipdup-7.5.4/src/demo_evm_events/abi/eth_usdt/abi.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_events/configs/dipdup.compose.yaml` & `dipdup-7.5.4/src/demo_evm_events/configs/dipdup.compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_events/configs/dipdup.swarm.yaml` & `dipdup-7.5.4/src/demo_evm_events/configs/dipdup.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_events/configs/replay.yaml` & `dipdup-7.5.4/src/demo_evm_events/configs/replay.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_events/deploy/.env.default` & `dipdup-7.5.4/src/demo_evm_events/deploy/.env.default`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_events/deploy/compose.swarm.yaml` & `dipdup-7.5.4/src/demo_evm_events/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_events/deploy/compose.yaml` & `dipdup-7.5.4/src/demo_evm_events/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_events/deploy/swarm.env.default` & `dipdup-7.5.4/src/demo_evm_events/deploy/swarm.env.default`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_events/dipdup.yaml` & `dipdup-7.5.4/src/demo_evm_events/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_events/handlers/on_transfer.py` & `dipdup-7.5.4/src/demo_evm_events/handlers/on_transfer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_events/pyproject.toml` & `dipdup-7.5.4/src/demo_evm_events/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by DipDup 7.5.3+editable
+# Generated by DipDup 7.5.4+editable
 [project]
 name = "demo_evm_events"
 version = "0.0.1"
 description = "ERC-20 token transfers (from event logs)"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" },
```

### Comparing `dipdup-7.5.3/src/demo_evm_transactions/Makefile` & `dipdup-7.5.4/src/demo_evm_transactions/Makefile`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_transactions/README.md` & `dipdup-7.5.4/src/demo_evm_transactions/README.md`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_transactions/abi/eth_usdt/abi.json` & `dipdup-7.5.4/src/demo_evm_transactions/abi/eth_usdt/abi.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_transactions/configs/dipdup.compose.yaml` & `dipdup-7.5.4/src/demo_evm_transactions/configs/dipdup.compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_transactions/configs/dipdup.swarm.yaml` & `dipdup-7.5.4/src/demo_evm_transactions/configs/dipdup.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_transactions/configs/replay.yaml` & `dipdup-7.5.4/src/demo_evm_transactions/configs/replay.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_transactions/deploy/.env.default` & `dipdup-7.5.4/src/demo_evm_transactions/deploy/.env.default`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_transactions/deploy/compose.swarm.yaml` & `dipdup-7.5.4/src/demo_evm_transactions/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_transactions/deploy/compose.yaml` & `dipdup-7.5.4/src/demo_evm_transactions/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_transactions/deploy/swarm.env.default` & `dipdup-7.5.4/src/demo_evm_transactions/deploy/swarm.env.default`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_transactions/dipdup.yaml` & `dipdup-7.5.4/src/demo_evm_transactions/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_transactions/handlers/on_transfer.py` & `dipdup-7.5.4/src/demo_evm_transactions/handlers/on_transfer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_evm_transactions/pyproject.toml` & `dipdup-7.5.4/src/demo_evm_transactions/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by DipDup 7.5.3+editable
+# Generated by DipDup 7.5.4+editable
 [project]
 name = "demo_evm_transactions"
 version = "0.0.1"
 description = "ERC-20 token transfers (from transactions)"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" },
```

### Comparing `dipdup-7.5.3/src/demo_factories/Makefile` & `dipdup-7.5.4/src/demo_factories/Makefile`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_factories/README.md` & `dipdup-7.5.4/src/demo_factories/README.md`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_factories/configs/dipdup.compose.yaml` & `dipdup-7.5.4/src/demo_factories/configs/dipdup.compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_factories/configs/dipdup.swarm.yaml` & `dipdup-7.5.4/src/demo_factories/configs/dipdup.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_factories/configs/replay.yaml` & `dipdup-7.5.4/src/demo_factories/configs/replay.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_factories/deploy/compose.swarm.yaml` & `dipdup-7.5.4/src/demo_factories/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_factories/deploy/compose.yaml` & `dipdup-7.5.4/src/demo_factories/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_factories/dipdup.yaml` & `dipdup-7.5.4/src/demo_factories/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_factories/handlers/on_factory_origination.py` & `dipdup-7.5.4/src/demo_factories/handlers/on_factory_origination.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_factories/handlers/on_transfer.py` & `dipdup-7.5.4/src/demo_factories/handlers/on_transfer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_factories/pyproject.toml` & `dipdup-7.5.4/src/demo_factories/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by DipDup 7.5.3+editable
+# Generated by DipDup 7.5.4+editable
 [project]
 name = "demo_factories"
 version = "0.0.1"
 description = "Example of spawning indexes in runtime"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" },
```

### Comparing `dipdup-7.5.3/src/demo_factories/types/factory/tezos_storage.py` & `dipdup-7.5.4/src/demo_factories/types/factory/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_factories/types/token/tezos_storage.py` & `dipdup-7.5.4/src/demo_factories/types/token/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_head/Makefile` & `dipdup-7.5.4/src/demo_head/Makefile`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_head/README.md` & `dipdup-7.5.4/src/demo_head/README.md`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_head/configs/dipdup.compose.yaml` & `dipdup-7.5.4/src/demo_head/configs/dipdup.compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_head/configs/dipdup.swarm.yaml` & `dipdup-7.5.4/src/demo_head/configs/dipdup.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_head/configs/replay.yaml` & `dipdup-7.5.4/src/demo_head/configs/replay.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_head/deploy/compose.swarm.yaml` & `dipdup-7.5.4/src/demo_head/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_head/deploy/compose.yaml` & `dipdup-7.5.4/src/demo_head/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_head/models/__init__.py` & `dipdup-7.5.4/src/demo_head/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_head/pyproject.toml` & `dipdup-7.5.4/src/demo_head/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by DipDup 7.5.3+editable
+# Generated by DipDup 7.5.4+editable
 [project]
 name = "demo_head"
 version = "0.0.1"
 description = "Processing head block metadata (realtime only)"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" },
```

### Comparing `dipdup-7.5.3/src/demo_nft_marketplace/Makefile` & `dipdup-7.5.4/src/demo_nft_marketplace/Makefile`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_nft_marketplace/README.md` & `dipdup-7.5.4/src/demo_nft_marketplace/README.md`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_nft_marketplace/configs/dipdup.compose.yaml` & `dipdup-7.5.4/src/demo_nft_marketplace/configs/dipdup.compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_nft_marketplace/configs/dipdup.swarm.yaml` & `dipdup-7.5.4/src/demo_nft_marketplace/configs/dipdup.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_nft_marketplace/configs/replay.yaml` & `dipdup-7.5.4/src/demo_nft_marketplace/configs/replay.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_nft_marketplace/deploy/.env.default` & `dipdup-7.5.4/src/demo_nft_marketplace/deploy/.env.default`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_nft_marketplace/deploy/compose.swarm.yaml` & `dipdup-7.5.4/src/demo_nft_marketplace/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_nft_marketplace/deploy/compose.yaml` & `dipdup-7.5.4/src/demo_nft_marketplace/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_nft_marketplace/deploy/swarm.env.default` & `dipdup-7.5.4/src/demo_nft_marketplace/deploy/swarm.env.default`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_nft_marketplace/dipdup.yaml` & `dipdup-7.5.4/src/demo_nft_marketplace/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_nft_marketplace/handlers/on_cancel_swap.py` & `dipdup-7.5.4/src/demo_nft_marketplace/handlers/on_cancel_swap.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_nft_marketplace/handlers/on_collect.py` & `dipdup-7.5.4/src/demo_nft_marketplace/handlers/on_collect.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_nft_marketplace/handlers/on_mint.py` & `dipdup-7.5.4/src/demo_nft_marketplace/handlers/on_mint.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_nft_marketplace/handlers/on_swap.py` & `dipdup-7.5.4/src/demo_nft_marketplace/handlers/on_swap.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_nft_marketplace/models/__init__.py` & `dipdup-7.5.4/src/demo_nft_marketplace/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_nft_marketplace/pyproject.toml` & `dipdup-7.5.4/src/demo_etherlink/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Generated by DipDup 7.5.3+editable
+# Generated by DipDup 7.5.4+editable
 [project]
-name = "demo_nft_marketplace"
+name = "demo_etherlink"
 version = "0.0.1"
-description = "NFT marketplace (hic at nunc)"
+description = "Etherlink smart rollup transactions"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
```

### Comparing `dipdup-7.5.3/src/demo_nft_marketplace/types/hen_minter/tezos_storage.py` & `dipdup-7.5.4/src/demo_nft_marketplace/types/hen_minter/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_nft_marketplace/types/hen_objkts/tezos_storage.py` & `dipdup-7.5.4/src/demo_nft_marketplace/types/hen_objkts/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_raw/Makefile` & `dipdup-7.5.4/src/demo_raw/Makefile`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_raw/README.md` & `dipdup-7.5.4/src/demo_raw/README.md`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_raw/configs/dipdup.compose.yaml` & `dipdup-7.5.4/src/demo_raw/configs/dipdup.compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_raw/configs/dipdup.swarm.yaml` & `dipdup-7.5.4/src/demo_raw/configs/dipdup.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_raw/configs/replay.yaml` & `dipdup-7.5.4/src/demo_raw/configs/replay.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_raw/deploy/compose.swarm.yaml` & `dipdup-7.5.4/src/demo_raw/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_raw/deploy/compose.yaml` & `dipdup-7.5.4/src/demo_raw/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_raw/pyproject.toml` & `dipdup-7.5.4/src/demo_raw/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by DipDup 7.5.3+editable
+# Generated by DipDup 7.5.4+editable
 [project]
 name = "demo_raw"
 version = "0.0.1"
 description = "Process raw operations without filtering and typed payloads"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" },
```

### Comparing `dipdup-7.5.3/src/demo_token/Makefile` & `dipdup-7.5.4/src/demo_token/Makefile`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token/README.md` & `dipdup-7.5.4/src/demo_token/README.md`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token/configs/dipdup.compose.yaml` & `dipdup-7.5.4/src/demo_token/configs/dipdup.compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token/configs/dipdup.swarm.yaml` & `dipdup-7.5.4/src/demo_token/configs/dipdup.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token/configs/replay.yaml` & `dipdup-7.5.4/src/demo_token/configs/replay.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token/deploy/compose.swarm.yaml` & `dipdup-7.5.4/src/demo_token/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token/deploy/compose.yaml` & `dipdup-7.5.4/src/demo_token/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token/dipdup.yaml` & `dipdup-7.5.4/src/demo_token/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token/handlers/on_mint.py` & `dipdup-7.5.4/src/demo_token/handlers/on_mint.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token/handlers/on_transfer.py` & `dipdup-7.5.4/src/demo_token/handlers/on_transfer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token/pyproject.toml` & `dipdup-7.5.4/src/demo_uniswap/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Generated by DipDup 7.5.3+editable
+# Generated by DipDup 7.5.4+editable
 [project]
-name = "demo_token"
+name = "demo_uniswap"
 version = "0.0.1"
-description = "FA1.2 token contract operations"
+description = "Uniswap V3 pools, positions, etc. (advanced, uses TimescaleDB)"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
```

### Comparing `dipdup-7.5.3/src/demo_token_balances/Makefile` & `dipdup-7.5.4/src/demo_token_balances/Makefile`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token_balances/README.md` & `dipdup-7.5.4/src/demo_token_balances/README.md`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token_balances/configs/dipdup.compose.yaml` & `dipdup-7.5.4/src/demo_token_balances/configs/dipdup.compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token_balances/configs/dipdup.swarm.yaml` & `dipdup-7.5.4/src/demo_token_balances/configs/dipdup.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token_balances/configs/replay.yaml` & `dipdup-7.5.4/src/demo_token_balances/configs/replay.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token_balances/deploy/compose.swarm.yaml` & `dipdup-7.5.4/src/demo_token_balances/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token_balances/deploy/compose.yaml` & `dipdup-7.5.4/src/demo_token_balances/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token_balances/pyproject.toml` & `dipdup-7.5.4/src/demo_token_balances/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by DipDup 7.5.3+editable
+# Generated by DipDup 7.5.4+editable
 [project]
 name = "demo_token_balances"
 version = "0.0.1"
 description = "FA1.2 token balances"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" },
```

### Comparing `dipdup-7.5.3/src/demo_token_transfers/Makefile` & `dipdup-7.5.4/src/demo_token_transfers/Makefile`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token_transfers/README.md` & `dipdup-7.5.4/src/demo_token_transfers/README.md`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token_transfers/configs/dipdup.compose.yaml` & `dipdup-7.5.4/src/demo_token_transfers/configs/dipdup.compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token_transfers/configs/dipdup.swarm.yaml` & `dipdup-7.5.4/src/demo_token_transfers/configs/dipdup.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token_transfers/configs/replay.yaml` & `dipdup-7.5.4/src/demo_token_transfers/configs/replay.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token_transfers/deploy/compose.swarm.yaml` & `dipdup-7.5.4/src/demo_token_transfers/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token_transfers/deploy/compose.yaml` & `dipdup-7.5.4/src/demo_token_transfers/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token_transfers/handlers/on_balance_update.py` & `dipdup-7.5.4/src/demo_token_transfers/handlers/on_balance_update.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token_transfers/handlers/on_token_transfer.py` & `dipdup-7.5.4/src/demo_token_transfers/handlers/on_token_transfer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_token_transfers/pyproject.toml` & `dipdup-7.5.4/src/demo_token_transfers/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by DipDup 7.5.3+editable
+# Generated by DipDup 7.5.4+editable
 [project]
 name = "demo_token_transfers"
 version = "0.0.1"
 description = "FA1.2 token transfers"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" },
```

### Comparing `dipdup-7.5.3/src/demo_uniswap/.ruff_cache/0.3.4/5362454613440678388` & `dipdup-7.5.4/src/demo_uniswap/.ruff_cache/0.3.5/7681863458869765244`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 00000000: 3000 0000 0000 0000 2f68 6f6d 652f 7275  0......./home/ru
 00000010: 6e6e 6572 2f77 6f72 6b2f 6469 7064 7570  nner/work/dipdup
 00000020: 2f64 6970 6475 702f 7372 632f 6465 6d6f  /dipdup/src/demo
 00000030: 5f75 6e69 7377 6170 0800 0000 0000 0000  _uniswap........
 00000040: 1200 0000 0000 0000 6d6f 6465 6c73 2f5f  ........models/_
-00000050: 5f69 6e69 745f 5f2e 7079 8377 c1de b94f  _init__.py.w...O
-00000060: 1e6c fe0e 4a82 8e01 0000 0101 0000 0000  .l..J...........
+00000050: 5f69 6e69 745f 5f2e 7079 05e4 c7f6 7a7c  _init__.py....z|
+00000060: 7fe6 e3d3 1ec5 8e01 0000 0101 0000 0000  ................
 00000070: 0000 001c 0000 0000 0000 0064 656d 6f5f  ...........demo_
 00000080: 756e 6973 7761 702e 6d6f 6465 6c73 2e5f  uniswap.models._
 00000090: 5f69 6e69 745f 5f03 0000 0000 0000 000d  _init__.........
 000000a0: 0000 0000 0000 0064 6970 6475 702e 6669  .......dipdup.fi
 000000b0: 656c 6473 1300 0000 1900 0000 1900 0000  elds............
 000000c0: 0000 0000 6469 7064 7570 2e6d 6f64 656c  ....dipdup.model
 000000d0: 732e 4361 6368 6564 4d6f 6465 6c34 0000  s.CachedModel4..
 000000e0: 003f 0000 0013 0000 0000 0000 0064 6970  .?...........dip
 000000f0: 6475 702e 6d6f 6465 6c73 2e4d 6f64 656c  dup.models.Model
 00000100: 5a00 0000 5f00 0000 0000 0000 0000 0000  Z..._...........
 00000110: 0000 0000 0000 0000 0000 0f00 0000 0000  ................
 00000120: 0000 6d6f 6465 6c73 2f74 6f6b 656e 2e70  ..models/token.p
-00000130: 7983 77c1 deb9 4f1e 6cfe 0e4a 828e 0100  y.w...O.l..J....
+00000130: 7905 e4c7 f67a 7c7f e6e3 d31e c58e 0100  y....z|.........
 00000140: 0001 0100 0000 0000 0000 1900 0000 0000  ................
 00000150: 0000 6465 6d6f 5f75 6e69 7377 6170 2e6d  ..demo_uniswap.m
 00000160: 6f64 656c 732e 746f 6b65 6e08 0000 0000  odels.token.....
 00000170: 0000 0013 0000 0000 0000 0063 6f6e 7465  ...........conte
 00000180: 7874 6c69 622e 7375 7070 7265 7373 1700  xtlib.suppress..
 00000190: 0000 1f00 0000 0f00 0000 0000 0000 6465  ..............de
 000001a0: 6369 6d61 6c2e 4465 6369 6d61 6c34 0000  cimal.Decimal4..
@@ -40,15 +40,15 @@
 00000270: 2e61 6269 2e67 6574 5f61 6269 0001 0000  .abi.get_abi....
 00000280: 0701 0000 2400 0000 0000 0000 6465 6d6f  ....$.......demo
 00000290: 5f75 6e69 7377 6170 2e6d 6f64 656c 732e  _uniswap.models.
 000002a0: 7265 706f 2e6d 6f64 656c 735f 7265 706f  repo.models_repo
 000002b0: 2d01 0000 3801 0000 0000 0000 0000 0000  -...8...........
 000002c0: 0000 0000 0000 0000 0000 0e00 0000 0000  ................
 000002d0: 0000 6d6f 6465 6c73 2f72 6570 6f2e 7079  ..models/repo.py
-000002e0: 8377 c1de b94f 1e6c fe0e 4a82 8e01 0000  .w...O.l..J.....
+000002e0: 05e4 c7f6 7a7c 7fe6 e3d3 1ec5 8e01 0000  ....z|..........
 000002f0: 0101 0000 0000 0000 0018 0000 0000 0000  ................
 00000300: 0064 656d 6f5f 756e 6973 7761 702e 6d6f  .demo_uniswap.mo
 00000310: 6465 6c73 2e72 6570 6f07 0000 0000 0000  dels.repo.......
 00000320: 000f 0000 0000 0000 0064 6563 696d 616c  .........decimal
 00000330: 2e44 6563 696d 616c 1400 0000 1b00 0000  .Decimal........
 00000340: 0a00 0000 0000 0000 7479 7069 6e67 2e41  ........typing.A
 00000350: 6e79 2f00 0000 3200 0000 0b00 0000 0000  ny/...2.........
@@ -61,27 +61,27 @@
 000003c0: 616e 646c 6572 436f 6e74 6578 7497 0000  andlerContext...
 000003d0: 00a5 0000 0007 0000 0000 0000 006c 7275  .............lru
 000003e0: 2e4c 5255 b600 0000 b900 0000 1300 0000  .LRU............
 000003f0: 0000 0000 6465 6d6f 5f75 6e69 7377 6170  ....demo_uniswap
 00000400: 2e6d 6f64 656c 73bb 0000 00df 0000 0000  .models.........
 00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000420: 000e 0000 0000 0000 006d 6f64 656c 732f  .........models/
-00000430: 7469 636b 2e70 7983 77c1 deb9 4f1e 6cfe  tick.py.w...O.l.
-00000440: 0e4a 828e 0100 0001 0100 0000 0000 0000  .J..............
+00000430: 7469 636b 2e70 7905 e4c7 f67a 7c7f e6e3  tick.py....z|...
+00000440: d31e c58e 0100 0001 0100 0000 0000 0000  ................
 00000450: 1800 0000 0000 0000 6465 6d6f 5f75 6e69  ........demo_uni
 00000460: 7377 6170 2e6d 6f64 656c 732e 7469 636b  swap.models.tick
 00000470: 0200 0000 0000 0000 0f00 0000 0000 0000  ................
 00000480: 6465 6369 6d61 6c2e 4465 6369 6d61 6c14  decimal.Decimal.
 00000490: 0000 001b 0000 0013 0000 0000 0000 0064  ...............d
 000004a0: 656d 6f5f 756e 6973 7761 702e 6d6f 6465  emo_uniswap.mode
 000004b0: 6c73 3600 0000 4600 0000 0000 0000 0000  ls6...F.........
 000004c0: 0000 0000 0000 0000 0000 0000 1200 0000  ................
 000004d0: 0000 0000 6d6f 6465 6c73 2f70 6f73 6974  ....models/posit
-000004e0: 696f 6e2e 7079 8377 c1de b94f 1e6c fe0e  ion.py.w...O.l..
-000004f0: 4a82 8e01 0000 0101 0000 0000 0000 001c  J...............
+000004e0: 696f 6e2e 7079 05e4 c7f6 7a7c 7fe6 e3d3  ion.py....z|....
+000004f0: 1ec5 8e01 0000 0101 0000 0000 0000 001c  ................
 00000500: 0000 0000 0000 0064 656d 6f5f 756e 6973  .......demo_unis
 00000510: 7761 702e 6d6f 6465 6c73 2e70 6f73 6974  wap.models.posit
 00000520: 696f 6e05 0000 0000 0000 001d 0000 0000  ion.............
 00000530: 0000 0064 6970 6475 702e 636f 6e74 6578  ...dipdup.contex
 00000540: 742e 4861 6e64 6c65 7243 6f6e 7465 7874  t.HandlerContext
 00000550: 1b00 0000 2900 0000 2500 0000 0000 0000  ....)...%.......
 00000560: 6574 685f 7574 696c 732e 6164 6472 6573  eth_utils.addres
@@ -93,16 +93,16 @@
 000005c0: 8f00 0000 1300 0000 0000 0000 6465 6d6f  ............demo
 000005d0: 5f75 6e69 7377 6170 2e6d 6f64 656c 7391  _uniswap.models.
 000005e0: 0000 00b5 0000 001f 0000 0000 0000 0064  ...............d
 000005f0: 656d 6f5f 756e 6973 7761 702e 6d6f 6465  emo_uniswap.mode
 00000600: 6c73 2e61 6269 2e67 6574 5f61 6269 da00  ls.abi.get_abi..
 00000610: 0000 e100 0000 0000 0000 0000 0000 0000  ................
 00000620: 0000 0000 0000 0000 0e00 0000 0000 0000  ................
-00000630: 6d6f 6465 6c73 2f70 6f6f 6c2e 7079 8377  models/pool.py.w
-00000640: c1de b94f 1e6c fe0e 4a82 8e01 0000 0101  ...O.l..J.......
+00000630: 6d6f 6465 6c73 2f70 6f6f 6c2e 7079 05e4  models/pool.py..
+00000640: c7f6 7a7c 7fe6 e3d3 1ec5 8e01 0000 0101  ..z|............
 00000650: 0000 0000 0000 0018 0000 0000 0000 0064  ...............d
 00000660: 656d 6f5f 756e 6973 7761 702e 6d6f 6465  emo_uniswap.mode
 00000670: 6c73 2e70 6f6f 6c09 0000 0000 0000 001d  ls.pool.........
 00000680: 0000 0000 0000 0064 6970 6475 702e 636f  .......dipdup.co
 00000690: 6e74 6578 742e 4861 6e64 6c65 7243 6f6e  ntext.HandlerCon
 000006a0: 7465 7874 1b00 0000 2900 0000 2800 0000  text....)...(...
 000006b0: 0000 0000 6469 7064 7570 2e6d 6f64 656c  ....dipdup.model
@@ -130,26 +130,26 @@
 00000810: 6576 656e 7473 2e62 7572 6e2e 4275 726e  events.burn.Burn
 00000820: 8d01 0000 9101 0000 2c00 0000 0000 0000  ........,.......
 00000830: 6465 6d6f 5f75 6e69 7377 6170 2e74 7970  demo_uniswap.typ
 00000840: 6573 2e70 6f6f 6c2e 6576 6d5f 6576 656e  es.pool.evm_even
 00000850: 7473 2e6d 696e 742e 4d69 6e74 c601 0000  ts.mint.Mint....
 00000860: ca01 0000 0000 0000 0000 0000 0000 0000  ................
 00000870: 0000 0000 0000 0d00 0000 0000 0000 6d6f  ..............mo
-00000880: 6465 6c73 2f61 6269 2e70 7983 77c1 deb9  dels/abi.py.w...
-00000890: 4f1e 6cfe 0e4a 828e 0100 0001 0100 0000  O.l..J..........
+00000880: 6465 6c73 2f61 6269 2e70 7905 e4c7 f67a  dels/abi.py....z
+00000890: 7c7f e6e3 d31e c58e 0100 0001 0100 0000  |...............
 000008a0: 0000 0000 1700 0000 0000 0000 6465 6d6f  ............demo
 000008b0: 5f75 6e69 7377 6170 2e6d 6f64 656c 732e  _uniswap.models.
 000008c0: 6162 6904 0000 0000 0000 000c 0000 0000  abi.............
 000008d0: 0000 0070 6174 686c 6962 2e50 6174 6814  ...pathlib.Path.
 000008e0: 0000 0018 0000 000a 0000 0000 0000 0074  ...............t
 000008f0: 7970 696e 672e 416e 792c 0000 002f 0000  yping.Any,.../..
 00000900: 000b 0000 0000 0000 0074 7970 696e 672e  .........typing.
 00000910: 6361 7374 4300 0000 4700 0000 0600 0000  castC...G.......
 00000920: 0000 0000 6f72 6a73 6f6e 4900 0000 5600  ....orjsonI...V.
 00000930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000940: 0000 0000 0b00 0000 0000 0000 5f5f 696e  ............__in
-00000950: 6974 5f5f 2e70 7983 77c1 deb9 4f1e 6cfe  it__.py.w...O.l.
-00000960: 0e4a 828e 0100 0001 0100 0000 0000 0000  .J..............
+00000950: 6974 5f5f 2e70 7905 e4c7 f67a 7c7f e6e3  it__.py....z|...
+00000960: d31e c58e 0100 0001 0100 0000 0000 0000  ................
 00000970: 1500 0000 0000 0000 6465 6d6f 5f75 6e69  ........demo_uni
 00000980: 7377 6170 2e5f 5f69 6e69 745f 5f00 0000  swap.__init__...
 00000990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000009a0: 0000 0000 0000 00                        .......
```

### Comparing `dipdup-7.5.3/src/demo_uniswap/Makefile` & `dipdup-7.5.4/src/demo_uniswap/Makefile`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/README.md` & `dipdup-7.5.4/src/demo_uniswap/README.md`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/abi/erc20/ERC20.json` & `dipdup-7.5.4/src/demo_uniswap/abi/erc20/ERC20.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/abi/factory/abi.json` & `dipdup-7.5.4/src/demo_uniswap/abi/factory/abi.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/abi/pool/abi.json` & `dipdup-7.5.4/src/demo_uniswap/abi/pool/abi.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/abi/position_manager/abi.json` & `dipdup-7.5.4/src/demo_uniswap/abi/position_manager/abi.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/configs/dipdup.compose.yaml` & `dipdup-7.5.4/src/demo_uniswap/configs/dipdup.compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/configs/dipdup.swarm.yaml` & `dipdup-7.5.4/src/demo_uniswap/configs/dipdup.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/configs/replay.yaml` & `dipdup-7.5.4/src/demo_uniswap/configs/replay.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/deploy/.env.default` & `dipdup-7.5.4/src/demo_uniswap/deploy/.env.default`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/deploy/compose.swarm.yaml` & `dipdup-7.5.4/src/demo_uniswap/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/deploy/compose.yaml` & `dipdup-7.5.4/src/demo_uniswap/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/deploy/swarm.env.default` & `dipdup-7.5.4/src/demo_uniswap/deploy/swarm.env.default`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/dipdup.yaml` & `dipdup-7.5.4/src/demo_uniswap/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/handlers/factory/pool_created.py` & `dipdup-7.5.4/src/demo_uniswap/handlers/factory/pool_created.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/handlers/pool/burn.py` & `dipdup-7.5.4/src/demo_uniswap/handlers/pool/burn.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/handlers/pool/initialize.py` & `dipdup-7.5.4/src/demo_uniswap/handlers/pool/initialize.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/handlers/pool/mint.py` & `dipdup-7.5.4/src/demo_uniswap/handlers/pool/mint.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/handlers/pool/swap.py` & `dipdup-7.5.4/src/demo_uniswap/handlers/pool/swap.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/handlers/position_manager/collect.py` & `dipdup-7.5.4/src/demo_uniswap/handlers/position_manager/collect.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/handlers/position_manager/decrease_liquidity.py` & `dipdup-7.5.4/src/demo_uniswap/handlers/position_manager/decrease_liquidity.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/handlers/position_manager/increase_liquidity.py` & `dipdup-7.5.4/src/demo_uniswap/handlers/position_manager/increase_liquidity.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/handlers/position_manager/transfer.py` & `dipdup-7.5.4/src/demo_uniswap/handlers/position_manager/transfer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/models/__init__.py` & `dipdup-7.5.4/src/demo_uniswap/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/models/pool.py` & `dipdup-7.5.4/src/demo_uniswap/models/pool.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/models/position.py` & `dipdup-7.5.4/src/demo_uniswap/models/position.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/models/repo.py` & `dipdup-7.5.4/src/demo_uniswap/models/repo.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/models/tick.py` & `dipdup-7.5.4/src/demo_uniswap/models/tick.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/models/token.py` & `dipdup-7.5.4/src/demo_uniswap/models/token.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/pyproject.toml` & `dipdup-7.5.4/src/demo_dao/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Generated by DipDup 7.5.3+editable
+# Generated by DipDup 7.5.4+editable
 [project]
-name = "demo_uniswap"
+name = "demo_dao"
 version = "0.0.1"
-description = "Uniswap V3 pools, positions, etc. (advanced, uses TimescaleDB)"
+description = "DAO registry (Homebase DAO)"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
```

### Comparing `dipdup-7.5.3/src/demo_uniswap/sql/on_reindex/20_create_ca_quotes_1m.sql` & `dipdup-7.5.4/src/demo_uniswap/sql/on_reindex/20_create_ca_quotes_1m.sql`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/sql/on_reindex/21_create_ca_quotes_1h.sql` & `dipdup-7.5.4/src/demo_uniswap/sql/on_reindex/21_create_ca_quotes_1h.sql`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/demo_uniswap/sql/on_reindex/22_create_ca_quotes_1d.sql` & `dipdup-7.5.4/src/demo_uniswap/sql/on_reindex/22_create_ca_quotes_1d.sql`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/api.py` & `dipdup-7.5.4/src/dipdup/api.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/cli.py` & `dipdup-7.5.4/src/dipdup/cli.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/codegen/__init__.py` & `dipdup-7.5.4/src/dipdup/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/codegen/evm_subsquid.py` & `dipdup-7.5.4/src/dipdup/codegen/evm_subsquid.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/codegen/tezos_tzkt.py` & `dipdup-7.5.4/src/dipdup/codegen/tezos_tzkt.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/config/__init__.py` & `dipdup-7.5.4/src/dipdup/config/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 from typing import Literal
 from typing import TypeVar
 from typing import cast
 from urllib.parse import quote_plus
 from urllib.parse import urlparse
 
 import orjson
+from pydantic import ConfigDict
+from pydantic import Extra
 from pydantic import validator
 from pydantic.dataclasses import dataclass
 from pydantic.json import pydantic_encoder
 
 from dipdup import env
 from dipdup.exceptions import ConfigInitializationException
 from dipdup.exceptions import ConfigurationError
@@ -63,15 +65,15 @@
 DEFAULT_POSTGRES_PORT = 5432
 DEFAULT_SQLITE_PATH = ':memory:'
 
 
 _logger = logging.getLogger(__name__)
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class SqliteDatabaseConfig:
     """
     SQLite connection config
 
     :param kind: always 'sqlite'
     :param path: Path to .sqlite3 file, leave default for in-memory database (`:memory:`)
     :param immune_tables: List of tables to preserve during reindexing
@@ -84,23 +86,28 @@
     @property
     def schema_name(self) -> str:
         # NOTE: Used only as identifier in `dipdup_schema` dable, since Hasura integration is not supported for SQLite.
         return DEFAULT_POSTGRES_SCHEMA
 
     @property
     def connection_string(self) -> str:
+        if self.path != DEFAULT_SQLITE_PATH:
+            path = Path(self.path).resolve()
+            path.parent.mkdir(parents=True, exist_ok=True)
+            return f'{self.kind}:///{path}'
+
         return f'{self.kind}://{self.path}'
 
     @property
     def connection_timeout(self) -> int:
         # NOTE: Fail immediately
         return 1
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class PostgresDatabaseConfig:
     """Postgres database connection config
 
     :param kind: always 'postgres'
     :param host: Host
     :param port: Port
     :param user: User
@@ -146,15 +153,15 @@
     def _valid_immune_tables(cls, v: set[str]) -> set[str]:
         for table in v:
             if table.startswith('dipdup'):
                 raise ConfigurationError("Tables with `dipdup` prefix can't be immune")
         return v
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class HttpConfig:
     """Advanced configuration of HTTP client
 
     :param retry_count: Number of retries after request failed before giving up
     :param retry_sleep: Sleep time between retries
     :param retry_multiplier: Multiplier for sleep time between retries
     :param ratelimit_rate: Number of requests per period ("drops" in leaky bucket)
@@ -180,15 +187,15 @@
     request_timeout: int | None = None
     batch_size: int | None = None
     polling_interval: float | None = None
     replay_path: str | None = None
     alias: str | None = None
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class ResolvedHttpConfig:
     __doc__ = HttpConfig.__doc__
 
     retry_count: int = 10
     retry_sleep: float = 1.0
     retry_multiplier: float = 2.0
     ratelimit_rate: int = 0
@@ -215,15 +222,15 @@
                 continue
             for k, v in merge_config.__dict__.items():
                 if v is not None:
                     setattr(config, k, v)
         return config
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class NameMixin:
     def __post_init_post_parse__(self) -> None:
         self._name: str | None = None
 
     @property
     def name(self) -> str:
         if self._name is None:
@@ -271,15 +278,15 @@
 
 class IndexDatasourceConfig(DatasourceConfig):
     """Datasource that can be used as a primary source of historical data"""
 
     ...
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class CodegenMixin(ABC):
     """Base for pattern config classes containing methods required for codegen"""
 
     @abstractmethod
     def iter_imports(self, package: str) -> Iterator[tuple[str, str]]: ...
 
     @abstractmethod
@@ -308,15 +315,15 @@
             kwargs[name] = cast(type | None, locate(cls))
         return kwargs
 
 
 ParentT = TypeVar('ParentT')
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class ParentMixin(Generic[ParentT]):
     """`parent` field for index and template configs"""
 
     def __post_init_post_parse__(self: ParentMixin[ParentT]) -> None:
         self._parent: ParentT | None = None
 
     @property
@@ -324,41 +331,41 @@
         return self._parent
 
     @parent.setter
     def parent(self, value: ParentT) -> None:
         self._parent = value
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class CallbackMixin(CodegenMixin):
     """Mixin for callback configs
 
     :param callback: Callback name
     """
 
     callback: str
 
     def __post_init_post_parse__(self) -> None:
         if self.callback and self.callback != pascal_to_snake(self.callback, strip_dots=False):
             raise ConfigurationError('`callback` field must be a valid Python module name')
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class HandlerConfig(CallbackMixin, ParentMixin['IndexConfig']):
     """Base class for index handlers
 
     :param callback: Callback name
     """
 
     def __post_init_post_parse__(self) -> None:
         CallbackMixin.__post_init_post_parse__(self)
         ParentMixin.__post_init_post_parse__(self)
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class IndexTemplateConfig(NameMixin):
     """Index template config
 
     :param kind: always 'template'
     :param values: Values to be substituted in template (`<key>` -> `value`)
     :param first_level: Level to start indexing from
     :param last_level: Level to stop indexing at
@@ -369,15 +376,15 @@
     kind = 'template'
     template: str
     values: dict[str, str]
     first_level: int = 0
     last_level: int = 0
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class IndexConfig(ABC, NameMixin, ParentMixin['ResolvedIndexConfigU']):
     """Index config
 
     :param kind: Defined by child class
     :param datasource: Alias of index datasource in `datasources` section
     """
 
@@ -407,15 +414,15 @@
     @classmethod
     def strip(cls, config_dict: dict[str, Any]) -> None:
         """Strip config from tunables that are not needed for hash calculation."""
         config_dict['datasource'].pop('http', None)
         config_dict['datasource'].pop('buffer_size', None)
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class HasuraConfig:
     """Config for the Hasura integration.
 
     :param url: URL of the Hasura instance.
     :param admin_secret: Admin secret of the Hasura instance.
     :param create_source: Whether source should be added to Hasura if missing.
     :param source: Hasura source for DipDup to configure, others will be left untouched.
@@ -449,15 +456,15 @@
     def headers(self) -> dict[str, str]:
         """Headers to include with every request"""
         if self.admin_secret:
             return {'X-Hasura-Admin-Secret': self.admin_secret}
         return {}
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class JobConfig(NameMixin):
     """Job schedule config
 
     :param hook: Name of hook to run
     :param args: Arguments to pass to the hook
     :param crontab: Schedule with crontab syntax (`* * * * *`)
     :param interval: Schedule with interval in seconds
@@ -476,15 +483,15 @@
             raise ConfigurationError('Only one of `crontab`, `interval` of `daemon` can be specified')
         if not schedules_enabled:
             raise ConfigurationError('One of `crontab`, `interval` or `daemon` must be specified')
 
         NameMixin.__post_init_post_parse__(self)
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class SentryConfig:
     """Config for Sentry integration.
 
     :param dsn: DSN of the Sentry instance
     :param environment: Environment; if not set, guessed from docker/ci/gha/local.
     :param server_name: Server name; defaults to obfuscated hostname.
     :param release: Release version; defaults to DipDup package version.
@@ -496,29 +503,29 @@
     environment: str | None = None
     server_name: str | None = None
     release: str | None = None
     user_id: str | None = None
     debug: bool = False
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class PrometheusConfig:
     """Config for Prometheus integration.
 
     :param host: Host to bind to
     :param port: Port to bind to
     :param update_interval: Interval to update some metrics in seconds
     """
 
     host: str
     port: int = 8000
     update_interval: float = 1.0
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class HookConfig(CallbackMixin):
     """Hook config
 
     :param callback: Callback name
     :param args: Mapping of argument names and annotations (checked lazily when possible)
     :param atomic: Wrap hook in a single database transaction
     """
@@ -535,15 +542,15 @@
         yield 'dipdup.context', 'HookContext'
         for _, annotation in self.args.items():
             with suppress(ValueError):
                 package, obj = annotation.rsplit('.', 1)
                 yield package, obj
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class SystemHookConfig(HookConfig):
     __doc__ = HookConfig.__doc__
 
 
 system_hooks = {
     # NOTE: Fires on every run after datasources and schema are initialized.
     # NOTE: Default: nothing.
@@ -569,27 +576,27 @@
     # NOTE: Default: nothing.
     'on_synchronized': SystemHookConfig(
         callback='on_synchronized',
     ),
 }
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class ApiConfig:
     """Management API config
 
     :param host: Host to bind to
     :param port: Port to bind to
     """
 
     host: str = '127.0.0.1'
     port: int = 46339  # dial INDEX 😎
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class AdvancedConfig:
     """This section allows users to tune some system-wide options, either experimental or unsuitable for generic configurations.
 
     :param reindex: Mapping of reindexing reasons and actions DipDup performs.
     :param scheduler: `apscheduler` scheduler config.
     :param postpone_jobs: Do not start job scheduler until all indexes reach the realtime state.
     :param early_realtime: Establish realtime connection and start collecting messages while sync is in progress (faster, but consumes more RAM).
```

### Comparing `dipdup-7.5.3/src/dipdup/config/abi_etherscan.py` & `dipdup-7.5.4/src/dipdup/config/abi_etherscan.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from typing import Literal
 
+from pydantic import ConfigDict
+from pydantic import Extra
 from pydantic.dataclasses import dataclass
 
 from dipdup.config import AbiDatasourceConfig
 from dipdup.config import HttpConfig
 
 DEFAULT_ETHERSCAN_URL = 'https://api.etherscan.io/api'
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class EtherscanDatasourceConfig(AbiDatasourceConfig):
     """Etherscan datasource config
 
     :param kind: always 'abi.etherscan'
     :param url: API URL
     :param api_key: API key
     :param http: HTTP client configuration
```

### Comparing `dipdup-7.5.3/src/dipdup/config/coinbase.py` & `dipdup-7.5.4/src/dipdup/config/coinbase.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from dataclasses import field
 from typing import Literal
 
+from pydantic import ConfigDict
+from pydantic import Extra
 from pydantic.dataclasses import dataclass
 
 from dipdup.config import DatasourceConfig
 from dipdup.config import HttpConfig
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class CoinbaseDatasourceConfig(DatasourceConfig):
     """Coinbase datasource config
 
     :param kind: always 'coinbase'
     :param api_key: API key
     :param secret_key: API secret key
     :param passphrase: API passphrase
```

### Comparing `dipdup-7.5.3/src/dipdup/config/evm.py` & `dipdup-7.5.4/src/dipdup/config/evm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from typing import Literal
 
 from eth_utils.address import is_address
 from eth_utils.address import to_normalized_address
+from pydantic import ConfigDict
+from pydantic import Extra
 from pydantic import validator
 from pydantic.dataclasses import dataclass
 
 from dipdup.config import ContractConfig
 from dipdup.exceptions import ConfigurationError
 
 EVM_ADDRESS_PREFIXES = ('0x',)
 EVM_ADDRESS_LENGTH = 42
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class EvmContractConfig(ContractConfig):
     """EVM contract config
 
     :param kind: Always `evm`
     :param address: Contract address
     :param abi: Contract ABI
     :param typename: Alias for the contract script
@@ -30,15 +32,15 @@
     @validator('address', 'abi', allow_reuse=True)
     def _valid_address(cls, v: str | None) -> str | None:
         # NOTE: It's a `config export` call with environment variable substitution disabled
         if not v or '$' in v:
             return v
 
         if not is_address(v):
-            raise ConfigurationError(f'{v} is not a valid EVM contract address')
+            raise ValueError(f'{v} is not a valid EVM contract address')
         # NOTE: Normalizing is converting address to a non-checksum form.
         # See https://coincodex.com/article/2078/ethereum-address-checksum-explained/
         return to_normalized_address(v)
 
     def get_address(self) -> str:
         if self.address is None:
             raise ConfigurationError(f'`contracts.{self.name}`: `address` field is required`')
```

### Comparing `dipdup-7.5.3/src/dipdup/config/evm_node.py` & `dipdup-7.5.4/src/dipdup/config/evm_node.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 from typing import Literal
 
+from pydantic import ConfigDict
+from pydantic import Extra
 from pydantic import validator
 from pydantic.dataclasses import dataclass
 
 from dipdup.config import HttpConfig
 from dipdup.config import IndexDatasourceConfig
-from dipdup.exceptions import ConfigurationError
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class EvmNodeDatasourceConfig(IndexDatasourceConfig):
     """Subsquid datasource config
 
     :param kind: Always 'evm.node'
     :param url: Ethereum node URL
     :param ws_url: Ethereum node WebSocket URL
     :param http: HTTP client configuration
@@ -30,15 +31,15 @@
     @property
     def merge_subscriptions(self) -> bool:
         return False
 
     @validator('url')
     def _valid_url(cls, v: str) -> str:
         if not v.startswith(('http://', 'https://')):
-            raise ConfigurationError('Ethereum node URL must start with http(s)://')
+            raise ValueError('Ethereum node URL must start with http(s)://')
         return v
 
     @validator('ws_url')
     def _valid_ws_url(cls, v: str | None) -> str | None:
         if v and not v.startswith(('ws://', 'wss://')):
-            raise ConfigurationError('Ethereum node WebSocket URL must start with ws(s)://')
+            raise ValueError('Ethereum node WebSocket URL must start with ws(s)://')
         return v
```

### Comparing `dipdup-7.5.3/src/dipdup/config/evm_subsquid.py` & `dipdup-7.5.4/src/dipdup/config/evm_subsquid.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from __future__ import annotations
 
 import random
 from abc import ABC
 from typing import Literal
 
+from pydantic import ConfigDict
+from pydantic import Extra
 from pydantic import validator
 from pydantic.dataclasses import dataclass
 
 from dipdup.config import HttpConfig
 from dipdup.config import IndexConfig
 from dipdup.config import IndexDatasourceConfig
 from dipdup.config.evm_node import EvmNodeDatasourceConfig
 from dipdup.exceptions import ConfigurationError
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class SubsquidDatasourceConfig(IndexDatasourceConfig):
     """Subsquid datasource config
 
     :param kind: always 'evm.subsquid'
     :param url: URL of Subsquid Network API
     :param node: One or more `evm.node` datasource(s) for the same network
     :param http: HTTP client configuration
@@ -46,15 +48,15 @@
     @validator('url')
     def _valid_url(cls, v: str) -> str:
         if not v.startswith(('http', 'https')):
             raise ConfigurationError('Subsquid Network URL must start with http(s)')
         return v
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class SubsquidIndexConfig(IndexConfig, ABC):
     """EVM index that use Subsquid Network as a datasource
 
     :param kind: starts with 'evm.subsquid'
     :param datasource: Subsquid datasource config
     """
```

### Comparing `dipdup-7.5.3/src/dipdup/config/evm_subsquid_events.py` & `dipdup-7.5.4/src/dipdup/config/evm_subsquid_events.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 from dataclasses import field
 from typing import TYPE_CHECKING
 from typing import Literal
 
+from pydantic import ConfigDict
+from pydantic import Extra
 from pydantic.dataclasses import dataclass
 
 from dipdup.config import AbiDatasourceConfig
 from dipdup.config import HandlerConfig
 from dipdup.config.evm import EvmContractConfig
 from dipdup.config.evm_subsquid import SubsquidDatasourceConfig
 from dipdup.config.evm_subsquid import SubsquidIndexConfig
@@ -18,15 +20,15 @@
 
 if TYPE_CHECKING:
     from collections.abc import Iterator
 
     from dipdup.subscriptions import Subscription
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class SubsquidEventsHandlerConfig(HandlerConfig):
     """Subsquid event handler
 
     :param callback: Callback name
     :param contract: EVM contract
     :param name: Event name
     """
@@ -46,15 +48,15 @@
 
     def iter_arguments(self) -> Iterator[tuple[str, str]]:
         event_cls = snake_to_pascal(self.name)
         yield 'ctx', 'HandlerContext'
         yield 'event', f'SubsquidEvent[{event_cls}]'
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class SubsquidEventsIndexConfig(SubsquidIndexConfig):
     """Subsquid datasource config
 
     :param kind: Always 'evm.subsquid.events'
     :param datasource: Subsquid datasource
     :param handlers: Event handlers
     :param abi: One or more `evm.abi` datasource(s) for the same network
```

### Comparing `dipdup-7.5.3/src/dipdup/config/evm_subsquid_traces.py` & `dipdup-7.5.4/src/dipdup/config/evm_subsquid_traces.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from __future__ import annotations
 
 from dataclasses import field
 from typing import Literal
 
+from pydantic import ConfigDict
+from pydantic import Extra
 from pydantic.dataclasses import dataclass
 
 from dipdup.config import AbiDatasourceConfig
 from dipdup.config import HandlerConfig
 from dipdup.config.evm_subsquid import SubsquidDatasourceConfig
 from dipdup.config.evm_subsquid import SubsquidIndexConfig
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class SubsquidTracesHandlerConfig(HandlerConfig): ...
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class SubsquidTracesIndexConfig(SubsquidIndexConfig):
     kind: Literal['evm.subsquid.traces']
 
     datasource: SubsquidDatasourceConfig
     handlers: tuple[SubsquidTracesHandlerConfig, ...] = field(default_factory=tuple)
     abi: AbiDatasourceConfig | tuple[AbiDatasourceConfig, ...] | None = None
     node_only: bool = False
```

### Comparing `dipdup-7.5.3/src/dipdup/config/evm_subsquid_transactions.py` & `dipdup-7.5.4/src/dipdup/config/evm_subsquid_transactions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 from dataclasses import field
 from typing import TYPE_CHECKING
 from typing import Literal
 
+from pydantic import ConfigDict
+from pydantic import Extra
 from pydantic.dataclasses import dataclass
 
 from dipdup.config import AbiDatasourceConfig
 from dipdup.config import CodegenMixin
 from dipdup.config import HandlerConfig
 from dipdup.config.evm import EvmContractConfig
 from dipdup.config.evm_subsquid import SubsquidDatasourceConfig
@@ -17,24 +19,25 @@
 from dipdup.utils import pascal_to_snake
 from dipdup.utils import snake_to_pascal
 
 if TYPE_CHECKING:
     from collections.abc import Iterator
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class SubsquidTransactionsHandlerConfig(HandlerConfig, CodegenMixin):
     """Subsquid transaction handler
 
     :param callback: Callback name
     :param from_: Transaction sender
     :param to: Transaction receiver
     :param method: Method name
     """
 
+    # FIXME: Can't use `from_` field alias in dataclasses (fixed in `next` with Pydantic v2)
     from_: EvmContractConfig | None = None
     to: EvmContractConfig | None = None
     method: str | None = None
 
     def iter_imports(self, package: str) -> Iterator[tuple[str, str]]:
         yield 'dipdup.context', 'HandlerContext'
         yield package, 'models as models'
@@ -61,15 +64,15 @@
     @property
     def typed_contract(self) -> EvmContractConfig | None:
         if self.method and self.to:
             return self.to
         return None
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class SubsquidTransactionsIndexConfig(SubsquidIndexConfig):
     """Index that uses Subsquid Network as a datasource for transactions
 
     :param kind: always 'evm.subsquid.transactions'
     :param datasource: Subsquid datasource config
     :param handlers: Transaction handlers
     :param abi: One or many ABI datasource(s)
```

### Comparing `dipdup-7.5.3/src/dipdup/config/ipfs.py` & `dipdup-7.5.4/src/dipdup/config/ipfs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from typing import Literal
 
+from pydantic import ConfigDict
+from pydantic import Extra
 from pydantic.dataclasses import dataclass
 
 from dipdup.config import DatasourceConfig
 from dipdup.config import HttpConfig
 
 DEFAULT_IPFS_URL = 'https://ipfs.io/ipfs'
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class IpfsDatasourceConfig(DatasourceConfig):
     """IPFS datasource config
 
     :param kind: always 'ipfs'
     :param url: IPFS node URL, e.g. https://ipfs.io/ipfs/
     :param http: HTTP client configuration
     """
```

### Comparing `dipdup-7.5.3/src/dipdup/config/tezos.py` & `dipdup-7.5.4/src/dipdup/config/tezos.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Literal
 
+from pydantic import ConfigDict
+from pydantic import Extra
 from pydantic import validator
 from pydantic.dataclasses import dataclass
 
 from dipdup.config import ContractConfig
 from dipdup.exceptions import ConfigurationError
 from dipdup.exceptions import FrameworkException
 
@@ -21,15 +23,15 @@
     return len(address) == ADDRESS_LENGTH and address.startswith(SMART_ROLLUP_PREFIX)
 
 
 def is_wallet_address(address: str) -> bool:
     return len(address) == ADDRESS_LENGTH and address.startswith(WALLET_PREFIXES)
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class TezosContractConfig(ContractConfig):
     """Tezos contract config.
 
     :param kind: Always `tezos`
     :param address: Contract address
     :param code_hash: Contract code hash or address to fetch it from
     :param typename: Alias for the contract script
```

### Comparing `dipdup-7.5.3/src/dipdup/config/tezos_tzkt.py` & `dipdup-7.5.4/src/dipdup/config/tezos_tzkt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Literal
 from urllib.parse import urlparse
 
+from pydantic import ConfigDict
+from pydantic import Extra
 from pydantic.dataclasses import dataclass
 
 from dipdup.config import HttpConfig
 from dipdup.config import IndexConfig
 from dipdup.config import IndexDatasourceConfig
 from dipdup.exceptions import ConfigurationError
 from dipdup.models.tezos_tzkt import HeadSubscription
@@ -18,15 +20,15 @@
 }
 
 
 DEFAULT_TZKT_URL = next(iter(TZKT_API_URLS.keys()))
 MAX_BATCH_SIZE = 10000
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class TzktDatasourceConfig(IndexDatasourceConfig):
     """TzKT datasource config
 
     :param kind: always 'tezos.tzkt'
     :param url: Base API URL, e.g. https://api.tzkt.io/
     :param http: HTTP client configuration
     :param buffer_size: Number of levels to keep in FIFO buffer before processing
@@ -52,15 +54,15 @@
         if '$' in self.url:
             return
         parsed_url = urlparse(self.url)
         if not (parsed_url.scheme and parsed_url.netloc):
             raise ConfigurationError(f'`{self.url}` is not a valid TzKT API URL')
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class TzktIndexConfig(IndexConfig):
     """TzKT index config
 
     :param kind: starts with 'tezos.tzkt'
     :param datasource: `tezos.tzkt` datasource to use
     """
```

### Comparing `dipdup-7.5.3/src/dipdup/config/tezos_tzkt_big_maps.py` & `dipdup-7.5.4/src/dipdup/config/tezos_tzkt_big_maps.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Literal
 
+from pydantic import ConfigDict
+from pydantic import Extra
 from pydantic.dataclasses import dataclass
 
 from dipdup.config import ContractConfig
 from dipdup.config import HandlerConfig
 from dipdup.config.tezos import TezosContractConfig
 from dipdup.config.tezos_tzkt import TzktDatasourceConfig
 from dipdup.config.tezos_tzkt import TzktIndexConfig
@@ -18,15 +20,15 @@
 
 if TYPE_CHECKING:
     from collections.abc import Iterator
 
     from dipdup.subscriptions import Subscription
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class TzktBigMapsHandlerConfig(HandlerConfig):
     """Big map handler config
 
     :param callback: Callback name
     :param contract: Contract to fetch big map from
     :param path: Path to big map (alphanumeric string with dots)
     """
@@ -61,15 +63,15 @@
         yield self.format_value_import(package, self.contract.module_name, self.path)
 
     def iter_arguments(self) -> Iterator[tuple[str, str]]:
         yield 'ctx', 'HandlerContext'
         yield self.format_big_map_diff_argument(self.path)
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class TzktBigMapsIndexConfig(TzktIndexConfig):
     """Big map index config
 
     :param kind: always 'tezos.tzkt.big_maps'
     :param datasource: Index datasource to fetch big maps with
     :param handlers: Mapping of big map diff handlers
     :param skip_history: Fetch only current big map keys ignoring historical changes
```

### Comparing `dipdup-7.5.3/src/dipdup/config/tezos_tzkt_events.py` & `dipdup-7.5.4/src/dipdup/config/tezos_tzkt_events.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 from dataclasses import field
 from typing import TYPE_CHECKING
 from typing import Literal
 
+from pydantic import ConfigDict
+from pydantic import Extra
 from pydantic.dataclasses import dataclass
 
 from dipdup.config import HandlerConfig
 from dipdup.config.tezos import TezosContractConfig
 from dipdup.config.tezos_tzkt import TzktDatasourceConfig
 from dipdup.config.tezos_tzkt import TzktIndexConfig
 from dipdup.models.tezos_tzkt import EventSubscription
@@ -16,15 +18,15 @@
 
 if TYPE_CHECKING:
     from collections.abc import Iterator
 
     from dipdup.subscriptions import Subscription
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class TzktEventsHandlerConfig(HandlerConfig):
     """Event handler config
 
     :param callback: Callback name
     :param contract: Contract which emits event
     :param tag: Event tag
     """
@@ -44,15 +46,15 @@
 
     def iter_arguments(self) -> Iterator[tuple[str, str]]:
         event_cls = snake_to_pascal(self.tag + '_payload')
         yield 'ctx', 'HandlerContext'
         yield 'event', f'TzktEvent[{event_cls}]'
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class TzktEventsUnknownEventHandlerConfig(HandlerConfig):
     """Unknown event handler config
 
     :param callback: Callback name
     :param contract: Contract which emits event
     """
 
@@ -67,15 +69,15 @@
         yield 'ctx', 'HandlerContext'
         yield 'event', 'TzktUnknownEvent'
 
 
 TzktEventsHandlerConfigU = TzktEventsHandlerConfig | TzktEventsUnknownEventHandlerConfig
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class TzktEventsIndexConfig(TzktIndexConfig):
     """Event index config
 
     :param kind: always 'tezos.tzkt.events'
     :param datasource: Datasource config
     :param handlers: Event handlers
     :param first_level: First block level to index
```

### Comparing `dipdup-7.5.3/src/dipdup/config/tezos_tzkt_head.py` & `dipdup-7.5.4/src/dipdup/config/tezos_tzkt_head.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from typing import Literal
 
+from pydantic import ConfigDict
+from pydantic import Extra
 from pydantic.dataclasses import dataclass
 
 from dipdup.config import HandlerConfig
 from dipdup.config.tezos_tzkt import TzktDatasourceConfig
 from dipdup.config.tezos_tzkt import TzktIndexConfig
 
 if TYPE_CHECKING:
     from collections.abc import Iterator
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class HeadHandlerConfig(HandlerConfig):
     """Head block handler config
 
     :param callback: Callback name
     """
 
     def iter_imports(self, package: str) -> Iterator[tuple[str, str]]:
@@ -26,15 +28,15 @@
         yield package, 'models as models'
 
     def iter_arguments(self) -> Iterator[tuple[str, str]]:
         yield 'ctx', 'HandlerContext'
         yield 'head', 'TzktHeadBlockData'
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class TzktHeadIndexConfig(TzktIndexConfig):
     """Head block index config
 
     :param kind: always 'tezos.tzkt.head'
     :param callback: Callback name
     :param datasource: Index datasource to receive head blocks
     :param handlers: Mapping of head block handlers
```

### Comparing `dipdup-7.5.3/src/dipdup/config/tezos_tzkt_operations.py` & `dipdup-7.5.4/src/dipdup/config/tezos_tzkt_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from dataclasses import field
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Literal
 from typing import cast
 
+from pydantic import ConfigDict
+from pydantic import Extra
 from pydantic.dataclasses import dataclass
 
 from dipdup.config import CodegenMixin
 from dipdup.config import HandlerConfig
 from dipdup.config.tezos import TezosContractConfig
 from dipdup.config.tezos_tzkt import TzktDatasourceConfig
 from dipdup.config.tezos_tzkt import TzktIndexConfig
@@ -24,15 +26,15 @@
 
 if TYPE_CHECKING:
     from collections.abc import Iterator
 
     from dipdup.subscriptions import Subscription
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class SubgroupIndexMixin:
     """`subgroup_index` field to track index of operation in group
 
     :param subgroup_index:
     """
 
     def __post_init_post_parse__(self) -> None:
@@ -123,15 +125,15 @@
     ) -> tuple[str, str]:
         arg_name = pascal_to_snake(alias or f'{type_}_{subgroup_index}')
         if optional:
             return arg_name, 'TzktOperationData | None'
         return arg_name, 'TzktOperationData'
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class OperationsHandlerTransactionPatternConfig(TezosPatternConfig, SubgroupIndexMixin):
     """Transaction handler pattern config
 
     :param type: always 'transaction'
     :param source: Match operations by source contract alias
     :param destination: Match operations by destination contract alias
     :param entrypoint: Match operations by contract entrypoint
@@ -183,15 +185,15 @@
     @property
     def typed_contract(self) -> TezosContractConfig | None:
         if self.entrypoint and self.destination:
             return self.destination
         return None
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class OperationsHandlerOriginationPatternConfig(TezosPatternConfig, SubgroupIndexMixin):
     """Origination handler pattern config
 
     :param type: always 'origination'
     :param source: Match operations by source contract alias
     :param originated_contract: Match origination of exact contract
     :param optional: Whether can operation be missing in operation group
@@ -232,15 +234,15 @@
     @property
     def typed_contract(self) -> TezosContractConfig | None:
         if self.originated_contract:
             return self.originated_contract
         return None
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class OperationsHandlerSmartRollupExecutePatternConfig(TezosPatternConfig, SubgroupIndexMixin):
     """Operation handler pattern config
 
     :param type: always 'sr_execute'
     :param source: Match operations by source contract alias
     :param destination: Match operations by destination contract alias
     :param optional: Whether can operation be missing in operation group
@@ -269,15 +271,15 @@
     @property
     def typed_contract(self) -> TezosContractConfig | None:
         if self.destination:
             return self.destination
         return None
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class TzktOperationsIndexConfig(TzktIndexConfig):
     """Operation index config
 
     :param kind: always 'tezos.tzkt.operations'
     :param datasource: Alias of index datasource in `datasources` section
     :param handlers: List of indexer handlers
     :param types: Types of transaction to fetch
@@ -333,15 +335,15 @@
 OperationsHandlerPatternConfigU = (
     OperationsHandlerTransactionPatternConfig
     | OperationsHandlerOriginationPatternConfig
     | OperationsHandlerSmartRollupExecutePatternConfig
 )
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class TzktOperationsHandlerConfig(HandlerConfig):
     """Operation handler config
 
     :param callback: Callback name
     :param pattern: Filters to match operation groups
     """
 
@@ -365,15 +367,15 @@
                         f' `{self.callback}`\n              entrypoint: `{arg}`'
                     ),
                 )
             arg_names.add(arg)
             yield arg, arg_type
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class OperationUnfilteredHandlerConfig(HandlerConfig):
     """Handler of unfiltered operation index
 
     :param callback: Callback name
     """
 
     def iter_imports(self, package: str) -> Iterator[tuple[str, str]]:
@@ -382,15 +384,15 @@
         yield package, 'models as models'
 
     def iter_arguments(self) -> Iterator[tuple[str, str]]:
         yield 'ctx', 'HandlerContext'
         yield 'operation', 'TzktOperationData'
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class TzktOperationsUnfilteredIndexConfig(TzktIndexConfig):
     """Operation index config
 
     :param kind: always 'tezos.tzkt.operations_unfiltered'
     :param datasource: Alias of index datasource in `datasources` section
     :param callback: Callback name
     :param types: Types of transaction to fetch
```

### Comparing `dipdup-7.5.3/src/dipdup/config/tezos_tzkt_token_balances.py` & `dipdup-7.5.4/src/dipdup/config/tezos_tzkt_token_balances.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from typing import Literal
 
+from pydantic import ConfigDict
+from pydantic import Extra
 from pydantic.dataclasses import dataclass
 from pydantic.fields import Field
 
 from dipdup.config import ContractConfig
 from dipdup.config import HandlerConfig
 from dipdup.config.tezos import TezosContractConfig
 from dipdup.config.tezos_tzkt import TzktDatasourceConfig
@@ -15,15 +17,15 @@
 
 if TYPE_CHECKING:
     from collections.abc import Iterator
 
     from dipdup.subscriptions import Subscription
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class TzktTokenBalancesHandlerConfig(HandlerConfig):
     """Token balance handler config
 
     :param callback: Callback name
     :param contract: Filter by contract
     :param token_id: Filter by token ID
     """
@@ -39,15 +41,15 @@
 
     def iter_arguments(self) -> Iterator[tuple[str, str]]:
         """This iterator result will be used in codegen to generate handler(s) template"""
         yield 'ctx', 'HandlerContext'
         yield 'token_balance', 'TzktTokenBalanceData'
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class TzktTokenBalancesIndexConfig(TzktIndexConfig):
     """Token balance index config
 
     :param kind: always 'tezos.tzkt.token_balances'
     :param datasource: Index datasource to use
     :param handlers: Mapping of token transfer handlers
```

### Comparing `dipdup-7.5.3/src/dipdup/config/tezos_tzkt_token_transfers.py` & `dipdup-7.5.4/src/dipdup/config/tezos_tzkt_token_transfers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from typing import Literal
 
+from pydantic import ConfigDict
+from pydantic import Extra
 from pydantic.dataclasses import dataclass
 from pydantic.fields import Field
 
 from dipdup.config import ContractConfig
 from dipdup.config import HandlerConfig
 from dipdup.config.tezos import TezosContractConfig
 from dipdup.config.tezos_tzkt import TzktDatasourceConfig
@@ -15,43 +17,42 @@
 
 if TYPE_CHECKING:
     from collections.abc import Iterator
 
     from dipdup.subscriptions import Subscription
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class TzktTokenTransfersHandlerConfig(HandlerConfig):
     """Token transfer handler config
 
     :param callback: Callback name
     :param contract: Filter by contract
     :param token_id: Filter by token ID
     :param from_: Filter by sender
     :param to: Filter by recipient
     """
 
     contract: TezosContractConfig | None = None
     token_id: int | None = None
-    # FIXME: Can't use `from_` field alias in dataclass
-    # FIXME: See https://github.com/pydantic/pydantic/issues/4286 (fixed in upcoming v2)
+    # FIXME: Can't use `from_` field alias in dataclasses (fixed in `next` with Pydantic v2)
     from_: TezosContractConfig | None = None
     to: TezosContractConfig | None = None
 
     def iter_imports(self, package: str) -> Iterator[tuple[str, str]]:
         yield 'dipdup.context', 'HandlerContext'
         yield 'dipdup.models.tezos_tzkt', 'TzktTokenTransferData'
         yield package, 'models as models'
 
     def iter_arguments(self) -> Iterator[tuple[str, str]]:
         yield 'ctx', 'HandlerContext'
         yield 'token_transfer', 'TzktTokenTransferData'
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class TzktTokenTransfersIndexConfig(TzktIndexConfig):
     """Token transfer index config
 
     :param kind: always 'tezos.tzkt.token_transfers'
     :param datasource: Index datasource to use
     :param handlers: Mapping of token transfer handlers
```

### Comparing `dipdup-7.5.3/src/dipdup/config/tzip_metadata.py` & `dipdup-7.5.4/src/dipdup/config/tzip_metadata.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from typing import Literal
 
+from pydantic import ConfigDict
+from pydantic import Extra
 from pydantic.dataclasses import dataclass
 
 from dipdup.config import DatasourceConfig
 from dipdup.config import HttpConfig
 from dipdup.models.tzip_metadata import TzipMetadataNetwork
 
 DEFAULT_TZIP_METADATA_URL = 'https://metadata.dipdup.net'
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra=Extra.forbid), kw_only=True)
 class TzipMetadataDatasourceConfig(DatasourceConfig):
     """DipDup Metadata datasource config
 
     :param kind: always 'tzip_metadata'
     :param network: Network name, e.g. mainnet, ghostnet, etc.
     :param url: GraphQL API URL, e.g. https://metadata.dipdup.net
     :param http: HTTP client configuration
```

### Comparing `dipdup-7.5.3/src/dipdup/context.py` & `dipdup-7.5.4/src/dipdup/context.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/database.py` & `dipdup-7.5.4/src/dipdup/database.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/datasources/__init__.py` & `dipdup-7.5.4/src/dipdup/datasources/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/datasources/abi_etherscan.py` & `dipdup-7.5.4/src/dipdup/datasources/abi_etherscan.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/datasources/coinbase.py` & `dipdup-7.5.4/src/dipdup/datasources/coinbase.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/datasources/evm_node.py` & `dipdup-7.5.4/src/dipdup/datasources/evm_node.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/datasources/evm_subsquid.py` & `dipdup-7.5.4/src/dipdup/datasources/evm_subsquid.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/datasources/ipfs.py` & `dipdup-7.5.4/src/dipdup/datasources/ipfs.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/datasources/tezos_tzkt.py` & `dipdup-7.5.4/src/dipdup/datasources/tezos_tzkt.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/datasources/tzip_metadata.py` & `dipdup-7.5.4/src/dipdup/datasources/tzip_metadata.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/dipdup.py` & `dipdup-7.5.4/src/dipdup/dipdup.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/env.py` & `dipdup-7.5.4/src/dipdup/env.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/exceptions.py` & `dipdup-7.5.4/src/dipdup/exceptions.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/fetcher.py` & `dipdup-7.5.4/src/dipdup/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/fields.py` & `dipdup-7.5.4/src/dipdup/fields.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/hasura.py` & `dipdup-7.5.4/src/dipdup/hasura.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/http.py` & `dipdup-7.5.4/src/dipdup/http.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/index.py` & `dipdup-7.5.4/src/dipdup/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/evm_node.py` & `dipdup-7.5.4/src/dipdup/indexes/evm_node.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/evm_subsquid.py` & `dipdup-7.5.4/src/dipdup/indexes/evm_subsquid.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/evm_subsquid_events/fetcher.py` & `dipdup-7.5.4/src/dipdup/indexes/evm_subsquid_events/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/evm_subsquid_events/index.py` & `dipdup-7.5.4/src/dipdup/indexes/evm_subsquid_events/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/evm_subsquid_events/matcher.py` & `dipdup-7.5.4/src/dipdup/indexes/evm_subsquid_events/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/evm_subsquid_traces/index.py` & `dipdup-7.5.4/src/dipdup/indexes/evm_subsquid_traces/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/evm_subsquid_transactions/fetcher.py` & `dipdup-7.5.4/src/dipdup/indexes/evm_subsquid_transactions/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/evm_subsquid_transactions/index.py` & `dipdup-7.5.4/src/dipdup/indexes/evm_subsquid_transactions/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/evm_subsquid_transactions/matcher.py` & `dipdup-7.5.4/src/dipdup/indexes/evm_subsquid_transactions/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_big_maps/fetcher.py` & `dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_big_maps/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_big_maps/index.py` & `dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_big_maps/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_big_maps/matcher.py` & `dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_big_maps/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_events/fetcher.py` & `dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_events/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_events/index.py` & `dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_events/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_events/matcher.py` & `dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_events/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_head/index.py` & `dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_head/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_operations/fetcher.py` & `dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_operations/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_operations/index.py` & `dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_operations/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_operations/matcher.py` & `dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_operations/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_operations/parser.py` & `dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_operations/parser.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_token_balances/index.py` & `dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_token_balances/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_token_balances/matcher.py` & `dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_token_balances/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_token_transfers/fetcher.py` & `dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_token_transfers/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_token_transfers/index.py` & `dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_token_transfers/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/indexes/tezos_tzkt_token_transfers/matcher.py` & `dipdup-7.5.4/src/dipdup/indexes/tezos_tzkt_token_transfers/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/install.py` & `dipdup-7.5.4/src/dipdup/install.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/models/__init__.py` & `dipdup-7.5.4/src/dipdup/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/models/coinbase.py` & `dipdup-7.5.4/src/dipdup/models/coinbase.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/models/evm_node.py` & `dipdup-7.5.4/src/dipdup/models/evm_node.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/models/evm_subsquid.py` & `dipdup-7.5.4/src/dipdup/models/evm_subsquid.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/models/tezos_tzkt.py` & `dipdup-7.5.4/src/dipdup/models/tezos_tzkt.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/package.py` & `dipdup-7.5.4/src/dipdup/package.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/performance.py` & `dipdup-7.5.4/src/dipdup/performance.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/project.py` & `dipdup-7.5.4/src/dipdup/project.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/base/Makefile.j2` & `dipdup-7.5.4/src/dipdup/projects/base/Makefile.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/base/README.md.j2` & `dipdup-7.5.4/src/dipdup/projects/base/README.md.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/base/configs/dipdup.compose.yaml.j2` & `dipdup-7.5.4/src/dipdup/projects/base/configs/dipdup.compose.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/base/configs/dipdup.swarm.yaml.j2` & `dipdup-7.5.4/src/dipdup/projects/base/configs/dipdup.swarm.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/base/deploy/compose.swarm.yaml.j2` & `dipdup-7.5.4/src/dipdup/projects/base/deploy/compose.swarm.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/base/deploy/compose.yaml.j2` & `dipdup-7.5.4/src/dipdup/projects/base/deploy/compose.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/base/pyproject.toml.j2` & `dipdup-7.5.4/src/dipdup/projects/base/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_auction/dipdup.yaml.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_auction/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_auction/handlers/on_bid.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_auction/handlers/on_bid.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_auction/handlers/on_create_auction.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_auction/handlers/on_create_auction.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_auction/handlers/on_withdraw.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_auction/handlers/on_withdraw.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_auction/models/__init__.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_auction/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_big_maps/dipdup.yaml.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_big_maps/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_big_maps/handlers/on_update_expiry_map.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_big_maps/handlers/on_update_expiry_map.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_big_maps/handlers/on_update_records.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_big_maps/handlers/on_update_records.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_big_maps/models/__init__.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_big_maps/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_dao/dipdup.yaml.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_dao/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_dao/handlers/on_propose.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_dao/handlers/on_propose.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_dao/models/__init__.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_dao/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_dex/dipdup.yaml.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_dex/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa12_divest_liquidity.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa12_divest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa12_invest_liquidity.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa12_invest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa12_origination.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa12_origination.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa12_tez_to_token.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa12_tez_to_token.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa12_token_to_tez.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa12_token_to_tez.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa12_transfer.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa12_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa12_withdraw_profit.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa12_withdraw_profit.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa2_divest_liquidity.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa2_divest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa2_invest_liquidity.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa2_invest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa2_origination.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa2_origination.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa2_tez_to_token.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa2_tez_to_token.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa2_token_to_tez.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa2_token_to_tez.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa2_transfer.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa2_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_dex/handlers/on_fa2_withdraw_profit.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_dex/handlers/on_fa2_withdraw_profit.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_dex/models/__init__.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_dex/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_domains/dipdup.yaml.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_domains/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_domains/handlers/on_update_expiry_map.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_domains/handlers/on_update_expiry_map.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_domains/handlers/on_update_records.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_domains/handlers/on_update_records.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_domains/hooks/check_expiration.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_domains/hooks/check_expiration.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_domains/models/__init__.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_domains/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_etherlink/dipdup.yaml.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_etherlink/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_events/dipdup.yaml.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_events/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_evm_events/dipdup.yaml.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_evm_events/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_evm_events/handlers/on_transfer.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_evm_events/handlers/on_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_evm_transactions/dipdup.yaml.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_evm_transactions/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_evm_transactions/handlers/on_transfer.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_evm_transactions/handlers/on_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_factories/dipdup.yaml.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_factories/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_factories/handlers/on_factory_origination.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_factories/handlers/on_factory_origination.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_factories/handlers/on_transfer.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_factories/handlers/on_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_nft_marketplace/dipdup.yaml.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_nft_marketplace/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_nft_marketplace/handlers/on_cancel_swap.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_nft_marketplace/handlers/on_cancel_swap.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_nft_marketplace/handlers/on_collect.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_nft_marketplace/handlers/on_collect.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_nft_marketplace/handlers/on_mint.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_nft_marketplace/handlers/on_mint.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_nft_marketplace/handlers/on_swap.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_nft_marketplace/handlers/on_swap.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_nft_marketplace/models/__init__.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_nft_marketplace/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_token/dipdup.yaml.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_token/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_token/handlers/on_mint.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_token/handlers/on_mint.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_token/handlers/on_transfer.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_token/handlers/on_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_token_transfers/handlers/on_balance_update.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_token_transfers/handlers/on_balance_update.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_token_transfers/handlers/on_token_transfer.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_token_transfers/handlers/on_token_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_uniswap/abi/erc20/ERC20.json.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_uniswap/abi/erc20/ERC20.json.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_uniswap/dipdup.yaml.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_uniswap/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_uniswap/handlers/factory/pool_created.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_uniswap/handlers/factory/pool_created.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_uniswap/handlers/pool/burn.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_uniswap/handlers/pool/burn.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_uniswap/handlers/pool/initialize.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_uniswap/handlers/pool/initialize.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_uniswap/handlers/pool/mint.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_uniswap/handlers/pool/mint.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_uniswap/handlers/pool/swap.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_uniswap/handlers/pool/swap.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_uniswap/handlers/position_manager/collect.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_uniswap/handlers/position_manager/collect.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_uniswap/handlers/position_manager/decrease_liquidity.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_uniswap/handlers/position_manager/decrease_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_uniswap/handlers/position_manager/increase_liquidity.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_uniswap/handlers/position_manager/increase_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_uniswap/handlers/position_manager/transfer.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_uniswap/handlers/position_manager/transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_uniswap/models/__init__.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_uniswap/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_uniswap/models/pool.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_uniswap/models/pool.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_uniswap/models/position.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_uniswap/models/position.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_uniswap/models/repo.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_uniswap/models/repo.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_uniswap/models/tick.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_uniswap/models/tick.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_uniswap/models/token.py.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_uniswap/models/token.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_uniswap/sql/on_reindex/20_create_ca_quotes_1m.sql.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_uniswap/sql/on_reindex/20_create_ca_quotes_1m.sql.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_uniswap/sql/on_reindex/21_create_ca_quotes_1h.sql.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_uniswap/sql/on_reindex/21_create_ca_quotes_1h.sql.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/projects/demo_uniswap/sql/on_reindex/22_create_ca_quotes_1d.sql.j2` & `dipdup-7.5.4/src/dipdup/projects/demo_uniswap/sql/on_reindex/22_create_ca_quotes_1d.sql.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/prometheus.py` & `dipdup-7.5.4/src/dipdup/prometheus.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/pysignalr.py` & `dipdup-7.5.4/src/dipdup/pysignalr.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/report.py` & `dipdup-7.5.4/src/dipdup/report.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/scheduler.py` & `dipdup-7.5.4/src/dipdup/scheduler.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/sentry.py` & `dipdup-7.5.4/src/dipdup/sentry.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/sql/dipdup_wipe.sql` & `dipdup-7.5.4/src/dipdup/sql/dipdup_wipe.sql`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/subscriptions.py` & `dipdup-7.5.4/src/dipdup/subscriptions.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/sys.py` & `dipdup-7.5.4/src/dipdup/sys.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/templates/models.py` & `dipdup-7.5.4/src/dipdup/templates/models.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/test.py` & `dipdup-7.5.4/src/dipdup/test.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/transactions.py` & `dipdup-7.5.4/src/dipdup/transactions.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/utils.py` & `dipdup-7.5.4/src/dipdup/utils.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/src/dipdup/yaml.py` & `dipdup-7.5.4/src/dipdup/yaml.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,17 +108,18 @@
     for match in re.finditer(ENV_VARIABLE_REGEX, config_yaml):
         variable, default_value = match.group('var_name'), match.group('default_value')
         environment[variable] = default_value or ''
 
     return environment
 
 
+# FIXME: Can't use `from_` field alias in dataclasses (fixed in `next` with Pydantic v2)
 def fix_dataclass_field_aliases(config: dict[str, Any]) -> None:
     for k, v in copy(config).items():
-        if 'callack' in config and k == 'from':
+        if 'callback' in config and k == 'from':
             config['from_'] = config.pop('from')
         elif isinstance(v, dict):
             fix_dataclass_field_aliases(v)
         elif isinstance(v, list):
             for item in v:
                 if isinstance(item, dict):
                     fix_dataclass_field_aliases(item)
@@ -160,10 +161,9 @@
             raise ConfigurationError(
                 f'Incompatible spec version: expected {__spec_version__}, got {config_spec_version}. See'
                 ' https://dipdup.io/docs/config/spec_version'
             )
 
     def _post_load_hooks(self) -> None:
         self.validate_version()
-        # FIXME: Can't use `from_` field alias in dataclass
-        # FIXME: See https://github.com/pydantic/pydantic/issues/4286 (fixed in upcoming v2)
+        # FIXME: Can't use `from_` field alias in dataclasses (fixed in `next` with Pydantic v2)
         fix_dataclass_field_aliases(self)
```

### Comparing `dipdup-7.5.3/tests/__init__.py` & `dipdup-7.5.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/demo_auction.yml` & `dipdup-7.5.4/tests/configs/demo_auction.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/demo_big_maps.yml` & `dipdup-7.5.4/tests/configs/demo_big_maps.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/demo_dao.yml` & `dipdup-7.5.4/tests/configs/demo_dao.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/demo_dex.yml` & `dipdup-7.5.4/tests/configs/demo_dex.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/demo_domains.yml` & `dipdup-7.5.4/tests/configs/demo_domains.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/demo_etherlink.yaml` & `dipdup-7.5.4/tests/configs/demo_etherlink.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/demo_events.yml` & `dipdup-7.5.4/tests/configs/demo_events.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/demo_evm_events.yml` & `dipdup-7.5.4/tests/configs/demo_evm_events.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/demo_evm_events_node.yml` & `dipdup-7.5.4/tests/configs/demo_evm_events_node.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/demo_evm_transactions.yml` & `dipdup-7.5.4/tests/configs/demo_evm_transactions.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/demo_evm_transactions_node.yml` & `dipdup-7.5.4/tests/configs/demo_evm_transactions_node.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/demo_factories.yml` & `dipdup-7.5.4/tests/configs/demo_factories.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/demo_nft_marketplace.yml` & `dipdup-7.5.4/tests/configs/demo_nft_marketplace.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/demo_raw.yml` & `dipdup-7.5.4/tests/configs/demo_raw.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/demo_token.yml` & `dipdup-7.5.4/tests/configs/demo_token.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/demo_token_transfers.yml` & `dipdup-7.5.4/tests/configs/demo_token_transfers.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/demo_token_transfers_2.yml` & `dipdup-7.5.4/tests/configs/demo_token_transfers_2.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/demo_token_transfers_3.yml` & `dipdup-7.5.4/tests/configs/demo_token_transfers_3.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/demo_token_transfers_4.yml` & `dipdup-7.5.4/tests/configs/demo_token_transfers_4.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/dipdup.yml` & `dipdup-7.5.4/tests/configs/dipdup.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/hen_subjkt.yml` & `dipdup-7.5.4/tests/configs/hen_subjkt.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/kolibri_ovens.yml` & `dipdup-7.5.4/tests/configs/kolibri_ovens.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/operation_filters.yml` & `dipdup-7.5.4/tests/configs/operation_filters.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/configs/yupana.yml` & `dipdup-7.5.4/tests/configs/yupana.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/profile_abi_decoding.py` & `dipdup-7.5.4/tests/profile_abi_decoding.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/0535b2dcc93076e6026fa48cc501adaed47b7b060e6483d8312f40c184d7287d` & `dipdup-7.5.4/tests/replays/0535b2dcc93076e6026fa48cc501adaed47b7b060e6483d8312f40c184d7287d`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/0eaaba2830dbdd3a80286fbc367084bce6e55c678e21da178a7eb16beef6c997` & `dipdup-7.5.4/tests/replays/0eaaba2830dbdd3a80286fbc367084bce6e55c678e21da178a7eb16beef6c997`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/1228b36594bb93d619170ad49373f1ceec52d10faafdd727b37f3cdeffd663db` & `dipdup-7.5.4/tests/replays/1228b36594bb93d619170ad49373f1ceec52d10faafdd727b37f3cdeffd663db`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/13afdf001ce3d6a0219c0f7f6d372d9b645770e5f4304576f7f7a37b45af96fc` & `dipdup-7.5.4/tests/replays/13afdf001ce3d6a0219c0f7f6d372d9b645770e5f4304576f7f7a37b45af96fc`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/27373c23411bf37b605c8d0ead9a0e6c6c1f1718ce7863b095b759811e44e155` & `dipdup-7.5.4/tests/replays/27373c23411bf37b605c8d0ead9a0e6c6c1f1718ce7863b095b759811e44e155`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/2a45ec6372b45e46199a6af24272cb93586777a0522cd1203b3eeef213ce4583` & `dipdup-7.5.4/tests/replays/2a45ec6372b45e46199a6af24272cb93586777a0522cd1203b3eeef213ce4583`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/383899084f79460e96fd311bb64e4925738c486b39d6281539456c5fcac41620` & `dipdup-7.5.4/tests/replays/383899084f79460e96fd311bb64e4925738c486b39d6281539456c5fcac41620`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/388fe9107380b6dd1e9ce3a87c23abd56ad39dfb6cb8a5a27b959e5b0434633b` & `dipdup-7.5.4/tests/replays/388fe9107380b6dd1e9ce3a87c23abd56ad39dfb6cb8a5a27b959e5b0434633b`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/39b8664d1bca5d374ff905c8a3a396b53d19ee469dc37545a8ca6b080bd0e9e0` & `dipdup-7.5.4/tests/replays/39b8664d1bca5d374ff905c8a3a396b53d19ee469dc37545a8ca6b080bd0e9e0`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/3a2bd8b6b72bf18152d2550c106789fa9b8abc98ea9d759a6597b7ebfbab0fc2` & `dipdup-7.5.4/tests/replays/3a2bd8b6b72bf18152d2550c106789fa9b8abc98ea9d759a6597b7ebfbab0fc2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/3f5927db41422038d8e2cc203ef56a769c66b25835cdee42b17bc61e600be550` & `dipdup-7.5.4/tests/replays/3f5927db41422038d8e2cc203ef56a769c66b25835cdee42b17bc61e600be550`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/43cb0ab415d8b8b3f7addc3e82ea27d93b2c66ff55c117e1e0c7c64a0fcfc3f2` & `dipdup-7.5.4/tests/replays/43cb0ab415d8b8b3f7addc3e82ea27d93b2c66ff55c117e1e0c7c64a0fcfc3f2`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/4a57776d93475adfd9c49b6c3295a7cedfc23b73733a1fb5f0c985ee039dc5dc` & `dipdup-7.5.4/tests/replays/4a57776d93475adfd9c49b6c3295a7cedfc23b73733a1fb5f0c985ee039dc5dc`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/4aa7f9b0657be0c44baf2caed8c7cb08d02097a4095cf6417f78cba3a25e8423` & `dipdup-7.5.4/tests/replays/4aa7f9b0657be0c44baf2caed8c7cb08d02097a4095cf6417f78cba3a25e8423`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/5483a0e11009e0f186bf70c214e2597d267a75a1e19152a9e7ed1ec257ce88ca` & `dipdup-7.5.4/tests/replays/5483a0e11009e0f186bf70c214e2597d267a75a1e19152a9e7ed1ec257ce88ca`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/587613799ebfae42b1884016d1a44a452d68e70e3ed80641d90b8e7657ba8ee5` & `dipdup-7.5.4/tests/replays/587613799ebfae42b1884016d1a44a452d68e70e3ed80641d90b8e7657ba8ee5`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/5b99bc4beb6a9a33f7d2f118426458e4c788e0ab6d9e51949d3ccbf8b4003fc1` & `dipdup-7.5.4/tests/replays/5b99bc4beb6a9a33f7d2f118426458e4c788e0ab6d9e51949d3ccbf8b4003fc1`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/607ecfd3653eda82aac502ac370c6ad7144d30c1e3c525ed520d44f9edf5b7e9` & `dipdup-7.5.4/tests/replays/607ecfd3653eda82aac502ac370c6ad7144d30c1e3c525ed520d44f9edf5b7e9`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/6d76a3c3f427ff534c551de1793cb1d1dfbd22ccad97f5917a9f9b201a3f9804` & `dipdup-7.5.4/tests/replays/6d76a3c3f427ff534c551de1793cb1d1dfbd22ccad97f5917a9f9b201a3f9804`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/6fa41b68da742cc7cf8a0d68baef77ce8b2e9abf765767318d7ff4cf453ded4c` & `dipdup-7.5.4/tests/replays/6fa41b68da742cc7cf8a0d68baef77ce8b2e9abf765767318d7ff4cf453ded4c`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/7b6cf9b8c69712bf26ed09059352ec740606969bf20eab0dedda870273f4fde9` & `dipdup-7.5.4/tests/replays/7b6cf9b8c69712bf26ed09059352ec740606969bf20eab0dedda870273f4fde9`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/803e05a8d0bb9e7cfb49530271d43ea62111b6419e7cded2d221f7e0e0c92ece` & `dipdup-7.5.4/tests/replays/803e05a8d0bb9e7cfb49530271d43ea62111b6419e7cded2d221f7e0e0c92ece`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/8060a1f95213d470ee947a12242ef76cb7fb0c05bbaecc385eb6ec4a20d694c4` & `dipdup-7.5.4/tests/replays/8060a1f95213d470ee947a12242ef76cb7fb0c05bbaecc385eb6ec4a20d694c4`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/93516225810a23a6799f2f9a1dee055ca79a66ee2b8d0f32be820c9c385e936b` & `dipdup-7.5.4/tests/replays/93516225810a23a6799f2f9a1dee055ca79a66ee2b8d0f32be820c9c385e936b`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/9e6e907842da2cd494c558ea5ecc211fd12e56bfc547450978fb7dfe03853e58` & `dipdup-7.5.4/tests/replays/9e6e907842da2cd494c558ea5ecc211fd12e56bfc547450978fb7dfe03853e58`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/a3ce91a1b0d505cc221f0e201781466ba1e2d6dc7b624b9bc75a03ce3dbb0f92` & `dipdup-7.5.4/tests/replays/a3ce91a1b0d505cc221f0e201781466ba1e2d6dc7b624b9bc75a03ce3dbb0f92`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/aa8fe6037996b296bf9a3011e45cd9ecb92fb728592a843f91b03b2848cb1fb1` & `dipdup-7.5.4/tests/replays/aa8fe6037996b296bf9a3011e45cd9ecb92fb728592a843f91b03b2848cb1fb1`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/acaa57345850f3b76471a7b3a8fb76b7f83e824f1520a2e0ee8ec93cdd6cb1c3` & `dipdup-7.5.4/tests/replays/acaa57345850f3b76471a7b3a8fb76b7f83e824f1520a2e0ee8ec93cdd6cb1c3`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/acc952ba1905717315212f952ed689d7b8f683165b31c0a7a25199aed9fda27f` & `dipdup-7.5.4/tests/replays/acc952ba1905717315212f952ed689d7b8f683165b31c0a7a25199aed9fda27f`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/b3af887f7ad8172af75b94a09bedfb9ae1e14f8819a36d6ce9f709721068263b` & `dipdup-7.5.4/tests/replays/b3af887f7ad8172af75b94a09bedfb9ae1e14f8819a36d6ce9f709721068263b`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/b89b0ea704071e273d3c74a4dbb7b4f6c6fd9ea1848c69b452dce4f04872d3b5` & `dipdup-7.5.4/tests/replays/b89b0ea704071e273d3c74a4dbb7b4f6c6fd9ea1848c69b452dce4f04872d3b5`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/bec4433b4206f00c2310a7961cff7f539434b9161b45673793aa5a3b50234313` & `dipdup-7.5.4/tests/replays/bec4433b4206f00c2310a7961cff7f539434b9161b45673793aa5a3b50234313`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/c1c3eef91f7149d7aa2da072f71598f3ad5e29250cfa441bb6d4411acd70d657` & `dipdup-7.5.4/tests/replays/c1c3eef91f7149d7aa2da072f71598f3ad5e29250cfa441bb6d4411acd70d657`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/cc5d3d4a58d5cb6bc7270d38c797b7740b79f913590ef0164abd50e58fba9405` & `dipdup-7.5.4/tests/replays/cc5d3d4a58d5cb6bc7270d38c797b7740b79f913590ef0164abd50e58fba9405`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/d0a594d14bcb3fbf916092ec6707dfd3c9f48f53f0a1ad40a32023e7a87f8ef5` & `dipdup-7.5.4/tests/replays/d0a594d14bcb3fbf916092ec6707dfd3c9f48f53f0a1ad40a32023e7a87f8ef5`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/d62748a927a09395579b5790c8f871cc8653081cf4475abc93173989f950b92b` & `dipdup-7.5.4/tests/replays/d62748a927a09395579b5790c8f871cc8653081cf4475abc93173989f950b92b`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/d94397f6ecec8ce25f87177fe410f6498d7d30a04360506c0cd300d291c167e7` & `dipdup-7.5.4/tests/replays/d94397f6ecec8ce25f87177fe410f6498d7d30a04360506c0cd300d291c167e7`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/dca9cf4f9f27623f10975d369444899458ab9ea85c22af2da6ce6ce8c09c2b58` & `dipdup-7.5.4/tests/replays/dca9cf4f9f27623f10975d369444899458ab9ea85c22af2da6ce6ce8c09c2b58`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/dd5d267c6e8e943a637ede23d708587123b9184560358d294be7fbed0d4b587a` & `dipdup-7.5.4/tests/replays/dd5d267c6e8e943a637ede23d708587123b9184560358d294be7fbed0d4b587a`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/e10e6552f0dce5124e0d72b74c508541a8098c407c9a3b0d2e10a7408b4d7cfe` & `dipdup-7.5.4/tests/replays/e10e6552f0dce5124e0d72b74c508541a8098c407c9a3b0d2e10a7408b4d7cfe`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/e4a563a0b19379a44e9d2dc398131e9fd30d6039ff4ffacf1252db0bf8b433aa` & `dipdup-7.5.4/tests/replays/e4a563a0b19379a44e9d2dc398131e9fd30d6039ff4ffacf1252db0bf8b433aa`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/eb8b6b33cb2e165d1a3a73c09938d3083671a82ad73d4c0cff1fb2a5e5715f76` & `dipdup-7.5.4/tests/replays/eb8b6b33cb2e165d1a3a73c09938d3083671a82ad73d4c0cff1fb2a5e5715f76`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/eb8e2c3ce2fe7792d2c8e81c61d37821275b64021343103b0c955042ae802189` & `dipdup-7.5.4/tests/replays/eb8e2c3ce2fe7792d2c8e81c61d37821275b64021343103b0c955042ae802189`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/f3d608f99e6b92e28a064bb9c10c3c605c9c817383c1eebcc68f663d1d23d650` & `dipdup-7.5.4/tests/replays/f3d608f99e6b92e28a064bb9c10c3c605c9c817383c1eebcc68f663d1d23d650`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/f7d244938de3e3d153e4ef8172cab0f1e896b801904a54ac034d3d14352ee64a` & `dipdup-7.5.4/tests/replays/f7d244938de3e3d153e4ef8172cab0f1e896b801904a54ac034d3d14352ee64a`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/f9fa1571c3d850f4a19c286205291893d184a9d124390d0358034a8b8366556d` & `dipdup-7.5.4/tests/replays/f9fa1571c3d850f4a19c286205291893d184a9d124390d0358034a8b8366556d`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/fe80425d17f2467fccc527a99b5a11da144f63f9a3cab83989be0f8fed737264` & `dipdup-7.5.4/tests/replays/fe80425d17f2467fccc527a99b5a11da144f63f9a3cab83989be0f8fed737264`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/replays/ff51b3535acc2972090ecd5db3af8f827464c9d92f1aa661630976e5b4ed4cbe` & `dipdup-7.5.4/tests/replays/ff51b3535acc2972090ecd5db3af8f827464c9d92f1aa661630976e5b4ed4cbe`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/responses/asdf.json` & `dipdup-7.5.4/tests/responses/asdf.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/responses/ftzfun.json` & `dipdup-7.5.4/tests/responses/ftzfun.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/responses/hen_subjkt.json` & `dipdup-7.5.4/tests/responses/hen_subjkt.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/responses/hjkl.json` & `dipdup-7.5.4/tests/responses/hjkl.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/responses/kolibri_ovens.json` & `dipdup-7.5.4/tests/responses/kolibri_ovens.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/responses/ooQuCAKBHkmWy2VciDAV9c6CFTywuMLupLzVoKDwS1xvR4EdRng.json` & `dipdup-7.5.4/tests/responses/ooQuCAKBHkmWy2VciDAV9c6CFTywuMLupLzVoKDwS1xvR4EdRng.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/responses/origination_amount.json` & `dipdup-7.5.4/tests/responses/origination_amount.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/responses/qwer.json` & `dipdup-7.5.4/tests/responses/qwer.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/responses/rewq.json` & `dipdup-7.5.4/tests/responses/rewq.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/responses/yupana.json` & `dipdup-7.5.4/tests/responses/yupana.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/responses/zxcv.json` & `dipdup-7.5.4/tests/responses/zxcv.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/schemas/asdf/storage.json` & `dipdup-7.5.4/tests/schemas/asdf/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/schemas/hen_subjkt/storage.json` & `dipdup-7.5.4/tests/schemas/hen_subjkt/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/schemas/hjkl/storage.json` & `dipdup-7.5.4/tests/schemas/hjkl/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/schemas/kolibri_ovens/storage.json` & `dipdup-7.5.4/tests/schemas/kolibri_ovens/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/schemas/qwer/storage.json` & `dipdup-7.5.4/tests/schemas/qwer/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/schemas/rewq/storage.json` & `dipdup-7.5.4/tests/schemas/rewq/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/schemas/yupana/storage.json` & `dipdup-7.5.4/tests/schemas/yupana/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/schemas/zxcv/storage.json` & `dipdup-7.5.4/tests/schemas/zxcv/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/test_config/test_callbacks.py` & `dipdup-7.5.4/tests/test_config/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/test_config/test_config.py` & `dipdup-7.5.4/tests/test_config/test_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 from pydantic import ValidationError
 
 from dipdup.config import DipDupConfig
 from dipdup.config import HasuraConfig
 from dipdup.config import HttpConfig
 from dipdup.config import PostgresDatabaseConfig
 from dipdup.config import ResolvedHttpConfig
+from dipdup.config.evm_subsquid_transactions import SubsquidTransactionsHandlerConfig
 from dipdup.config.tezos import TezosContractConfig
 from dipdup.config.tezos_tzkt import TzktDatasourceConfig
 from dipdup.config.tezos_tzkt_operations import TzktOperationsIndexConfig
 from dipdup.exceptions import ConfigurationError
 from dipdup.models.tezos_tzkt import HeadSubscription
 from dipdup.models.tezos_tzkt import OriginationSubscription
 from dipdup.models.tezos_tzkt import TransactionSubscription
 from dipdup.models.tezos_tzkt import TzktOperationType
+from dipdup.yaml import DipDupYAMLConfig
 
 
 def create_config(merge_subs: bool = False, origs: bool = False) -> DipDupConfig:
     path = Path(__file__).parent.parent / 'configs' / 'dipdup.yaml'
     config = DipDupConfig.load([path])
     if origs:
         config.indexes['hen_mainnet'].types += (TzktOperationType.origination,)  # type: ignore
@@ -74,14 +76,33 @@
         TezosContractConfig(kind='tezos', address='KT1lalala')
     with pytest.raises(ValidationError):
         TezosContractConfig(kind='tezos', address='lalalalalalalalalalalalalalalalalala')
     with pytest.raises(ConfigurationError):
         TzktDatasourceConfig(kind='tezos.tzkt', url='not_an_url')
 
 
+async def test_reserved_keywords() -> None:
+    assert (
+        SubsquidTransactionsHandlerConfig(  # type: ignore[comparison-overlap]
+            callback='test',
+            from_='from',  # type: ignore[arg-type]
+        ).from_
+        == 'from'
+    )
+
+    # FIXME: Can't use `from_` field alias in dataclasses (fixed in `next` with Pydantic v2)
+    raw_config, _ = DipDupYAMLConfig.load(
+        paths=[Path(__file__).parent.parent / 'configs' / 'demo_token_transfers_4.yml']
+    )
+    assert raw_config['indexes']['tzbtc_holders_mainnet']['handlers'][1]['from_'] == 'tzbtc_mainnet'
+
+    config = DipDupConfig.load([Path(__file__).parent.parent / 'configs' / 'demo_token_transfers_4.yml'])
+    assert config.indexes['tzbtc_holders_mainnet'].handlers[1].from_ == 'tzbtc_mainnet'  # type: ignore[union-attr]
+
+
 async def test_dump() -> None:
     config = create_config()
 
     tmp_path = Path(tempfile.mkstemp(suffix='yaml')[1])
     tmp_path.write_text(config.dump())
 
     config = DipDupConfig.load([tmp_path], environment=False)
```

### Comparing `dipdup-7.5.3/tests/test_config/test_custom_config.py` & `dipdup-7.5.4/tests/test_config/test_custom_config.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/test_datasources/test_ipfs.py` & `dipdup-7.5.4/tests/test_datasources/test_ipfs.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/test_datasources/test_metadata.py` & `dipdup-7.5.4/tests/test_datasources/test_metadata.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/test_datasources/test_tzkt.py` & `dipdup-7.5.4/tests/test_datasources/test_tzkt.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/test_datasources/test_tzkt_blocks.py` & `dipdup-7.5.4/tests/test_datasources/test_tzkt_blocks.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/test_datasources/test_tzkt_buffer.py` & `dipdup-7.5.4/tests/test_datasources/test_tzkt_buffer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/test_datasources/test_tzkt_quotes.py` & `dipdup-7.5.4/tests/test_datasources/test_tzkt_quotes.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/test_demos.py` & `dipdup-7.5.4/tests/test_demos.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,29 +172,30 @@
     ('demo_token.yml', 'demo_token', 'run', assert_run_token),
     ('demo_token.yml', 'demo_token', 'init', None),
     ('demo_nft_marketplace.yml', 'demo_nft_marketplace', 'run', assert_run_nft_marketplace),
     ('demo_nft_marketplace.yml', 'demo_nft_marketplace', 'init', None),
     ('demo_auction.yml', 'demo_auction', 'run', assert_run_auction),
     ('demo_auction.yml', 'demo_auction', 'init', None),
     ('demo_token_transfers.yml', 'demo_token_transfers', 'run', partial(assert_run_token_transfers, 4, '-0.01912431')),
-    # FIXME: Why so many token transfer tests?
+    # TODO: Too many token transfer runs
     ('demo_token_transfers.yml', 'demo_token_transfers', 'init', None),
     (
         'demo_token_transfers_2.yml',
         'demo_token_transfers',
         'run',
         partial(assert_run_token_transfers, 12, '0.26554711'),
     ),
     ('demo_token_transfers_3.yml', 'demo_token_transfers', 'run', partial(assert_run_token_transfers, 9, '0.15579888')),
-    (
-        'demo_token_transfers_4.yml',
-        'demo_token_transfers',
-        'run',
-        partial(assert_run_token_transfers, 2, '-0.02302128'),
-    ),
+    # FIXME: Reenable after fixing fetcher
+    # (
+    #     'demo_token_transfers_4.yml',
+    #     'demo_token_transfers',
+    #     'run',
+    #     partial(assert_run_token_transfers, 2, '-0.02302128'),
+    # ),
     ('demo_token_balances.yml', 'demo_token_balances', 'run', assert_run_balances),
     ('demo_token_balances.yml', 'demo_token_balances', 'init', None),
     ('demo_big_maps.yml', 'demo_big_maps', 'run', assert_run_big_maps),
     ('demo_big_maps.yml', 'demo_big_maps', 'init', None),
     ('demo_domains.yml', 'demo_domains', 'run', assert_run_domains),
     ('demo_domains.yml', 'demo_domains', 'init', None),
     ('demo_dex.yml', 'demo_dex', 'run', assert_run_dex),
```

### Comparing `dipdup-7.5.3/tests/test_dipdup.py` & `dipdup-7.5.4/tests/test_dipdup.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/test_hasura.py` & `dipdup-7.5.4/tests/test_hasura.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,16 +63,16 @@
 
     fake_api = web.Application()
     fake_api.router.add_get('/healthz', healthcheck_response)
     fake_api.router.add_get('/v1/version', version_response)
     fake_client: TestClient = await aiohttp_client(fake_api)
 
     fake_client_url = f'http://{fake_client.server.host}:{fake_client.server.port}'
-    hasura_config = HasuraConfig(fake_client_url)
-    postgres_config = PostgresDatabaseConfig('postgres', 'localhost')
+    hasura_config = HasuraConfig(url=fake_client_url)
+    postgres_config = PostgresDatabaseConfig(kind='postgres', host='localhost')
 
     hasura_gateway = HasuraGateway('demo_nft_marketplace', hasura_config, postgres_config)
 
     with pytest.raises(UnsupportedAPIError):
         async with hasura_gateway:
             async with tortoise_wrapper('sqlite://:memory:', 'demo_nft_marketplace.models'):
                 await Tortoise.generate_schemas()
```

### Comparing `dipdup-7.5.3/tests/test_index/test_tzkt_operations.py` & `dipdup-7.5.4/tests/test_index/test_tzkt_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,58 +52,58 @@
 
 async def test_get_origination_filters(
     tzkt: TzktDatasource,
     index_config: TzktOperationsIndexConfig,
 ) -> None:
     index_config.handlers = (
         TzktOperationsHandlerConfig(
-            'address_origination',
-            (
+            callback='address_origination',
+            pattern=(
                 OperationsHandlerOriginationPatternConfig(
                     originated_contract=index_config.contracts[0],
                 ),
             ),
         ),
     )
     addresses, hashes = await get_origination_filters(index_config, tzkt)
     assert addresses == {'KT1RJ6PbjHpwc3M5rw5s2Nbmefwbuwbdxton'}
     assert not hashes
 
     index_config.handlers = (
         TzktOperationsHandlerConfig(
-            'hash_origination',
-            (
+            callback='hash_origination',
+            pattern=(
                 OperationsHandlerOriginationPatternConfig(
                     originated_contract=index_config.contracts[1],
                 ),
             ),
         ),
     )
     addresses, hashes = await get_origination_filters(index_config, tzkt)
     assert not addresses
     assert hashes == {-1585533315}
 
     index_config.handlers = (
         TzktOperationsHandlerConfig(
-            'hash_address_origination',
-            (
+            callback='hash_address_origination',
+            pattern=(
                 OperationsHandlerOriginationPatternConfig(
                     originated_contract=index_config.contracts[2],
                 ),
             ),
         ),
     )
     # NOTE: Resolved earlier
     with pytest.raises(FrameworkException):
         await get_origination_filters(index_config, tzkt)
 
     index_config.handlers = (
         TzktOperationsHandlerConfig(
-            'address_source',
-            (
+            callback='address_source',
+            pattern=(
                 OperationsHandlerOriginationPatternConfig(
                     source=index_config.contracts[0],
                 ),
             ),
         ),
     )
     addresses, hashes = await get_origination_filters(index_config, tzkt)
```

### Comparing `dipdup-7.5.3/tests/test_introspection.py` & `dipdup-7.5.4/tests/test_introspection.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/test_models.py` & `dipdup-7.5.4/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/test_rollback.py` & `dipdup-7.5.4/tests/test_rollback.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/test_schema.py` & `dipdup-7.5.4/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/test_utils.py` & `dipdup-7.5.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/types/bazaar/storage.py` & `dipdup-7.5.4/tests/types/bazaar/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/types/ftzfun/storage.py` & `dipdup-7.5.4/tests/types/ftzfun/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/types/hen_subjkt/storage.py` & `dipdup-7.5.4/tests/types/hen_subjkt/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/types/hjkl/storage.py` & `dipdup-7.5.4/tests/types/hjkl/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/types/rewq/storage.py` & `dipdup-7.5.4/tests/types/rewq/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/types/tezotop/storage.py` & `dipdup-7.5.4/tests/types/tezotop/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/types/yupana/storage.py` & `dipdup-7.5.4/tests/types/yupana/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/tests/types/zxcv/storage.py` & `dipdup-7.5.4/tests/types/zxcv/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.5.3/PKG-INFO` & `dipdup-7.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dipdup
-Version: 7.5.3
+Version: 7.5.4
 Summary: Modular framework for creating selective indexers and featureful backends for dapps
 Keywords: api backend blockchain crypto cryptocurrencies dapp declarative ethereum evm framework indexer indexers michelson scheduler sdk smart-contracts tezos tzkt web3
 Author-Email: Lev Gorodetskii <dipdup@drsr.io>, Vladimir Bobrikov <vladimir_bobrikov@pm.me>, Michael Zaikin <mz@baking-bad.org>
 Maintainer-Email: Lev Gorodetskii <dipdup@drsr.io>, Vladimir Bobrikov <vladimir_bobrikov@pm.me>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```


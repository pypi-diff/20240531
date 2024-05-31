# Comparing `tmp/skibidi_orm-0.1.2.tar.gz` & `tmp/skibidi_orm-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skibidi_orm-0.1.2.tar", last modified: Thu May 30 14:06:50 2024, max compression
+gzip compressed data, was "skibidi_orm-0.1.21.tar", last modified: Fri May 31 12:48:48 2024, max compression
```

## Comparing `skibidi_orm-0.1.2.tar` & `skibidi_orm-0.1.21.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0       26 2024-05-30 14:06:36.673241 skibidi_orm-0.1.2/README.md
--rw-r--r--   0        0        0      775 2024-05-30 14:06:50.049237 skibidi_orm-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/__init__.py
--rw-r--r--   0        0        0     2653 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/cli/run.py
--rw-r--r--   0        0        0      596 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/cli/utils.py
--rw-r--r--   0        0        0      136 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/exceptions/cli_exceptions.py
--rw-r--r--   0        0        0      190 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/exceptions/constraints.py
--rw-r--r--   0        0        0      172 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/exceptions/db_mutator_exceptions.py
--rw-r--r--   0        0        0      309 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/exceptions/operations.py
--rw-r--r--   0        0        0        0 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/adapters/__init__.py
--rw-r--r--   0        0        0     1299 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/adapters/base_adapter.py
--rw-r--r--   0        0        0        0 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/adapters/database_objects/__init__.py
--rw-r--r--   0        0        0     2192 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/adapters/database_objects/constraints.py
--rw-r--r--   0        0        0      901 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/adapters/database_objects/migration_element.py
--rw-r--r--   0        0        0     1614 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/adapters/sqlite3_adapter.py
--rw-r--r--   0        0        0      515 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/adapters/sqlite3_typing.py
--rw-r--r--   0        0        0     3410 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/converters/base/interfaces.py
--rw-r--r--   0        0        0     1065 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/converters/sqlite3/all.py
--rw-r--r--   0        0        0     3904 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/converters/sqlite3/columns.py
--rw-r--r--   0        0        0     1974 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/converters/sqlite3/constraints.py
--rw-r--r--   0        0        0     5440 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/converters/sqlite3/tables.py
--rw-r--r--   0        0        0     1053 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/data_mutator/base_data_mutator.py
--rw-r--r--   0        0        0     2508 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/data_mutator/sqlite3_data_mutatorr.py
--rw-r--r--   0        0        0     1062 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/db_config/base_config.py
--rw-r--r--   0        0        0      192 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/db_config/postgres_config.py
--rw-r--r--   0        0        0      392 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/db_config/sqlite3_config.py
--rw-r--r--   0        0        0      671 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/db_inspectors/base_inspector.py
--rw-r--r--   0        0        0     6025 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/db_inspectors/sqlite3_inspector.py
--rw-r--r--   0        0        0     6589 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/operations/column_operations.py
--rw-r--r--   0        0        0      280 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/operations/operation_type.py
--rw-r--r--   0        0        0     2286 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/operations/table_operations.py
--rw-r--r--   0        0        0      585 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/sql_executor/base_sql_executor.py
--rw-r--r--   0        0        0     2173 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/sql_executor/sqlite3_executor.py
--rw-r--r--   0        0        0      694 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/state_manager/i_state_manager.py
--rw-r--r--   0        0        0     5556 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/state_manager/state_manager.py
--rw-r--r--   0        0        0     3053 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/server.py
--rw-r--r--   0        0        0      436 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/.eslintrc.cjs
--rw-r--r--   0        0        0      248 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/.gitignore
--rw-r--r--   0        0        0     1300 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/README.md
--rw-r--r--   0        0        0      339 2024-05-30 14:06:36.677240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/components.json
--rw-r--r--   0        0        0  2063635 2024-05-30 14:06:36.685240 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CT5dnm0u.js
--rw-r--r--   0        0        0   318663 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CU2I10C2.css
--rw-r--r--   0        0        0      283 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index.lazy-CokS8x6w.js
--rw-r--r--   0        0        0      464 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/index.html
--rw-r--r--   0        0        0     1497 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/vite.svg
--rw-r--r--   0        0        0      366 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/index.html
--rw-r--r--   0        0        0     1617 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/package.json
--rw-r--r--   0        0        0   134211 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0       80 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/postcss.config.js
--rw-r--r--   0        0        0     1497 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/public/vite.svg
--rw-r--r--   0        0        0     4126 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/assets/react.svg
--rw-r--r--   0        0        0      926 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Providers.tsx
--rw-r--r--   0        0        0     1038 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Sidebar.tsx
--rw-r--r--   0        0        0     1337 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/WorkspaceEditor.tsx
--rw-r--r--   0        0        0     2121 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/commands-hisotry-dialog.tsx
--rw-r--r--   0        0        0     1377 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/mode-toggle.tsx
--rw-r--r--   0        0        0     1322 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/queryResultsTable.tsx
--rw-r--r--   0        0        0     1730 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/theme-provider.tsx
--rw-r--r--   0        0        0     1835 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/button.tsx
--rw-r--r--   0        0        0      315 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/collapsible.tsx
--rw-r--r--   0        0        0     3835 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dialog.tsx
--rw-r--r--   0        0        0     7295 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dropdown-menu.tsx
--rw-r--r--   0        0        0     1709 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/resizable.tsx
--rw-r--r--   0        0        0      772 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/textarea.tsx
--rw-r--r--   0        0        0     1361 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/delete-table-row.ts
--rw-r--r--   0        0        0     1529 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/edit-row.ts
--rw-r--r--   0        0        0     1224 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-data.ts
--rw-r--r--   0        0        0     1054 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-info.ts
--rw-r--r--   0        0        0      945 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/run-command.ts
--rw-r--r--   0        0        0     1140 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandResult.tsx
--rw-r--r--   0        0        0     1726 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandsHistory.tsx
--rw-r--r--   0        0        0     1595 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/index.css
--rw-r--r--   0        0        0      764 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/react-query.ts
--rw-r--r--   0        0        0      355 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/table-data-utils.ts
--rw-r--r--   0        0        0      166 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/utils.ts
--rw-r--r--   0        0        0      790 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/main.tsx
--rw-r--r--   0        0        0     1409 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routeTree.gen.ts
--rw-r--r--   0        0        0     1173 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/__root.tsx
--rw-r--r--   0        0        0      343 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/index.lazy.tsx
--rw-r--r--   0        0        0     7445 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/table/$tableName.tsx
--rw-r--r--   0        0        0     1211 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/styles/ag-custom.css
--rw-r--r--   0        0        0       38 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/vite-env.d.ts
--rw-r--r--   0        0        0     2143 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tailwind.config.js
--rw-r--r--   0        0        0      711 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.json
--rw-r--r--   0        0        0      233 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.node.json
--rw-r--r--   0        0        0      378 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/vite.config.ts
--rw-r--r--   0        0        0      617 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/utils/db_config_dynamic_import.py
--rw-r--r--   0        0        0      784 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/utils/get_db_inspector.py
--rw-r--r--   0        0        0      566 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/utils/get_db_seeder.py
--rw-r--r--   0        0        0     3476 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/table_example.py
--rw-r--r--   0        0        0        0 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/tests/skibidi-orm/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/tests/skibidi-orm/cli/schema.py
--rw-r--r--   0        0        0     2136 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/tests/skibidi-orm/cli/test_run.py
--rw-r--r--   0        0        0     1654 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/conftest.py
--rw-r--r--   0        0        0     7281 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/converters/sqlite3/test_column_operations_conversion.py
--rw-r--r--   0        0        0     2619 2024-05-30 14:06:36.689241 skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/converters/sqlite3/test_constraint_conversion.py
--rw-r--r--   0        0        0     4963 2024-05-30 14:06:36.693241 skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/converters/sqlite3/test_table_operations_conversion.py
--rw-r--r--   0        0        0     1447 2024-05-30 14:06:36.693241 skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/db_config/test_config.py
--rw-r--r--   0        0        0     6182 2024-05-30 14:06:36.693241 skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/db_inspector/test_db_inspectors.py
--rw-r--r--   0        0        0     9737 2024-05-30 14:06:36.693241 skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/db_mutators/test_sqlite3_mutator.py
--rw-r--r--   0        0        0     7425 2024-05-30 14:06:36.693241 skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/operations/test_operations.py
--rw-r--r--   0        0        0      967 2024-05-30 14:06:36.693241 skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/sql_executor/test_sqlite3_executor.py
--rw-r--r--   0        0        0    17111 2024-05-30 14:06:36.693241 skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/state_manager/test_state_manager.py
--rw-r--r--   0        0        0     2146 2024-05-30 14:06:36.693241 skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/studio/test_db_config_dynamic_import.py
--rw-r--r--   0        0        0      805 2024-05-30 14:06:36.693241 skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/studio/test_get_db_inspector.py
--rw-r--r--   0        0        0      736 2024-05-30 14:06:36.693241 skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/studio/test_get_db_mutator.py
--rw-r--r--   0        0        0     4268 2024-05-30 14:06:36.693241 skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/studio/test_routes.py
--rw-r--r--   0        0        0    17767 2024-05-30 14:06:36.693241 skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/test_module_cooperation.py
--rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 skibidi_orm-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       26 2024-05-31 12:48:35.997451 skibidi_orm-0.1.21/README.md
+-rw-r--r--   0        0        0      776 2024-05-31 12:48:48.045357 skibidi_orm-0.1.21/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/__init__.py
+-rw-r--r--   0        0        0     2653 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/cli/run.py
+-rw-r--r--   0        0        0      596 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/cli/utils.py
+-rw-r--r--   0        0        0      136 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/exceptions/cli_exceptions.py
+-rw-r--r--   0        0        0      190 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/exceptions/constraints.py
+-rw-r--r--   0        0        0      172 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/exceptions/db_mutator_exceptions.py
+-rw-r--r--   0        0        0      309 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/exceptions/operations.py
+-rw-r--r--   0        0        0        0 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/__init__.py
+-rw-r--r--   0        0        0     1299 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/base_adapter.py
+-rw-r--r--   0        0        0        0 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/database_objects/__init__.py
+-rw-r--r--   0        0        0     2192 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/database_objects/constraints.py
+-rw-r--r--   0        0        0      901 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/database_objects/migration_element.py
+-rw-r--r--   0        0        0     1614 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/sqlite3_adapter.py
+-rw-r--r--   0        0        0      515 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/sqlite3_typing.py
+-rw-r--r--   0        0        0     3410 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/converters/base/interfaces.py
+-rw-r--r--   0        0        0     1065 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/converters/sqlite3/all.py
+-rw-r--r--   0        0        0     3904 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/converters/sqlite3/columns.py
+-rw-r--r--   0        0        0     1974 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/converters/sqlite3/constraints.py
+-rw-r--r--   0        0        0     5440 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/converters/sqlite3/tables.py
+-rw-r--r--   0        0        0     1053 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/data_mutator/base_data_mutator.py
+-rw-r--r--   0        0        0     2508 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/data_mutator/sqlite3_data_mutatorr.py
+-rw-r--r--   0        0        0     1062 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/db_config/base_config.py
+-rw-r--r--   0        0        0      192 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/db_config/postgres_config.py
+-rw-r--r--   0        0        0      392 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/db_config/sqlite3_config.py
+-rw-r--r--   0        0        0      671 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/db_inspectors/base_inspector.py
+-rw-r--r--   0        0        0     6025 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/db_inspectors/sqlite3_inspector.py
+-rw-r--r--   0        0        0     6589 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/operations/column_operations.py
+-rw-r--r--   0        0        0      280 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/operations/operation_type.py
+-rw-r--r--   0        0        0     2286 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/operations/table_operations.py
+-rw-r--r--   0        0        0      585 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/sql_executor/base_sql_executor.py
+-rw-r--r--   0        0        0     2173 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/sql_executor/sqlite3_executor.py
+-rw-r--r--   0        0        0      694 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/state_manager/i_state_manager.py
+-rw-r--r--   0        0        0     5556 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/state_manager/state_manager.py
+-rw-r--r--   0        0        0     3113 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/server.py
+-rw-r--r--   0        0        0      436 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/.eslintrc.cjs
+-rw-r--r--   0        0        0      248 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/.gitignore
+-rw-r--r--   0        0        0     1300 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/README.md
+-rw-r--r--   0        0        0      339 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/components.json
+-rw-r--r--   0        0        0  2063635 2024-05-31 12:48:36.009451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CT5dnm0u.js
+-rw-r--r--   0        0        0   318663 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CU2I10C2.css
+-rw-r--r--   0        0        0      283 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index.lazy-CokS8x6w.js
+-rw-r--r--   0        0        0      464 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/index.html
+-rw-r--r--   0        0        0     1497 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/vite.svg
+-rw-r--r--   0        0        0      366 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/index.html
+-rw-r--r--   0        0        0     1617 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/package.json
+-rw-r--r--   0        0        0   134211 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0       80 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/postcss.config.js
+-rw-r--r--   0        0        0     1497 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/public/vite.svg
+-rw-r--r--   0        0        0     4126 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/assets/react.svg
+-rw-r--r--   0        0        0      926 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Providers.tsx
+-rw-r--r--   0        0        0     1038 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Sidebar.tsx
+-rw-r--r--   0        0        0     1337 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/WorkspaceEditor.tsx
+-rw-r--r--   0        0        0     2121 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/commands-hisotry-dialog.tsx
+-rw-r--r--   0        0        0     1377 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/mode-toggle.tsx
+-rw-r--r--   0        0        0     1322 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/queryResultsTable.tsx
+-rw-r--r--   0        0        0     1730 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/theme-provider.tsx
+-rw-r--r--   0        0        0     1835 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/button.tsx
+-rw-r--r--   0        0        0      315 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/collapsible.tsx
+-rw-r--r--   0        0        0     3835 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dialog.tsx
+-rw-r--r--   0        0        0     7295 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dropdown-menu.tsx
+-rw-r--r--   0        0        0     1709 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/resizable.tsx
+-rw-r--r--   0        0        0      772 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/textarea.tsx
+-rw-r--r--   0        0        0     1361 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/delete-table-row.ts
+-rw-r--r--   0        0        0     1529 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/edit-row.ts
+-rw-r--r--   0        0        0     1224 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-data.ts
+-rw-r--r--   0        0        0     1054 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-info.ts
+-rw-r--r--   0        0        0      945 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/run-command.ts
+-rw-r--r--   0        0        0     1140 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandResult.tsx
+-rw-r--r--   0        0        0     1726 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandsHistory.tsx
+-rw-r--r--   0        0        0     1595 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/index.css
+-rw-r--r--   0        0        0      764 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/react-query.ts
+-rw-r--r--   0        0        0      355 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/table-data-utils.ts
+-rw-r--r--   0        0        0      166 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/utils.ts
+-rw-r--r--   0        0        0      790 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/main.tsx
+-rw-r--r--   0        0        0     1409 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routeTree.gen.ts
+-rw-r--r--   0        0        0     1173 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/__root.tsx
+-rw-r--r--   0        0        0      343 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/index.lazy.tsx
+-rw-r--r--   0        0        0     7445 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/table/$tableName.tsx
+-rw-r--r--   0        0        0     1211 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/styles/ag-custom.css
+-rw-r--r--   0        0        0       38 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/vite-env.d.ts
+-rw-r--r--   0        0        0     2143 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tailwind.config.js
+-rw-r--r--   0        0        0      711 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.json
+-rw-r--r--   0        0        0      233 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.node.json
+-rw-r--r--   0        0        0      378 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/vite.config.ts
+-rw-r--r--   0        0        0      617 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/utils/db_config_dynamic_import.py
+-rw-r--r--   0        0        0      784 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/utils/get_db_inspector.py
+-rw-r--r--   0        0        0      566 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/utils/get_db_seeder.py
+-rw-r--r--   0        0        0     3476 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/table_example.py
+-rw-r--r--   0        0        0        0 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/tests/skibidi-orm/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/tests/skibidi-orm/cli/schema.py
+-rw-r--r--   0        0        0     2136 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/tests/skibidi-orm/cli/test_run.py
+-rw-r--r--   0        0        0     1654 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/conftest.py
+-rw-r--r--   0        0        0     7281 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/converters/sqlite3/test_column_operations_conversion.py
+-rw-r--r--   0        0        0     2619 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/converters/sqlite3/test_constraint_conversion.py
+-rw-r--r--   0        0        0     4963 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/converters/sqlite3/test_table_operations_conversion.py
+-rw-r--r--   0        0        0     1447 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/db_config/test_config.py
+-rw-r--r--   0        0        0     6182 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/db_inspector/test_db_inspectors.py
+-rw-r--r--   0        0        0     9737 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/db_mutators/test_sqlite3_mutator.py
+-rw-r--r--   0        0        0     7425 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/operations/test_operations.py
+-rw-r--r--   0        0        0      967 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/sql_executor/test_sqlite3_executor.py
+-rw-r--r--   0        0        0    17111 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/state_manager/test_state_manager.py
+-rw-r--r--   0        0        0     2146 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/studio/test_db_config_dynamic_import.py
+-rw-r--r--   0        0        0      805 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/studio/test_get_db_inspector.py
+-rw-r--r--   0        0        0      736 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/studio/test_get_db_mutator.py
+-rw-r--r--   0        0        0     4268 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/studio/test_routes.py
+-rw-r--r--   0        0        0    17767 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/test_module_cooperation.py
+-rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 skibidi_orm-0.1.21/PKG-INFO
```

### Comparing `skibidi_orm-0.1.2/pyproject.toml` & `skibidi_orm-0.1.21/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "SkiBiDi-ORM"
-version = "0.1.2"
+version = "0.1.21"
 description = "Python ORM"
 authors = [
     { name = "xDepcio", email = "olek.drwal@gmail.com" },
     { name = "jedrzej-grabski", email = "jedrzej@grabski.pl" },
     { name = "mbienkowski", email = "bienkowski.maksym@gmail.com" },
 ]
 dependencies = [
```

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/cli/run.py` & `skibidi_orm-0.1.21/src/skibidi_orm/cli/run.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/cli/utils.py` & `skibidi_orm-0.1.21/src/skibidi_orm/cli/utils.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/adapters/base_adapter.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/base_adapter.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/adapters/database_objects/constraints.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/database_objects/constraints.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/adapters/database_objects/migration_element.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/database_objects/migration_element.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/adapters/sqlite3_adapter.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/sqlite3_adapter.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/adapters/sqlite3_typing.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/sqlite3_typing.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/converters/base/interfaces.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/converters/base/interfaces.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/converters/sqlite3/all.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/converters/sqlite3/all.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/converters/sqlite3/columns.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/converters/sqlite3/columns.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/converters/sqlite3/constraints.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/converters/sqlite3/constraints.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/converters/sqlite3/tables.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/converters/sqlite3/tables.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/data_mutator/base_data_mutator.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/data_mutator/base_data_mutator.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/data_mutator/sqlite3_data_mutatorr.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/data_mutator/sqlite3_data_mutatorr.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/db_config/base_config.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/db_config/base_config.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/db_inspectors/base_inspector.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/db_inspectors/base_inspector.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/db_inspectors/sqlite3_inspector.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/db_inspectors/sqlite3_inspector.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/operations/column_operations.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/operations/column_operations.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/operations/table_operations.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/operations/table_operations.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/sql_executor/base_sql_executor.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/sql_executor/base_sql_executor.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/sql_executor/sqlite3_executor.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/sql_executor/sqlite3_executor.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/state_manager/i_state_manager.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/state_manager/i_state_manager.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/state_manager/state_manager.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/state_manager/state_manager.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/server.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from typing import cast
 from fastapi import FastAPI, Body
 from fastapi.responses import FileResponse
 from fastapi.staticfiles import StaticFiles
 import uvicorn
 from skibidi_orm.migration_engine.data_mutator.base_data_mutator import (
     BaseDataMutator,
@@ -28,15 +29,17 @@
     allow_methods=["*"],
     allow_headers=["*"],
 )
 
 app.mount(
     "/assets",
     StaticFiles(
-        directory="src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets"
+        directory=os.path.join(
+            os.path.dirname(__file__), "./skibidi-orm-studio-frontend/dist/assets"
+        )
     ),
     name="static",
 )
 
 
 def run_server(schema_file: str):
     global db_inspector
@@ -45,15 +48,17 @@
     db_mutator = get_db_mutator(db_inspector)
     uvicorn.run(app, host="0.0.0.0", port=8000)
 
 
 @app.get("/")
 def read_index():
     return FileResponse(
-        "src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/index.html"
+        os.path.join(
+            os.path.dirname(__file__), "./skibidi-orm-studio-frontend/dist/index.html"
+        )
     )
 
 
 @app.get("/db")
 def get_db():
     """Get the tables in the database."""
     tables = db_inspector.get_tables()
```

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/README.md` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/README.md`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CT5dnm0u.js` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CT5dnm0u.js`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CU2I10C2.css` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CU2I10C2.css`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/vite.svg` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/package.json` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/package.json`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/pnpm-lock.yaml` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/public/vite.svg` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/public/vite.svg`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/assets/react.svg` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/assets/react.svg`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Providers.tsx` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Providers.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Sidebar.tsx` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Sidebar.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/WorkspaceEditor.tsx` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/WorkspaceEditor.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/commands-hisotry-dialog.tsx` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/commands-hisotry-dialog.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/mode-toggle.tsx` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/mode-toggle.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/queryResultsTable.tsx` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/queryResultsTable.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/theme-provider.tsx` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/theme-provider.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/button.tsx` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/button.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dialog.tsx` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dialog.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dropdown-menu.tsx` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dropdown-menu.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/resizable.tsx` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/resizable.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/textarea.tsx` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/textarea.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/delete-table-row.ts` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/delete-table-row.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/edit-row.ts` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/edit-row.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-data.ts` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-data.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-info.ts` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-info.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/run-command.ts` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/run-command.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandResult.tsx` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandResult.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandsHistory.tsx` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandsHistory.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/index.css` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/index.css`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/react-query.ts` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/react-query.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/main.tsx` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/main.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routeTree.gen.ts` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routeTree.gen.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/__root.tsx` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/__root.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/table/$tableName.tsx` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/table/$tableName.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/styles/ag-custom.css` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/styles/ag-custom.css`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tailwind.config.js` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.json` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/utils/db_config_dynamic_import.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/utils/db_config_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/utils/get_db_inspector.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/utils/get_db_inspector.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/studio/utils/get_db_seeder.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/utils/get_db_seeder.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/src/skibidi_orm/migration_engine/table_example.py` & `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/table_example.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/tests/skibidi-orm/cli/test_run.py` & `skibidi_orm-0.1.21/tests/skibidi-orm/cli/test_run.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/conftest.py` & `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/conftest.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/converters/sqlite3/test_column_operations_conversion.py` & `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/converters/sqlite3/test_column_operations_conversion.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/converters/sqlite3/test_constraint_conversion.py` & `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/converters/sqlite3/test_constraint_conversion.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/converters/sqlite3/test_table_operations_conversion.py` & `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/converters/sqlite3/test_table_operations_conversion.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/db_config/test_config.py` & `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/db_config/test_config.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/db_inspector/test_db_inspectors.py` & `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/db_inspector/test_db_inspectors.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/db_mutators/test_sqlite3_mutator.py` & `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/db_mutators/test_sqlite3_mutator.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/operations/test_operations.py` & `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/operations/test_operations.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/sql_executor/test_sqlite3_executor.py` & `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/sql_executor/test_sqlite3_executor.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/state_manager/test_state_manager.py` & `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/state_manager/test_state_manager.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/studio/test_db_config_dynamic_import.py` & `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/studio/test_db_config_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/studio/test_get_db_inspector.py` & `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/studio/test_get_db_inspector.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/studio/test_get_db_mutator.py` & `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/studio/test_get_db_mutator.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/studio/test_routes.py` & `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/studio/test_routes.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.2/tests/skibidi-orm/migration_engine/test_module_cooperation.py` & `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/test_module_cooperation.py`

 * *Files identical despite different names*


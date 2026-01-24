# test-repo-jenkiness
# **Final recommended folder structure**

azure-adf-e2e/
│
├── arm-templates/
│
│   ├── resource-group/
│   │   ├── rg.json
│   │   └── rg.parameters.json
│
│   ├── storage-account/
│   │   ├── storage.json
│   │   └── storage.parameters.json
│
│   ├── sql-database/
│   │   ├── sql-server.json
│   │   ├── sql-db.json
│   │   └── sql.parameters.json
│
│   ├── data-factory/
│   │   ├── factory.json
│   │   ├── factory.parameters.json
│   │
│   │   ├── linkedServices/
│   │   │   ├── ls_sql.json
│   │   │   └── ls_blob.json
│   │
│   │   ├── datasets/
│   │   │   ├── ds_sql.json
│   │   │   └── ds_blob.json
│   │
│   │   ├── pipelines/
│   │   │   └── copy_sql_to_blob.json
│   │
│   │   └── integrationRuntimes/
│   │       └── self_hosted_ir.json
│
├── jenkins/
│   └── Jenkinsfile
│
├── scripts/
│   └── sql/
│       ├── schema.sql
│       ├── tables.sql
│       └── insert_data.sql
│
├── README.md


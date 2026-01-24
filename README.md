# test-repo-jenkiness
# **Final recommended folder structure**

arm-templates/
├── sql-database/
│   ├── sql-server.json
│   ├── sql-db.json
│   └── sql.parameters.json
│
├── data-factory/
│   ├── ARMTemplateForFactory.json
│   ├── ARMTemplateParametersForFactory.json
│   ├── factory/
│   │   ├── CloudFrameDataFactory_ARMTemplateForFactory.json
│   │   └── CloudFrameDataFactory_ARMTemplateParametersForFactory.json
│   └── linkedTemplates/
│       ├── ArmTemplate_master.json
│       ├── ArmTemplate_0.json
│       └── ArmTemplateParameters_master.json
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
└── README.md



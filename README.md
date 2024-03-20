# poc-liquibase-docker
Liquibase Docker POC

### 1- Run database
```bash
   Docker-compose -f docker-compose.database.yml up
```

### 2- Run Liquibase update
```bash
   Docker-compose -f docker-compose.liquibase.update.yml up
```

All scripts in /scripts will be executed
if not exists databasechangelog and databasechangeloglock tables will be created 

### 3- Run Liquibase generate-changelog
```bash
   Docker-compose -f docker-compose.liquibase.generate.yml up
```

script will be generated under /generate



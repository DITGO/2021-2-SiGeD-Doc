# Seeds

## Introdução

Este documento tem como objetivo auxiliar no processo de execução das seeds já presentes dentro do projeto. Pelo projeto ser dividido em vários repositórios gera o problema da informação ficar implícita em cada "README".
Diante disto foi feita a unificação das seeds dentro de um script só para que fique mais simples o onboarding do desenvolvedor com o ambiente.

### Script

Após subir os containers rode em seu terminal as seguintes linhas:

> Seed de demandas

```cmd
docker exec -it backend_demands bash -c "node src/seeders/seedAlerts.js && node src/seeders/seedCategories.js && node src/seeders/seedDemands.js && node src/seeders/seedFiles.js"
```

> Seed de clientes

```cmd
docker exec -it backend_clients bash -c "node src/seeders/seedClient.js && node src/seeders/seedFeature.js && node src/seeders/seedLotacao.js"
```

> Seed de setores

```cmd
docker exec -it backend_sector bash -c "node src/seeders/seedSector.js"
```

> Seed de patrimônios

```cmd
docker exec -it backend_patrimony bash -c "node src/seeders/seedPatrimony.js"
```

> Seed de usuários

```cmd
docker exec -it backend_users bash -c "node src/seeders/seedUsers.js"
```

Caso seja necessário apagar os dados usando um "docker-compose -rm" e alimentar o banco de forma mais ágil basta fazer um documento ".sh", por exemplo

> seeding_db.sh

```cmd
docker exec -it backend_demands bash -c "node src/seeders/seedAlerts.js && node src/seeders/seedCategories.js && node src/seeders/seedDemands.js && node src/seeders/seedFiles.js"
docker exec -it backend_clients bash -c "node src/seeders/seedClient.js && node src/seeders/seedFeature.js && node src/seeders/seedLotacao.js"
docker exec -it backend_sector bash -c "node src/seeders/seedSector.js"
docker exec -it backend_users bash -c "node src/seeders/seedUsers.js"
docker exec -it backend_patrimony bash -c "node src/seeders/seedPatrimony.js"
```

E rodar no terminal usando:

```
bash seeding_db.sh
```

**_IMPORTANTE_**: Este script deve estar na mesma pasta em que foi feito o git clone do projeto.

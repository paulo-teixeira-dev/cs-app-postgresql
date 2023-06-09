# ⚡ CÓDIGO STORM - POSTGRE SQL #

### Stack utilizada

- PostgreSQL
- PgAdmin

### Configurando ambiente e construindo containers

Criando o diretório de volumes do PostgreSQL.

```
mkdir database database/postgre-sql
```

Criando rede local da base de dados.
```
sudo docker network create cs-network
```

Criando containers

```
sudo docker compose up -d
```

Após criado com sucesso, navegue até `http://localhost:3400/` e efetue o login com usuário `localdev@example.com`e senha `localdev`


### Registrando o servidor da base de dados

Navege até Servers > Register > Server para preecher os campos necessarios de conexão.

| Campo  | Valor |
| --- | --- |
| General > Name | cs-postgresql | 
| Connection > Host name/address | cs-postgresql |
| Connection > Port | 5432 |
| Connection > Maintenance database | db_cs |
| Connection > Username | localdev |
| Connection > Password | localdev@123 |

### Portas
| Serviço  | Porta |
| --- | --- |
| PostgreSQL | 5432 |
| PgAdmin | 3400 |

## 🚀 Sobre o desenvolvedor

Este projeto é desenvolvido e mantido por Paulo Teixeira.

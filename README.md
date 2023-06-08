# ⚡ CÓDIGO STORM - POSTGRE SQL #

### Stack utilizada

- PostgreSQL
- PgAdmin

### Criar diretório base de dados

No diretório raiz execute o comando para criar o diretorio de volumes.

```
mkdir database database/postgre-sql
```

### Construindo container

Execute o comando para criar e executar containers com base nas configurações definidas no arquivo docker-compose.yml.

```
sudo docker-compose up -d
```

Após criado com sucesso, navegue até `http://localhost:3400/` e efetue o login com usuário `localdev@cs.com.br`e senha `@localdev`


### Registrando o servidor da base de dados

Navege até Servers > Register > Server para preecher os campos necessarios de conexão.

| Campo  | Valor |
| --- | --- |
| General > Name | cs-postgre-sql | 
| Connection > Host name/address | cs-postgre-sql |
| Connection > Port | 5432 |
| Connection > Maintenance database | cs_db |
| Connection > Username | localdev |
| Connection > Password | @localdev |

### Portas
| Serviço  | Porta |
| --- | --- |
| PostgreSQL | 5432 |
| PgAdmin | 3400 |

## 🚀 Sobre o desenvolvedor

Este projeto é desenvolvido e mantido por Paulo Teixeira.

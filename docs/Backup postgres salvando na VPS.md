## pegar número da instancia docker descobrir qual id postgresql
```bash
docker ps
```
## Ao descobrir o ID substituir os XXXXXXXXX
Pelo ID do postgres
Rodar o mando abaixo
```bash
docker exec -i a0b1ae1a6e8c /bin/bash -c "PGPASSWORD=AKwWM4Qu2GRppJ7 pg_dump --username whazing postgres" > dump.sql
```
## para compactar arquivo que foi criado na VPS gzip dump.sql
```bash
gzip public
```

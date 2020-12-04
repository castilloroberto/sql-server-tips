# lista de comandos utiles en sql server

## Listar tablas
En sql server es necesario crear un diagrama para visualizar las tablas por supuesto que no

```sql
SELECT
  table_name,table_type
FROM
  INFORMATION_SCHEMA.TABLES
where table_type ='BASE TABLE'
GO
```
El **table_ type** es importante ya que si se omite se muestran tambien las **vistas** que son consideras como tablas.


## Listar vistas
Este coamndo es similar an anterios lo unico que cambia es la condicion **where**
```sql
SELECT
  table_name,table_type
FROM
  INFORMATION_SCHEMA.TABLES
where table_type ='view'
GO
```




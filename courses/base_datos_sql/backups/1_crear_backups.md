### Crear backups

pg_dump -U usuario -h localhost -d nombre_base_datos > backup.sql

### Reestablecer base de datos

psql -U usuario -d nombre_base_datos -f backup.sql

## Filtrar patrones de texto

Registros que col termina con una letra
```sql
SELECT * FROM my_table
WHERE col LIKE '%c'
```

Registros que col inicia con una letra
```sql
SELECT * FROM my_table
WHERE col LIKE 'c%'
```
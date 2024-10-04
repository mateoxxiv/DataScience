## Operadores logicos

Registros que cumplan dos condiciones
```sql
SELECT * FROM my_table
WHERE col1 > 1 AND col2 lIKE '%C%'
```

Registros que cumpla tan siquiera uno de los criterios
```sql
SELECT * FROM my_table
WHERE col1 > 1 OR col2 lIKE '%C%'
```

Registros que no sean nulos
```sql
SELECT * FROM my_table
WHERE col1 IS NOT NULL
```

Registros que no pertenezcan a un conjunto de datos
```sql
SELECT * FROM my_table
WHERE col1 NOT IN (20, 21, 22, 23)
```
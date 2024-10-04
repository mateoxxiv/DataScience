## Tipos de filtros
Igualdad simple

```sql
SELECT * FROM my_table
WHERE col = 1
```

Igualdad multiple
```sql
SELECT * FROM my_table
WHERE col ON (1,2,3,4)
```

Diferencia
```sql
SELECT * FROM my_table
WHERE col <> 1
```
```sql
SELECT * FROM my_table
WHERE col != 1
```

Menor que
```sql
SELECT * FROM my_table
WHERE col < 4000
```

entre
```sql
SELECT * FROM my_table
WHERE col between 1 and 10
```
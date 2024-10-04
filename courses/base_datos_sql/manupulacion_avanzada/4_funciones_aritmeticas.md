## Operadores artimeticos

Contar items grupada por un dato
```sql
SELECT course, COUNT(user_id) FROM my_table
GROUP BY course
```

Sumar items grupada por un dato
```sql
SELECT course, COUNT(salary) FROM my_table
GROUP BY employee
```

Promedio items grupada por un dato
```sql
SELECT course, AVG(salary) FROM my_table
GROUP BY employee
```

Minimo items 
```sql
SELECT MIN(salary) FROM my_table
```

MAXIMO items 
```sql
SELECT MAX(salary) FROM my_table
```

REDONDEAR items 
```sql
SELECT ROUND(salary) FROM my_table
```
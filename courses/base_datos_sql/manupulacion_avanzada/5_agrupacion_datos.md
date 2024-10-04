## Operadores de agrupación

Contar items grupada por un dato
```sql
SELECT course, COUNT(*) FROM my_table
GROUP BY course
```

Filtrar por la informació  que estamos filtrando, en el ejemplo solo se mostrará los registros que tengan una cuenta mayor a 3
```sql
SELECT course, COUNT(*) FROM my_table
GROUP BY course
HAVING COUNT(*) > 3
```

on base en un criterio le asigno un valor a los registros
```sql
SELECT
    CASE
        WHEN salary > 1000 THEN 'group1'
        ELSE 'group2'
    END AS salary_group
FROM my_tablex
```
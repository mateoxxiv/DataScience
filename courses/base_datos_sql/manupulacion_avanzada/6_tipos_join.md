## Tipos de Joins

Inner: información que esté es dos tablas al mismo tiempo
```sql
SELECT * FROM my_table
INNER JOIN my_table_2
```

Left: información que este en la tabla princial my table
```sql
SELECT * FROM my_table
LEFT JOIN my_table_2
```

Right: información que este en la tabla secuendaria my table 2
```sql
SELECT * FROM my_table
RIGHT JOIN my_table_2
```

outter: que se encuentra en ambas tablas pero no son compartidos entre ellos
```sql
SELECT * FROM my_table
FULL OUTER JOIN my_table_2
```

cross: Enlaza todo con todo
```sql
SELECT * FROM my_table
CROSS JOIN my_table_2
```
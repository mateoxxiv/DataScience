## CTE

Crear constantes, llemarlas y relacionarlas posteriormente

```sql
WITH
cte1 AS (
    SELECT
        *
    FROM course
),
cte2 AS (
    SELECT
        *
    FROM city
)
SELECT
*
FROM cte1
LEFT JOIN cte2 ON cte2.id = cte1.id
```
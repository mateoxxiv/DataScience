## Trigger

Una vista materializada son datos guadados en disco, requieren ser actualizado de forma conatante.
Tiene como ventaja que las consultas son mas ligeras.

Crear un indice de una tabla
```sql
CREATE MATERIALIZED VIEW ventas_por_cliente AS
SELECT cliente_id, SUM(total_venta) AS total
FROM ventas
GROUP BY cliente_id;
```
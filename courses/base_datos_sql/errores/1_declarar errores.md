### Declarar errores

```sql
CREATE PROCEDURE actualizar_salario(emp_id INT, nuevo_salario NUMERIC)
LANGUAGE plpgsql
AS $$
BEGIN
    -- Iniciar la transacción
    BEGIN
        -- Intentar actualizar el salario
        UPDATE empleados SET salario = nuevo_salario WHERE id = emp_id;

        -- Intentar registrar el cambio en la tabla de logs
        INSERT INTO log_cambios(id_empleado, cambio, fecha)
        VALUES (emp_id, 'Salario actualizado', NOW());

        -- Confirmar la transacción si todo salió bien
        COMMIT;
    EXCEPTION
        -- Si ocurre un error, deshacer todos los cambios
        WHEN OTHERS THEN
            ROLLBACK;
            RAISE NOTICE 'Hubo un error, se ha ejecutado un ROLLBACK.';
    END;
END;
$$;

$$;
```
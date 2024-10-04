## Trigger

Un trigger es un procedimiento almacenado que ue se ejecuta automaticamente una vez se produce un evento:
- Inserciones
- Actualizaciones
- Eliminaciones

Crear un indice de una tabla
```sql
CREATE TRIGGER update_salary
AFTER UPDATE ON EMPLOYEES
FOR EACH ROW
BEGIN
    IF NEW.SALARY > OLD.SALARY THEN
        INSERT INTO SALARY_HISTORY (EMPLOYEE_ID, OLD_SALARY, NEW_SALARY, CHANGE_DATE)
        VALUES (NEW.EMPLOYEE_ID, OLD.SALARY, NEW.SALARY, NOW());
    END IF;
END;
```
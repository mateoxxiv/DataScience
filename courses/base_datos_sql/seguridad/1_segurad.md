### Crear un rol con contraseña

```sql
CREATE ROLE nombre_usuario WITH LOGIN PASSWORD 'contraseña';
```


### Crear rol super usuari

```sql
CREATE ROLE super_usuario WITH SUPERUSER LOGIN PASSWORD 'contraseña';
ALTER ROLE nombre_usuario WITH SUPERUSER;
```

### Modificar roles

```sql
ALTER ROLE nombre_usuario WITH CREATEDB;
```

### Modificar roles

```sql
GRANT SELECT, INSERT, UPDATE, DELETE ON TABLE nombre_tabla TO nombre_usuario;

REVOKE ALL PRIVILEGES ON DATABASE nombre_base_datos FROM nombre_usuario;
REVOKE INSERT, DELETE ON TABLE nombre_tabla FROM nombre_usuario;

```

### Heredar permisos o desheredarlo
```sql
GRANT admin TO usuario_bd;
REVOKE nombre_rol FROM nombre_usuario;
```

### Bloquear un rol
```sql
ALTER ROLE nombre_usuario NOLOGIN;
```




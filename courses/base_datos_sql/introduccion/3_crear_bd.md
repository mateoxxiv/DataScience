## Hay que tener en cuenta
### 1. Tres reglas de normalización
Las reglas de normalización son una serie de principios usados en la organización de bases de datos para reducir la redundancia y mejorar la integridad de los datos:

- **Primera Forma Normal (1NF)**: Cada columna debe contener valores atómicos (indivisibles) y todas las entradas en una columna deben ser del mismo tipo. Además, la tabla no debe tener filas duplicadas.
- **Segunda Forma Normal (2NF)**: Debe cumplir con 1NF y, además, todos los atributos que no son claves deben depender completamente de la clave primaria. No debe haber dependencias parciales, es decir, que una columna dependa solo de una parte de la clave primaria.
- **Tercera Forma Normal (3NF)**: Debe cumplir con 2NF y, además, no debe haber dependencias transitivas, es decir, que un campo no clave dependa de otro campo no clave.

### 2. Primary Key (Clave primaria)
Es una columna (o conjunto de columnas) que identifica de manera única cada fila de una tabla. No pueden tener valores nulos y no pueden repetirse. Su función principal es permitir identificar de manera inequívoca una fila en la tabla.

### 3. Foreign Key (Clave foránea)
Es una columna (o conjunto de columnas) en una tabla que establece una relación con la clave primaria de otra tabla. Sirve para mantener la integridad referencial entre dos tablas, asegurando que los valores de la clave foránea coincidan con valores válidos de la clave primaria en la tabla relacionada.

### 4. Claves de negocio
Son aquellas claves o columnas que tienen un significado en el contexto del negocio y que se utilizan para identificar de manera única a una entidad. Por ejemplo, un número de seguridad social, número de cliente, o número de factura puede ser considerado una clave de negocio.

### 5. Claves subrogadas
Son claves artificiales o generadas por el sistema que no tienen significado en el negocio pero que se utilizan para identificar de manera única a una fila en la tabla. Un ejemplo típico es un identificador numérico secuencial (ID) que se asigna automáticamente a cada fila cuando se inserta un nuevo registro.

### 6. Tipos de datos
Los tipos de datos definen el tipo de valores que pueden almacenarse en una columna de una tabla. Algunos ejemplos comunes incluyen:

- **VARCHAR**: Para cadenas de texto de longitud variable.
- **INT**: Para números enteros.
- **FLOAT**: Para números con decimales.
- **DATE**: Para almacenar fechas.
- **BOOLEAN**: Para valores de verdadero/falso.

## Sintaxis

### Crear base de datos
```sql
(CREATE DATABASE MyDatabase;)
```
### Crear una tabla
```sql
CREATE TABLE ESTUDIANTES (
    IDESTRUDIANTE INT PRIMARY KEY,
    NOMBRE VARCHAR(20),
    APELLIDO VARCHAR(20),
    TIPO_IDENTIFICACION VARCHAR(20),
    IDENTIFICACION VARCHAR(15),
    GENERO VARCHAR (10),
    FECHA_NACIMIENTO TIMESTAMP,
    LOAD_DATE: TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    UPTDATE_DATE: TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

CREATE TABLE INSTRUCTORES (
    IDINSTRUCTOR INT PRIMARY KEY,
    NOMBRE VARCHAR(20),
    APELLIDO VARCHAR(20),
    TIPO_IDENTIFICACION VARCHAR(20),
    IDENTIFICACION VARCHAR(15),
    GENERO VARCHAR (10),
    FECHA_NACIMIENTO TIMESTAMP,
    LOAD_DATE: TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    UPTDATE_DATE: TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

CREATE TABLE CURSO (
    IDCURSO INT PRIMARY KEY,
    NOMBRE VARCHAR(20),
    DESCRIPCION TEXT,
    CUPO INT,
    IDINSTRUCTOR INT,
    FECHA_INICIO TIMESTAMP,
    FECHA_FIN TIMESTAMP,
    LOAD_DATE: TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    UPTDATE_DATE: TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    FOREIGN KEY (IDINSTRUCTOR) REFERENCES INSTRUCTORES(IDINSTRUCTOR)
);

```
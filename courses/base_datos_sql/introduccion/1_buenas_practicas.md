## Buenas prácticas de bases de datos con SQL
### 1. Normalización
Nos sirve para conservar la integridad de nuestros datos, organizar la información, esteucturarla de manera adecuada y relacionar las tablas de manera adecuada.

#### Primera Forma
- Datos atómicos: Sus datos son indivisibles
- Clave primaría: deben estar especificados con una
- Información centralizada: por columna, no debe haber nada separado por comas

#### Segunda forma
- Los atributos que no forman parte de ninguna clave han de depender funcionalmente de toda la clave primaria.

#### Tercera forma
- Los atributos no clave deben ser independientes

#### Cuarta forma
- Generación de tablas muchos a muchos. Esto para resolver las dependencias multivaluadas.

#### Quinta forma
- Generación de tablas muchos a muchos, pero usando únicamente llaves foráneas.
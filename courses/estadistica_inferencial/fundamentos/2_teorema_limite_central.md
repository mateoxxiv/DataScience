## Teorema del Límite Central

El Teorema del Límite Central (TLC) es un principio fundamental en teoría de probabilidades y estadística. Este teorema establece que, bajo ciertas condiciones, la distribución de la media de una muestra de tamaño $n$ tomada de una población con cualquier distribución se aproxima a una distribución normal a medida que el tamaño de la muestra $n$ aumenta, independientemente de la forma de la distribución original de la población.

### Enunciado del Teorema

Sea $X_1, X_2, \ldots, X_n$ una muestra aleatoria de tamaño $n$ tomada de una población con media $\mu$ y desviación estándar $\sigma$. El teorema afirma que, cuando $n$ es suficientemente grande, la distribución de la media muestral $\bar{X}$ se aproxima a una distribución normal:

$$
\frac{\bar{X} - \mu}{\sigma / \sqrt{n}} \sim \mathcal{N}(0, 1)
$$

donde:

- $\bar{X}$ es la media muestral,
- $\mu$ es la media de la población,
- $\sigma$ es la desviación estándar de la población,
- $n$ es el tamaño de la muestra,
- $\mathcal{N}(0, 1)$ representa la distribución normal estándar con media 0 y desviación estándar 1.

### Interpretación

El Teorema del Límite Central nos dice que:

- La media muestral $\bar{X}$ es una estimación imparcial de la media de la población $\mu$,
- A medida que el tamaño de la muestra $n$ aumenta, la distribución de $\bar{X}$ se aproxima a una distribución normal, independientemente de la forma de la distribución original de la población,
- La distribución de $\bar{X}$ tiene una media igual a $\mu$ y una desviación estándar igual a $\frac{\sigma}{\sqrt{n}}$.

### Importancia del Teorema

El Teorema del Límite Central es fundamental porque permite a los estadísticos hacer inferencias sobre una población basándose en la distribución normal, incluso cuando la distribución de la población no es normal. Esto es esencial para la mayoría de las técnicas estadísticas inferenciales, como la estimación de intervalos de confianza y las pruebas de hipótesis.

## Métodos de Muestreo

En estadística, el muestreo es el proceso de seleccionar una parte de una población para hacer inferencias sobre toda la población. Existen varios métodos de muestreo, entre ellos el muestreo aleatorio, sistemático y estratificado. A continuación se describen estos métodos.

### Muestreo Aleatorio

El **muestreo aleatorio** es un método en el que cada miembro de la población tiene una probabilidad igual de ser seleccionado en la muestra. Este método asegura que la muestra sea representativa de la población, lo que permite hacer inferencias válidas.

**Ventajas:**
- Proporciona una muestra representativa de la población.
- Permite realizar inferencias estadísticas válidas.

**Desventajas:**
- Puede ser costoso y difícil de implementar si la población es muy grande o difícil de acceder.
- No garantiza que todos los subgrupos de la población estén representados adecuadamente.

**Ejemplo:**
Si tienes una lista de 1000 empleados y quieres seleccionar una muestra de 100, puedes utilizar un generador de números aleatorios para seleccionar 100 empleados de manera que cada uno tenga la misma probabilidad de ser elegido.

### Muestreo Sistemático

El **muestreo sistemático** es un método en el que se selecciona un punto de inicio aleatorio y luego se elige cada $k$-ésimo miembro de la población a partir de ese punto. El valor de $k$ se determina dividiendo el tamaño de la población entre el tamaño de la muestra deseado.

**Ventajas:**
- Más sencillo de implementar que el muestreo aleatorio.
- Puede ser más eficiente en términos de tiempo y recursos.

**Desventajas:**
- Puede introducir sesgos si hay un patrón en la población que se alinea con el intervalo de muestreo.
- No garantiza que la muestra sea completamente representativa si el patrón de la población es desconocido.

**Ejemplo:**
Si quieres seleccionar una muestra de 100 empleados de una lista de 1000, puedes seleccionar un punto de inicio aleatorio y luego elegir cada $10$-ésimo empleado de la lista.

### Muestreo Estratificado

El **muestreo estratificado** es un método en el que la población se divide en subgrupos o estratos que son homogéneos internamente pero diferentes entre sí. Luego, se realiza un muestreo aleatorio dentro de cada estrato. Este método asegura que todos los subgrupos importantes estén representados en la muestra.

**Ventajas:**
- Mejora la precisión de las estimaciones al asegurar que todos los subgrupos importantes estén representados.
- Puede ser más eficiente que el muestreo aleatorio simple si los estratos son homogéneos.

**Desventajas:**
- Requiere información previa para dividir la población en estratos.
- Puede ser más complejo de implementar que otros métodos.

**Ejemplo:**
Si estás estudiando el desempeño académico de estudiantes en una escuela y quieres asegurarte de que los estudiantes de diferentes grados estén representados, puedes dividir a los estudiantes en estratos basados en su grado (por ejemplo, primero, segundo, tercer grado) y luego realizar un muestreo aleatorio dentro de cada grado.


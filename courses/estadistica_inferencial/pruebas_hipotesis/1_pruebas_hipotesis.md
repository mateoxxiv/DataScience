## Pruebas de hipotesis
Es una herramienta que nos ayuda a jusgar si existe una diferrencia significativa entre el tamaño de la muestra y el parámetro general.
## Pasos a seguir
### 1. Definir nuestras hipotesis
- **Hipotesis nula:** Esta es la hipótesis que se asume como verdadera al inicio del análisis. Generalmente, la hipótesis nula representa la idea de que no hay efecto, no hay diferencia, o no hay relación entre las variables que se están estudiando. Es una afirmación de "no cambio" o "no efecto". Por ejemplo, si estás probando si un nuevo medicamento tiene un efecto diferente al de un placebo, la hipótesis nula podría ser que "el medicamento no tiene ningún efecto diferente al placebo".
- **Hipotesis alternativa:**  Esta es la hipótesis que se propone como alternativa a la hipótesis nula. Representa lo que el investigador realmente quiere probar o descubrir. La hipótesis alternativa sugiere que hay un efecto, una diferencia, o una relación entre las variables que se están estudiando. En el ejemplo anterior del medicamento, la hipótesis alternativa podría ser que "el medicamento tiene un efecto diferente al del placebo".
### 2. Seleccionar el nivel de significancia
Es un umbral que predefinimos, el cual va indicar el nivel maximo que vamos a tolarear opara el error tipo 1 **FALSOS POSITIVOS**.
- Comunmente se usa un nivel de significancia de: 0.01, 0.05, 0.10
### 3. Seleccionar el estadistico de prueba
Es un valor calculado a partir de los datos muestrales que se utiliza para decidir si se rechaza la hipótesis nula. Este valor mide la distancia entre lo observado en la muestra y lo esperado bajo la hipótesis nula.  
  
- **Cálculo:** El estadístico de prueba varía dependiendo del tipo de prueba que se esté realizando (por ejemplo, prueba t, prueba z, prueba chi-cuadrado, etc.). Cada tipo de prueba tiene su propia fórmula para calcular el estadístico.

- **Comparación con la distribución:** Una vez calculado, el estadístico de prueba se compara con una distribución teórica (como la distribución normal, t de Student, o chi-cuadrado) para determinar la probabilidad de observar un valor extremo, dado que la hipótesis nula es verdadera.  
  
### 4. Definir la regla de decisión
La regla de decisión es un criterio establecido antes de realizar la prueba de hipótesis que determina cuándo se debe rechazar la hipótesis nula en función del estadístico de prueba calculado.

- **Valor crítico:** En la mayoría de las pruebas, se define un valor crítico a partir del nivel de significancia 
𝛼
α. Este valor crítico es el umbral contra el cual se compara el estadístico de prueba.

    - Si el estadístico de prueba cae en la región de rechazo (es decir, es mayor o menor que el valor crítico dependiendo de la prueba), se rechaza la hipótesis nula.
    - Si el estadístico de prueba no cae en la región de rechazo, no se rechaza la hipótesis nula.
Región de rechazo: Es el conjunto de todos los valores del estadístico de prueba para los cuales se rechazaría la hipótesis nula. Esta región depende del nivel de significancia 𝛼 α y la naturaleza de la prueba (unilateral o bilateral).
## Tipos de pruebas de hipotesis
### 1. Distribución t-student
**Uso:** Cuando queremos una media de una población normalmente distribuida a partir de una muestra pequeña que sigue una distribuvión normal y de la que desconocemos la desviación estandar:  
  
  $$t = \frac{x_1-x_2}{\sqrt{\frac{S_1^2}{n_1} + \frac{S_2^2}{n_2}}}$$

### 2. Coeficiente de Pearson
**Uso:** MEdir dependencia lineal (correlación), entre dos dos vairables aleatorias cuantitativas
  
  $$r = 1 \text{ correlación perfecta} \\ 0.8 < r < 1 \text{ correlación muy alta} \\ 0.6 < r < 0.8 \text{ correlación alta} \\ 0.4 < r < 0.6 \text{ correlación moderada} \\  0.2 < r < 0.4 \text{ correlación baja} \\  0 < r < 0.2 \text{ correlación muy baja} \\ r = 0 \text{ correlación nula}$$

### 3. ANOVA
**Uso:** Se usa para comparar las variazas entre las medias de diferentes grupos.
## Tipos de errores
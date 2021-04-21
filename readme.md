# Curso de Matemáticas para Data Science: Cálculo Básico

- [Curso de Matemáticas para Data Science: Cálculo Básico](#curso-de-matemáticas-para-data-science-cálculo-básico)
  - [📚 Módulo 1. Introducción](#-módulo-1-introducción)
    - [Clase 2. Qué es el Cálculo](#clase-2-qué-es-el-cálculo)
  - [📚 Módulo 2. Funciones y límites](#-módulo-2-funciones-y-límites)
    - [Clase 3. ¿Qué es una función?](#clase-3-qué-es-una-función)
      - [Formas de representar una función](#formas-de-representar-una-función)
    - [Clase 5. Dominio y rango de una función](#clase-5-dominio-y-rango-de-una-función)
      - [Dominio](#dominio)
      - [Rango](#rango)
      - [Algunos conceptos extra:](#algunos-conceptos-extra)
    - [Clase 6. Cómo programar funciones algebraicas](#clase-6-cómo-programar-funciones-algebraicas)
      - [Funciones Algebraicas](#funciones-algebraicas)
    - [Clase 7. Cómo programar funciones trascendentes](#clase-7-cómo-programar-funciones-trascendentes)
    - [Clase 8. ¿Cómo manipular funciones?](#clase-8-cómo-manipular-funciones)
    - [Clase 9. Funciones dentro de otras funciones](#clase-9-funciones-dentro-de-otras-funciones)
    - [Clase 10. Características de las funciones](#clase-10-características-de-las-funciones)
    - [Clase 11. ¿Cómo se compone una neurona?](#clase-11-cómo-se-compone-una-neurona)
    - [Clase 12. Funciones de activación en una neurona](#clase-12-funciones-de-activación-en-una-neurona)
    - [Clase 13. Función de coste: calcula qué tan erradas son tus predicciones](#clase-13-función-de-coste-calcula-qué-tan-erradas-son-tus-predicciones)
    - [Clase 14. ¿Qué es un límite?](#clase-14-qué-es-un-límite)
  - [📚 Módulo 3. Cálculo diferencial](#-módulo-3-cálculo-diferencial)
    - [Clase 15. ¿De dónde surge la derivada?](#clase-15-de-dónde-surge-la-derivada)
    - [Clase 16. Notación de la derivada](#clase-16-notación-de-la-derivada)
    - [Clase 17. Empecemos a derivar](#clase-17-empecemos-a-derivar)
    - [Clase 18. ¿Por qué es importante la derivada?](#clase-18-por-qué-es-importante-la-derivada)
      - [La derivada para encontrar la velocidad](#la-derivada-para-encontrar-la-velocidad)
      - [La razón de cambio](#la-razón-de-cambio)
    - [Clase 19. Máximos y mínimos: subidas y bajadas en una montaña rusa](#clase-19-máximos-y-mínimos-subidas-y-bajadas-en-una-montaña-rusa)
      - [Formas de calcular los máximos y los mínimos](#formas-de-calcular-los-máximos-y-los-mínimos)
        - [Teorema de la primera derivada](#teorema-de-la-primera-derivada)
        - [Teorema de las segunda derivada](#teorema-de-las-segunda-derivada)
    - [Clase 20. ¿Cómo optimizar una función?](#clase-20-cómo-optimizar-una-función)
  - [📚 Módulo 4. Cálculo multivariable](#-módulo-4-cálculo-multivariable)
    - [Clase 21. Más dimensiones para tus funciones](#clase-21-más-dimensiones-para-tus-funciones)
    - [Clase 22. Diseñando mapas: curvas de nivel](#clase-22-diseñando-mapas-curvas-de-nivel)
    - [Clase 23. Derivadas parciales](#clase-23-derivadas-parciales)
    - [Clase 24. Ejemplos de derivadas parciales](#clase-24-ejemplos-de-derivadas-parciales)
    - [Clase 25. Regla de la cadena y su utilidad en cálculo multivariable](#clase-25-regla-de-la-cadena-y-su-utilidad-en-cálculo-multivariable)
    - [Clase 26. Subamos con el gradiente](#clase-26-subamos-con-el-gradiente)
  - [Módulo 5. 📚 Proyecto: descenso del gradiente](#módulo-5--proyecto-descenso-del-gradiente)
    - [Clase 27. ¿Qué es el descenso del gradiente?](#clase-27-qué-es-el-descenso-del-gradiente)

## 📚 Módulo 1. Introducción

### Clase 2. Qué es el Cálculo

Realizar operaciones de una manera dada para llegar a un resultado.

- #### Calculo infinitesimal

  Cálculo aplicado a cantidades muy pequeñas, que son casi cero. Esto se aplica por ejemplo cuando las funciones y sus valores tienen razones de cambio que se aproximan a cero.

- #### Calculo diferencial

  Estudia la tasa de cambio de las funciones cuando esos cambios son muy pequeños (se aproximan a cero). Su principal herramienta es| la derivada. En otras palabras parte de una función y realiza una derivada. 

  Este rama del cálculo tiene muchas aplicaciones en Data Science.

- #### Calculo integral

  Al derivar una función se obtiene una función nueva, en el cálculo integral se hace el proceso inverso para obtener la función original. En otras palabras parte de una derivada para obtener una función más una constante.
  
  

## 📚 Módulo 2. Funciones y límites

### Clase 3. ¿Qué es una función?

Una *función* es una **regla** en la que a cada elemento de un conjunto A se le **asigna** un elemento de un conjunto B.

Una función no es una relación, ya que a cada elemento de un conjunto A se le asigna un elemento de un conjunto B. Son valores exclusivos.

![](https://i.ibb.co/sPVXtWf/que-es-una-funcion-1.png)

**y** = variable dependiente

**x** = variable independiente

![](https://i.ibb.co/5YsvpmS/que-es-una-funccion-2.png)

⬆ A cada letra del conjunto *x* se le va a asignar un número **diferente** del conjunto *y*.

No se puede asignar a dos elementos del conjunto *x* el mismo elemento del conjunto *y*.

#### Formas de representar una función

- ##### Verbalmente

  "A cada letra del abecedario se le asigna un número diferente".

  "El precio aumenta en 2 USD por cada km recorrido".

- ##### Numéricamente

  Se representan los datos de *x* y *y* en una tabla:

  ![](https://i.ibb.co/hBCkGtN/que-es-una-funcion-3.png)

- ##### Visualmente

  ![](https://i.ibb.co/2sn447q/que-es-una-funcion-4.png)

- ##### Algebraicamente

  ![](https://i.ibb.co/NtgbCtv/que-una-funcion-5.png)

  **ℹ Nota:** se pueden ejecutar todas las celdas de un Notebook en Colab con *Ctrl + F9*

  

### Clase 5. Dominio y rango de una función

#### Dominio

Son los valores que toma **x** y están definidos en la función **f(x)**. En otras palabras son los valores que puede recibir la función, todos los valores de **x** que puede recibir la función y que respetan la regla impuesta en la función.

#### Rango

Son todos los resultados que puede dar una función.



Si se ejemplificaran los conceptos anteriores con una máquina que prepara café:

![](https://i.ibb.co/bP8NtSX/ejemplo-dominio-rango.png)

Del tipo de grano de café que se ingrese a la máquina (dominio) depende el tipo de café que preparará la máquina (rango). De la misma manera la máquina sólo puede recibir café como ingrediente, si se ingresa algo diferente esta se puede estropear, esto ejemplifica el concepto de los valores posibles de **x** que cumplen con la regla definida en la función.



![](https://i.ibb.co/9svcPmM/funcion-dominio-recorrido.webp)



#### Algunos conceptos extra:

**Dominio, codominio y rango**
Hay nombres especiales para lo que puede entrar, y también lo que puede salir de una función:

- Lo que puede entrar en una función se llama el dominio
- Lo que es posible que salga de una función se llama el codominio    
- Lo que en realidad sale de una función se llama rango o imagen

### Clase 6. Cómo programar funciones algebraicas
#### Funciones Algebraicas
Toda función que se puede definir con una serie de polinomios o una relación de álgebra.

- **Funciones lineales**
  
  Tienen la forma 
  $$f(x) = mx + b$$

  Donde $m$ es la pendiente
  $m$ puede ser calculada como la diferencia entre $y2 - y1$ ($y2$ es un punto sobre la recta y $y1$ es un punto menor) sobre la diferencia entre $x2$ entre $x1$.

  $b$ es el punto en que la línea corta al eje $y$. Este parámetro es opcional.
  
  $m$ y $b$  $\in R$ ($m$ y $b$ pertenecen a los números reales)

  **ℹ Nota:** *imagen* ($Im$) es otro nombre que se puede usar para referirse al *rango* 

  ```python
  x = np.linspace(-10, 10, num=res)
  ```
  `linspace` genera una serie de puntos en un rango y los guarda en un array. El primer parámetro es el inicio, el segundo es el final y el tercero es la cantidad de elementos

- **Funciones polinómicas**
  
  Son básicamente funciones que tienen la forma de un polinomio. 

  - **Funciones potencia**

    Son un caso especial de las funciones polinómicas.
  

### Clase 7. Cómo programar funciones trascendentes

A diferencia de las funciones algebraicas las funciones trascendentes no se pueden definir con una serie se polinomios. Algunos ejemplos de este tipo de funciones son las *funciones trigonométricas*, las *funciones exponenciales*, las *funciones logarítmicas* y las *funciones seccionadas*.

```python
np.zeros(len(X))
```
Crea una lista que va contener la cantidad de ceros que se le pasen por parámetro.


### Clase 8. ¿Cómo manipular funciones?

Alterar los parámetros de entrada para mover la función a la derecha, a la izquierda, subirla, bajarla, hacerle una reflexión, alargarla o comprimirla.

Estas movimientos son muy útiles pues en ocasiones hay operaciones en las que se necesitan normalizar datos, meterlos en un rango que por ejemplo vaya de -1 a 1 (estas 2 cosas son muy comunes en Data Science).

Gracias a esto se puede partir de una función conocida, hacerle diferentes manipulaciones y al final dar con una función que explique como se modelan determinados datos.


### Clase 9. Funciones dentro de otras funciones

Composición = funciones dentro de otras funciones

**Explicación con un ejemplo:**

Se quiere hacer una máquina que sea capaz de hacer pasteles. La máquina funciona en 2 etapas, en la primera se elige el sabor y se crea el pan que sirve de base para el pastel, en la segunda se toma la base que se crea en el primer paso y se le agrega una cobertura y la decoración. 

![](https://i.ibb.co/JFrrM3N/proceso-pastel.png)

La composición funciona de la misma manera. Se tiene una variable **x** (sabor), se pasa esta variable a una función **g** (la máquina que hace la base) y el resultado de esta función (la base terminada) se pasa después a una función **f** (la máquina que hace la decoración).

![](https://i.ibb.co/MkRxMw2/composicion-funciones.png)

La **Composición** es en esencia ese proceso en el que se pasa una variable a una función y lo que sale de esa función se pasa por parámetro a otra.

La composición se puede representar de las siguientes maneras.

![](https://i.ibb.co/d0W25bg/definicion-composicion.png)


### Clase 10. Características de las funciones

**Funciones Reales**

Se llaman así porque tanto su dominio como el codominio (rango o imagen) están contenidos dentro del conjunto de los números reales, es decir el conjunto que contiene a los números racionales e irracionales. En otras palabras cualquier número que se te ocurra que no sea imaginario.

**Características de las funciones Reales**
- **Función par**
  
  Una función es par si cumple con la siguiente relación a lo largo de su dominio:

  ![](https://i.ibb.co/0C1Cj8x/regla-funcion-par.png)

  Esta relación dice que una función es par si es simétrica al eje vertical (eje Y). Por ejemplo, una parábola es una función es par.

- **Función impar**
  Una función es impar si cumple la siguiente relación a lo largo de su dominio:

  ![](https://i.ibb.co/QHC7nmL/regla-funcion-impar.png)

  Esta relación indica que una función es impar si es simétrica al eje horizontal (eje X). Por ejemplo, una función cúbica es impar.

- **Función acotada**
  
  Una función es acotada si su codominio (también conocido como rango o imagen) se encuentra entre dos valores, es decir, está acotado. Esta definición se define como que hay un número m que para todo valor del dominio de la función se cumple que:

  ![](https://i.ibb.co/zxvF2bW/regla-funcion-acotada.png)

  Por ejemplo, la función seno o coseno están acotadas en el intervalo [-1, 1] dentro de su co-dominio.

- **Funciones monótonas**

  Estas funciones son útiles de reconocer o analizar debido a que nos permiten saber si una función crece o decrece en alguno de sus intervalos. Que algo sea monótono significa que no tiene variaciones. Entonces las funciones monótonas son aquellas que dentro de un intervalo I, perteneciente a los números reales, cumple alguna de estas propiedades:

  - **La función es monótona y estrictamente creciente:**
  
  ![](https://i.ibb.co/hKsphH0/funcion-monotona-estrictamente-creciente.png)

  Si para todo x1 y x2 que pertenecen al intervalo I, tal que x1 sea menor a x2, si y solo si f(x1) sea menor a f(x2)”. En palabras mucho más sencillas, lo que nos dice esta definición es que x1 siempre tiene que ser menor que x2 en nuestro intervalo I, y que al evaluar x2 en la función el resultado de esto siempre será mayor que si evaluamos la función en x1. Para las siguientes tres definiciones restantes no cambia mucho la forma en la que se interpretan.

  - **La función es monótona y estrictamente decreciente:**
  
    ![](https://i.ibb.co/xDkxNxW/funcion-monotona-estrictamente-decreciente.png)

  - **La función es monótona y creciente:**

    ![](https://i.ibb.co/SBKPfL3/funcion-monotona-creciente.png)

  - **La función es monótona y decreciente:**
    
    ![](https://i.ibb.co/LpKQXz4/funcion-monotona-decreciente.png)

- **Funciones periódicas**

  Las funciones periódicas son aquellas que se repiten cada cierto periodo, este periodo se denomina con la letra T. La relación que debe cumplir la función para ser periódica es la siguiente.

  ![](https://i.ibb.co/3myHvJG/funciones-periodicas.png)

  Por ejemplo, la función seno y coseno son funciones periódicas con un periodo T = 2π. Es decir que si nosotros calculamos f(x) y calculamos f(x + 2π) en la función seno el valor que nos den ambas expresiones es el mismo.

- **Funciones cóncavas y convexas**

  La forma de demostrar la concavidad de una función se puede hacer a través del análisis de derivadas consecutivas (a través del análisis de la segunda derivada), no obstante hay un método más intuitivo que consiste en analizar la gráfica de la función.

  Se dice que una función dentro de un intervalo es cóncava si la función “abre hacia arriba”. Es decir si se ve la siguiente manera:

  ![](https://i.ibb.co/r6Sp2mc/funcion-concava.png)

  Ahora, ¿qué sería una función convexa? Pues así es, lo contrario de una cóncava. Se dice que una función dentro de un intervalo es convexa si la función “abre hacia abajo”. Es decir si se ve la siguiente manera:

  ![](https://i.ibb.co/zVNWtkv/funcion-convexa.png)


### Clase 11. ¿Cómo se compone una neurona?

Una **neurona** es una parte fundamental de una **red neuronal**. Básicamente es una forma fancy de referirse a una función.
Estas necesitan recibir estímulos al igual que ocurre con las neuronas biológicas. Dichos *"estímulos"* se usan para hacer una **suma ponderada** dentro de la función

**Componentes de una Neurona:**

![](https://i.ibb.co/cr4WBnR/1.png)
![](https://i.ibb.co/gwzVTv8/2.png)


### Clase 12. Funciones de activación en una neurona

Las funciones de activación se encargan de activar o desactivar las neuronas dependiendo del valor de entrada, por ejemplo si el valor es muy alto o muy bajo. Estas funciones se representan con la letra **φ** (fi).

**Cómo funcionan**
![](https://i.ibb.co/Nsq72Ws/funcion-de-activacion.png)

Los valores de entrada pasan a la neurona y luego el resultado de esto pasa a la función de activación. Esta regresa un resultado más normalizado (0 - 1, -1 - 1, etc) dependiendo de la función de activación que se utilice.

Si se mira desde el punto de vista de las gráficas de las funciones, la ***neurona*** regresa un **gráfico lineal** que luego la **función de activación convierte en un gráfico no lineal**. Esto es útil porque en el mundo real es muy poco probable que los datos sean lineales, puesto que lo común es que estén dispersos.

**Algunas funciones de activación**
- **Función escalón de Heaviside:** 
  También conocida como función de paso escalonado o escalón binario.

  **Fórmula:**

  ![](https://i.ibb.co/phNWPbT/funcion-heaviside.jpg)

  **Grafica**

  ![](https://i.ibb.co/2YFZVfD/heviside-grafica.webp)

- **Función Sigmoide:** 
  Es una función muy usada en el mundo del Data Science y el ML esto se debe que dadas sus características es muy útil en el calculo de probabilidades. La función sigmoide transforma los valores introducidos a una escala (0,1), donde los valores altos tienen de manera asintótica a 1 y los valores muy bajos tienden de manera asintótica a 0. No obstante no importa que que tan grandes sean los valores, estos nunca llegaran a ser 0 ó 1 como tal.
  Esta función se suele representar con el símbolo $\sigma$ (sigma)

  **Fórmula:**

  ![](https://i.ibb.co/jWWX3ns/funcion-sigmoide-formula.jpg)

  **Código:**

  ```python
  import numpy as np
  import matplotlib.pyplot as plt
  import math

  N = 100

  x = np.linspace(-10,10,num=N)

  z= 1/(1 + np.exp(-x))

  fig, ax = plt.subplots()
  ax.plot(x,z)
  ax.axhline(y=0, color='red')
  ax.axvline(x=0, color='red')
  plt.grid()
  ```

  **Gráfica:**

  ![](https://i.ibb.co/d5MNrF3/funcion-sigmoide-grafico.jpg)

  El punto del medio es exactamente *0.5*.

  El *rango* se esta función es:
  $R = (0, 1)$  Los paréntesis indican un *intervalo abierto* es decir que el rango esta entre 0 y 1 pero nunca alcanza a ser 0 ó 1 como tal.

- **Función tangente hiperbólica:**
  Se suele representar como $\tanh$. Es la relación del seno hiperbólico al coseno hiperbólico: $tannhx = sinhx / cosh$. A diferencia de la Función Sigmoidea, el rango normalizado de tanh es de (−1,1) . La ventaja de tanh es que puede manejar más fácilmente los números negativos.

  **Fórmula:**

  ![](https://i.ibb.co/SRTnn97/funcion-tanh.webp)

  **Código:**
  
  ```python
  import numpy as np
  import matplotlib.pyplot as plt
  import math

  N = 100
  x = np.linspace(-5,5,num=N)
  z= (np.exp(x) - np.exp(-x))/(np.exp(x) + np.exp(-x))

  fig, ax = plt.subplots()
  ax.plot(x,z)
  ax.axhline(y=0, color='black')
  ax.axvline(x=0, color='black')
  plt.grid()
  ```

  **Gráfica:**

  ![](https://i.ibb.co/4TtxRcg/funcion-tanh-grafica.jpg)

- **Función ReLU o Rectificación lineal**

  *(Rectified Linear Unit)* Las* funciones de Rectificado lineal son transformaciones que activan un nodo sólo si la entrada está por encima de una cierta cantidad. Mientras la entrada es inferior a cero, la salida es cero, pero cuando la entrada supera un cierto umbral, tiene una relación lineal con el dependiente variable. 
  Esta función muy usada en redes convolucionales y Deep Learning.

  **Fórmula:**

  ![](https://i.ibb.co/tcY44pK/funcion-RELU.jpg)

  0 para $x <= 0$

  $x$ para $x > 0$

  El rango de esta función es: $R = [0, \infty)$

  **Código:**

  ```python
  import numpy as np
  import matplotlib.pyplot as plt

  deff(x):
    y = np.zeros(len(x))
    for idx,x in enumerate(x):
      if x >= 0:
        y[idx] = x
    return y

  x = np.linspace(-10, 10, num=100)

  y= f(x)

  fig, ax = plt.subplots()

  ax.plot(x,y)
  # ax.axhline(y=0, color='black')
  ax.axvline(x=0, color='black')

  ax.grid()
  ```

  **Gráfica:**
  
  ![](https://i.ibb.co/YDH1YmR/funcion-RELU-grafica.jpg)


### Clase 13. Función de coste: calcula qué tan erradas son tus predicciones

![](https://i.ibb.co/yQph011/ECM-ejemplo-1.webp)

Los puntos representan la relación entre el gasto en publicidad y las ventas en una empresa($y$). La línea representa una predicción sobre el comportamiento de los datos ($ŷ$).

Para calcular que tan alejados están los datos reales de la predicción hay que calcular el **error**:

$error = ŷ - y$

Para normalizar el valor del error en un número positivo y además "castigar" dicha diferencia haciendo que el error sea más pequeño si la diferente es pequeña y viceversa se eleva la diferencia entre la predicción y los datos reales al cuadrado.

$E = (ŷ - y)^2$

El anterior sería el valor del error en uno solo de los puntos, para calcular el error de todos los datos y condensarlo en un sólo valor se usa la siguiente fórmula:

![](https://i.ibb.co/Lv40HKf/ECM-formula.webp)

Esta es la ecuación del **Error Cuadrático Medio**, una ecuación muy usada en el Data Science. Su nombre se debe a que parte desde un *error*, lo *eleva al cuadrado* y finalmente se saca un *promedio*. Esta es una **función de coste** de las más sencillas que hay, aunque no es la única función de coste que existe. Una función de coste representa que tan alejada esta la predicción con respecto a los datos reales.


### Clase 14. ¿Qué es un límite?

![](https://i.ibb.co/wQp4bgz/notacion-limite.png)

![](https://i.ibb.co/CJW7VfX/explicacion-notacion-limite.png)

El límite evaluá que pasa si se toma un punto A y se aproxima este hasta un punto B. En otras palabras los límites describen cómo se comporta una función cerca de un punto, en vez de en ese punto. Esta simple pero poderosa idea es la base de todo el cálculo.

Por ejemplo si se tiene la función $f(x)=x+2$

![](https://i.ibb.co/S0XxsF0/func-1.png)

El límite de $f$ en $x = 3$ es el valor al cual se aproxima $f$ a medida que nos acercamos más y más a $x = 3$. Gráficamente, es el valor de $y$ al que tendemos en la gráfica de $f$ al acercarnos más y más al punto de la gráfica donde $x = 3$.

Por ejemplo, si partimos del punto (1,3) y nos movemos en la gráfica hasta estar muy cerca de $x = 3$, entonces nuestro valor $y$ (es decir, el valor de la función) está muy cerca de 5.

![](https://i.ibb.co/PF47j02/7f460d0a673f5af283702fccf1d9da7462a48a5a.gif)

Similarmente, si empezamos en (5,7) y nos movemos a la izquierda hasta estar muy cerca de $x = 3$, el valor $y$ nuevamente estará muy cerca de 5.

![](https://i.ibb.co/Bj0X52Z/11ab15823702ab90d5198a2dcd37d65d52627e7b.gif)

Por estas razones, decimos que el límite de $f$ en $x =3$ es 5.

![](https://i.ibb.co/nzvCdkG/ejemplo-limite.png)

Tal vez te preguntes cuál es la diferencia entre el *límite* de $f$ en $x =3$, 3 y el *valor* de $f$ en $x 0= 3$, es decir, $f(3)$.

Y sí, el límite de $f(x) =x + 2$ en $x = 3$ es igual a $f(3$, pero este no siempre es el caso. Para entender esto, consideremos la función $g$. Esta función es igual a $f$, excepto que no está definida para $x = 3$

![](https://i.ibb.co/MGs1MD9/func-2.png)

Tal como con $f$, el límite de $g$ en $ x = 3$ es 5. Esto se debe a que aún podemos acercarnos mucho a $x = 3$ y los valores de la función se acercarán mucho a 5.

![](https://i.ibb.co/NFnP0gN/func-2-1.png)

Así que el límite de $g$ en $x = 3$ es igual a 5, ¡Pero el valor de $g$ en $x = 3$ no está definido! ¡No son lo mismo!

Esa es la belleza de los límites: no dependen del valor real de la función en el límite. Describen cómo se comporta la función al acercarse al límite.

*Fuente de la explicación anterior* ➡ https://es.khanacademy.org/math/ap-calculus-ab/ab-limits-new/ab-1-2/a/limits-intro

_**Ejemplo:**_

Si se pidiera calcular el valor de la función $f(x)=\frac{x^2 - 4}{x - 2}$ cuando $x = 2$ tendríamos una indeterminación debido a que $f(2) = \frac{2^2 - 4}{2 - 2} = \frac{4 - 4}{0} = \frac{0}{0}$. No obstante aunque el valor de la función en $x = 2$ es indeterminado lo que si se puede hacer es calcular su límite pues este no depende del valor real de la función.

$$\lim_{x \to 2} \frac{x^2 - 4}{x - 2} = \frac{(x - 2)(x + 2)}{x - 2}$$

Lo anterior se resuelve fácilmente debido a que el comportamiento de los polinomios es una *diferencia de cuadrados*.

$$\lim_{x \to 2} = x + 2 = 2 + 2 = 4$$

**Límites laterales:**

Establecen cuál es el valor que toma una función cuando se hace una aproximación desde la izquierda o la derecha.

![](https://i.ibb.co/263Tgfp/limites-laterales-1.png)

Se agrega el super-índice con un signo de $-$ para denotar que se esta acercando al valor por la izquierda.

![](https://i.ibb.co/MGH8CNf/limites-laterales-2.png)

Es lo mismo sólo que se pone un $+$ en el super-índice para denotar que se esta acercando al valor por la derecha.

![](https://i.ibb.co/sPptZ1Y/limites-laterales-3.png)

**ℹ Nota:** que pasa cuando el límite tiende a 0 de $\frac{1}{x}$. En otras palabras que valor tiene la función cuando nos aproximamos a cero por la izquierda y la derecha.

![](https://i.ibb.co/bXYBDw0/limite-cero.png)

En ese caso el límite por la derecha tienda al infinito $+$ --> +1/0.0000000000001... al igual que el límite por la izquierda $-$ --> -1/0.0000000000001…

Entre más nos acerquemos a cero el valor crece mucho y los límites por derecha e izquierda son muy distintos. Prácticamente están tendiendo a infinito.


## 📚 Módulo 3. Cálculo diferencial
### Clase 15. ¿De dónde surge la derivada?

La derivada surge a partir de la necesidad de tener un método para calcular al tangente de una curva. Este problema ya estaba resuelto con otro  tipo de figuras, pero cuando se trataba de curvas o funciones era muy difícil calcular la tangente.

La **tangente** es una línea recta que toca a la curva en un sólo punto.

![](https://i.ibb.co/Bn8Y9Jy/tangente-curva.png)

No obstante calcular la tangente de una curva no es tan sencillo como trazar una línea que toque la curva y ya, por eso se usa a la **secante** como una ayuda para este proceso.

**La secante** es una línea recta que corta a la curva en 2 puntos.

![](https://i.ibb.co/7YHxvYn/derivadas-1.png)

$\Delta$ (Delta) es un símbolo que se utiliza para representar incrementos. De ahora en adelante en esta explicación $\Delta x = h$ para efectos prácticos.

Ahora que se tiene la secante, para calcular la tangente lo que hay que hacer es aproximar lo máximo posible el punto $x + \Delta x$ al punto $x$. A medida que se hace el desplazamiento la pendiente va cambiando.

![](https://i.ibb.co/XZJ1gbQ/derivadas-2.png)

Mientras más pequeña sea la diferencia entre los 2 puntos (aproximándose a 0), más se aproximará la pendiente de la recta a la pendiente de la tangente. Debido a que estos valores son muy pequeños y tienden a cero se expresan en notación de límite.

$$m = \frac{y_2 - y_1}{x_2 - x_1}$$

Si se sustituyen los valores:

$$m = \frac{f(x+h)-f(x)}{x+h-x}=\frac{f(x+h)-f(x)}{h}$$

Al usar la notación de límite para representar que la distancia se aproxima a cero:

$$\lim_{h \to 0} \frac{f(x+h)-f(x)}{h}$$

⬆ Esta es la **definición formal de la derivada**.

**ℹ Nota:** las derivadas no se pueden calcular en todas las funciones, ya que por ejemplo en las funciones discontinuas existe un salto por lo que el limite lateral izquierdo es diferente al derecho por lo que el límite no existe y ya que las derivadas están dadas por el límite, no es posible calcular la derivada en este tipo de funciones.


### Clase 16. Notación de la derivada

Existen diferentes formas de expresar la derivada. Cada una de ellas fue propuesta por un científico diferente al momento de desarrollar los principios del cálculo.

- **Notación de Leibniz:**
  La notación de Leibniz surge del símbolo $dy/dx$ que representa un operador de diferenciación y no debemos confundirlo como una división. 
  
  Si quisiéramos expresar una segunda derivada usando la notación de Leibniz se puede mostrar como:

  ![](https://i.ibb.co/JzC2c8r/notacion-Leibniz-segunda-derivada.png)

  Y para mostrar la n-ésima derivada se expresa de la forma:

  ![](https://i.ibb.co/dJhVgtw/notacion-Leibniz-n-esima-derivada.png)

  Esta notación nos sirve para entender como la derivada puede ser expresada como los incrementos tanto de x como de y cuando el incremento de x tiende a cero. 
  
  ![](https://i.ibb.co/pZwbtNC/DwA8heo.png)

  La notación de Leibniz es útil cuando se tienen ecuaciones con más de una variable, ya que especifica con respecto a que variable se quiere derivar.

- **Notación de Lagrange:**
  La notación más sencilla de todas es la de Lagrange. Esta notación expresa que la función es una derivada usando una comilla simple antes del argumento, llamada *prima*.

  ![](https://i.ibb.co/2SwRHW7/shUJtc0.png)

  Esta expresión se lee como “efe prima de equis”. La cual representa la primera derivada de una función. Si deseamos expresar la segunda derivada sería:

  ![](https://i.ibb.co/G9JtqWk/Z1Vboyd.png)

  Y para mostrar la n-ésima derivada se expresa de la forma:

  ![](https://i.ibb.co/YNqW1v3/udihVSe.png)

- **Notación de Newton:**
  Por último tenemos la notación de Newton. Esta notación es muy usada en campos como la física y la ingeniería debido a su simplicidad para expresar la primera y segunda derivada. Se usa sobre todo en funciones relacionadas al tiempo en campos como la mecánica. Por ejemplo, como una función que representa el movimiento de una partícula.

  Su representación de la primera y segunda derivada es la siguiente: 
  $$ẋ ẍ$$


### Clase 17. Empecemos a derivar

Todas las definiciones de las derivadas dependiendo de la función parten de la definición de límite de la derivada.

**Reglas de Derivación**

![](https://i.ibb.co/k8dC2Zh/reglas-derivadas-1.png)

![](https://i.ibb.co/wg1fS2G/reglas-derivadas-2.png)

![](https://i.ibb.co/fYqrhsq/reglas-derivadas-3.png)

Permite calcular la derivada de una composición de funciones

_**Ejemplos:**_

- **Suma:**
  
  *Fórmula:*
  $$(f+g)'(x) = f(x)'+g(x)'$$

  Fórmula para calcular la derivada de $x^n$:

  $$x^n = nx^{n-1}$$
  ***

  $$f(x) = x^2$$

  $$g(x) = 4x^2$$

  Así se resolvería directamente, sumando ambas funciones y derivando después.

  $$\frac{d(5x^2)}{dx} = 5*2x = 10x$$
  
  ⬆ **Explicación:** $5x^2$ es el resultado de la suma de $x^2 + 4x^2$. $10x$ es el resultado de aplicar la fórmula para calcular la derivada de $x^n$.
  ***

  Así se resolvería aplicando la regla de la suma en la derivación, en la que se saca la derivada de cada función y luego se suman.

  $$\frac{df}{dx} = x^2 = 2x$$

  $$\frac{dg}{dx} = 4x^2 = 4*2x = 8x$$

  $$2x+8x=10x$$

- **Producto:**

  *Fórmula:*

  $$(f*g)'(x)=f(x)g'(x)+g(x)f'(x)$$

  La derivada del $\cos$ es $-\sin(x)$

  La derivada del $\sin$ es el $\cos$
  ***

  $$f(x)=\cos(x)$$

  $$g(x)=\sin(x)$$

  $$(f*g)(x)=\cos(x)\sin(x)$$

  $$f'(x)=-\sin(x)$$

  $$g'(x)=\cos(x)$$

  $$(f*g)'(x)=\cos(x)\cos(x)+\sin(x)[-\sin(x)]$$

  Al realizar el cálculo al final queda:

  $$(f*g)'(x)=\cos^2(x)-\sin^2(x)$$

- **Composición de funciones (regla de la cadena):**
  
  *Fórmula:*

  $$(f \circ g)'(x)=f'(g(x))*g'(x)$$

  $$f(x)=\sin(x)$$

  $$g(x)=x^3$$

  $$f \circ g = \sin(x^3)$$

  Derivadas de las funciones:

  $$f'(x)=\cos(x)$$

  $$g'(x)=3x^2$$

  $$(f \circ g)'(x)=\cos(x^3)*3x^2$$

### Clase 18. ¿Por qué es importante la derivada?

Algunas aplicaciones que tiene la derivada.

#### La derivada para encontrar la velocidad

La derivada puede usarse para encontrar la velocidad instantánea en determinado punto. Suponiendo que se tiene una función $s=d(t)$, que representa la distancia recorrida por alguien al salir a trotar en las mañanas dicha función tiene como variable independiente el tiempo y como dependiente la distancia.

Para conocer la velocidad promedio en un intervalo de tiempo entre $t=a$ y $t=h$ ($a$ y $h$ son 2 constantes positivas) se puede aplicar la conocida fórmula para encontrar la velocidad ($v=\frac{d}{t}$) que aplicada a este ejemplo quedaría:

![](https://i.ibb.co/LtBVGsr/6kyYpyU.png)

Al realizar la resta del denominador quedaría como:

![](https://i.ibb.co/LrCNghr/FJpDJiB.png)

En un gráfico todo esto se vería de la siguiente forma:

![](https://i.ibb.co/58TJ5rP/Yb2rCe8.jpg)

⬆ La velocidad promedio es la recta que esta entre los 2 intervalos de tiempo ($P$ y $Q$), pero si se quiere saber cuál es la velocidad instantánea en alguno de los puntos, como por ejemplo $P$ que es cuando el tiempo t=a es necesario aplicar el límite a medida que $h$ (la distancia entre $P$ y $Q$) tiende a cero, al hacer esto estaríamos usando una derivada para calcular la velocidad instantánea en alguno de los puntos.

![](https://i.ibb.co/dcbm0Pz/9Ci9LcD.png)

#### La razón de cambio

Las derivadas se pueden interpretar de una forma más general, y es como la **razón de cambio**. Las funciones son dos cantidades que dependen una de otra y en la vida práctica ese comportamiento esta por todos lados (la cocción de un alimento depende del tiempo en que lo dejemos en el fuego, el precio de un producto depende de su demanda en el mercado, etc) por lo que se pueden usar derivadas para calcular que tanto cambia una función en un momento determinado, lo cuál brinda un mundo de posibilidades para estudiar el comportamiento de diversos datos y la “velocidad” con la que estos cambian en un sinfín de casos prácticos.

Si estudiamos las funciones como pequeños cambios tenemos que estudiar sus incrementos. Para hacer eso hay que tener presente que si tenemos la función $y=f(x)$, entonces su incremento en $x$ cuando pasamos de $x_1$ a $x_2$ es:

![](https://i.ibb.co/Q70cM1J/sLqSAFm.png)
**ℹ Nota:** el símbolo delta en mayúscula sirve para indicar el cambio entre dos cantidades.

Para el cambio en **y** se usaría:

![](https://i.ibb.co/xGXVKkn/UcEl3gp.png)

A la división de estos dos incrementos la llamamos razón de cambio promedio de y con respecto a x.

![](https://i.ibb.co/RS9KKkw/z117ffz.png)

Las razones de cambio nos dicen qué tanto cambia una cantidad y con respecto a $x$. Específicamente la razón de cambio promedio nos dice que tanto cambia y en un intervalo entre $x_1$ y $x_2$. Por lo que si queremos saber qué tanto cambia una función en un instante determinado debemos aplicar la razón de cambio instantánea que es la definición de la derivada.

![](https://i.ibb.co/Jrp3Yxz/yuhEZrR.png)

Si nuestra derivada es muy grande significa que y crece muy rápido con respecto a x, pero si la derivada es muy pequeña o casi cero entonces el crecimiento de y respecto a x es mínimo.


### Clase 19. Máximos y mínimos: subidas y bajadas en una montaña rusa

Los valores **máximos** y **mínimos** de una función son los valores **más altos** y **más bajos** respectivamente.

![](https://i.ibb.co/196NsX7/maximo-minimo-funcion.png)

El máximo y el mínimo de una función serían los puntos en los que la pendiente de la tangente es exactamente 0.

Cuando la derivada sea mayor a cero la pendiente estará subiendo y cuando la derivada sea menor a 0 la pendiente estará bajando.

La función completa puede tener varios máximos y mínimos, así como un **máximo global**, que es el valor más alto, y un **mínimo global** que sería el valor más bajo.

También se pueden analizar secciones específicas de una función en las que el valor más alto y más bajo se llamarían **máximo global** y **mínimo global** respectivamente.

#### Formas de calcular los máximos y los mínimos
##### Teorema de la primera derivada
- Si $f'(x)>0$ hacia la izquierda de un punto a y si $f'(x)<0$ hacia la derecha del punto $a$, entonces $f$ tiene un máximo relativo en $(a, f(a))$
  
- Si $f'(x)<0$ hacia la izquierda de un punto a y si $f'(x)>0$ hacia la derecha del punto $a$, entonces $$ tiene un minino relativo en $(a, f(a))$
  
- Si $f'(x)$ es menor o mayor de ambos lados, no es ni un máximo ni un mínimo

##### Teorema de las segunda derivada
- Si $f''(x)<0$ entonces $f$ tiene un máximo relativo en $(x, f(x))$

- Si $f''(x)>0$ entonces $f$ tiene un mínimo relativo en $(x, f(x))$

- Si $f''(x)=0$ no se puede determinar si es un máximo o un mínimo o ninguno de los dos. Se debe utilizar el teorema de la primera derivada para poder determinarlo


### Clase 20. ¿Cómo optimizar una función?

**Problema:**

![](https://i.ibb.co/qpZytgk/optimizar-funcion-ejemplo.png)

Encontrar el tamaño de los muros que permita obtener la mayor área en m², o en otras palabras, encontrar el tamaño de los muros que permita tener una oficina más  grande. *Sólo se pueden construir 50 metros de muro*.

**Desarrollo:**

Para *calcular el área* se usar la fórmula super conocida: $A=xy$

Para *calcular el perímetro* hay que sumar cada lado. En este ejemplo el perímetro total son los 50 metros de muro que se pueden construir: $x+y+x=50=2x+y=5$

A partir del punto anterior se puede despejar $y$:

$$y=50-2x$$

Con esto ya se puede sustituir $y$ en la ecuación del área:

$$A=x(50-2x)=50x-2x^2$$

Ahora que ya se tiene el área expresada en función de $x$ se puede convertir esto en una función, es precisamente este función la que se va a optimizar.

$$A(x)=50x-2x^2$$

Para optimizar la función anterior y encontrar el valor máximo se usa la derivada:

$$A'(x)=50-4x=0$$
⬆ Para encontrar el punto en que la pendiente es igual a cero (el máximo y el mínimo) hay que igualar la derivada a cero

Para encontrar cuando la ecuación anterior se vuelve cero hay que despejar $x$.

$$x=\frac{-50}{-4}=\frac{25}{2}=12.5$$

Ahora hay que corroborar que $12.5$ sea el valor máximo, esto normalmente se hace usando el teorema de la primera/segunda derivada, pero en este ejemplo se va usar un método más sencillo y intuitivo para principiantes y es evaluar la derivada en un valor cercano a la derecha y a la izquierda, el valor de la izquierda debe ser positivo y el de la derecha negativo para que $12.5$ sea el valor máximo.

$$A'(x=12.45)=50-4(12.45)=\frac{1}{5}$$

$$A'(x=12.55)=50-4(12.55)=-\frac{1}{5}$$

Ahora que ya se tiene el valor de $x$ sólo hay que sustituirlo en la ecuación de $y$ para encontrar el valor de esta última variable:

$$y=50-2(12.5)=25$$

Ya con eso sabemos que para obtener el área más grande en las oficinas usando sólo los 50 metros de muro disponibles los muros deben ser de 12.5m y 25m.

![](https://i.ibb.co/YDpGq15/optimizar-funcion-ejemplo-2.png)


## 📚 Módulo 4. Cálculo multivariable

### Clase 21. Más dimensiones para tus funciones

A lo largo del curso se ha trabajado con funciones que sólo reciben una sola variable por parámetro (univariable). No obstante las funciones pueden tener más de una variable.

Sin importar las variables que tenga la función, al final siempre va a salir un resultado.

![](https://i.ibb.co/nLVL07T/funciones-multivariable.png)


### Clase 22. Diseñando mapas: curvas de nivel

Este tipo de representaciones son útiles para representar múltiples datos en un espacio tridimensional. Algunos ejemplos de uso de este tipo de gráficas son la representación de alturas, temperaturas y preferencias de usuarios.

[Información sobre Numpy meshgrid](https://interactivechaos.com/es/manual/tutorial-de-numpy/la-funcion-meshgrid)


### Clase 23. Derivadas parciales

Las derivadas parciales permiten encontrar la derivada en funciones de más de una variable.

[Explicación de las derivadas parciales](https://es.khanacademy.org/math/multivariable-calculus/multivariable-derivatives/partial-derivative-and-gradient-articles/a/introduction-to-partial-derivatives)


### Clase 24. Ejemplos de derivadas parciales

![Ejemplo 1](https://i.ibb.co/McBFvCC/ejemplo-derivadas-parciales-1.png)

![Ejemplo 21](https://i.ibb.co/2j4Kh7M/ejemplo-derivadas-parciales-2.png)

**Dato Matemático:**

1. El conjunto de primeras derivadas parciales se le conoce como **Gradiente**.
2. La Matriz de segundas derivadas parciales se le comoce como **Hessiana**.
3. El determinante de la matriz Hessiana se le conoce como **Jacobiano**
4. El **Jacobiano es útil cuando queremos hacer transformaciones**. Por ejemplo: Pasar del plano cartesiano a coordenadas polares.

**Herramientas para calcular la derivada parcial:**

- https://www.wolframalpha.com/
- https://www.sympy.org/en/index.html
- https://es.symbolab.com/


### Clase 25. Regla de la cadena y su utilidad en cálculo multivariable

La regla de la cadena aplicada en el cálculo multivariable es muy usada en un proceso de las redes neuronales llamado **Backpropagation**.

la regla de la cadena para una sola variable es sencilla relativamente pues su proceso es lineal, encadenando las funciones. En el caso del cálculo multivariable esto funciona de forma diferente. Al tener más de una función, surgen divisiones en la forma en la que la variable inicial llega a la variable final. Por ejemplo si tenemos una función $w=f(x,y)$ que depende de dos variables $x$ y $y$, pero a su vez estas dependen de una variable $t$. La función que describimos anteriormente se escribe como:

![Ecuación 1](https://imgur.com/LsA97Kk.jpg)

La función $w=f(x,y)$ depende de dos variables, por lo que el cálculo de alguna derivada de esta función concretamente debe ser parcial. Pero tanto las variables $x$ y $y$ solo son respecto a una variable, la variable $t$, por lo que el cálculo de cualquier clase de derivada debe ser total.

En el siguiente diagrama se explica cómo se reacionan estas variables desde $t$ hasta $w$:

![Diagrama 1](https://imgur.com/OgEfDgI.jpg)

En el diagrama se puede apreciar como $t$ es la variable inicial y $w$ termina siendo la variable final de salida. Si se añaden las derivadas en cada una de estas relaciones el diagrama quedaría de la siguiente forma:

![Diagrama 2](https://imgur.com/YYbrIvH.jpg)

Las  derivadas de las funciones $x$ y $y$ son totales porque solo dependen de una única variable $t$. Sin embargo, las derivadas con respecto a $w$ son parciales porque tiene más de dos variables, que en este caso son funciones de $t$. Es por esto que se puede observar en el diagrama que la relación entre variables en algunos puntos es lineal (se conectan consecutivamente) y en otros puntos las relaciones para llegar a $w$ siguen más de un camino (se ven en paralelo).

En las relaciones que sean lineales, se multiplica siguiendo la regla de la cadena para una sola variable. Con esto se obtiene una porción de todas las relaciones, para obtener todas las relaciones y porciones hasta llegar a $w$ hay que agruparlas mediante una suma. Quedan la razón de cambio total (o derivada total) de $w$ respecto a $t$ como:

![Ecuación 2](https://imgur.com/w8CEmQx.jpg)

La constitución de la regla de la cadena en multivariable cambia dependiendo del número de variables intermedias que pueda haber en el proceso de llegar al valor final, no obstante el principio sigue siendo el mismo.

La regla de la cadena tiene una gran importancia pues nos permite relacionar diferentes funciones que otorgan un valor final de salida contra su variable de entrada. Esto es muy útil cuando estudiamos el comportamiento, como puede ser el precio de un producto, que está determinado por diferentes factores.

[Video explicativo](https://www.youtube.com/watch?v=DFn9wUEBnbU)


### Clase 26. Subamos con el gradiente

Es un vector que, dependiendo de una superficie, va a establecer cuál es la forma más rápida de ascender dicha superficie. Su puede pensar en esto como una especie de brújula que muestra por donde subir una montaña más rápido.

El gradiente de una función se representa con el símbolo $\nabla$ (nabla).

![Fórmula gradiente](https://i.ibb.co/ncnwL2c/formula-gradiente.png)

$i$ y $j$ son *vectores unitarios*. a los valores de $x$ se le asigna $i$, a $y$ se le asigna $j$, hay que recordar que un vector tiene ademas de su valor, una dirección, y eso es lo que indican $i$ y $j$.

_**Ejemplo:**_

![Ejemplo gradiente](https://i.ibb.co/NNZbqtp/ejemplo-gradiente.png)

El gradiente almacena toda la información de la derivadas parciales de una función multivariable. Pero es más que un simple dispositivo de almacenamiento, tiene muchas aplicaciones en muchas área de las ciencias.
El gradiente es una función escalar multivariable que empaqueta toda la información de sus derivadas parciales en un vector.

![Gradiente 1](https://i.ibb.co/YBRHD13/gradiente-1.webp)

Cabe resaltar el la forma del gradiente varia dependiendo las coordenadas que utilicemos, tiene las misma interpretación, pero se utiliza se escribe de destina manera.

![Gradiente 2](https://i.ibb.co/k5hRfZx/gradiente-2.webp)


## Módulo 5. 📚 Proyecto: descenso del gradiente

### Clase 27. ¿Qué es el descenso del gradiente?

El descenso del gradiente permite optimizar una función, es decir, encontrar el mínimo de una función de coste. El descenso del gradiente se puede aplicar en diferentes mediciones, no obstante en este ejemplo para fines prácticos sólo se usarán 2.

![Explicación descenso del gradiente](https://i.ibb.co/8cvPmh4/desc-gradiente-info.png)

[Vídeo explicativo](https://www.youtube.com/watch?v=A6FiCDoz8_4)

**ℹ Nota:** el descenso del gradiente sólo es útil en funciones que tienen un único valor mínimo. EN el caso de funciones que tengan varios mínimos locales lo que hará este algoritmo es buscar el mínimo local más cercano.
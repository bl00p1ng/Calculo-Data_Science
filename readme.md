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


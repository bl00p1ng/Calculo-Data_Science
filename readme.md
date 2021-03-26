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

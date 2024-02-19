# Asymptotes

Se presenta el código de diferentes algoritmos que permiten comprobar el comportamiento asintótico de dos curvas algebraicas planas.

En primer lugar, el **Algoritmo 1.1** determina el comportamiento asintótico de dos curvas, es decir, si se aproximan todas sus ramas infinitas entre sí. 

El **Algoritmo 1.2** calcula las asíntotas de una curva a partir de su expresión implícita, considerando las ramas infinitas que convergen con la curva dada, mientras que el **Algoritmo 1.3** realiza la construcción de las asíntotas a partir de la expresión paramétrica de la curva. Para ambos casos se requiere el cómputo de las series de Puiseux.

Así mismo, se presenta el **Algoritmo 2.1** y el **Algoritmo 2.2**, que muestran un incremento de la eficiencia alcanzada con los métodos previos para la construcción de asíntotas, empleando límites y derivadas, respectivamente.

Es importante destacar que, para cada una de estas implementaciones se han de cumplir las siguientes condiciones de entrada:

1. Por cuestiones de aplicabilidad, se asume que la curva dada es real (aunque los resultados pueden aplicarse al caso complejo).
2. (0 : 1 : 0) no es un punto de infinito de la curva algebraica plana irreducible. En caso contrario, se considera un cambio lineal de coordenadas.
3. La curva algebraica plana irreducible de entrada está definida por:
- La Ecuación 1.6 para el Algoritmo 1.3. Obsérvese que mcd(p_i1, pi2) = 1.
- La Ecuación 1.6 para el Algoritmo 2.1. Nótese que mcd(pi1, pi2) = 1 y grado(pi1)  grado(pi2).
- La Ecuación 2.2 para el Algoritmo 2.2. Obsérvese mcd(q1, q2, q) = 1.

Para cada uno de los métodos propuestos, se implementa el correspondiente algoritmo y se añade un conjunto de órdenes que permiten calcular diversas características específicas de las curvas dadas. Estos procedimientos se definen a continuación.
1. Procedimientos generales:
- EIndex: Calcula el índice de ramificación de una serie.
- NonNegativeOps: Extrae los términos no negativos de una serie.
- ImplicitToParametric: Calcula la ecuación paramétrica a partir de la implícita.
- ParametricToImplicit: Determina la ecuación implícita a partir de la paramétrica.




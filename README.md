# Redes Neuronales para compuertas lógicas (Wolfram Language)

Este proyecto implementa una Red Neuronal Artificial (RNA) en Wolfram
Language para resolver las compuertas lógicas clásicas:

-   Compuerta AND\
-   Compuerta OR\
-   Compuerta XOR

------------------------------------------------------------------------

## Requisitos

-   Wolfram Mathematica o Wolfram Cloud , también se puede notebook de wolfram one.\
-   Copiar y ejecutar el archivo `.wl` en un Notebook.

------------------------------------------------------------------------

## Implementación

El código entrena una red neuronal con los datos de entrada y salida de
cada compuerta.\
Cada compuerta se entrena de manera independiente con sus respectivas
tablas de verdad:

### AND

  x1   x2   salida
  ---- ---- --------
  0    0    0
  0    1    0
  1    0    0
  1    1    1

### OR

  x1   x2   salida
  ---- ---- --------
  0    0    0
  0    1    1
  1    0    1
  1    1    1

### XOR

  x1   x2   salida
  ---- ---- --------
  0    0    0
  0    1    1
  1    0    1
  1    1    0

------------------------------------------------------------------------

## Arquitectura de la Red

-   Capa de entrada: 2 neuronas (x1, x2).\
-   Capa oculta: 2--4 neuronas con función de activación sigmoide.\
-   Capa de salida: 1 neurona con activación sigmoide.

La compuerta XOR requiere una capa oculta porque no es linealmente
separable.\
AND y OR pueden entrenarse con redes más simples.

------------------------------------------------------------------------

## Ejecución

1.  Cargar el archivo `wolfram_Actividad.wl` en Wolfram.\
2.  Ejecutar cada bloque de código para entrenar la red de AND, OR o
    XOR.\
3.  Probar las predicciones:

``` wolfram
andNet[{1, 1}]
orNet[{0, 1}]
xorNet[{1, 0}]
```

------------------------------------------------------------------------

## Archivos

-   `wolfram_Actividad.wl`: Código fuente en Wolfram Language.\
-   `README.md`: Documento de documentación.

------------------------------------------------------------------------

## Autores

-   Ana Hernández

Proyecto académico -- Redes Neuronales y Lógica Booleana

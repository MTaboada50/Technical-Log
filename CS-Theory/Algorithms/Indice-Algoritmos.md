# Catálogo de Algoritmos y Estrategias de Resolución

Este documento centraliza los algoritmos estudiados, clasificados por su metodología y eficiencia. Sirve como referencia teórica para la implementación en diversos lenguajes de programación.

## 1. Algoritmos de Búsqueda
Procedimientos para localizar un elemento específico dentro de una estructura de datos.

* **Búsqueda Lineal $O(n)$:** Recorre uno a uno los elementos. Es el método por defecto para datos no ordenados.
* **Búsqueda Binaria $O(\log n)$:** Utiliza la técnica de *Divide y Vencerás*. Requiere que el conjunto de datos esté previamente ordenado. Reduce el tiempo de búsqueda de forma logarítmica.

## 2. Algoritmos de Ordenamiento (Sorting)
Fundamentales para optimizar la organización de la información y permitir búsquedas eficientes.

* **Selection Sort $O(n^2)$:** Encuentra el elemento más pequeño y lo coloca al principio. Simple pero ineficiente en grandes volúmenes.
* **Bubble Sort $O(n^2)$:** Compara elementos adyacentes y los intercambia si están en el orden incorrecto.
* **Merge Sort $O(n \log n)$:** Algoritmo basado en *Divide y Vencerás* que divide la lista en mitades, las ordena y luego las combina.

## 3. Metodologías de Diseño
* **Divide y Vencerás:** Estrategia que consiste en descomponer un problema complejo en subproblemas más pequeños del mismo tipo, hasta que sean lo suficientemente sencillos para ser resueltos directamente.
* **Bucketizing:** Técnica de distribución de elementos en "baldes" o contenedores basados en una propiedad (como en las Tablas de Hash).

---
Para entender cómo medir la eficiencia de estos algoritmos, consultar [Análisis de Complejidad (Big O)](./Complexity-Analysis.md).
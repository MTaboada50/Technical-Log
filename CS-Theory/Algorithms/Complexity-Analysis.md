# Análisis de Complejidad Computacional (Big O)

El análisis de complejidad permite predecir el comportamiento de un algoritmo ante el crecimiento de los datos de entrada ($n$).

## Notaciones Comunes
* **$O(1)$ - Tiempo Constante:** El tiempo de ejecución no cambia (ej. acceder a un índice de un Array).
* **$O(\log n)$ - Tiempo Logarítmico:** El espacio de búsqueda se reduce a la mitad en cada paso (ej. Búsqueda Binaria).
* **$O(n)$ - Tiempo Lineal:** El tiempo crece proporcionalmente a los datos (ej. Búsqueda Lineal).
* **$O(n^2)$ - Tiempo Cuadrático:** Común en algoritmos con bucles anidados.

> **Importancia:** En el desarrollo profesional, optimizar de $O(n^2)$ a $O(n \log n)$ puede significar la diferencia entre un programa que tarda horas y uno que tarda segundos.
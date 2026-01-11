# Introducción a la Programación (Argentec / Harvard CS50)
Este documento registra los fundamentos de computación abordados en el primer módulo del trayecto CapacitAR, enfocándose en la transición del pensamiento lógico a la arquitectura de datos.

## 🧠 Pensamiento Computacional y Abstracción
El pensamiento computacional es la metodología para resolver problemas mediante el desglose de procesos en una secuencia lógica de pasos. Se basa en el modelo de **Input -> Proceso -> Output**.

Para gestionar la complejidad, se utiliza la **Abstracción**: la capacidad de omitir detalles de implementación de bajo nivel (como el flujo de electrones en el hardware) para concentrarse en la lógica de capas superiores.

### Representación de Información
Las computadoras procesan datos mediante distintas capas de representación:

* **Sistema Binario (Base 2):** La unidad mínima es el bit (0 o 1), que representa estados lógicos (Encendido/Apagado). Los números se construyen mediante potencias de 2. Por ejemplo, el decimal `13` se representa como `1101` ($1 \cdot 2^3 + 1 \cdot 2^2 + 0 \cdot 2^1 + 1 \cdot 2^0$).
* **ASCII y Unicode:** Estándares que asignan valores numéricos a caracteres. Mientras que ASCII usa 8 bits (limitado a 256 caracteres), Unicode extiende este mapa para incluir alfabetos globales y símbolos.
* **Sistema RGB:** Representación de colores mediante la combinación de tres canales (Rojo, Verde, Azul). Cada canal suele tener 8 bits de profundidad, permitiendo 256 intensidades por color.

---

## ⚡ Algoritmos y Lógica de Programación

### Pseudocódigo
Es una descripción de alto nivel de un algoritmo que emplea las convenciones estructurales de un lenguaje de programación real, pero está diseñado para la lectura humana. Facilita el diseño de la lógica antes de la codificación final.
> **Conceptos relacionados:** [Documentación de Pseudocódigo](../../../../../CS-Theory/Fundamentos/Pseudocodigo.md)

### Complejidad Computacional (Eficiencia)
La eficiencia de un programa no se mide en segundos (ya que depende del hardware), sino en cómo escala el número de operaciones a medida que aumenta el volumen de datos de entrada ($n$).
> **Nota técnica:** Para una explicación mas profunda sobre crecimiento asintótico y análisis de rendimiento, consultar: [Análisis de Complejidad (Big O)](../../../../../CS-Theory/Algorithms/Complexity-Analysis.md)

### Algoritmos de Búsqueda y Ordenamiento
Los algoritmos son instrucciones finitas y ordenadas para resolver una tarea. Algunos enfoques fundamentales son:

1.  **Búsqueda Binaria:** Basada en la estrategia de **Divide y Vencerás**. En una lista ordenada, el algoritmo divide el conjunto a la mitad en cada iteración, descartando la sección donde el dato no puede estar.
2.  **Búsqueda Lineal:** Revisa cada elemento uno por uno. Es ineficiente en grandes volúmenes de datos.
3.  **Algoritmos de Ordenamiento (Sorting):** Procedimientos como *Selection Sort* o *Bubble Sort* que organizan datos bajo un criterio específico.
> **Referencia extensa:** [Catálogo de Algoritmos](../../../../../CS-Theory/Algorithms/Indice-Algoritmos.md)

---

## 🗄️ Estructuras de Datos y Memoria

### Almacenamiento en Memoria
La memoria de la computadora puede visualizarse como una matriz de celdas numeradas (direcciones de memoria) donde se almacenan bits. El **Acceso Aleatorio (RAM)** permite llegar a cualquier dirección de forma inmediata.

### Estructuras de Datos
Son formas de organizar la información en la memoria para que pueda ser utilizada de manera eficiente:
* **Arrays:** Colecciones contiguas en memoria que permiten acceso directo por índice.
* **Listas Enlazadas:** Elementos dispersos conectados mediante punteros.
* **Tablas de Hash:** Estructuras que usan una función matemática para mapear claves a valores, permitiendo búsquedas de tiempo constante.
> **Exploración profunda:** [Estructuras de Datos y Gestión de Memoria](../../../../../CS-Theory/Data-Structures/Intro-Estructuras.md)
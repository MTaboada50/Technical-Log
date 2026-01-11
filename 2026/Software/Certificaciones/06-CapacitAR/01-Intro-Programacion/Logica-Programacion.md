# Módulo 02: Lógica de Programación (Fundación Aprende)

Este módulo profundiza en la mecánica interna de los lenguajes, desde la aritmética básica hasta paradigmas avanzados como la programación paralela y declarativa.

## 🛠️ Herramientas de Construcción de Algoritmos
Los algoritmos cuantitativos se apoyan en operadores para transformar inputs en outputs.

### Operadores Aritméticos y Prioridad
Se sigue el orden matemático estándar para garantizar la precisión del cálculo:
1. **Potencias y Raíces**
2. **Multiplicación y División**
3. **Módulo $MOD$ y Residuo:** Cruciales para algoritmos de paridad o ciclos.
4. **Suma y Resta**

### Operadores Relacionales y Lógicos
Permiten la toma de decisiones mediante la evaluación de valores de verdad.
* **Relacionales:** `<`, `>`, `<=`, `>=`, `!=`, `=`.
* **Lógicos:** `AND` (&&), `OR` (||), `NOT` (!). 
> Ver detalles y tablas de verdad en: [Lógica Proposicional](../../../../CS-Theory/Fundamentos/Logica-Proposicional.md)

---

## 💻 El Lenguaje y la Computadora
Un programa es un bloque de código fuente que requiere traducción para ser ejecutado por el hardware.

* **Intérprete:** Traducción y ejecución línea a línea (en tiempo real).
* **Compilador:** Traducción integral previa a la ejecución (genera un ejecutable).

### Gestión de Memoria: Variables y Punteros
Las variables son espacios reservados en memoria con un tipo de dato definido (int, float, char, bool). 
* **Punteros:** Herramienta de bajo nivel (visto en lenguaje C) que almacena la **dirección de memoria** de otra variable. 
  * Operador de dirección (`&`): Obtiene la ubicación.
  * Operador de indirección (`*`): Accede al contenido de la ubicación.

---

## 📐 Diseño y Estructuras de Control
Para representar algoritmos visualmente se utilizan **Diagramas de Flujo (DFD)**.
> Ver catálogo de símbolos en: [Diagramación Lógica](../../../../CS-Theory/Fundamentos/Diagramas-Flujo.md)

### Estructuras de Control
1. **Condicionales:** Simple (if), Compuesta (if else) y Múltiple (switch).
2. **Iterativas (Bucles):**
   * `For`: Iteración definida (Inicio, Condición, Incremento).
   * `While`: Iteración basada en condición (puede no ejecutarse nunca).
   * `Do-While`: Garantiza al menos una ejecución previa a la evaluación.

---

## 🏗️ Paradigmas de Programación
Los paradigmas son enfoques metodológicos para la resolución de problemas:
* [**Estructurada**](../../../../../CS-Theory/Paradigmas/Estructurada.md): Diseño top-down y modularización.
* [**Orientada a Objetos (POO)**](../../../../../CS-Theory/Paradigmas/POO.md): Interacción entre objetos y clases.
* [**Declarativa**](../../../../../CS-Theory/Paradigmas/Declarativa.md): Enfoque en la lógica y el "qué" del problema.
* [**Paralela**](../../../../../CS-Theory/Paradigmas/Paralela.md): Optimización mediante ejecución simultánea.

---

## ⚡ Algoritmos y Estructuras Avanzadas
* **Recursividad:** Funciones que se invocan a sí mismas hasta alcanzar un caso base.
* **Matrices:** Estructuras multidimensionales contiguas en memoria.
* **Ordenamiento:** [Bubble Sort y Selección](../../../../CS-Theory/Algorithms/Indice-Algoritmos.md)

---

## ⚡ Lenguaje C
Se exploraron los fundamentos sintácticos del lenguaje, incluyendo gestión de entrada/salida y control de flujo.
* [**Guía de Sintaxis de C**](../../../Languages/C/Sintaxis-Basica.md)
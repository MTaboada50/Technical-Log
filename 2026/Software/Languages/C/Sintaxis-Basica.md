# Sintaxis Básica de Lenguaje C

C es un lenguaje compilado de propósito general que permite un control preciso sobre el hardware y la memoria. Es la base de muchos sistemas operativos y otros lenguajes de programación.

## 🏗️ Estructura de un Programa
Todo programa en C requiere una función principal `main` y la inclusión de bibliotecas estándar para realizar operaciones básicas mediante la directiva `#include`.

```c
#include <stdio.h> // Biblioteca estándar de entrada y salida

int main() {
    printf("Hola, Mundo\n");
    return 0; // Indica que el programa finalizó con éxito
}   

---

## 📥 Entrada y Salida de Datos

* **`printf()`**: Función para imprimir datos formateados en la consola.
* **`scanf()`**: Función para leer datos del usuario. Requiere el operador de dirección `&` (referencia) para conocer la ubicación en memoria donde debe almacenar el dato.

```c
int edad;
printf("Ingresa tu edad: ");
scanf("%d", &edad); // %d es el especificador para enteros

---

## 📦 Tipos de Datos y Especificadores

C utiliza especificadores de formato para la comunicación con el flujo de datos. Estos le indican al compilador cómo interpretar los bits almacenados en la memoria al momento de leerlos o imprimirlos:

| Especificador | Tipo de Dato | Descripción |
|:---:|:---:|:---|
| `%d` | `int` | Números enteros (positivos o negativos). |
| `%f` | `float` | Números con punto decimal (precisión simple). |
| `%c` | `char` | Un solo carácter o letra (basado en código ASCII). |
| `%s` | `string` | Cadena de caracteres (técnicamente un array de `char`). |


### Ejemplo de uso en código:
```c
int unidades = 10;
float precio = 15.50;
char categoria = 'A';

printf("Stock: %d unidades de la categoria %c a $%.2f", unidades, categoria, precio);

---

## 🔀 Estructuras de Control

Permiten modificar el flujo de ejecución del programa basándose en condiciones o repeticiones.

### Condicionales
Se utilizan para ejecutar diferentes bloques de código según el valor de verdad de una expresión.

```c
if (condicion) {
    // Código si es verdadero
} else if (otra_condicion) {
    // Código alternativo
} else {
    // Código por defecto
}

// Estructura de decisión múltiple
switch(variable) {
    case 1: 
        // código si variable == 1
        break;
    case 2:
        // código si variable == 2
        break;
    default: 
        // código si no coincide ningún caso
}

### Bucles (Iteración)
Permiten repetir un bloque de instrucciones múltiples veces mientras se cumpla una condición determinada.

* **`for`**: Utilizado cuando el número de iteraciones es conocido de antemano. Requiere una inicialización, una condición de parada y un incremento/decremento.
* **`while`**: Evalúa la condición **antes** de entrar al bucle. Si la condición es falsa desde el inicio, el código nunca se ejecuta.
* **`do-while`**: Ejecuta el bloque de código y **luego** evalúa la condición. Esto garantiza que el código se ejecute al menos una vez.


#### Ejemplos de implementación en C:

```c
// Ejemplo de While: Evalúa y luego ejecuta
while (contador < 10) {
    printf("%d ", contador);
    contador++;
}

// Ejemplo de Do-While: Ejecuta y luego evalúa
do {
    printf("Este mensaje aparece al menos una vez");
} while (condicion_falsa);

---

## 📍 Punteros y Gestión de Memoria

Un puntero es una variable especializada que almacena la **dirección de memoria** de otra variable, permitiendo la manipulación directa de los datos y una gestión eficiente de los recursos.

### Mecánica de los Punteros
* **Declaración (`int *p;`)**: El asterisco indica que la variable no guardará un valor entero directo, sino la ubicación de uno.
* **Asignación (`p = &mi_variable;`)**: El operador de dirección `&` extrae la ubicación física (hexadecimal) de `mi_variable` y la guarda en `p`.
* **Indirección (`*p`)**: También llamado desreferenciación, permite acceder o modificar el valor real almacenado en la dirección que guarda el puntero.

#### Ejemplo de uso:
```c
int numero = 42;
int *p = &numero; // p ahora apunta a la dirección de memoria de numero

printf("Direccion: %p\n", (void*)p); // Imprime la ubicación en memoria
printf("Valor: %d\n", *p);           // Accede al 42 mediante el puntero

## 📦 Programación Modular (Funciones)

La programación modular consiste en dividir un programa en partes más pequeñas o "módulos" llamados funciones. Esto facilita la reutilización de código y la organización lógica (Diseño *Top-Down*).

### Estructura de una Función
Una función consta de un tipo de retorno, un nombre, parámetros (opcionales) y el cuerpo de la función.

```c
// Definición de la función
int sumar(int a, int b) {
    return a + b;
}

int main() {
    int resultado = sumar(5, 3); // Invocación
    printf("El resultado es: %d", resultado);
    return 0;
}

---

### Conceptos Importantes:

void: Se utiliza como tipo de retorno cuando la función realiza una acción (como imprimir) pero no devuelve ningún valor numérico o de dato.

Prototipo: Es una declaración previa de la función al inicio del archivo (antes del main) para que el compilador sepa que existe antes de ser usada.

Paso por Valor vs. Referencia:

Valor: Se pasa una copia del dato.

Referencia: Se pasa el puntero (&variable), permitiendo que la función modifique el valor original de la variable fuera de su ámbito local.

---

## 📚 Creación de Librerías

Las librerías son conjuntos de funciones almacenadas en archivos externos que simplifican el desarrollo y permiten la reutilización de código en diversos proyectos.

### Componentes de una Librería
* **Archivos de Cabecera (`.h`)**: Contienen los prototipos de las funciones y las definiciones de constantes o estructuras. Actúan como la "interfaz".
* **Archivos de Implementación (`.c`)**: Contienen el código real (la lógica) de las funciones declaradas en la cabecera.

### Inclusión en el Proyecto
Para utilizar una librería personalizada situada en el mismo directorio que el archivo principal, se utiliza la directiva `#include` con comillas en lugar de corchetes angulares:

```c
#include "mi_libreria.h" // Inclusión de una librería personalizada del programador
#include <stdio.h>       // Inclusión de una librería estándar del sistema
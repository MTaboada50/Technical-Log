# Pseudocódigo: Diseño Lógico de Soluciones

El pseudocódigo es una herramienta de planificación que utiliza una mezcla de lenguaje natural y convenciones de programación para describir la lógica de un algoritmo sin preocuparse por la sintaxis específica de un lenguaje (como Python o C++).

## Características Principales
* **Legibilidad:** Diseñado para ser comprendido por humanos.
* **Independencia:** No depende de un entorno de ejecución.
* **Estructura:** Utiliza identación y palabras clave para definir el flujo.

## Palabras Clave Comunes (Convención)
Para mantener el rigor técnico, se suelen estandarizar los términos:
* `IF / ELSE`: Para toma de decisiones (Condicionales).
* `FOR / WHILE`: Para repeticiones (Bucles/Loops).
* `FUNCTION / PROCEDURE`: Para bloques de código reutilizables.
* `RETURN`: Para entregar un resultado.
* `PRINT / READ`: Para salida y entrada de datos.

## Ejemplo: Búsqueda Lineal
```text
FUNCTION buscar_numero(lista, objetivo)
    FOR cada 'numero' en 'lista'
        IF 'numero' es igual a 'objetivo'
            RETURN Verdadero
    RETURN Falso
END
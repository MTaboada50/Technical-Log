# Lógica Proposicional y Tablas de Verdad

La lógica proposicional es la base de las condiciones en programación. Evalúa expresiones que solo pueden ser Verdaderas $V$ o Falsas $F$.

## Tablas de Verdad Principales

| $p$ | $q$ | $p \land q$ (AND) | $p \lor q$ (OR) | $p \oplus q$ (XOR) | $p \rightarrow q$ (Cond) |
|:---:|:---:|:---:|:---:|:---:|:---:|
| V | V | **V** | V | F | V |
| V | F | F | **V** | V | F |
| F | V | F | V | **V** | V |
| F | F | F | F | F | **V** |

### Operadores Adicionales (Programación Declarativa)
* **Bicondicional $\leftrightarrow$:** Verdadero solo si ambos valores son iguales.
* **Negación $\neg$:** Invierte el valor de verdad.
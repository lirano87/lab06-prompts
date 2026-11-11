# Bitacora de prompts
 
Laboratorio 06: Fundamentos de Ingenieria de Prompts.
 
Herramienta de IA usada: GEMINI
 
## Ejercicio 2: Tokens y ventana de contexto
 
| Texto | Caracteres | Tokens |
|-------|------------:|--------:|
| Los estudiantes programan en Java. | 34 | 7 |
| The students program in Java. | 29 | 6|
| desafortunadamente | 18 | 4 |


## Ejercicio 3: Temperatura

| Temperatura | % de BiblioTec | Nombres en los 5 intentos |
|-------------|:----------------|:---------------------------|
| 0 | 100 | BiblioTec, BiblioTec, BiblioTec, BiblioTec, BiblioTec |
| 0.5 | 65,3 | BiblioTec, BiblioTec, PrestaLibro, BiblioTec, BiblioTec |
| 1 | 44,5 | NubeDeTinta, BiblioTec, LibroYa, BiblioTec, LibroYa |
| 1.8 | 32,2 | PaginaLibre, LectoGo, PrestaLibro, BiblioTec, BiblioTec |

Conforme la temperatura aumenta, también aumentarán las probabilidades de que aparezcan los 5 nombres distribuídos.

El simulador nunca inventará nombres nuevos porque no se encuentran dentro de las opciones del arreglo del programa.

## Ejercicio 4: Prompt vago vs estructurado
 
 | Criterio | Prompt vago | Prompt estructurado |
|----------|:-------------|:---------------------|
| Menciona el objetivo del sistema | Sí | Sí |
| Menciona a los usuarios principales | Sí | Sí |
| Tiene exactamente 3 funcionalidades | No | Sí |
| Esta en 3 parrafos | No | Sí |
| Lo usaria en un informe real | No | Sí |


## Ejercicio 5: Anatomia de un prompt

| Componente | Texto de mi prompt |
|------------|:--------------------|
| Rol | Actua como desarrollador Java. |
| Instruccion | Crea un programa en Java usando una clase Producto con los atributos codigo, nombre, precio y stock. |
| Contexto | Para gestionar los productos de una tienda. |
| Ejemplo | Usa este estilo para los metodos: getPrecio(), setPrecio(double precio). |
| Formato | Explica primero la estructura de la clase y luego presenta el codigo Java. |

### Observaciones de los cambios por nivel

- Nivel 1: Gemini generó un gestor de tareas porque el prompt no especificaba qué programa desarrollar.
- Nivel 2: Generó otro gestor de tareas, pero incorporó una estructura más orientada a objetos.
- Nivel 3: Creó un programa para gestionar productos de una tienda al recibir un contexto específico.
- Nivel 4: Utilizó los cuatro atributos solicitados para la clase Producto: codigo, nombre, precio y stock.
- Nivel 5: Explicó primero la estructura de la clase y después presentó el código Java.
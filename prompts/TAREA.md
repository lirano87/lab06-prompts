# Tarea: Mi prompt profesional
 
## Funcionalidad elegida

Desarrollo de un programa en Java que calcule el promedio de tres notas de un estudiante y muestre el resultado.
 
## Version 1: prompt basico

```text
Crea un programa en Java para calcular el promedio de las notas de un alumno.
```

**Resultado:** Gemini generó un programa que permite ingresar cualquier cantidad de notas y calcular su promedio.

**Qué falta mejorar:** Especificar que se utilizarán tres notas y definir un rango válido para las calificaciones.
 
## Version 2: 

```text
Crea un programa en Java para calcular el promedio de las notas de un alumno en el rango de 0 a 20. El programa solicita las tres notas, calcula el promedio y muestra el resultado.
```
**Qué cambié:** Especifiqué que el programa trabaje con tres notas y que estas deben estar entre 0 y 20.

**Por qué:** En la primera versión, Gemini permitía ingresar cualquier cantidad de notas y no validaba sus valores.

**Qué mejoró:** Gemini generó un programa que solicita tres notas, valida que sean numéricas y estén dentro del rango permitido.

**Qué falta mejorar:** Evitar funcionalidades adicionales que no se le haya solicitado, como determinar si el estudiante aprobó o desaprobó.


## Version 3: prompt final

```text
Actúa como desarrollador Java. Crea un programa sencillo en Java para calcular el promedio de tres notas de un alumno de instituto.

El programa debe solicitar exactamente tres notas por consola, validar que cada una esté entre 0 y 20 luego calcula el promedio aritmético y muestra el resultado con dos decimales.

Ejemplo: si las notas son 12, 15 y 18, el promedio debe ser 15.00.

Explica brevemente como funciona el programa y luego presenta el código Java completo.

No uses librerias externas ni agregues funcionalidades que no se te indiquen, como por ejemplo: determinar si el alumno aprobó o desaprobó.
```

**Qué cambié:** Agregué un rol, un ejemplo de cálculo, un formato de respuesta y restricciones específicas.

**Por qué:** En la versión 2, Gemini añadió funcionalidades que no había solicitado.

**Qué mejoró:** Gemini generó un programa que solicita y valida tres notas, calcula el promedio con dos decimales y explica su funcionamiento antes de mostrar el código, sin clasificar las notas como aprobado o desaprobado.

## Componentes del prompt final

| Componente | Texto de mi prompt |
|------------|--------------------|
| Rol | Actúa como desarrollador Java. |
| Instrucción | Crear un programa sencillo en Java para calcular el promedio de tres notas. |
| Contexto | Un alumno de instituto, tres notas entre 0 y 20. |
| Ejemplo | Si las notas son 12, 15 y 18, el promedio será 15.00. |
| Formato | Explica brevemente cómo funciona el programa y luego presenta el código Java completo. |
| Restricción adicional | No uses librerías externas ni agregues funcionalidades no solicitadas. |

## Evaluacion del resultado

| Criterio | Cumple |
|----------|--------:|
| Solicita exactamente tres notas | Sí |
| Valida que las notas estén entre 0 y 20 | Sí |
| Calcula el promedio aritmético | Sí |
| Muestra el promedio con dos decimales | Sí |
| Explica el funcionamiento antes del código | Sí |
| No agrega funcionalidades no solicitadas | Sí |
 
## Errores que evité

**Error 1: Ser demasiado general.**

En la primera versión no indiqué cuántas notas debía utilizar el programa ni su rango permitido. Lo corregí especificando tres notas entre 0 y 20.

**Error 2: Asumir información no proporcionada.**

En la segunda versión, Gemini agregó una función para determinar si el alumno aprobaba o desaprobaba. Lo corregí incorporando una restricción en el prompt final para que no agregue funcionalidades no solicitadas.

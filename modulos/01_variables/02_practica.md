# Práctica: Variables en Python

## Instrucciones

Completa los ejercicios en orden. No saltes niveles. Si necesitas ayuda, escribe `/hint`.

**Importante**: Todos los ejercicios se realizan en tu workspace de Codespaces. Los archivos `.py` están en la carpeta de este módulo. Edítalos directamente y cuando termines escribe `/review`.

---

## Archivos de Ejercicio

Los siguientes archivos están en tu workspace para que los completes:

| Archivo | Nivel | Descripción |
|---------|-------|-------------|
| `ejercicio_nivel1.py` | 1 | Crear variables y mostrar sus tipos |
| `ejercicio_nivel2.py` | 2 | Completar código con espacios en blanco |
| `ejercicio_nivel3.py` | 3 | Modificar código existente |
| `ejercicio_nivel4.py` | 4 | Resolver problemas desde cero |
| `ejercicio_nivel5.py` | 5 | Mini desafío: conversor de temperatura |

Para ejecutar un ejercicio:
```bash
python modulos/01_variables/ejercicio_nivel1.py
```

---

## Nivel 1 — Reconocimiento

**Objetivo**: Identificar tipos de datos y crear variables básicas.

**Archivo**: `ejercicio_nivel1.py`

Debes:
- Crear 4 variables (nombre, edad, estatura, es_estudiante)
- Mostrar el tipo de cada variable con `type()`

<details>
<summary>Pista</summary>
Recuerda: strings van entre comillas, números sin comillas, booleanos son True o False.
</details>

---

## Nivel 2 — Completar Código

**Objetivo**: Completar código con partes faltantes.

**Archivo**: `ejercicio_nivel2.py`

Debes reemplazar los `___` con el código correcto para que funcione.

<details>
<summary>Pista</summary>
Para convertir texto a número usa `int()`. Para intercambiar variables necesitas una tercera variable temporal.
</details>

---

## Nivel 3 — Modificar Código

**Objetivo**: Modificar código existente para cambiar su comportamiento.

**Archivo**: `ejercicio_nivel3.py`

Debes:
1. Cambiar valores fijos por `input()` para pedir datos al usuario
2. Encontrar y corregir un error de tipo (TypeError)
3. Modificar cálculo de promedio para que use `input()`

<details>
<summary>Pista</summary>
`input()` siempre devuelve texto. Si necesitas hacer operaciones matemáticas, convierte con `int()` o `float()`.
</details>

---

## Nivel 4 — Resolver Problema

**Objetivo**: Escribir código desde cero para resolver un problema.

**Archivo**: `ejercicio_nivel4.py`

Dos problemas:
1. **Calculadora de propina**: Pedir cuenta y porcentaje, calcular total
2. **Conversor de kilómetros a millas**: Usar fórmula 1 milla = 1.60934 km

<details>
<summary>Pista</summary>
La propina se calcula: `cuenta * (porcentaje / 100)`. El total es: `cuenta + propina`.
</details>

---

## Nivel 5 — Mini Desafío

**Objetivo**: Aplicar todo lo aprendido en un proyecto pequeño.

**Archivo**: `ejercicio_nivel5.py`

**Desafío**: Conversor de temperatura Celsius ↔ Fahrenheit

Fórmulas:
- C a F: `F = C * 9/5 + 32`
- F a C: `C = (F - 32) * 5/9`

<details>
<summary>Pista</summary>
Usa `if` para decidir qué fórmula aplicar según la opción del usuario. Si aún no viste condicionales, puedes crear dos programas separados.
</details>

---

> **Nota**: Después de completar cada nivel, escribe `/review` para que revise tu código.

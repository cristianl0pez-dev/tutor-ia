# Práctica: Variables en Python

## Instrucciones

Completa los ejercicios en orden. No saltes niveles. Si necesitas ayuda, escribe `/hint`.

---

## Nivel 1 — Reconocimiento

**Objetivo**: Identificar tipos de datos y conceptos básicos.

### Ejercicio 1.1

¿Qué tipo de dato es cada valor?

a) `"hola"`
b) `42`
c) `3.14`
d) `True`
e) `"3.14"`

<details>
<summary>Pista</summary>
Piensa en: ¿tiene comillas? ¿tiene punto decimal? ¿es verdadero/falso?
</details>

### Ejercicio 1.2

¿Cuáles de estos nombres de variables son válidos en Python?

a) `mi_variable`
b) `2nombre`
c) `nombre completo`
d) `_edad`
e) `for`
f) `EDAD`

<details>
<summary>Pista</summary>
Recuerda: no empezar con número, sin espacios, no usar palabras reservadas.
</details>

---

## Nivel 2 — Completar Código

**Objetivo**: Completar código con partes faltantes.

### Ejercicio 2.1

Completa los espacios marcados con `___` para que el código funcione:

```python
# Crea una variable llamada nombre con tu nombre
nombre = ___

# Crea una variable llamada edad con tu edad
___ = 25

# Muestra un mensaje
print("Me llamo " + ___ + " y tengo " + str(___) + " años")
```

<details>
<summary>Pista</summary>
Para crear una variable: `nombre_variable = valor`. Para usarla, escribe su nombre.
</details>

### Ejercicio 2.2

Completa el código para sumar dos números ingresados por el usuario:

```python
numero1 = input("Ingresa el primer número: ")
numero2 = input("Ingresa el segundo número: ")

# Convierte los strings a integers
num1 = ___(numero1)
num2 = int(___)

# Calcula la suma
suma = num1 ___ num2

print("La suma es:", ___)
```

<details>
<summary>Pista</summary>
Recuerda que `input()` devuelve texto. Necesitas convertir a número con `int()`.
</details>

---

## Nivel 3 — Modificar Código

**Objetivo**: Modificar código existente para cambiar su comportamiento.

### Ejercicio 3.1

Este código calcula el área de un rectángulo:

```python
base = 10
altura = 5
area = base * altura
print("El área es:", area)
```

**Modifícalo** para que:
1. Pida la base y altura al usuario
2. Calcule el área
3. Muestre el resultado con un mensaje claro

<details>
<summary>Pista</summary>
Usa `input()` para pedir datos y `int()` para convertir. Recuerda que `input()` devuelve texto.
</details>

### Ejercicio 3.2

Este código intercambia dos valores pero tiene un error:

```python
a = 10
b = 20

# Intercambiar valores
a = b
b = a

print("a =", a)
print("b =", b)
```

**Encuentra el error** y corrígalo. Pista: después del intercambio, ambos valores son iguales.

<details>
<summary>Pista</summary>
Necesitas una tercera variable temporal para guardar el valor original de `a` antes de sobreescribirlo.
</details>

---

## Nivel 4 — Resolver Problema

**Objetivo**: Escribir código desde cero para resolver un problema.

### Ejercicio 4.1 — Calculadora de Propina

**Problema**: Crea un programa que calcule cuánto debe pagar una persona en un restaurante incluyendo la propina.

**Requisitos**:
- Pedir el total de la cuenta
- Pedir el porcentaje de propina deseado
- Calcular el monto de la propina
- Calcular el total a pagar
- Mostrar ambos valores

**Ejemplo de entrada/salida**:
- Entrada: cuenta = 100, propina = 15%
- Salida: Propina: $15.0, Total: $115.0

<details>
<summary>Pista</summary>
La propina se calcula: `cuenta * (porcentaje / 100)`. El total es: `cuenta + propina`.
</details>

---

## Nivel 5 — Mini Desafío

**Objetivo**: Aplicar todo lo aprendido en un proyecto pequeño.

### Desafío 5.1 — Conversor de Temperatura

**Descripción**: Crea un programa que convierta temperaturas entre Celsius y Fahrenheit.

**Requisitos**:
- Preguntar al usuario qué conversión quiere hacer (C a F o F a C)
- Pedir la temperatura
- Realizar la conversión correcta
- Mostrar el resultado con formato claro

**Fórmulas**:
- Celsius a Fahrenheit: `F = C * 9/5 + 32`
- Fahrenheit a Celsius: `C = (F - 32) * 5/9`

**Criterios de éxito**:
- [ ] El programa pide la opción de conversión
- [ ] Pide la temperatura
- [ ] Calcula correctamente ambas conversiones
- [ ] Muestra el resultado de forma clara

<details>
<summary>Pista</summary>
Usa `if` para decidir qué fórmula aplicar según la opción del usuario. Si aún no viste condicionales, puedes crear dos programas separados.
</details>

---

> **Nota**: Después de completar cada nivel, explica tu razonamiento antes de pasar al siguiente.

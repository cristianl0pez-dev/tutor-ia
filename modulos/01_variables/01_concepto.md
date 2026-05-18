# 01 — Variables en Python

## ¿Qué es una variable?

Una **variable** es como una **caja con etiqueta** donde guardas información.

- La **etiqueta** es el nombre de la variable
- El **contenido** es el valor que guardas
- Puedes cambiar el contenido cuando quieras

---

## 💡 Analogía

Piensa en una **nevera con tuppers**:

| Concepto | En la nevera | En Python |
|----------|-------------|-----------|
| Variable | Un tupper con etiqueta | `edad = 25` |
| Etiqueta | "Comida lunes" | `nombre = "Ana"` |
| Contenido | Pasta | `"Ana"` |
| Cambiar valor | Guardar otra cosa en el mismo tupper | `edad = 26` |

---

## Cómo crear una variable en Python

En Python es muy simple: solo escribes el nombre, un igual `=`, y el valor:

```python
nombre = "Cristian"
edad = 25
```

¡Listo! Eso es todo. No necesitas palabras raras ni símbolos especiales.

---

## Tipos de datos básicos

Las variables pueden guardar diferentes **tipos** de información:

### 1. Texto (string)
Va entre comillas `""` o `''`:
```python
nombre = "Cristian"
ciudad = 'Bogotá'
```

### 2. Números enteros (int)
Sin comillas, sin decimales:
```python
edad = 25
cantidad = 100
```

### 3. Números decimales (float)
Con punto decimal:
```python
precio = 19.99
temperatura = 36.5
```

### 4. Verdadero o Falso (bool)
Solo dos valores posibles:
```python
es_mayor = True
tiene_hijos = False
```

> ⚠️ **Importante**: `True` y `False` van con mayúscula inicial.

---

## Ejemplos progresivos

### Ejemplo 1: Variable simple
```python
mensaje = "Hola mundo"
print(mensaje)  # muestra: Hola mundo
```

### Ejemplo 2: Usar una variable en otra
```python
nombre = "Cristian"
saludo = "Hola " + nombre
print(saludo)  # muestra: Hola Cristian
```

### Ejemplo 3: Cambiar el valor
```python
edad = 25
print(edad)   # muestra: 25
edad = 26
print(edad)   # muestra: 26
```

### Ejemplo 4: Operaciones con variables
```python
precio = 10
cantidad = 3
total = precio * cantidad
print(total)  # muestra: 30
```

---

## Reglas para nombrar variables

✅ **Sí puedes:**
- Usar letras: `nombre`, `edad`
- Usar números (no al inicio): `precio1`, `nota2`
- Usar guion bajo: `mi_nombre`, `fecha_nacimiento`

❌ **No puedes:**
- Empezar con número: `1nombre` ❌
- Usar espacios: `mi nombre` ❌
- Usar palabras reservadas: `if`, `for`, `class` ❌
- Usar caracteres especiales: `@`, `$`, `%` ❌

> 💡 **Convención en Python**: usa `snake_case` (minúsculas con guion bajo): `mi_variable`, `nombre_completo`

---

## 🚫 Errores comunes

### Error 1: Olvidar las comillas en texto
```python
# MAL ❌
nombre = Cristian

# BIEN ✅
nombre = "Cristian"
```

### Error 2: Usar una variable antes de crearla
```python
# MAL ❌
print(saludo)
saludo = "Hola"

# BIEN ✅
saludo = "Hola"
print(saludo)
```

### Error 3: Confundir `=` con `==`
```python
# = asigna un valor
edad = 25

# == compara valores
edad == 25  # ¿es edad igual a 25? → True o False
```

### Error 4: Mayúsculas importan
```python
nombre = "Cristian"
print(Nombre)  # ERROR: Nombre ≠ nombre
```

---

## ✅ Buenas prácticas

1. **Nombres descriptivos**: `edad` es mejor que `e`
2. **Un concepto por variable**: No guardes todo junto
3. **Consistencia**: Usa el mismo estilo de nombres
4. **No abusar de variables cortas**: `x`, `y` solo para matemáticas

---

## 🧪 Mini preguntas de verificación

Responde sin ejecutar código:

1. ¿Qué imprime este código?
```python
x = 10
x = 20
print(x)
```

2. ¿Cuál es el error aquí?
```python
2nombre = "Cristian"
```

3. ¿Qué tipo de dato es `3.14`?

4. ¿Qué diferencia hay entre `"5"` y `5`?

---

## 📝 Resumen

| Concepto | Explicación |
|----------|-------------|
| Variable | Caja con nombre que guarda un valor |
| Crear | `nombre = valor` |
| Tipos | string, int, float, bool |
| Cambiar | Reasignar: `x = nuevo_valor` |
| Reglas | Sin espacios, no empezar con número |

---

## 🔗 Enlaces externos

- [Variables en Python - Documentación oficial](https://docs.python.org/3/tutorial/introduction.html#using-python-as-a-calculator)
- [Tipos de datos en Python](https://www.w3schools.com/python/python_datatypes.asp)
- [Nomenclatura en Python (PEP 8)](https://peps.python.org/pep-0008/#naming-conventions)

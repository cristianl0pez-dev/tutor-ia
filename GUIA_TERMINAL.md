# Guía de Terminal — Cómo Ejecutar tus Prácticas

## ¿Qué es la Terminal?

La terminal es una **ventana donde escribes comandos** para que la computadora haga cosas. Es como un chat, pero con tu sistema operativo.

**No te preocupes**, para este curso solo necesitas unos pocos comandos muy simples.

---

## Abrir la Terminal en Codespaces

### Opción 1 — Menú superior

1. Mira la parte superior de tu Codespace
2. Haz clic en **Terminal** → **New Terminal**

### Opción 2 — Atajo de teclado

Presiona `Ctrl + ñ` (o `` Ctrl + ` `` en teclados en inglés)

### Opción 3 — Desde el explorador

1. Haz clic derecho en cualquier carpeta del explorador de archivos
2. Selecciona **Open in Integrated Terminal**

Verás una ventana negra o gris en la parte inferior de tu pantalla. Ahí escribirás los comandos.

---

## Navegar en la Terminal

### Ver en qué carpeta estás

```bash
pwd
```

Te mostrará algo como `/workspaces/tutor-ia`.

### Ver los archivos en la carpeta actual

```bash
ls
```

Te mostrará una lista de archivos y carpetas.

### Entrar a una carpeta

```bash
cd nombre-de-la-carpeta
```

Ejemplo:
```bash
cd modulos/variables
```

### Volver a la carpeta anterior

```bash
cd ..
```

---

## Ejecutar tus Ejercicios

### Python

```bash
python modulos/<tema>/ejercicio_nivel1.py
```

Ejemplo real:
```bash
python modulos/variables/ejercicio_nivel1.py
```

### JavaScript / Node.js

```bash
node modulos/<tema>/ejercicio_nivel1.js
```

Ejemplo real:
```bash
node modulos/variables/ejercicio_nivel1.js
```

### TypeScript

```bash
npx ts-node modulos/<tema>/ejercicio_nivel1.ts
```

### Rust

```bash
rustc modulos/<tema>/ejercicio_nivel1.rs && ./ejercicio_nivel1
```

### HTML

- Abre el archivo `.html` en tu navegador
- En Codespaces: clic derecho en el archivo → **Open in Browser**

### SQL

```bash
sqlite3 < modulos/<tema>/ejercicio_nivel1.sql
```

### Bash

```bash
bash modulos/<tema>/ejercicio_nivel1.sh
```

### C

```bash
gcc modulos/<tema>/ejercicio_nivel1.c -o ejercicio && ./ejercicio
```

### Java

```bash
javac modulos/<tema>/ejercicio_nivel1.java && java ejercicio_nivel1
```

---

## Flujo de Trabajo Típico

1. El tutor te dice qué archivo crear o editar
2. Abre el archivo en el editor (clic izquierdo en el explorador)
3. Escribe tu código y guarda con `Ctrl + S`
4. Abre la terminal (si no está abierta)
5. Escribe el comando para ejecutar tu archivo
6. Revisa el resultado
7. Si hay errores, corrige y vuelve a ejecutar
8. Cuando funcione, escribe `/review` en OpenCode

---

## Errores Comunes

### "python: command not found"

Significa que Python no está instalado. En Codespaces generalmente ya viene. Si no:

```bash
sudo apt update && sudo apt install python3
```

### "No such file or directory"

La terminal no encuentra el archivo. Verifica:
- Que estás en la carpeta correcta (usa `pwd` y `ls`)
- Que el nombre del archivo está bien escrito

### "SyntaxError" o "Error"

El código tiene un error. Lee el mensaje de error, te dice en qué línea está el problema. Corrige y vuelve a ejecutar.

---

## Tips

- Usa la **flecha arriba** en la terminal para repetir el último comando
- Usa **Tab** para autocompletar nombres de archivos
- Puedes tener **varias terminales** abiertas al mismo tiempo

---

## ¿Aún no entiendes?

No te preocupes. Escribe `/simplify terminal` y el tutor te lo explicará paso a paso.

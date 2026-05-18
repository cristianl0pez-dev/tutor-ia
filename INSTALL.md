# Instalación del Tutor IA Pedagógico

## Requisitos

- Cuenta de [GitHub](https://github.com/)
- Acceso a [GitHub Codespaces](https://github.com/features/codespaces)

## Instalación en 4 Pasos

### Paso 1 — Clonar el repositorio

```bash
git clone https://github.com/cristianl0pez-dev/tutor-ia.git
```

### Paso 2 — Abrir en GitHub Codespaces

1. Ve a tu repositorio en GitHub
2. Haz clic en **Code** → **Codespaces** → **Create codespace**
3. Espera a que se configure el entorno

### Paso 3 — Instalar y configurar OpenCode

1. Instala la extensión de **OpenCode** en tu Codespace
2. **IMPORTANTE — Deshabilitar el atajo `Ctrl + P`**:
   - OpenCode usa `Ctrl + P` para enviar mensajes
   - VS Code usa el mismo atajo para abrir la paleta de comandos
   - Debes deshabilitarlo para que funcione correctamente

   **Cómo deshabilitar `Ctrl + P` en VS Code:**
   1. Presiona `Ctrl + Shift + P` para abrir la paleta de comandos
   2. Escribe: `Preferences: Open Keyboard Shortcuts` y presiona Enter
   3. En la barra de búsqueda escribe: `Ctrl+P`
   4. Busca el atajo **Go to File...** (o similar)
   5. Haz clic derecho sobre él → **Remove Keybinding**
   6. También busca cualquier otro atajo que use `Ctrl + P` y elimínalo

   **Verificación:**
   - Presiona `Ctrl + P`
   - Debería abrir el chat de OpenCode, **NO** la paleta de comandos de VS Code

### Paso 4 — Iniciar el tutor

Abre el panel de **OpenCode** en tu Codespace y escribe:

```
/teach <tema> en <lenguaje>
```

Ejemplos:
```
/teach variables en Python
/teach loops en JavaScript
/teach HTML
/teach funciones en Rust
```

## Estructura del Proyecto

```
tutor-ia/
├── AGENTS.md                          # Reglas del tutor
├── README.md                          # Guía general
├── .opencode/
│   ├── agents/
│   │   └── tutor.md                   # Agente principal
│   ├── commands/                      # Comandos personalizados
│   │   ├── teach.md
│   │   ├── practice.md
│   │   ├── review.md
│   │   ├── next.md
│   │   ├── hint.md
│   │   └── simplify.md
│   └── templates/                     # Templates de contenido
├── modulos/                           # Se crean dinámicamente
│   └── <tema>/
│       ├── 01_concepto.md
│       ├── 02_practica.md
│       └── ejercicios...
└── progreso/
    └── student_progress.md            # Tu progreso
```

## Comandos Disponibles

| Comando | Descripción |
|---------|-------------|
| `/teach <tema>` | Enseña un concepto nuevo |
| `/practice <tema>` | Genera ejercicios prácticos |
| `/review` | Revisa tu trabajo |
| `/next` | Avanza al siguiente nivel |
| `/hint` | Pide una pista |
| `/simplify <tema>` | Pide una explicación más simple |

## Lenguajes Soportados

Python, JavaScript, TypeScript, Rust, HTML/CSS, SQL, Bash, C, Java, y cualquier otro lenguaje.

## Uso

1. Pide un tema con `/teach`
2. Responde las preguntas del diagnóstico
3. Lee el concepto generado en `01_concepto.md`
4. Pide práctica con `/practice`
5. Completa los ejercicios editando los archivos en tu workspace
6. Escribe `/review` cuando termines
7. Avanza con `/next` cuando estés listo

## Notas

- Los módulos se crean automáticamente según lo que necesites
- Tu progreso se guarda en `progreso/student_progress.md`
- Puedes aprender cualquier tema en cualquier lenguaje

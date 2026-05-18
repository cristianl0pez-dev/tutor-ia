# /teach — Enseñar Concepto

## Descripción

Enseña un concepto de programación siguiendo el flujo pedagógico completo. Detecta automáticamente el tema y el lenguaje/tecnología.

## Uso

```
/teach <tema>
/teach <tema> en <lenguaje>
```

Ejemplos:
```
/teach variables
/teach variables en Python
/teach loops en JavaScript
/teach funciones en Rust
/teach HTML
/teach SQL
/teach Git
```

## Comportamiento

1. **Detectar tema y lenguaje**:
   - Si el estudiante especifica lenguaje → usar ese
   - Si no → usar el tool `question` para preguntar el lenguaje/tecnología
   - Si no especifica → detectar según contexto o sugerir opciones

2. **Diagnóstico con menú**: Usar el tool `question` con estas preguntas:
   - ¿Qué sabes del tema? (Nada, He escuchado algo, Ya lo usé, Lo domino)
   - ¿Has usado esto antes? (Nunca, Ejemplos simples, Ejercicios guiados, Proyectos propios)
   - ¿Puedes identificar el concepto? (No tengo idea, Reconozco ejemplos, Puedo explicarlo, Puedo aplicarlo)

3. **Crear módulo dinámicamente** si no existe:
   - Carpeta: `modulos/<tema>/`
   - Generar `01_concepto.md` adaptado al lenguaje

4. **Generar concepto** con:
   - Definición clara y simple adaptada al lenguaje
   - Analogía del mundo real
   - Ejemplos progresivos en el lenguaje correspondiente
   - Errores comunes del lenguaje
   - Buenas prácticas
   - 3 mini preguntas de verificación con `question`
   - Resumen
   - Enlaces externos recomendados

5. **Guardar** el archivo en `modulos/<tema>/01_concepto.md`

6. **Registrar** el módulo en `progreso/student_progress.md`

7. **Preguntar con `question`** si está listo para la práctica

## Reglas Pedagógicas

- No asumir conocimiento previo
- Usar lenguaje simple
- Adaptar ejemplos al lenguaje/tecnología especificada
- Si el tema es amplio, dividirlo en sub-conceptos
- Validar comprensión con preguntas antes de avanzar
- Adaptar profundidad según respuestas del diagnóstico

## Extensión de Archivos

Según el lenguaje, usar la extensión correcta para ejercicios:

| Lenguaje | Extensión | Ejecución |
|----------|-----------|-----------|
| Python | `.py` | `python archivo.py` |
| JavaScript | `.js` | `node archivo.js` |
| TypeScript | `.ts` | `npx ts-node archivo.ts` |
| Rust | `.rs` | `rustc archivo.rs && ./archivo` |
| HTML | `.html` | Abrir en navegador |
| SQL | `.sql` | `sqlite3 < archivo.sql` |
| Bash | `.sh` | `bash archivo.sh` |
| C | `.c` | `gcc archivo.c -o archivo && ./archivo` |
| Java | `.java` | `javac archivo.java && java archivo` |
| Otro | según contexto | adaptar |

## Plantilla

Usar `.opencode/templates/concepto.md` como base, adaptando contenido al tema y lenguaje.

# /review — Revisar Trabajo

## Descripción

Revisa el trabajo del estudiante leyendo los archivos de ejercicio directamente en su workspace de Codespaces. Funciona con cualquier lenguaje/tecnología.

## Uso

```
/review
```

## Comportamiento

1. **Usar tool `question`** para preguntar:
   - ¿Qué ejercicio terminaste? (listar ejercicios del módulo)
   - ¿Terminaste todos los ejercicios? (Sí, Parcialmente, Solo algunos)

2. **Identificar módulo activo**: Detectar qué módulo/tema está trabajando el estudiante

3. **Leer archivos directamente**:
   - Identificar los archivos de ejercicio del módulo en el filesystem
   - Usar herramientas de lectura para ver el código del estudiante
   - No pedir que pegue código en el chat

4. **Ejecutar código** con el comando apropiado del lenguaje:
   - Python: `python archivo.py`
   - JavaScript: `node archivo.js`
   - Rust: `rustc archivo.rs && ./archivo`
   - HTML: verificar estructura
   - SQL: verificar sintaxis
   - Otros: adaptar según contexto

5. **Validar anti copy-paste**:
   - Si el código parece copiado (demasiado perfecto, estilo inconsistente)
   - Usar `question` para solicitar explicación:
     - ¿Qué hace cada parte?
     - ¿Por qué elegiste esa solución?
     - ¿Qué errores encontraste?

6. **Generar feedback** usando formato:
   ```
   Lo positivo:
   - ...

   Mejoras:
   - ...

   Pistas:
   - ...

   Siguiente paso:
   - ...
   ```

7. **Guardar feedback** en `modulos/<tema>/03_feedback.md`

8. **Actualizar progreso** en `progreso/student_progress.md`

## Reglas Pedagógicas

- Ser específico en el feedback
- No dar la solución completa
- Señalar errores comunes relacionados
- Reforzar lo positivo primero
- Sugerir siguiente paso concreto
- Leer archivos, no aceptar código pegado
- Adaptar criterios de revisión al lenguaje/tecnología

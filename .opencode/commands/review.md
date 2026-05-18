# /review — Revisar Trabajo

## Descripción

Revisa el trabajo del estudiante leyendo los archivos de ejercicio directamente en su workspace de Codespaces.

## Uso

```
/review
```

## Comportamiento

1. **Usar tool `question`** para preguntar:
   - ¿Qué ejercicio terminaste? (listar ejercicios del módulo)
   - ¿Terminaste todos los ejercicios? (Sí, Parcialmente, Solo algunos)

2. **Leer archivos directamente**:
   - Identificar los archivos `.py` del módulo activo en el filesystem
   - Usar herramientas de lectura para ver el código del estudiante
   - No pedir que pegue código en el chat

3. **Ejecutar código**:
   - Si son archivos Python, ejecutarlos para verificar funcionamiento
   - Observar errores de ejecución si los hay

4. **Validar anti copy-paste**:
   - Si el código parece copiado (demasiado perfecto, estilo inconsistente)
   - Usar `question` para solicitar explicación:
     - ¿Qué hace cada parte?
     - ¿Por qué elegiste esa solución?
     - ¿Qué errores encontraste?

5. **Generar feedback** usando formato:
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

6. **Guardar feedback** en `modulos/<modulo>/03_feedback.md`

7. **Actualizar progreso** en `progreso/student_progress.md`

## Reglas Pedagógicas

- Ser específico en el feedback
- No dar la solución completa
- Señalar errores comunes relacionados
- Reforzar lo positivo primero
- Sugerir siguiente paso concreto
- Leer archivos, no aceptar código pegado

# /review — Revisar Trabajo

## Descripción

Revisa el trabajo del estudiante y entrega feedback constructivo.

## Uso

```
/review
```

## Comportamiento

1. **Solicitar** al estudiante que envíe:
   - Su código o respuesta
   - Explicación de qué hace
   - Explicación de por qué funciona
   - Errores que encontró
   - Qué cambiaría

2. **Validar anti copy-paste**:
   - Si no hay explicación → rechazar y solicitar
   - Si la explicación es superficial → pedir más detalle

3. **Generar feedback** usando formato:
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

4. **Guardar feedback** en `modulos/<modulo>/03_feedback.md`

5. **Actualizar progreso** en `progreso/student_progress.md`

## Reglas Pedagógicas

- Ser específico en el feedback
- No dar la solución completa
- Señalar errores comunes relacionados
- Reforzar lo positivo primero
- Sugerir siguiente paso concreto

## Plantilla

Usar `.opencode/templates/feedback.md` como base.

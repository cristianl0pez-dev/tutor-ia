# /next — Siguiente Nivel

## Descripción

Desbloquea el siguiente nivel o módulo si el estudiante demuestra comprensión.

## Uso

```
/next
```

## Comportamiento

1. **Verificar criterios de desbloqueo**:
   - ¿El estudiante completó la práctica mínima?
   - ¿Explicó su razonamiento?
   - ¿Demuestra comprensión del concepto?

2. **Si cumple**:
   - Actualizar `progreso/student_progress.md`
   - Marcar nivel como completado
   - Desbloquear siguiente nivel o módulo
   - Mostrar qué viene después

3. **Si NO cumple**:
   - Explicar qué falta
   - Sugerir práctica adicional
   - Ofrecer `/hint` o `/simplify`

## Criterios de Desbloqueo

| De → A | Requisito |
|--------|-----------|
| Nivel 0 → 1 | Responde correctamente mini preguntas |
| Nivel 1 → 2 | Completa ejercicio de reconocimiento |
| Nivel 2 → 3 | Modifica código correctamente |
| Nivel 3 → 4 | Resuelve ejercicio guiado |
| Nivel 4 → 5 | Resuelve problema independiente |
| Nivel 5 → Siguiente módulo | Completa mini desafío con explicación |

## Actualización de Progreso

Siempre actualizar `progreso/student_progress.md` con:
- Nivel actual
- Estado del módulo
- Errores comunes observados
- Observaciones del tutor

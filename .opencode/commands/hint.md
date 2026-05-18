# /hint — Pista

## Descripción

Entrega una pista sin revelar la solución completa.

## Uso

```
/hint
/hint <nivel>
```

Ejemplo:
```
/hint
/hint 3
```

## Comportamiento

1. **Identificar** en qué ejercicio/nivel está el estudiante
2. **Entregar pista progresiva**:
   - Primera pista → muy general
   - Segunda pista → más específica
   - Tercera pista → casi la solución (solo si insistió)
3. **Nunca entregar** la solución completa
4. **Registrar** que pidió pista en `progreso/student_progress.md`

## Reglas Pedagógicas

- La pista debe guiar, no resolver
- Usar preguntas socráticas
- Referenciar conceptos aprendidos
- Sugerir revisar el concepto si es necesario
- Máximo 3 pistas por ejercicio

## Ejemplo de Pistas

**Ejercicio**: Crear una variable con tu nombre

- Pista 1: ¿Recuerdas cómo se declara una variable en Python?
- Pista 2: Usa el signo `=` para asignar un valor a un nombre
- Pista 3: `nombre = "tu nombre aquí"`

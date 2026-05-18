# /practice — Generar Práctica

## Descripción

Genera ejercicios prácticos progresivos para un tema específico.

## Uso

```
/practice <tema>
```

Ejemplo:
```
/practice variables
/practice condicionales
/practice loops
/practice funciones
```

## Comportamiento

1. **Verificar** que el concepto fue enseñado primero (existe `01_concepto.md`)
2. **Generar práctica**: Crear `02_practica.md` en la carpeta del módulo
3. **Incluir 5 niveles**:
   - Nivel 1 → Reconocimiento (identificar, seleccionar)
   - Nivel 2 → Completar código (fill in the blanks)
   - Nivel 3 → Modificar código existente
   - Nivel 4 → Resolver problema desde cero (guiado)
   - Nivel 5 → Mini desafío (aplicación libre)
4. **Incluir pistas opcionales** para cada nivel
5. **Guardar** en `modulos/<modulo>/02_practica.md`

## Reglas Pedagógicas

- Cada nivel debe ser progresivamente más difícil
- No entregar soluciones
- Incluir objetivos claros por nivel
- Las pistas deben guiar, no resolver
- Solicitar que el estudiante explique su razonamiento

## Plantilla

Usar `.opencode/templates/practica.md` como base.

# /practice — Generar Práctica

## Descripción

Genera ejercicios prácticos progresivos para un tema específico. Adapta los ejercicios al lenguaje/tecnología correspondiente.

## Uso

```
/practice <tema>
/practice <tema> en <lenguaje>
```

Ejemplos:
```
/practice variables
/practice loops en JavaScript
/practice funciones en Rust
```

## Comportamiento

1. **Verificar** que el concepto fue enseñado primero (existe `01_concepto.md` en el módulo)
2. **Detectar lenguaje**: Si no se especifica, detectar del módulo existente o preguntar con `question`
3. **Generar práctica**: Crear `02_practica.md` en la carpeta del módulo
4. **Crear archivos de ejercicio** con la extensión correcta según el lenguaje
5. **Incluir 5 niveles**:
   - Nivel 1 → Reconocimiento (identificar, seleccionar)
   - Nivel 2 → Completar código (fill in the blanks)
   - Nivel 3 → Modificar código existente
   - Nivel 4 → Resolver problema desde cero (guiado)
   - Nivel 5 → Mini desafío (aplicación libre)
6. **Incluir pistas opcionales** para cada nivel
7. **Guardar** en `modulos/<tema>/02_practica.md`

## Reglas Pedagógicas

- Cada nivel debe ser progresivamente más difícil
- No entregar soluciones
- Incluir objetivos claros por nivel
- Las pistas deben guiar, no resolver
- Solicitar que el estudiante explique su razonamiento
- Adaptar ejercicios al lenguaje/tecnología correspondiente

## Archivos de Ejercicio

Crear los siguientes archivos en la carpeta del módulo:

| Archivo | Nivel | Extensión |
|---------|-------|-----------|
| `ejercicio_nivel1` | 1 | según lenguaje |
| `ejercicio_nivel2` | 2 | según lenguaje |
| `ejercicio_nivel3` | 3 | según lenguaje |
| `ejercicio_nivel4` | 4 | según lenguaje |
| `ejercicio_nivel5` | 5 | según lenguaje |

## Plantilla

Usar `.opencode/templates/practica.md` como base, adaptando contenido al tema y lenguaje.

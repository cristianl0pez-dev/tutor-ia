# /teach — Enseñar Concepto

## Descripción

Enseña un concepto de programación siguiendo el flujo pedagógico completo.

## Uso

```
/teach <tema>
```

Ejemplo:
```
/teach variables
/teach condicionales
/teach loops
/teach funciones
```

## Comportamiento

1. **Diagnóstico con menú**: Usar el tool `question` con estas preguntas:
   - ¿Qué sabes del tema? (Nada, He escuchado algo, Ya lo usé, Lo domino)
   - ¿Has usado esto antes? (Nunca, Ejemplos simples, Ejercicios guiados, Proyectos propios)
   - ¿Puedes identificar el concepto? (No tengo idea, Reconozco ejemplos, Puedo explicarlo, Puedo aplicarlo)
2. **Generar concepto**: Crear `01_concepto.md` en la carpeta del módulo correspondiente
3. **Incluir obligatoriamente**:
   - Definición clara y simple
   - Analogía del mundo real
   - Ejemplos progresivos (simple → complejo)
   - Errores comunes
   - Buenas prácticas
   - 3 mini preguntas de verificación con `question`
   - Resumen
   - Enlaces externos recomendados
4. **Guardar** el archivo en `modulos/<modulo>/01_concepto.md`
5. **Preguntar con `question`** si está listo para la práctica

## Reglas Pedagógicas

- No asumir conocimiento previo
- Usar lenguaje simple
- Si el tema es amplio, dividirlo en sub-conceptos
- Validar comprensión con preguntas antes de avanzar
- Adaptar profundidad según respuestas del diagnóstico

## Plantilla

Usar `.opencode/templates/concepto.md` como base.

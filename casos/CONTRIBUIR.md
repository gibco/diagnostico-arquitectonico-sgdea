
# Cómo contribuir con casos de uso

Este espacio está destinado a registrar aplicaciones reales del instrumento de diagnóstico en entidades públicas y privadas.

## Condiciones para contribuir

- Los datos de la entidad deben estar **anonimizados** (sin nombre, sector o país identificables si la entidad no ha dado consentimiento explícito).
- El caso debe incluir los resultados del diagnóstico por dimensión, no solo el puntaje final.
- Se debe indicar qué fase de transición (si alguna) fue iniciada como resultado del diagnóstico.

## Formato del caso

Crea un archivo `.md` en esta carpeta con el nombre: `caso-YYYY-MM-sector.md`

Ejemplo: `caso-2026-03-sector-salud.md`

### Estructura mínima del caso

```markdown
# Caso: [Sector] — [Año]

## Contexto
- Tipo de entidad: (pública / privada / mixta)
- Sector: (salud / educación / tributario / judicial / otro)
- Tamaño aproximado: (número de usuarios del SGDEA)
- Plataforma evaluada: (puede omitirse o anonimizarse)

## Resultados por dimensión

| Dimensión | Puntuación | Observación |
|-----------|------------|-------------|
| 1. Separación creación / clasificación | X/20 | ... |
| 2. Independencia del expediente | X/20 | ... |
| 3. Versionamiento de la TRD | X/20 | ... |
| 4. Patrón común de integración | X/20 | ... |
| 5. Gobernanza de metadatos | X/20 | ... |
| **Total** | **X/100** | **Nivel:** |

## Hallazgos principales
(máximo 3 párrafos)

## Acciones derivadas
(si las hubo)

## Notas del contribuidor
(opcional)
```

## Proceso

1. Haz un fork del repositorio.
2. Crea tu archivo de caso en `/casos/`.
3. Abre un Pull Request con el título: `Caso: [sector] [año]`.

Las contribuciones serán revisadas antes de ser incorporadas al repositorio principal.

---

*La trazabilidad no se negocia. La arquitectura se diseña.*

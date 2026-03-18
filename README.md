# Instrumento de Diagnóstico Arquitectónico
### Arquitecturas Acopladas y Desacopladas en Gestión Documental Electrónica

> **Pruebas estructurales para verificar el nivel de desacoplamiento en sistemas de gestión documental**

[![Licencia: CC BY-NC-SA 4.0](https://img.shields.io/badge/Licencia-CC%20BY--NC--SA%204.0-blue.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.es)
[![Basado en el libro](https://img.shields.io/badge/Basado%20en-Arqdes%20KDP%202026-orange.svg)](https://www.archivistadigital.com)
[![GitHub Pages](https://img.shields.io/badge/Instrumento%20interactivo-GitHub%20Pages-brightgreen.svg)](https://jhon-gonzalez.github.io/diagnostico-arquitectonico-sgdea/)

---

## ¿Qué es este repositorio?

Este repositorio es la extensión práctica del libro:

**[Arquitecturas Acopladas y Desacopladas en Gestión Documental Electrónica: Cómo diseñar sistemas que sobrevivan al cambio institucional](http://www.archivistadigital.com)**  
*Jhon Alexander González Flórez — ISBN 9798251584622*

El libro define los criterios de diseño. Este instrumento los hace verificables.

La sostenibilidad de un sistema documental no depende de la herramienta implementada, sino del diseño arquitectónico que la antecede. Una arquitectura mal diseñada no colapsa el primer año — lo vuelve cada vez más costoso de transformar.

**Este instrumento permite responder la pregunta crítica:**

> ¿Tiene su institución una arquitectura documental que sobrevivirá al cambio institucional en los próximos 10 a 15 años?

---

## El modelo nuclear

Todo diagnóstico parte del núcleo estructural inalterable:

```
Evento documental → Documento → Expediente → Clasificación (TRD) → Retención
```

Cada nivel cumple una función distinta y pertenece a una capa diferente de responsabilidad. **Invertir este orden es el origen del acoplamiento estructural.**

---

## Estructura del repositorio

```
/
├── README.md                          → Este documento
├── instrumento/
│   ├── index.html                     → Instrumento interactivo (GitHub Pages)
│   └── diagnostico-imprimible.md      → Versión imprimible en Markdown
├── criterios/
│   └── criterios-tecnicos.md          → Los 7 criterios técnicos del Capítulo 5
├── matriz/
│   └── evento-sistema-responsabilidad.md  → Modelo operativo (plantilla)
├── casos/
│   └── CONTRIBUIR.md                  → Cómo aportar casos de uso
├── CITATION.md                        → Cómo citar este instrumento
└── LICENSE                            → Creative Commons BY-NC-SA 4.0
```

---

## Instrumento interactivo

El instrumento de diagnóstico está disponible en:

🔗 **[https://jhon-gonzalez.github.io/diagnostico-arquitectonico-sgdea/instrumento/](https://jhon-gonzalez.github.io/diagnostico-arquitectonico-sgdea/instrumento/)**

Evalúa 5 dimensiones estructurales con 25 pruebas verificables y genera:

- Puntuación por dimensión
- Nivel de desacoplamiento (Declarativo / Parcial / Real / Sostenible)
- Mapa visual de riesgo arquitectónico
- Recomendaciones priorizadas por fase de transición

---

## Las 5 dimensiones del diagnóstico

| # | Dimensión | Prueba estructural clave |
|---|-----------|--------------------------|
| 1 | **Separación creación / clasificación** | ¿Puede eliminarse del sistema misional cualquier referencia a códigos de TRD sin afectar la producción documental? |
| 2 | **Independencia del expediente** | ¿Puede modificarse el proceso operativo sin alterar la estructura histórica del expediente? |
| 3 | **Versionamiento de la TRD** | ¿Puede identificarse qué versión de TRD estaba vigente cuando se clasificó un expediente específico? |
| 4 | **Patrón común de integración** | ¿Puede incorporarse un nuevo sistema productor sin rediseñar el modelo nuclear? |
| 5 | **Gobernanza de metadatos** | ¿Pueden exportarse expedientes completos con sus metadatos esenciales sin depender del proveedor? |

---

## Verificación rápida de desacoplamiento

Si la respuesta es afirmativa en **todos** los casos, el desacoplamiento es real. Si no, es declarativo.

- [ ] ¿Puede el sistema misional operar sin conocer la estructura detallada de la TRD?
- [ ] ¿Puede el SGDEA consolidar expedientes sin depender del workflow original?
- [ ] ¿Puede el Archivo actualizar la TRD sin intervención directa del proveedor?
- [ ] ¿Puede incorporarse un nuevo sistema productor sin rediseñar el núcleo?
- [ ] ¿Puede reconstruirse un expediente dentro de 15 años sin el proveedor original?

---

## Niveles de resultado

| Puntuación | Nivel | Interpretación |
|------------|-------|----------------|
| 0 – 30% | 🔴 **Acoplamiento crítico** | El sistema no sobrevivirá cambios institucionales mayores sin intervención estructural urgente. |
| 31 – 55% | 🟠 **Desacoplamiento declarativo** | Existe intención de separación pero persisten acoplamientos estructurales que generarán deuda técnica. |
| 56 – 79% | 🟡 **Desacoplamiento parcial** | El núcleo está parcialmente estabilizado. Existen fases de transición pendientes identificables. |
| 80 – 100% | 🟢 **Arquitectura sostenible** | El sistema cumple condiciones estructurales para sobrevivir al cambio institucional en horizonte de 10–15 años. |

---

## Uso recomendado

Este instrumento está diseñado para:

- **Directores de Gestión Documental** que evalúan la arquitectura actual antes de una migración o reforma.
- **Arquitectos de sistemas** que diseñan la integración de un SGDEA con sistemas misionales.
- **Consultores y auditores** que realizan diagnósticos de madurez archivística.
- **Responsables de contratación pública** que evalúan propuestas de implementación SGDEA.

No es un cuestionario de funcionalidades. Es una prueba estructural.

---

## Contribuciones

Este instrumento es un documento vivo. Las contribuciones son bienvenidas en dos modalidades:

**Casos de uso:** Si has aplicado el instrumento en una entidad real (con datos anonimizados), puedes aportar el caso en `/casos/`. Ver instrucciones en [CONTRIBUIR.md](casos/CONTRIBUIR.md).

**Mejoras al instrumento:** Abre un *issue* describiendo la prueba estructural que consideras debe incorporarse, con referencia al criterio técnico correspondiente del libro.

---

## Cómo citar

Si utilizas este instrumento en un trabajo académico, diagnóstico institucional o publicación técnica, consulta el archivo [CITATION.md](CITATION.md).

Referencia rápida:

```
González Flórez, J. A. (2026). Instrumento de Diagnóstico Arquitectónico: 
Arquitecturas Acopladas y Desacopladas en Gestión Documental Electrónica. 
GitHub. https://github.com/jhon-gonzalez/diagnostico-arquitectonico-sgdea

Basado en: González Flórez, J. A. (2026). Arquitecturas Acopladas y Desacopladas 
en Gestión Documental Electrónica: Cómo diseñar sistemas que sobrevivan al 
cambio institucional. Independently published. ISBN 9798251584622.
```

---

## Licencia

Este instrumento se distribuye bajo licencia [Creative Commons BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.es).

Puedes usarlo y adaptarlo libremente con fines no comerciales, siempre que cites la fuente y mantengas la misma licencia en obras derivadas.

---

## Sobre el autor

**Jhon Alexander González Flórez**  
Consultor especializado en Gestión Documental Electrónica, Preservación Digital y Accesibilidad Web.

[archivistadigital.com](http://www.archivistadigital.com)  
[Patreon: ArchivistaDigital](https://www.patreon.com/c/ArchivistaDigital)
[Linkedin: ArchivistaDigital](https://www.linkedin.com/newsletters/archivista-digital-7268276454386196480/)



---

*La trazabilidad no se negocia. La arquitectura se diseña.*


# Criterios Técnicos para Arquitecturas Sostenibles

> Extraídos del Capítulo 5 del libro *Arquitecturas Acopladas y Desacopladas en Gestión Documental Electrónica* (ISBN 9798251584622).

Una arquitectura desacoplada no se valida por su declaración conceptual. Se valida por su comportamiento frente al cambio.

---

## Criterio 1 — Separación efectiva entre creación y clasificación

La clasificación debe aplicarse como capa **posterior** a la producción documental. No nominal: real.

**Prueba estructural:**
- ¿Puede eliminarse del sistema misional cualquier referencia a códigos de TRD sin afectar la producción documental?
- ¿Puede aplicarse una nueva versión de TRD sin modificar la lógica interna del sistema productor?

> Si la respuesta es negativa, existe acoplamiento residual.

---

## Criterio 2 — Independencia del expediente frente al flujo

El expediente debe ser una unidad lógica **independiente del workflow operativo**. Si el proceso cambia, el expediente no debe cambiar.

**Prueba estructural:**
- ¿Puede modificarse el proceso operativo sin alterar la estructura histórica del expediente?
- ¿Puede reconstruirse un expediente completo sin necesidad de reproducir el workflow original?

> Si la respuesta es negativa, la arquitectura es vulnerable.

---

## Criterio 3 — Versionamiento formal de la TRD

Las TRD evolucionan. La arquitectura debe permitir coexistencia de versiones y aplicación prospectiva.

**Prueba estructural:**
- ¿Puede identificarse qué versión de TRD estaba vigente cuando se clasificó un expediente específico?
- ¿Puede actualizarse la TRD sin reprocesar expedientes históricos?
- ¿Puede versionarse la TRD sin intervención profunda del proveedor?

> Si no es posible, la arquitectura compromete la autoridad archivística.

---

## Criterio 4 — Integraciones bajo patrón común

La sostenibilidad no depende de la primera integración. Depende de la décima.

**Patrón mínimo exigible a todo sistema productor:**
1. Registrar el evento en origen.
2. Generar documento con metadatos funcionales mínimos.
3. Transferir evidencia al núcleo documental bajo protocolo común.
4. Consolidar el expediente de forma independiente.
5. Aplicar clasificación y retención centralmente.

**Prueba estructural:**
- ¿Existe un protocolo único de integración aplicable a cualquier sistema productor?
- ¿Puede incorporarse un nuevo sistema sin rediseñar el modelo nuclear?

> Si cada incorporación exige redefinición estructural, la arquitectura no es sostenible.

---

## Criterio 5 — Gobernanza clara de metadatos

Deben distinguirse tres capas:
- **Metadatos funcionales** — propios del sistema productor.
- **Metadatos estructurales** — propios del expediente.
- **Metadatos archivísticos** — propios de clasificación y retención.

**Prueba estructural:**
- ¿Pueden exportarse expedientes completos con sus metadatos esenciales sin depender del proveedor?
- ¿Puede interpretarse la estructura del expediente fuera de la plataforma original?

> Si no es posible, la preservación futura estará comprometida.

---

## Criterio 6 — Control de deuda técnica estructural

La deuda técnica en gestión documental no se manifiesta como falla operativa inmediata. Se manifiesta como incapacidad de evolución.

**Indicadores tempranos de deuda estructural:**
- TRD que no se actualiza por temor al impacto tecnológico.
- Dependencia del proveedor para ajustes menores.
- Dificultad para integrar nuevos sistemas.
- Imposibilidad de reconstruir expedientes fuera de la plataforma original.

> La sostenibilidad exige monitorear estos indicadores como parte del gobierno del sistema.

---

## Criterio 7 — Resiliencia temporal a 10–15 años

El criterio definitivo. Una arquitectura madura permite que dentro de una década:

- La institución se reorganice sin fragmentar su memoria.
- Se cambie de proveedor sin redefinir el modelo estructural.
- Se migre infraestructura sin perder trazabilidad.
- Se implemente preservación digital sin rediseñar el núcleo.

**Preguntas de cierre:**
- ¿Puede reconstruirse el expediente sin rehacer el sistema?
- ¿Puede la institución trasladar su memoria digital a una nueva plataforma sin redefinir su modelo estructural?

> Si la migración es transición controlada, la arquitectura es madura. Si es reconstrucción traumática, el colapso es previsible.

---

*La trazabilidad no se negocia. La arquitectura se diseña.*


# Modelo Operativo: Evento × Sistema × Responsabilidad

> Extraído del Capítulo 4 del libro *Arquitecturas Acopladas y Desacopladas en Gestión Documental Electrónica* (ISBN 9798251584622).

## Propósito

Este modelo formaliza la separación estructural entre lógica misional, lógica documental y gobierno archivístico. No es una herramienta de gestión de tareas. Es un instrumento de control arquitectónico.

---

## Matriz de responsabilidades

| Elemento | Responsable | Función principal | Lo que NO debe hacer |
|----------|-------------|-------------------|----------------------|
| **Evento documental** | Sistema misional | Registrar la ocurrencia del hecho administrativo y generar evidencia asociada | Clasificar bajo TRD. Determinar retención. Consolidar expediente archivístico. |
| **Documento** | Sistema productor | Generar y transferir evidencia con metadatos funcionales mínimos al núcleo documental | Definir serie. Aplicar retención. Construir expediente. |
| **Expediente** | SGDEA | Consolidar la unidad estructural independiente del flujo | Sustituir sistemas misionales. Crear eventos. Definir procesos funcionales. |
| **Clasificación (TRD)** | SGDEA bajo gobierno archivístico | Asignar contexto orgánico-funcional versionable | Condicionar la creación documental. Definir plantillas operativas. Programar flujos. |
| **Retención** | Archivo institucional | Determinar permanencia y disposición final conforme a política archivística | Programarse como automatismo en sistemas funcionales. Depender de estados operativos. |

---

## Preguntas de verificación

El modelo permite formular preguntas críticas sobre el estado actual de la arquitectura:

**Sobre el sistema misional:**
- [ ] ¿Opera sin conocer la estructura detallada de la TRD?
- [ ] ¿Sus campos de captura son independientes de los códigos de clasificación?
- [ ] ¿Transfiere evidencia al núcleo bajo un protocolo estándar?

**Sobre el SGDEA:**
- [ ] ¿Consolida expedientes sin depender del workflow original?
- [ ] ¿Aplica clasificación como capa posterior a la producción documental?
- [ ] ¿Registra la versión de TRD vigente al momento de clasificación?

**Sobre el Archivo institucional:**
- [ ] ¿Puede actualizar la TRD sin intervención directa del proveedor?
- [ ] ¿Las reglas de retención están versionadas y documentadas?
- [ ] ¿La disposición final se aplica bajo autoridad archivística, no como automatismo técnico?

**Sobre la arquitectura en conjunto:**
- [ ] ¿Puede incorporarse un nuevo sistema productor sin rediseñar el núcleo?
- [ ] ¿Puede reconstruirse un expediente dentro de 15 años sin el proveedor original?

---

## Riesgos de superposición competencial

| Superposición | Consecuencia |
|---------------|--------------|
| El sistema misional clasifica bajo TRD | Duplicidad estructural. Versiones divergentes. |
| El SGDEA define procesos misionales | Invasión funcional. Resistencia operativa. |
| El Archivo programa automatismos directamente en sistemas productores | Dependencia tecnológica. Pérdida de autoridad archivística. |
| La retención se gestiona desde el sistema funcional | Dispersión de la política archivística. |

> Cada superposición genera acoplamiento residual.

---

## Señal de desacoplamiento real

Si la respuesta es **afirmativa en todos los casos**, el desacoplamiento es real.  
Si alguna respuesta es negativa, el desacoplamiento es **declarativo**.

| Verificación | Estado |
|-------------|--------|
| El sistema misional puede operar sin conocer la TRD | ✓ / ✗ |
| El SGDEA puede consolidar expedientes sin el workflow original | ✓ / ✗ |
| El Archivo puede actualizar la TRD sin el proveedor | ✓ / ✗ |
| Un nuevo sistema puede incorporarse sin rediseñar el núcleo | ✓ / ✗ |
| El expediente puede reconstruirse en 15 años sin el proveedor | ✓ / ✗ |

---

*La trazabilidad no se negocia. La arquitectura se diseña.*

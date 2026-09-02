# Discovery Validation — Sistema de Gestión Escolar

**versión del cuestionario auditado:** `institutional-discovery.md` — Revisión 2 corregida (Q-001…Q-085)
**Tipo de auditoría:** **Re-auditoría final** (00.3C) tras la corrección de trazabilidad (00.3B).
**Fecha:** 2026-09-02
**Estado del proyecto:** DISCOVERY (no se avanza a Foundation).

Re-auditoría final del cuestionario institucional corregido contra `discovery-audit.md`
(UNKNOWN/DECISION_REQUIRED/RISK), `Vision.md` (funcionalidades V1 y tecnologías) y los 14 dominios del
cuestionario. Las auditorías anteriores (R1, R2) se conservan íntegras en el Anexo A.

---

## 1. Validation Summary

| Aspecto | Resultado |
| --- | --- |
| Total de preguntas definidas (Q-001…Q-085) | **83** (Q-046 y Q-065 retiradas; Q-071…Q-085 añadidas) |
| Preguntas `VALID` | **83** |
| Preguntas `NEEDS_REFINEMENT` | **0** |
| Preguntas `DUPLICATE` | **0** |
| Preguntas `LOW_VALUE` | **0** |
| GAPs remanentes del Discovery (cobertura) | **0** (GAP-001…GAP-005 resueltos) |
| Inconsistencias de identificación/etiquetas | **0** (corregidas en 00.3B) |
| Evidencia faltante (Evidence Required) | Correctamente concentrada en la sección 8; sin faltantes estructurales |
| Trazabilidad Q-011–Q-015, Q-019–Q-027, Q-063, Q-068 | **OK — alineada con su contenido** |
| Respuestas institucionales | **83/83 en `PENDING`** (sin respuestas emitidas) |
| **Veredicto final** | **DISCOVERY QUESTIONNAIRE READY** |

**Conclusión de una línea:** El único bloqueante restante —las 13 etiquetas desplazadas de la sección 4
(Q-011–Q-015, Q-019–Q-027)— fue corregido en el PIPELINE 00.3B y verificado. El cuestionario cumple ya
todos los criterios de `DISCOVERY QUESTIONNAIRE READY`: trazabilidad correcta, integridad, cobertura
completa (GAP-001…GAP-005 resueltos y todos los dominios/funcionalidades V1 cubiertos) y calidad sin
ambigüedades, duplicados, soluciones técnicas implícitas ni contradicciones.

---

## 2. Question Audit

Clasificación por pregunta. **83 de 83 `VALID`** tras la corrección de trazabilidad.

| ID (contenido real) | Prioridad | Clasificación | Observación |
| --- | --- | --- | --- |
| Q-001 — Institución / Contexto | CRITICAL | VALID | — |
| Q-002 — Institución / Tamaño | HIGH | VALID | — |
| Q-003 — Institución / Usuarios del sistema (incl. V1) | CRITICAL | VALID | Absorbe a Q-046 (consolidada). |
| Q-004 — Institución / Vista de procesos | CRITICAL | VALID | Reformulada; detalle en Q-015/023/031/035. |
| Q-005 — Institución / Ciclo académico | HIGH | VALID | — |
| Q-006 — Estudiantes / Datos existentes | CRITICAL | VALID | — |
| Q-007 — Estudiantes / Estructura de la planilla | CRITICAL | VALID | Ejemplo anónimo movido a sección 8. |
| Q-008 — Estudiantes / Identificación oficial | CRITICAL | VALID | — |
| Q-009 — Estudiantes / Datos personales | HIGH | VALID | — |
| Q-010 — Estudiantes / Estados | CRITICAL | VALID | Alineada. |
| Q-011 — Estudiantes / Historial | HIGH | VALID | Alineada (antes mal etiquetada). |
| Q-012 — Estudiantes / Altas y bajas | HIGH | VALID | Alineada (antes mal etiquetada). |
| Q-013 — Estudiantes / Correcciones | HIGH | VALID | Alineada (antes mal etiquetada). |
| Q-014 — Estudiantes / Documentos asociados | HIGH | VALID | Alineada (antes mal etiquetada). |
| Q-015 — Matrícula / Proceso y periodicidad | HIGH | VALID | Alineada (antes mal etiquetada). |
| Q-016 — Matrícula / Grados y secciones | CRITICAL | VALID | — |
| Q-017 — Matrícula / Documentación | CRITICAL | VALID | — |
| Q-018 — Matrícula / Reingresos y traslados | CRITICAL | VALID | — |
| Q-019 — Matrícula / Históricos | HIGH | VALID | Alineada (antes mal etiquetada). |
| Q-020 — Encargados / Relación | HIGH | VALID | Alineada (antes mal etiquetada). |
| Q-021 — Encargados / Datos | HIGH | VALID | Alineada (antes mal etiquetada). |
| Q-022 — Encargados / Responsabilidades | CRITICAL | VALID | — |
| Q-023 — Asistencia / Quién y cuándo | HIGH | VALID | Alineada (antes mal etiquetada). |
| Q-024 — Asistencia / Estados posibles | HIGH | VALID | Alineada (antes mal etiquetada). |
| Q-025 — Asistencia / Reglas | HIGH | VALID | Alineada (antes mal etiquetada). |
| Q-026 — Asistencia / Correcciones | HIGH | VALID | Alineada (antes mal etiquetada). |
| Q-027 — Asistencia / Reportes | HIGH | VALID | Alineada (antes mal etiquetada). |
| Q-028 — Pagos / Conceptos | CRITICAL | VALID | — |
| Q-029 — Pagos / Periodicidad | HIGH | VALID | — |
| Q-030 — Pagos / Parciales y saldos | CRITICAL | VALID | — |
| Q-031 — Pagos / Forma de pago | HIGH | VALID | — |
| Q-032 — Pagos / Recibos | HIGH | VALID | — |
| Q-033 — Pagos / Anulaciones | CRITICAL | VALID | — |
| Q-034 — Pagos / Historial | HIGH | VALID | — |
| Q-035 — Reportes / Actualmente usados | HIGH | VALID | — |
| Q-036 — Reportes / Formato de salida | HIGH | VALID | — |
| Q-037 — Reportes / Adicionales | HIGH | VALID | — |
| Q-038 — Reportes / Periodicidad y destinatarios | HIGH | VALID | — |
| Q-039 — Documentos / Qué se almacena | HIGH | VALID | — |
| Q-040 — Documentos / Formatos | HIGH | VALID | — |
| Q-041 — Documentos / Acceso | HIGH | VALID | — |
| Q-042 — Documentos / Retención | HIGH | VALID | — |
| Q-043 — Datos / Excel y otros archivos | HIGH | VALID | — |
| Q-044 — Datos / Calidad | MEDIUM | VALID | — |
| Q-045 — Datos / Fuente oficial | MEDIUM | VALID | — |
| Q-047 — Usuarios / Futuros | MEDIUM | VALID | Reformulada (inducción eliminada). |
| Q-048 — Usuarios / Responsabilidades | MEDIUM | VALID | Absorbe parte de Q-046. |
| Q-049 — Seguridad / Acceso físico | HIGH | VALID | — |
| Q-050 — Seguridad / Credenciales | HIGH | VALID | Ajuste de neutralidad. |
| Q-051 — Seguridad / Confidencial | CRITICAL | VALID | Solapamiento parcial con Q-077 (no duplicado, ver §6). |
| Q-052 — Seguridad / Auditoría | HIGH | VALID | — |
| Q-053 — Seguridad / Recuperación | HIGH | VALID | — |
| Q-054 — Backups / Qué respaldar | HIGH | VALID | — |
| Q-055 — Backups / Frecuencia | HIGH | VALID | — |
| Q-056 — Backups / Destinos | MEDIUM | VALID | — |
| Q-057 — Backups / Responsable | MEDIUM | VALID | — |
| Q-058 — Backups / Restauración | MEDIUM | VALID | — |
| Q-059 — Backups / Protocolo ante fallo | HIGH | VALID | — |
| Q-060 — Infraestructura / Computadora y SO | HIGH | VALID | — |
| Q-061 — Infraestructura / Conectividad | HIGH | VALID | Reformulada (solución técnica implícita eliminada). |
| Q-062 — Infraestructura / Restricciones | MEDIUM | VALID | — |
| Q-063 — Infraestructura / Acceso físico | CRITICAL | VALID | Alineada; etiqueta correcta en sección 3. |
| Q-064 — Operación / Administrador | MEDIUM | VALID | — |
| Q-066 — Operación / Continuidad del desarrollador | LOW | VALID | — |
| Q-067 — Operación / Actualizaciones | LOW | VALID | — |
| Q-068 — Alcance / Datos en V1 | CRITICAL | VALID | Alineada; etiqueta correcta en sección 3. |
| Q-069 — Alcance / Prioridad de V1 | HIGH | VALID | — |
| Q-070 — Alcance / Documento maestro | CRITICAL | VALID | — |
| Q-071 — Matrícula / Asignaturas (GAP-001) | HIGH | VALID | — |
| Q-072 — Matrícula / Asignaturas (GAP-001) | HIGH | VALID | — |
| Q-073 — Matrícula / Asignaturas (GAP-001) | HIGH | VALID | — |
| Q-074 — Pagos / Descuentos (GAP-002) | HIGH | VALID | — |
| Q-075 — Pagos / Becas y exoneraciones (GAP-002) | HIGH | VALID | — |
| Q-076 — Pagos / Reglas de descuentos (GAP-002) | HIGH | VALID | — |
| Q-077 — Seguridad / Confidencialidad de datos (GAP-003) | HIGH | VALID | Solapamiento parcial con Q-051 (no duplicado). |
| Q-078 — Seguridad / Políticas institucionales (GAP-003) | HIGH | VALID | — |
| Q-079 — Seguridad / Obligaciones de protección (GAP-003) | HIGH | VALID | — |
| Q-080 — Seguridad / Acceso autorizado (GAP-003) | HIGH | VALID | — |
| Q-081 — Seguridad / Restricciones y validación legal (GAP-003) | HIGH | VALID | Incluye `EXTERNAL_VALIDATION_REQUIRED`. |
| Q-082 — Alcance / Funcionamiento correcto (GAP-004) | MEDIUM | VALID | — |
| Q-083 — Alcance / Procesos críticos y errores (GAP-004) | MEDIUM | VALID | — |
| Q-084 — Alcance / Condiciones mínimas de V1 (GAP-004) | MEDIUM | VALID | — |
| Q-085 — Alcance / Patrocinador institucional (GAP-005) | LOW | VALID | — |

---

## 3. Critical Coverage

Cobertura de los ítems críticos del `discovery-audit.md` (UNKNOWN/DECISION/RISK).

| Ítem crítico | Cobertura | Preguntas |
| --- | --- | --- |
| Institución (identidad, tamaño, contexto) | COMPLETE | Q-001, Q-002 |
| Roles y usuarios del sistema (incl. V1) | COMPLETE | Q-003, Q-047, Q-048 |
| Documento maestro de alcance (fuente de verdad) | COMPLETE | Q-070 |
| Procesos y estructura académica (asignaturas, grados, secciones) | COMPLETE | Q-004, Q-015, Q-016, Q-071, Q-072, Q-073 |
| Datos existentes / importación / formato / esquema | COMPLETE | Q-006, Q-007, Q-043, Q-044, Q-045 |
| Estudiantes (identificación, datos, estados, historial) | COMPLETE | Q-008…Q-011 |
| Matrícula (proceso, grados, documentación, reingresos) | COMPLETE | Q-015…Q-018 |
| Encargados (relación, datos, responsabilidades) | COMPLETE | Q-020…Q-022 |
| Asistencia (registro, estados, reglas, correcciones, reportes) | COMPLETE | Q-023…Q-027 |
| Pagos (conceptos, periodicidad, parciales, recibo, anulaciones, historial) | COMPLETE | Q-028…Q-034 |
| Descuentos, becas y exoneraciones | COMPLETE | Q-074…Q-076 |
| Reportes (usados, formato, adicionales, periodicidad) | COMPLETE | Q-035…Q-038 |
| Datos de menores / privacidad / regulación | COMPLETE | Q-051, Q-077…Q-081 |
| Autenticación / credenciales / acceso | COMPLETE | Q-049, Q-050, Q-080 |
| Backups y recuperación | COMPLETE | Q-053…Q-059 |
| Infraestructura / despliegue / conectividad | COMPLETE | Q-060…Q-063 |
| Administración / operación / actualizaciones | COMPLETE | Q-064, Q-066, Q-067 |
| Alcance y prioridad de V1 / estrategia de datos | COMPLETE | Q-068, Q-069 |
| Criterios de aceptación de V1 | COMPLETE | Q-082…Q-084 |
| Patrocinador institucional | COMPLETE | Q-085 |

**Resultado:** sin lagunas críticas de contenido. Todas las funcionalidades V1 de `Vision.md`
(estudiantes, asistencia, pagos, reportes, respaldos, actualización) y las tecnologías
(React/FastAPI/SQLite) están cubiertas a nivel de requerimiento institucional.

---

## 4. Discovery Gaps

| GAP | Descripción | Estado | Preguntas que lo resuelven |
| --- | --- | --- | --- |
| GAP-001 | Asignaturas y su relación con grados/secciones | **RESUELTO** | Q-071, Q-072, Q-073 |
| GAP-002 | Descuentos, becas/exoneraciones y reglas de pago | **RESUELTO** | Q-074, Q-075, Q-076 |
| GAP-003 | Privacidad/cumplimiento de datos (incl. menores) | **RESUELTO** | Q-077…Q-081 |
| GAP-004 | Criterios de aceptación de V1 | **RESUELTO** | Q-082, Q-083, Q-084 |
| GAP-005 | Patrocinador institucional | **RESUELTO** | Q-085 |

**GAPs remanentes:** **0**.

---

## 5. Questions Requiring Refinement

**Ninguna** tras la corrección de trazabilidad (00.3B).

Los **13** IDs previamente `NEEDS_REFINEMENT` (Q-011…Q-015, Q-019…Q-027) fueron corregidos en la sección 4:
cada etiqueta describe ahora el contenido real de su propia pregunta. Verificación realizada:

| ID | Etiqueta en sección 4 (corregida) | Contenido real del dominio | Alineado |
| --- | --- | --- | --- |
| Q-011 | Historial académico del estudiante (qué se conserva) | Estudiantes / Historial | ✅ |
| Q-012 | Proceso de altas y bajas de estudiantes | Estudiantes / Altas y bajas | ✅ |
| Q-013 | Correcciones de información de estudiantes | Estudiantes / Correcciones | ✅ |
| Q-014 | Documentos asociados al estudiante | Estudiantes / Documentos asociados | ✅ |
| Q-015 | Proceso de matrícula y su periodicidad | Matrícula / Proceso y periodicidad | ✅ |
| Q-019 | Matrícula: históricos (matriculados en años anteriores) | Matrícula / Históricos | ✅ |
| Q-020 | Relación estudiante-encargado (uno o múltiples) | Encargados / Relación | ✅ |
| Q-021 | Datos registrados del encargado | Encargados / Datos | ✅ |
| Q-023 | Quién y cuándo registra la asistencia | Asistencia / Quién y cuándo | ✅ |
| Q-024 | Estados posibles de la asistencia (presente, falta, tarde) | Asistencia / Estados posibles | ✅ |
| Q-025 | Reglas de asistencia (tardías, faltas, justificaciones) | Asistencia / Reglas | ✅ |
| Q-026 | Correcciones de la asistencia | Asistencia / Correcciones | ✅ |
| Q-027 | Reportes de asistencia necesarios | Asistencia / Reportes | ✅ |

Además, **Q-063** (Infraestructura / Acceso físico) y **Q-068** (Alcance / Datos en V1) mantienen sus
etiquetas correctas en la sección 3 (Critical), sin residuos en otras secciones de prioridad.

---

## 6. Duplicate or Low-Value Questions

| ID(s) | Tipo | Detalle |
| --- | --- | --- |
| Q-046 | Retirada | Consolidada en Q-003 (usuarios, incl. V1) y Q-048 (responsabilidades). Trazada en el historial. |
| Q-065 | Retirada | `LOW_VALUE` (canal/formato de solicitudes de cambio propio de operación/handover). Aprobación en Q-070, patrocinio en Q-085. Trazada en el historial. |
| Q-051 ↔ Q-077 | Solapamiento parcial (no duplicado) | Q-051 (seguridad/confidencial) y Q-077 (GAP-003, más específico: estudiantes + encargados + acceso). No requieren cambio. |
| Q-049 ↔ Q-063 | Temas próximos (no duplicado) | Acceso físico a PCs/archivos (Q-049) frente a ubicación/despliegue del equipo (Q-063). Distintos. |

**Resultado:** **0** `DUPLICATE` y **0** `LOW_VALUE`.

---

## 7. Missing Evidence

La solicitud de evidencia está correctamente concentrada en la sección 8 del cuestionario, separada de
las preguntas.

| Evidencia requerida | Estado |
| --- | --- |
| Ejemplo anónimo de la planilla de estudiantes (estructura/campos) | SOLICITADA (sección 8) |
| Datos existentes (matrícula, pagos, reportes) — anonimizados | SOLICITADA (sección 8) |
| Formularios de autorización/aviso de privacidad firmados | SOLICITADA (sección 8; GAP-003) |
| Políticas/procedimientos de manejo, retención o privacidad de datos | SOLICITADA (sección 8; GAP-003) |
| Definición/ejemplos de "funciona correctamente" para V1 | SOLICITADA (sección 8; GAP-004) |

**Resultado:** sin faltantes estructurales. Nota de privacidad presente: no se requiere compartir datos
personales identificables; el marcador `EXTERNAL_VALIDATION_REQUIRED` (Q-081) cubre el caso de obligaciones
legales no confirmables por la institución.

---

## 8. Coverage Matrix

| Dominio | Preguntas | Prioridad | GAP | V1 |
| --- | --- | --- | --- | --- |
| 1. Institución | Q-001…Q-005 | CRITICAL/HIGH | — | ✓ |
| 2. Estudiantes | Q-006…Q-014 | CRITICAL/HIGH | — | ✓ |
| 3. Matrícula | Q-015…Q-019, Q-071…Q-073 | CRITICAL/HIGH | GAP-001 | ✓ |
| 4. Encargados | Q-020…Q-022 | CRITICAL/HIGH | — | ✓ |
| 5. Asistencia | Q-023…Q-027 | HIGH | — | ✓ |
| 6. Pagos | Q-028…Q-034, Q-074…Q-076 | CRITICAL/HIGH | GAP-002 | ✓ |
| 7. Reportes | Q-035…Q-038 | HIGH | — | ✓ |
| 8. Documentos | Q-039…Q-042 | HIGH | — | ✓ |
| 9. Datos existentes | Q-043…Q-045 | HIGH/MEDIUM | — | ✓ |
| 10. Usuarios | Q-047…Q-048 | MEDIUM | — | ✓ |
| 11. Seguridad | Q-049…Q-053, Q-077…Q-081 | CRITICAL/HIGH | GAP-003 | ✓ |
| 12. Backup y Restore | Q-054…Q-059 | HIGH/MEDIUM | — | ✓ |
| 13. Infraestructura | Q-060…Q-063 | HIGH/CRITICAL/MEDIUM | — | ✓ |
| 14. Operación y mantenimiento | Q-064, Q-066…Q-067 | MEDIUM/LOW | — | ✓ |
| Alcance / V1 | Q-068…Q-070, Q-082…Q-085 | CRITICAL/HIGH/MEDIUM/LOW | GAP-004, GAP-005 | ✓ |

**Cobertura global:** los **14 dominios** presentes, todos los **GAP-001…GAP-005** resueltos y todas las
funcionalidades V1 cubiertas. **Sin dominios `MISSING`** y **sin GAPs críticos/HIGH sin pregunta asociada**.

---

## 9. Validation Conclusion

### Veredicto final: **DISCOVERY QUESTIONNAIRE READY**

**Diagnóstico:** el único bloqueante de la auditoría anterior (13 etiquetas desplazadas en la sección 4,
Q-011…Q-015 y Q-019…Q-027) fue corregido en el PIPELINE 00.3B y confirmado en esta re-auditoría final. Ya
no existen inconsistencias de identificación/etiqueta, y el resto de métricas (GAPs=0, DUPLICATE=0,
LOW_VALUE=0, cobertura COMPLETA) se mantiene. El cuestionario está listo en su integridad formal para ser
entregado y respondido por la institución.

**Checklist de las 5 validaciones:**
1. **Trazabilidad** — ✅ Q-011…Q-015, Q-019…Q-027, Q-063 y Q-068: cada ID corresponde exactamente con su
   contenido real (sección 4 corregida y verificada; Q-063/Q-068 en Critical con etiquetas correctas).
2. **Integridad** — ✅ 83 IDs únicos; Q-046 y Q-065 retiradas y trazadas; Q-071…Q-085 presentes;
   83/83 respuestas en `PENDING`.
3. **Contenido** — ✅ GAP-001…GAP-005 resueltos con sus preguntas dedicadas.
4. **Cobertura** — ✅ contra `discovery-audit.md`, `Vision.md`, funcionalidades V1 y los 14 dominios:
   sin GAPs críticos/HIGH sin pregunta asociada.
5. **Calidad** — ✅ sin preguntas ambiguas, sin soluciones técnicas implícitas, sin duplicados, sin
   preguntas de bajo valor relevantes y sin contradicciones entre secciones.

**Criterios de éxito (sección 3 del audit) aplicados (todos CUMPLEN):**
1. Preguntas cerradas/abiertas correctas para la institución — **CUMPLE**.
2. Trazabilidad de los UNKNOWN/DECISION_REQUIRED/RISK — **CUMPLE**.
3. Cobertura de funcionalidades V1 — **CUMPLE**.
4. Preguntas privadas y neutrales (sin inducción/solución implícita) — **CUMPLE**.
5. Consistencia interna de IDs y etiquetas — **CUMPLE** (corregido).
6. Exterioridad de la fuente de verdad — **CUMPLE** (Q-070).
7. Sin casos `DUPLICATE`/`LOW_VALUE` — **CUMPLE**.
8. Sin ambigüedad que requiera re-auditoría — **CUMPLE**.

> **DISTINCIÓN IMPORTANTE:** `DISCOVERY QUESTIONNAIRE READY` significa que el **cuestionario** es
> formalmente correcto, completo y trazable, y puede ser entregado a la institución. **NO** significa que
> el proyecto esté listo para Foundation: las respuestas siguen `PENDING` y los dominios siguen `UNKNOWN`
> hasta que la institución responda. El avance a Foundation queda bloqueado hasta completar el Discovery
> institucional.

> **NO se emite `FOUNDATION READY`.** No se avanza de fase.

---

## Anexo A — Historial de auditorías (evidencia conservada)

Se conservan íntegras las auditorías anteriores como evidencia del proceso de corrección.

### A.1 Re-auditoría R2 (PIPELINE 00.3) — Veredicto: NOT READY

Previo a la corrección de trazabilidad 00.3B, la auditoría R2 determinó (resumen preservado):
- Total: 83 preguntas; `VALID`=70, `NEEDS_REFINEMENT`=13, `DUPLICATE`=0, `LOW_VALUE`=0.
- GAPs de contenido: **0** (GAP-001…GAP-005 resueltos en contenido).
- Bloqueante único: **13 etiquetas desplazadas en la sección 4** (Q-011…Q-015, Q-019…Q-027), donde el
  texto de cada etiqueta describía el contenido de otra pregunta (p. ej., Q-011 etiquetada como
  "Documentación requerida para matrícula" [contenido de Q-017]; Q-012 como "Estados" [Q-010]; etc.).
- Q-063/Q-068 correctamente etiquetadas en Critical; restantes secciones (Critical/Medium/Low) consistentes.
- Conclusión R2: **NOT READY** con acción correctiva: corregir la etiqueta de las 13 preguntas de la
  sección 4 y registrar el cambio en la historia de revisión.

### A.2 Corrección 00.3B — Trazabilidad

- Se corrigieron exclusivamente las 13 etiquetas de la sección 4 (Q-011…Q-015, Q-019…Q-027).
- Sin cambios de contenido, prioridades, dominios ni respuestas; sin preguntas añadidas/eliminadas.
- Se registró la entrada en la historia de revisión del cuestionario (sección 10 de
  `institutional-discovery.md`). Responde a la tabla de correspondencia de la sección 5 de R2.

### A.3 Re-auditoría final (R3, este documento) — Veredicto: DISCOVERY QUESTIONNAIRE READY

- Verificadas las 13 correcciones (trazabilidad), la integridad, el contenido (GAPs), la cobertura y la
  calidad. Todos los criterios CUMPLEN. Veredicto: `DISCOVERY QUESTIONNAIRE READY`.
- Sin avance de fase; el proyecto permanece en Discovery hasta obtener respuestas institucionales.

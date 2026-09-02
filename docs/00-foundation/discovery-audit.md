# Discovery Audit

> PIPELINE 00 — Discovery Audit previo a la fase Foundation.
> Este documento registra exclusivamente el **estado real y verificable** del proyecto.
> Clasificaciones usadas: `CONFIRMED`, `UNKNOWN`, `INFERENCE`, `DECISION_REQUIRED`, `RISK`.
> No se ha programado, modificado código ni diseñado solución alguna en esta fase.

---

## 1. Executive Summary

El proyecto **Sistema de Gestión Escolar** se encuentra en un estado **greenfield (en blanco)**.
Existe un único documento sustantivo de visión (`docs/Vision.md`), un archivo vacío (`Agents.md`)
y un conjunto de directorios de estructura planificada pero completamente vacíos
(`backend`, `frontend`, `database`, `backups`, `installers`, `specs`).

No existe código, ni tests, ni configuraciones, ni esquema de base de datos, ni especificaciones
adicionales, ni documentación de procesos institucionales. El repositorio remoto (`origin`) contiene
únicamente un `README.md` sin contenido sustantivo ("# SistemaEscolar").

En consecuencia, **la inmensa mayoría de la información necesaria para Foundation es `UNKNOWN`**.
La visión documentada confirma la intención de tecnología e intención general de funcionalidad,
pero no existe respaldo institucional ni definición de negocio detallada.

**El proyecto NO está listo para Foundation.** Antes de avanzar es indispensable obtener
información institucional, resolver decisiones fundamentales y aclarar ambigüedades del documento
de visión (ver secciones 5, 8 y 10-12).

---

## 2. Confirmed Facts

Hechos respaldados directamente por las fuentes del proyecto (`docs/Vision.md`, estructura del
repositorio, configuración de git).

- `CONFIRMED` — El proyecto se denomina **Sistema de Gestión Escolar**.
- `CONFIRMED` — La aplicación está destinada a **una directora escolar** (rollo singular, no se
  mencionan otros actores).
- `CONFIRMED` — La intención funcional declarada en la visión cubre:
  - Gestionar estudiantes.
  - Registrar asistencia.
  - Gestionar pagos.
  - Generar reportes.
  - Crear respaldos (backups).
  - Actualizar el sistema.
- `CONFIRMED` — Tecnologías declaradas en la visión: **React**, **FastAPI**, **SQLite**.
- `CONFIRMED` — Existen directorios de estructura planificada vacíos:
  `backend`, `frontend`, `database`, `backups`, `installers`, `specs`, `docs`.
- `CONFIRMED` — El contenido del repositorio local consta únicamente de:
  - `docs/Vision.md` (18 líneas, 274 bytes).
  - `Agents.md` (0 bytes, vacío).
- `CONFIRMED` — No existen archivos de código, tests, configuraciones, esquemas, ni especificaciones
  en el repositorio local.
- `CONFIRMED` — El repositorio git local no tiene commits ("No commits yet"); todos los archivos
  están sin seguimiento (untracked).
- `CONFIRMED` — Rama local: `master`. Rama remota por defecto: `main`.
- `CONFIRMED` — El remoto configurado es `https://github.com/Marc02E/SistemaEscolar.git`.
- `CONFIRMED` — El remoto (`origin/main`, commit `fab8f6d`) contiene únicamente un `README.md`
  cuyo contenido es el título "# SistemaEscolar" (sin contenido sustantivo).

---

## 3. Unknowns

Información que actualmente no conocemos y que **no está respaldada por ninguna fuente**.

- `UNKNOWN` — Identidad, datos de contacto y alcance administrativo real de la institución/escuela.
- `UNKNOWN` — Si la directora escolar es el **único** usuario o si existen otros roles
  (docentes, secretaría, personal administrativo, tutores, alumnos).
- `UNKNOWN` — Si existe un "Documento Maestro" formal más allá de la visión (no se encontró).
- `UNKNOWN` — El dominio/contexto educativo concreto (nivel: inicial, primaria, secundaria,
  mixto; número de estudiantes, de grupos/grados, de docentes).
- `UNKNOWN` — Los procesos reales institucionales (inscripción, registro de asignaturas,
  gestión de grupos/cursos, calendario académico, ciclo escolar).
- `UNKNOWN` — Los datos históricos existentes y su formato (¿existen archivos Excel u otros?).
- `UNKNOWN` — Esquema/modelo de datos deseado o esperado.
- `UNKNOWN` — Requisitos de seguridad y autenticación específicos (p. ej., si existe autenticación,
  contraseñas, roles, cifrado de datos personales).
- `UNKNOWN` — Requisitos de privacidad/regulación (p. ej., protección de datos de menores).
- `UNKNOWN` — Requisitos funcionales de asistencia (qué se registra, resúmenes, faltas/justificaciones).
- `UNKNOWN` — Requisitos funcionales de pagos (tipos de pago, moneda, aranceles, morosidad,
  recibos, facturación).
- `UNKNOWN` — Requisitos funcionales de reportes (qué reportes, formatos, destinatarios).
- `UNKNOWN` — Requisitos de backups y restore (frecuencia, destino, retención, interoperabilidad).
- `UNKNOWN` — Requisitos de instalación y despliegue (¿local en la escuela?, ¿nube?, ¿equipo único?).
- `UNKNOWN` — Requisitos de actualización del sistema (qué se actualiza, dónde se aloja el binario).
- `UNKNOWN` — Estrategia de testing y expectativas de calidad.
- `UNKNOWN` — Requisitos UX y navegación no derivados de la visión.
- `UNKNOWN` — Requisitos de importación de datos (formato Excel específico, plantillas, validaciones).
- `UNKNOWN` — Estándares, estilo de código y convenciones del equipo (si los hubiera).
- `UNKNOWN` — Cualquier requerimiento de aceptación/criterios de éxito definidos por la institución.

---

## 4. Inferences

Interpretaciones razonables que **todavía requieren validación institucional**.

- `INFERENCE` — Los directorios vacíos (`backend`, `frontend`, `database`, `backups`, `installers`,
  `specs`) sugieren una arquitectura prevista en capas: frontend React, backend FastAPI, SQLite
  como base de datos, con artefactos de instalación y respaldos. No se ha confirmado si esta
  estructura es vinculante.
- `INFERENCE` — La mención a "instaladores" (`installers`) sugiere un despliegue local/on-premise en
  la escuela, en contraposición a un despliegue exclusivamente en la nube.
- `INFERENCE` — "Gestionar estudiantes" probablemente implica un CRUD con datos personales y de
  contacto del estudiante (y posiblemente de tutores/padres). No confirmado.
- `INFERENCE` — "Registrar asistencia" probablemente implica registro diario por estudiante/clase y
  reportes derivados. No confirmado.
- `INFERENCE` — "Gestionar pagos" probablemente implica cobros, registro de pagos, saldos y deudas.
  No confirmado.
- `INFERENCE` — Las tecnologías React/FastAPI/SQLite sugieren una SPA (Single Page Application) con
  API REST y base de datos relacional embebida. No confirmado como requisito definitivo.
- `INFERENCE` — `Agents.md` (vacío) podría estar destinado a convenciones para agentes de IA, pero
  no contiene información.

> Regla de aplicación: ninguna de estas inferencias constituye un requisito confirmado. Toda
> inferencia debe validarse (sección 8) antes de Foundation.

---

## 5. Decisions Required

Decisiones que deben tomarse antes de continuar. Todas están abiertas y requieren interlocución
institucional o del responsable del proyecto.

- `DECISION_REQUIRED` — ¿`docs/Vision.md` es el "Documento Maestro" definitivo o existe/debe crearse
  un documento maestro más completo con el cliente?
- `DECISION_REQUIRED` — ¿Qué usuarios/roles oficiales existen en el sistema (solo directora vs.
  directora + docentes + secretaría + otros)?
- `DECISION_REQUIRED` — ¿Alcance de la primera versión (MVP): qué funcionalidades se entregan en cada
  iteración y cuál es el orden de prioridad?
- `DECISION_REQUIRED` — ¿Estrategia de datos: el sistema parte de datos existentes (importación) o
  de cero? En caso de existir datos, ¿en qué formato?
- `DECISION_REQUIRED` — ¿Autenticación: se requiere login/contraseñas, roles y control de acceso?
- `DECISION_REQUIRED` — ¿Modelo de pagos: moneda, tipos de aranceles, ciclos de facturación,
  manejo de morosidad/descuentos?
- `DECISION_REQUIRED` — ¿Modelo de reportes: qué reportes concretos, formato de salida (PDF/Excel),
  y quiénes los consumen?
- `DECISION_REQUIRED` — ¿Estrategia de despliegue/instalación: local en la escuela, servidor de la
  escuela, o nube?
- `DECISION_REQUIRED` — ¿Política de backups y restore: frecuencia, ubicación de respaldos,
  retención, y procedimiento de restauración avalado por la institución?
- `DECISION_REQUIRED` — ¿Política de actualizaciones: qué se actualiza, canal de distribución y
  compatibilidad de datos?
- `DECISION_REQUIRED` — ¿Quién es el responsable/patrocinador del proyecto del lado de la institución
  para validar decisiones y procesos?

---

## 6. Contradictions and Ambiguities

- `INFERENCE / DECISION_REQUIRED` — Existe una **discrepancia nominal entre el remoto y el local**:
  la rama local es `master`, mientras que la rama remota por defecto es `main`, y `git` informa
  "No commits yet" en local pese a existir contenido remoto. Ambigüedad de configuración de
  repositorio que debe resolverse (qué rama es la fuente de verdad y cómo se integrarán).
- `DECISION_REQUIRED` — El término "Documento Maestro" del pipeline no corresponde a ningún artefacto
  físico encontrado. La única fuente documental es `docs/Vision.md`. Es ambiguo si la visión es el
  maestro o si falta un documento maestro por crear.
- `INFERENCE` — El `README.md` del remoto dice únicamente "# SistemaEscolar" (solo título), lo que
  no aporta información de negocio pero indica que el repositorio remoto fue inicializado.
- `DECISION_REQUIRED` — La visión lista funcionalidades amplias ("generar reportes", "actualizar el
  sistema") sin detallar la profundidad esperada de cada una; esta falta de granularidad es ambigua
  y exige aclaración.

---

## 7. Risks

Situaciones que pueden comprometer arquitectura, datos, seguridad, operación o mantenimiento.

- `RISK` — **No hay Documento Maestro ni requisitos detallados**: avanzar a Foundation sin fuentes
  de requisitos completas derivaría en diseño especulativo y retrabajo (riesgo alto).
- `RISK` — **Sin validación de procesos institucionales**: diseñar asistencia/pagos/reportes sin
  conocer los procesos reales de la escuela puede generar funciones incorrectas o inutilizables
  (riesgo alto).
- `RISK` — **Tratamiento de datos personales de menores** (estudiantes): sin requisitos de seguridad
  y privacidad definidos, el sistema podría incumplir normativa o exponer datos sensibles (riesgo alto).
- `RISK` — **Riesgo de un solo usuario/no escalado**: la visión menciona solo a la directora;
  silenciar roles adicionales puede limitar el alcance inicial (riesgo medio).
- `RISK` — **Migración/importación de datos sin conocer su formato**: si existen datos históricos en
  Excel y no se especifica estructura, la importación puede fallar o producir datos corruptos
  (riesgo alto).
- `RISK` — **Backups y restore indefinidos**: sin política de respaldo institucional, se arriesga la
  pérdida de datos operativos críticos (riesgo alto).
- `RISK` — **Despliegue/instalación sin infraestructura definida**: la suposición de despliegue local
  no validada podría chocar con el entorno real de la escuela (riesgo medio).
- `RISK` — **Actualizaciones sin canal definido**: sin definir el mecanismo, el mantenimiento a
  largo plazo puede volverse insostenible (riesgo medio).
- `RISK` — **Confusión de ramas `master` vs. `main` y ausencia de commits**: configuración de
  repositorio ambigua que puede causar pérdida de trabajo o integración errónea (riesgo medio/bajo).

---

## 8. Institutional Information Required

Información que **debe obtenerse de la institución** antes de poder diseñar con criterio.

- Existencia y contenido del "Documento Maestro" oficial del proyecto.
- Datos generales de la institución: nivel educativo, tamaño (número de estudiantes, grupos,
  docentes), cantidad de sedes/campus.
- Roles y usuarios oficiales del sistema (¿solo directora u otros?).
- Procesos reales:
  - Inscripción y registro de estudiantes (datos recolectados, documentos).
  - Organización académica (grados/grupos/asignaturas, calendario escolar).
  - Registro de asistencia (qué información se captura, quién la registra, justificaciones/faltas).
  - Proceso de pagos (aranceles, moneda, periodicidad, recibos, manejo de deudas/morosidad, descuentos).
  - Reportes necesarios (lista de reportes, formato de salida, periodicidad, destinatarios).
- Datos existentes: ¿hay registros previos? ¿en qué formato (Excel, papel, otro sistema)? ¿se deben
  importar? ¿qué campos/columnas tienen?
- Requisitos de seguridad y privacidad: ¿se requiere autenticación? ¿manejo de roles? ¿protección de
  datos de menores conforme a normativa aplicable?
- Entorno de despliegue/operación: ¿equipo local en la escuela, servidor propio o nube? ¿hay persona
  técnica de soporte?
- Política de backups y restauración acordada.
- Política de actualización del sistema y canal de mantenimiento.
- Criterios de aceptación / qué constituye una entrega satisfactoria desde la perspectiva institucional.

> Todo lo anterior está `UNKNOWN` o `DECISION_REQUIRED` hasta obtener respuesta institucional.

---

## 9. Existing Project Assets

Inventario de lo reutilizable/ya presente en el proyecto.

- `CONFIRMED` — `docs/Vision.md`: documento de visión (fuente principal y reutilizable).
- `CONFIRMED` — `Agents.md`: archivo presente pero **vacío** (sin contenido aprovechable; se
  reintegrará solo si se define su propósito).
- `CONFIRMED` — Estructura de directorios planificada: `backend`, `frontend`, `database`, `backups`,
  `installers`, `specs`, `docs` (reutilizable como esqueleto de organización del proyecto).
- `CONFIRMED` — Configuración de repositorio git con remoto
  `https://github.com/Marc02E/SistemaEscolar.git` (reutilizable para handover/colaboración).
- `CONFIRMED` — `README.md` en el remoto (contenido mínimo; útil solo como marcador del repositorio).

> No hay código, tests, configuraciones, esquemas ni documentación de negocio adicionales.

---

## 10. Areas Ready for Further Discovery

Áreas donde ya existe un punto de partida suficiente (la visión) para profundizar el descubrimiento
mediante preguntas institucionales.

- Usuarios y roles (a partir de la mención de la "directora escolar"; falta expandir).
- Gestión de estudiantes (declarado en visión; falta detalle).
- Registro de asistencia (declarado; falta detalle).
- Gestión de pagos (declarado; falta detalle).
- Generación de reportes (declarado; falta detalle).
- Respaldos (backups) (declarado; falta detalle).
- Actualización del sistema (declarado; falta detalle).

> Estos dominios están "listos para más descubrimiento" porque la visión los nombra, no porque estén
> definidos.

---

## 11. Areas NOT Ready for Foundation

Dominios que **NO deben diseñarse todavía**, por falta de respaldo informacional.

- Modelo de datos / esquema de base de datos (sin requisitos de datos confirmados).
- Arquitectura definitiva de backend y frontend (más allá de las tecnologías nominales de la visión).
- Seguridad y autenticación (sin requisitos institucionales).
- UX y navegación (sin flujos de usuario aprobados).
- Excel/importación (sin conocer los datos reales y su formato).
- Asistencia (detalle de negocio desconocido).
- Pagos (detalle de negocio, moneda, aranceles y flujos desconocidos).
- Reportes (conjunto y formatos desconocidos).
- Backups y restore (política no definida).
- Instalación y despliegue (entorno no definido).
- Actualizaciones (mecanismo no definido).
- Testing (sin especificación ni criterios de aceptación).
- Continuidad y handover (sin acuerdos de operación ni responsables).

> Fundación de diseño en estos dominios es prematura. `Discovery primero`.

---

## 12. Discovery Conclusion

**¿Qué sabemos?** — El nombre del proyecto, su usuario destinatario declarado (una directora
escolar), la intención funcional general (estudiantes, asistencia, pagos, reportes, respaldos,
actualizaciones), las tecnologías declaradas (React, FastAPI, SQLite), la estructura de directorios
planificada y el estado greenfield del repositorio.

**¿Qué no sabemos?** — Casi todo lo referente al negocio: usuarios/roles, procesos institucionales,
datos existentes, modelo de datos, seguridad, requisitos de asistencia/pagos/reportes, entorno de
despliegue, políticas de respaldo, actualización, testing y handover. Todo esto está `UNKNOWN`.

**¿Qué estamos suponiendo?** — Que la estructura de carpetas implica una arquitectura en capas, que
"instaladores" implica despliegue local, y que los términos funcionales implican ciertos flujos;
todas inferencias sin confirmar.

**¿Qué debemos preguntarle a la institución?** — Toda la sección 8: documento maestro oficial,
datos institucionales, roles, procesos reales, datos existentes, requisitos de seguridad, entorno,
políticas y criterios de aceptación.

**¿Qué decisiones debemos tomar?** — Las de la sección 5 (alcance, roles, MVP, data, seguridad,
pagos, reportes, despliegue, respaldos, actualizaciones, responsable institucional).

**¿Estamos listos para Foundation?** — **NO.** El proyecto carece de un Documento Maestro formal,
de requisitos institucionales confirmados y de la mayoría de la información de negocio. Avanzar a
Foundation en este estado implicaría diseñar sobre suposiciones (riesgo alto de retrabajo).

**Estado global:** greenfield. La incertidumbre dominante es el dominio de negocio. La acción
siguiente correcta es **Discovery institucional**, no Foundation.

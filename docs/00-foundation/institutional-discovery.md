# Institutional Discovery

> PIPELINE 00.2 — Cuestionario estructurado para la institución.
> Documento instrumento para entrevistar a la institución y eliminar incertidumbres del proyecto.
> Elaborado a partir de `docs/00-foundation/discovery-audit.md` y `docs/Vision.md`.
> **Revisión 2** — corregido según `docs/00-foundation/discovery-validation.md`.
> Ninguna pregunta ha sido respondida: todas se documentan como `PENDING`.
> Este documento NO diseña soluciones, arquitectura ni base de datos.

---

## 1. Purpose

El objetivo de este cuestionario es **descubrir cómo trabaja actualmente la institución** y qué
requiere realmente del sistema que se llamará Sistema de Gestión Escolar.

Hoy el proyecto está en estado greenfield: la única fuente disponible es una visión breve
(`docs/Vision.md`) que menciona la intención de gestionar estudiantes, registrar asistencia,
gestionar pagos, generar reportes, crear respaldos y actualizar el sistema. No se conoce nada del
entorno real: institución, procesos, datos, usuarios, seguridad o infraestructura.

Este cuestionario convierte los vacíos (`UNKNOWN`) y decisiones pendientes
(`DECISION_REQUIRED`) detectados en el Discovery Audit en **preguntas concretas y accionables**
que una persona de la institución puede responder para orientar un diseño correcto.

Esta revisión incorpora las correcciones resultantes de la auditoría
(`docs/00-foundation/discovery-validation.md`): se resolvieron inconsistencias de identificación,
se reformularon preguntas problemáticas, se agregaron preguntas para los vacíos (GAPs)
identificados y se consolidó/eliminó lo duplicado o de bajo valor. Ver `Revision History`
(sección 10).

Cada pregunta indica por qué se formula y qué impacto tiene si la respuesta se desconoce. Todas
deben responder los responsables institucionales con la evidencia correspondiente (ver sección 8).

---

## 2. Instructions for the Institution

Gracias por participar. Antes de responder, tenga en cuenta:

- **Responda con sus propias palabras.** No necesita lenguaje técnico; describa cómo trabaja
  realmente la institución hoy.
- **No adivine.** Si algo no aplica o no sabe la respuesta, escríbalo así; es preferible decir
  "no aplica" o "no sé" a inventar una respuesta.
- **Indique la persona que responde** en cada dominio (o al inicio del cuestionario) y su cargo,
  para saber a quién consultar en caso de dudas posteriores.
- **Si una pregunta describe un proceso que usted no realiza**, indique quién lo realiza.
- **Algunas preguntas pueden no aplicar** (por ejemplo, sobre asignaturas, descuentos, becas o
  políticas de datos). Si algo no existe en la institución, responde simplemente "no aplica"; no se
  asume que todas las instituciones manejan lo mismo.
- **Adjunte evidencia cuando la tenga** (formatos, capturas, plantillas de Excel, recibos,
  formularios, reportes, procedimientos escritos). Vea la sección 8 para saber qué se necesita.
- **La prioridad de cada pregunta** (CRITICAL / HIGH / MEDIUM / LOW) indica cuánto afecta la
  respuesta a la definición del sistema; responda primero las CRITICAL y HIGH.
- Se puede responder en varias sesiones; no es necesario completarlo de corrido.

---

## 3. Critical Questions

Preguntas cuya respuesta puede cambiar el modelo de dominio, los procesos, la arquitectura, la
seguridad, la persistencia, la migración de datos o el alcance de V1.

- Q-001 — Datos generales de la institución (nivel educativo, tamaño, número de sedes).
- Q-003 — Roles y usuarios oficiales del sistema (¿solo la directora u otros?).
- Q-004 — Visión general del orden de los procesos del año (matrícula, asistencia, cobros, reportes).
- Q-006 — ¿Existen registros actuales de estudiantes? (datos históricos / importación).
- Q-007 — Estructura (campos) de la hoja/planilla donde se registran los estudiantes.
- Q-008 — Identificación oficial única de un estudiante.
- Q-010 — Estados del estudiante a lo largo de su ciclo.
- Q-016 — Grados y secciones (estructura académica).
- Q-017 — Documentación y validaciones exigidas para la matrícula.
- Q-018 — Reingresos y traslados.
- Q-022 — Responsabilidades y acceso del encargado.
- Q-028 — Conceptos cobrados (aranceles, cuotas) y moneda.
- Q-030 — Pagos parciales, saldos y deudas.
- Q-033 — Anulaciones/correcciones de pagos.
- Q-051 — Información considerada confidencial/protegida.
- Q-063 — Ubicación y condiciones de acceso físico del equipo (despliegue).
- Q-068 — ¿V1 parte de datos existentes o de cero? (estrategia de datos).
- Q-070 — ¿La visión es el documento maestro definitivo? / responsable de aprobación.

---

## 4. High Priority Questions

- Q-002 — Número aproximado de estudiantes y personal involucrado.
- Q-005 — Ciclo académico (calendario, fechas, periodos).
- Q-009 — Datos personales del estudiante que se registran y cuáles son obligatorios.
- Q-011 — Historial académico del estudiante (qué se conserva).
- Q-012 — Proceso de altas y bajas de estudiantes.
- Q-013 — Correcciones de información de estudiantes.
- Q-014 — Documentos asociados al estudiante.
- Q-015 — Proceso de matrícula y su periodicidad.
- Q-019 — Matrícula: situación de estudiantes matriculados en años anteriores (históricos).
- Q-020 — Relación estudiante-encargado (uno o múltiples).
- Q-021 — Datos registrados del encargado.
- Q-023 — Quién y cuándo registra la asistencia.
- Q-024 — Estados posibles de la asistencia (presente, falta, tarde).
- Q-025 — Reglas de asistencia (llegadas tardías, faltas, justificaciones).
- Q-026 — Correcciones de la asistencia.
- Q-027 — Reportes de asistencia necesarios.
- Q-029 — Periodicidad y vencimientos de cobros.
- Q-031 — Forma de pago recibida actualmente (efectivo, transferencia, otro).
- Q-032 — Emisión de recibos/constancias de pago.
- Q-034 — Historial de pagos (qué se conserva y por cuánto tiempo).
- Q-035 — Reportes actualmente usados (detalle).
- Q-036 — Formato/salida de los reportes (papel, PDF, Excel).
- Q-037 — Reportes adicionales necesarios pero no disponibles hoy.
- Q-038 — Periodicidad y destinatarios de cada reporte.
- Q-039 — Dónde se guardan los documentos (papel, digital, ubicación).
- Q-040 — Formatos de los documentos almacenados.
- Q-041 — Quién accede a los documentos.
- Q-042 — Tiempo de retención de los documentos/registros.
- Q-043 — Datos existentes en Excel u otros archivos (inventario).
- Q-049 — Acceso físico a las computadoras/archivos.
- Q-050 — Manejo de credenciales hoy (perfiles, contraseñas, acceso compartido).
- Q-052 — ¿Se requiere registrar quién hizo cada cambio (auditoría)?
- Q-053 — Necesidad de recuperación ante pérdida de datos (severidad/tiempo).
- Q-054 — Qué debe respaldarse.
- Q-055 — Frecuencia esperada de respaldo.
- Q-059 — Protocolo ante un incidente/fallo del sistema.
- Q-060 — Computadora/s disponible y sistema operativo.
- Q-061 — Disponibilidad de internet y su efecto en el trabajo diario.
- Q-069 — Prioridad de funciones para V1 (qué se entrega primero).
- Q-071 — Asignaturas o materias y su relación con grados/secciones (GAP-001).
- Q-072 — ¿El sistema debe registrar asignaturas o solo grado/sección? (GAP-001).
- Q-073 — ¿Asistencia y reportes se organizan por asignatura, grado/sección o ambos? (GAP-001).
- Q-074 — Descuentos en los pagos (GAP-002).
- Q-075 — Becas o exoneraciones de pago (GAP-002).
- Q-076 — Reglas de aplicación de descuentos/becas (GAP-002).
- Q-077 — Información confidencial de estudiantes y encargados (GAP-003).
- Q-078 — Políticas institucionales sobre datos (GAP-003).
- Q-079 — Obligaciones/procedimientos de protección de datos existentes (GAP-003).
- Q-080 — Quién está autorizado a acceder a la información (GAP-003).
- Q-081 — Restricciones sobre guardar/compartir datos (GAP-003).

---

## 5. Medium Priority Questions

- Q-044 — Calidad de los datos existentes (duplicados, incompletos, desactualizados).
- Q-045 — Fuente oficial de los datos.
- Q-047 — Posibles usuarios futuros del sistema (escalabilidad).
- Q-048 — Responsabilidades por usuario/rol.
- Q-056 — Destinos disponibles para guardar respaldos.
- Q-057 — Responsable de los respaldos.
- Q-058 — Procedimiento esperado de restauración ante fallo.
- Q-062 — Restricciones técnicas/regulatorias de la infraestructura.
- Q-064 — Quién administrará el sistema a diario.
- Q-082 — Qué significa "funciona correctamente" para la institución (GAP-004).
- Q-083 — Procesos críticos y errores inaceptables (GAP-004).
- Q-084 — Condiciones mínimas para aceptar la primera versión (GAP-004).

---

## 6. Low Priority Questions

- Q-066 — Qué ocurre si el desarrollador original no está disponible.
- Q-067 — Expectativas de actualización y mantenimiento del sistema.
- Q-085 — Responsable/patrocinador institucional del proyecto (GAP-005).

---

## 7. Questions by Domain

### 1. Institución

#### Q-001 — Institución / Contexto
**Dominio:** Institución — Contexto operativo.
**Pregunta:** ¿Cuál es el nombre oficial de la institución, su nivel educativo (por ejemplo, inicial,
primaria, secundaria, mixto) y cuántas sedes o campus tiene?
**Por qué necesitamos saberlo:** Para dimensionar el alcance del sistema y conocer el contexto en el
que operará.
**Impacto si no se conoce:** `UNKNOWN` → Riesgo de diseñar un sistema a escala incorrecta o con
supuestos de nivel educativo equivocados.
**Respuesta:** `PENDING`

#### Q-002 — Institución / Tamaño
**Dominio:** Institución — Personal y dimensión.
**Pregunta:** ¿Cuántos estudiantes tiene aproximadamente la institución y cuántas personas participan
en la gestión (directora, docentes, secretaría, administración, otros)?
**Por qué necesitamos saberlo:** Determina la escala de datos, el número probable de usuarios y la
complejidad de la gestión diaria.
**Impacto si no se conoce:** `UNKNOWN` → No es posible dimensionar rendimiento, volúmenes ni usuarios.
**Respuesta:** `PENDING`

#### Q-003 — Institución / Usuarios del sistema
**Dominio:** Institución — Personal involucrado.
**Pregunta:** ¿Quién usará el sistema (incluida la primera versión)? ¿Solo la directora, o también
docentes, secretaría, personal administrativo u otros? Indique quién realizará cada tarea.
**Por qué necesitamos saberlo:** Define los roles y permisos del sistema y qué actividades necesita
soportar; consolida la información de quién usa el sistema y quién lo hará en V1.
**Impacto si no se conoce:** `UNKNOWN` → Riesgo de omitir roles o funcionalidades necesarias en V1.
**Respuesta:** `PENDING`

#### Q-004 — Institución / Vista de procesos
**Dominio:** Institución — Procesos de negocio.
**Pregunta:** En general, ¿en qué orden se realizan durante el año la matrícula, el registro de
asistencia, los cobros de pagos y la generación de reportes? Solo necesita darme una visión general;
más adelante preguntaré el detalle de cada proceso.
**Por qué necesitamos saberlo:** Confirma el orden y la secuencia de los procesos sin pedir un flujo
extenso que ya se aborda en las preguntas específicas (Q-015, Q-023, Q-031, Q-035).
**Impacto si no se conoce:** `UNKNOWN` → Riesgo de diseñar procesos en un orden o con dependencias
incorrectos.
**Respuesta:** `PENDING`

#### Q-005 — Institución / Ciclo académico
**Dominio:** Institución — Ciclo académico.
**Pregunta:** ¿Cuáles son las fechas del ciclo académico? ¿En qué fechas inicia y termina el ciclo,
cuántos periodos/meses tiene el año escolar, y hay fechas clave (inicio de clases, vacaciones, cierre)?
**Por qué necesitamos saberlo:** El ciclo afecta matrícula, asistencia, cobros y reportes.
**Impacto si no se conoce:** `UNKNOWN` → No es posible modelar periodos ni calendarios del sistema.
**Respuesta:** `PENDING`

---

### 2. Estudiantes

#### Q-006 — Estudiantes / Datos existentes
**Dominio:** Estudiantes / Datos existentes.
**Pregunta:** ¿Existen actualmente registros de estudiantes en algún formato (Excel, papeles, otro
sistema)? ¿Cuántos y en qué forma se guardan?
**Por qué necesitamos saberlo:** Determina si V1 debe importar datos o partir de cero, y condiciona la
migración.
**Impacto si no se conoce:** `UNKNOWN` → Riesgo alto de fracaso de migración o de no cubrir la
necesidad real.
**Respuesta:** `PENDING`

#### Q-007 — Estudiantes / Estructura de la planilla
**Dominio:** Estudiantes / Datos existentes.
**Pregunta:** ¿Existe una hoja, planilla o archivo donde actualmente se registren los estudiantes (por
ejemplo, un documento de Excel o un cuaderno)? Si existe, ¿qué datos incluye por estudiante (por
ejemplo, nombre, documento, grado, contacto)?
**Por qué necesitamos saberlo:** Determina la estructura de datos existente que el sistema deberá
conservar o importar. La solicitud del ejemplo anónimo se realiza en la sección de evidencia
(sección 8), no aquí.
**Impacto si no se conoce:** `UNKNOWN` → Estructura de datos especulativa y migración riesgosa.
**Respuesta:** `PENDING`

#### Q-008 — Estudiantes / Identificación oficial
**Dominio:** Estudiantes — Identificación.
**Pregunta:** ¿Qué documento o campo sirve para identificar de forma única a un estudiante (por
ejemplo, un número de identidad, un código interno, o el nombre completo)? ¿Existe algún caso de dos
estudiantes con el mismo nombre?
**Por qué necesitamos saberlo:** Define la clave de identidad y cómo evitar duplicados.
**Impacto si no se conoce:** `UNKNOWN` → Riesgo de datos duplicados y errores de identificación.
**Respuesta:** `PENDING`

#### Q-009 — Estudiantes / Datos personales
**Dominio:** Estudiantes — Datos personales.
**Pregunta:** ¿Qué datos personales de un estudiante registran actualmente (por ejemplo, nombre,
fecha de nacimiento, dirección, contacto, otro) y cuáles consideran obligatorios para matricularlo?
**Por qué necesitamos saberlo:** Define exactamente los campos del estudiante y cuáles son requeridos.
**Impacto si no se conoce:** `UNKNOWN` → Campos incorrectos o incompletos en el modelo.
**Respuesta:** `PENDING`

#### Q-010 — Estudiantes / Estados
**Dominio:** Estudiantes — Estados del estudiante.
**Pregunta:** ¿Qué estados atraviesa un estudiante a lo largo de su tiempo en la institución (por
ejemplo, activo, retirado, egresado, trasladado, de baja)? ¿Quién decide y registra cada estado?
**Por qué necesitamos saberlo:** Define estados de ciclo de vida y transiciones de datos.
**Impacto si no se conoce:** `UNKNOWN` → No se modelan estados ni historial correctamente.
**Respuesta:** `PENDING`

#### Q-011 — Estudiantes / Historial
**Dominio:** Estudiantes — Historial.
**Pregunta:** ¿Qué información histórica de un estudiante debe conservarse pese a haber terminado su
paso por la institución (por ejemplo, ciclo cursado, estado, fechas)?
**Por qué necesitamos saberlo:** Determina qué mantener tras la baja/egreso y la retención de datos.
**Impacto si no se conoce:** `UNKNOWN` → Pérdida de información histórica útil o retención excesiva.
**Respuesta:** `PENDING`

#### Q-012 — Estudiantes / Altas y bajas
**Dominio:** Estudiantes — Altas y bajas.
**Pregunta:** ¿Cómo se da de alta a un estudiante nuevo y cómo se da de baja a uno que se retira?
¿Quién lo autoriza y qué datos deben registrarse en ese momento?
**Por qué necesitamos saberlo:** Define los flujos de alta/baja y quién puede ejecutarlos.
**Impacto si no se conoce:** `UNKNOWN` → Procesos de alta/baja mal soportados.
**Respuesta:** `PENDING`

#### Q-013 — Estudiantes / Correcciones
**Dominio:** Estudiantes — Correcciones de información.
**Pregunta:** ¿Con qué frecuencia corrigen o actualizan los datos de un estudiante (por ejemplo,
dirección, teléfono, nombre mal escrito) y quién autoriza la corrección?
**Por qué necesitamos saberlo:** Define si se requiere control/auditoría al editar datos.
**Impacto si no se conoce:** `UNKNOWN` → Edición sin control puede corromper datos.
**Respuesta:** `PENDING`

#### Q-014 — Estudiantes / Documentos asociados
**Dominio:** Estudiantes / Documentos.
**Pregunta:** ¿Qué documentos o papeles de un estudiante deben conservarse (por ejemplo, acta de
nacimiento, comprobante de pago, formulario de inscripción, otros) y dónde se guardan hoy?
**Por qué necesitamos saberlo:** Determina si el sistema debe almacenar documentos y en qué formato.
**Impacto si no se conoce:** `UNKNOWN` → Puede omitirse una necesidad central de la institución.
**Respuesta:** `PENDING`

---

### 3. Matrícula

#### Q-015 — Matrícula / Proceso y periodicidad
**Dominio:** Matrícula — Proceso actual.
**Pregunta:** ¿Cuál es el proceso actual de matrícula? ¿Con qué periodicidad se realiza (una vez al
año, por periodo, continua) y en qué fechas?
**Por qué necesitamos saberlo:** Define el flujo y el calendario de matrícula.
**Impacto si no se conoce:** `UNKNOWN` → No se modela el proceso de matrícula correctamente.
**Respuesta:** `PENDING`

#### Q-016 — Matrícula / Grados y secciones
**Dominio:** Matrícula — Grados/Secciones.
**Pregunta:** ¿Cuáles son los grados y secciones que existen (por ejemplo, grados A/B/C, niveles) y
cómo se asigna un estudiante a un grado/sección?
**Por qué necesitamos saberlo:** Define la estructura académica usada en matrícula, asistencia y reportes.
**Impacto si no se conoce:** `UNKNOWN` → Modelo organizativo académico incorrecto.
**Respuesta:** `PENDING`

#### Q-017 — Matrícula / Documentación
**Dominio:** Matrícula — Documentación.
**Pregunta:** ¿Qué documentos se exigen al matricular a un estudiante y qué debe comprobarse antes de
aceptar la matrícula?
**Por qué necesitamos saberlo:** Define requisitos de validación de la matrícula.
**Impacto si no se conoce:** `UNKNOWN` → Controles de matrícula incompletos.
**Respuesta:** `PENDING`

#### Q-018 — Matrícula / Reingresos y traslados
**Dominio:** Matrícula — Reingresos/Traslados.
**Pregunta:** ¿Cómo manejan los reingresos (un estudiante que vuelve) y los traslados (entrada o
salida hacia otra institución)? ¿Se conserva su historial?
**Por qué necesitamos saberlo:** Define flujos especiales y continuidad del historial.
**Impacto si no se conoce:** `UNKNOWN` → Casos frecuentes no soportados.
**Respuesta:** `PENDING`

#### Q-019 — Matrícula / Históricos
**Dominio:** Matrícula — Históricos.
**Pregunta:** ¿Necesitan conservar el historial de matrículas de años anteriores de cada estudiante
y consultarlo? ¿Por cuánto tiempo?
**Por qué necesitamos saberlo:** Define persistencia de históricos de matrícula.
**Impacto si no se conoce:** `UNKNOWN` → Datos históricos perdidos o irrelevantes.
**Respuesta:** `PENDING`

#### Q-071 — Matrícula / Asignaturas (GAP-001)
**Dominio:** Matrícula — Asignaturas.
**Prioridad:** HIGH
**Pregunta:** ¿Existen asignaturas o materias específicas que se enseñen en la institución? Si es así,
¿puede enumerarlas y, en la medida que corresponda, indicar a qué grado o sección pertenece cada una?
**Por qué necesitamos saberlo:** El Discovery Audit registra como desconocido el registro de
asignaturas y la organización académica; no se asume que todas las instituciones manejan las mismas
asignaturas.
**Impacto si no se conoce:** `UNKNOWN` → Modelo académico incorrecto si se asumen asignaturas o su
relación con los grados.
**Respuesta:** `PENDING`

#### Q-072 — Matrícula / Asignaturas (GAP-001)
**Dominio:** Matrícula — Asignaturas.
**Prioridad:** HIGH
**Pregunta:** ¿El sistema debe registrar las asignaturas de cada grado/sección, o solo basta con
registrar el grado y la sección de cada estudiante?
**Por qué necesitamos saberlo:** Define si las asignaturas forman parte del modelo de datos, sin
presuponer que son necesarias.
**Impacto si no se conoce:** `UNKNOWN` → El modelo de datos podría incluir o excluir asignaturas de
forma incorrecta.
**Respuesta:** `PENDING`

#### Q-073 — Matrícula / Asignaturas (GAP-001)
**Dominio:** Matrícula — Asignaturas.
**Prioridad:** HIGH
**Pregunta:** La asistencia y los reportes, ¿se organizan por asignatura, por grado/sección, o por
ambos?
**Por qué necesitamos saberlo:** Determina el nivel de detalle de asistencia y reportes.
**Impacto si no se conoce:** `UNKNOWN` → Asistencia y reportes con granularidad incorrecta.
**Respuesta:** `PENDING`

---

### 4. Encargados

#### Q-020 — Encargados / Relación
**Dominio:** Encargados — Relación estudiante-encargado.
**Pregunta:** ¿Quién es el encargado o responsable de cada estudiante (padre, madre, tutor, otro)?
¿Un estudiante puede tener más de un encargado?
**Por qué necesitamos saberlo:** Define si se modelan uno o varios encargados por estudiante.
**Impacto si no se conoce:** `UNKNOWN` → Modelo de encargados incorrecto.
**Respuesta:** `PENDING`

#### Q-021 — Encargados / Datos
**Dominio:** Encargados — Datos registrados.
**Pregunta:** ¿Qué datos registran de cada encargado (por ejemplo, nombre, teléfono, correo,
dirección, parentesco)? ¿Cuáles son obligatorios?
**Por qué necesitamos saberlo:** Define campos y requisitos del encargado.
**Impacto si no se conoce:** `UNKNOWN` → Campos de contacto incompletos.
**Respuesta:** `PENDING`

#### Q-022 — Encargados / Responsabilidades
**Dominio:** Encargados — Responsabilidades.
**Pregunta:** ¿Qué responsabilidades tiene el encargado ante la institución (por ejemplo, pagos,
asistencia, comunicaciones, retiro del estudiante)? ¿Debe dársele acceso al sistema o solo a datos?
**Por qué necesitamos saberlo:** Determina si el encargado interactúa con el sistema.
**Impacto si no se conoce:** `UNKNOWN` → Rol de encargado mal definido.
**Respuesta:** `PENDING`

---

### 5. Asistencia

#### Q-023 — Asistencia / Quién y cuándo
**Dominio:** Asistencia — Registro.
**Pregunta:** ¿Quién registra la asistencia y en qué momento del día se hace (entrada, cada clase,
fin de jornada)? ¿Es por estudiante o por grupo?
**Por qué necesitamos saberlo:** Define quién usa la función de asistencia y cuándo.
**Impacto si no se conoce:** `UNKNOWN` → Asistencia mal diseñada para el flujo real.
**Respuesta:** `PENDING`

#### Q-024 — Asistencia / Estados posibles
**Dominio:** Asistencia — Estados.
**Pregunta:** ¿Qué estados de asistencia usan (presente, ausente, tardanza, permiso, justificado,
otro)? ¿Cómo se representa a un estudiante que no asiste?
**Por qué necesitamos saberlo:** Define el conjunto de estados de asistencia.
**Impacto si no se conoce:** `UNKNOWN` → Categorías de asistencia incompletas.
**Respuesta:** `PENDING`

#### Q-025 — Asistencia / Reglas
**Dominio:** Asistencia — Reglas de negocio.
**Pregunta:** ¿Qué reglas aplican a la asistencia (llegada tardía a partir de cuántos minutos, límite
de faltas, cómo se justifica una falta y quién autoriza la justificación)?
**Por qué necesitamos saberlo:** Define lógica de negocio de asistencia.
**Impacto si no se conoce:** `UNKNOWN` → Reglas incorrectas o inexistentes.
**Respuesta:** `PENDING`

#### Q-026 — Asistencia / Correcciones
**Dominio:** Asistencia — Correcciones.
**Pregunta:** ¿Con qué frecuencia necesitan corregir o modificar una asistencia registrada por error
y quién autoriza la corrección?
**Por qué necesitamos saberlo:** Define si se requiere edición controlada de asistencia.
**Impacto si no se conoce:** `UNKNOWN` → Correcciones sin control o imposibles.
**Respuesta:** `PENDING`

#### Q-027 — Asistencia / Reportes
**Dominio:** Asistencia — Reportes.
**Pregunta:** ¿Qué reportes de asistencia necesitan (por ejemplo, resumen mensual por estudiante, por
grupo, total de faltas) y quién los usa?
**Por qué necesitamos saberlo:** Define reportes de asistencia necesarios.
**Impacto si no se conoce:** `UNKNOWN` → Reportes de asistencia no cubiertos.
**Respuesta:** `PENDING`

---

### 6. Pagos

#### Q-028 — Pagos / Conceptos
**Dominio:** Pagos — Conceptos cobrados.
**Pregunta:** ¿Qué conceptos se cobran a los estudiantes (por ejemplo, matrícula, mensualidad,
cuotas, uniformes, otros) y en qué moneda?
**Por qué necesitamos saberlo:** Define los conceptos de cobro y la moneda del sistema.
**Impacto si no se conoce:** `UNKNOWN` → Modelo de pagos incorrecto.
**Respuesta:** `PENDING`

#### Q-029 — Pagos / Periodicidad
**Dominio:** Pagos — Periodicidad.
**Pregunta:** ¿Con qué periodicidad se cobra cada concepto (mensual, trimestral, anual, único)?
¿Hay fechas límite de pago?
**Por qué necesitamos saberlo:** Define la periodicidad y los vencimientos de cobros.
**Impacto si no se conoce:** `UNKNOWN` → Cobros y vencimientos mal modelados.
**Respuesta:** `PENDING`

#### Q-030 — Pagos / Parciales y saldos
**Dominio:** Pagos — Pagos parciales/Saldos.
**Pregunta:** ¿Permiten pagos parciales de un concepto, abonos, o solo pagos completos? ¿Cómo manejan
los saldos o deudas pendientes de un estudiante?
**Por qué necesitamos saberlo:** Define el manejo de abonos y saldos.
**Impacto si no se conoce:** `UNKNOWN` → Saldos y abonos mal gestionados.
**Respuesta:** `PENDING`

#### Q-031 — Pagos / Forma de pago
**Dominio:** Pagos — Forma de pago.
**Pregunta:** ¿Cómo se reciben los pagos hoy (efectivo, transferencia, tarjeta, otro) y quién los
recibe y registra?
**Por qué necesitamos saberlo:** Define cómo se ingresa y registra el pago.
**Impacto si no se conoce:** `UNKNOWN` → Flujo de cobro mal soportado.
**Respuesta:** `PENDING`

#### Q-032 — Pagos / Recibos
**Dominio:** Pagos — Recibos.
**Pregunta:** ¿Emiten recibos, comprobantes o constancias de pago a los encargados? ¿Con qué
formato (papel, digital) y qué datos deben tener?
**Por qué necesitamos saberlo:** Define la emisión de recibos y sus campos.
**Impacto si no se conoce:** `UNKNOWN` → Necesidad de recibos no cubierta.
**Respuesta:** `PENDING`

#### Q-033 — Pagos / Anulaciones
**Dominio:** Pagos — Anulaciones.
**Pregunta:** ¿Cómo manejan una anulación o corrección de un pago registrado por error, y quién lo
autoriza?
**Por qué necesitamos saberlo:** Define el control de anulaciones de pagos.
**Impacto si no se conoce:** `UNKNOWN` → Pagos mal anulados sin control.
**Respuesta:** `PENDING`

#### Q-034 — Pagos / Historial
**Dominio:** Pagos — Historial.
**Pregunta:** ¿Qué historial de pagos de un estudiante debe conservarse y por cuánto tiempo (por
ejemplo, todos los años o solo el ciclo actual)?
**Por qué necesitamos saberlo:** Define retención y consulta del historial de pagos.
**Impacto si no se conoce:** `UNKNOWN` → Historial insuficiente o excesivo.
**Respuesta:** `PENDING`

#### Q-074 — Pagos / Descuentos (GAP-002)
**Dominio:** Pagos — Descuentos.
**Prioridad:** HIGH
**Pregunta:** ¿Otorgan descuentos en los pagos a algunos estudiantes (por ejemplo, un porcentaje menor,
un monto fijo, o solo sobre ciertos conceptos)?
**Por qué necesitamos saberlo:** El Discovery Audit cita "descuentos" como decisión pendiente del
modelo de pagos; no se asume que existan.
**Impacto si no se conoce:** `UNKNOWN` → Modelo de cobro y saldo incorrecto si existen descuentos.
**Respuesta:** `PENDING`

#### Q-075 — Pagos / Becas y exoneraciones (GAP-002)
**Dominio:** Pagos — Becas y exoneraciones.
**Prioridad:** HIGH
**Pregunta:** ¿Otorgan becas o exoneraciones de pago (total o parcial) a algunos estudiantes? ¿Cómo se
deciden y quién las autoriza?
**Por qué necesitamos saberlo:** Define si existen becas/exoneraciones y su autorización, para modelar
el saldo correctamente.
**Impacto si no se conoce:** `UNKNOWN` → Deudas y saldos mal calculados al no contemplar becas.
**Respuesta:** `PENDING`

#### Q-076 — Pagos / Reglas de descuentos (GAP-002)
**Dominio:** Pagos — Reglas de descuentos.
**Prioridad:** HIGH
**Pregunta:** Si se aplica un descuento, beca o exoneración, ¿qué reglas se siguen (por ejemplo, un
solo descuento a la vez, sobre qué monto, y cómo afecta el saldo final que debe pagar el estudiante)?
**Por qué necesitamos saberlo:** Captura las reglas de negocio de los descuentos sin diseñar la solución.
**Impacto si no se conoce:** `UNKNOWN` → Reglas de cálculo de pago y saldo incorrectas.
**Respuesta:** `PENDING`

---

### 7. Reportes

#### Q-035 — Reportes / Actualmente usados
**Dominio:** Reportes — Uso actual.
**Pregunta:** ¿Qué listados o reportes produce la institución hoy (por ejemplo, listas de estudiantes,
reportes de asistencia, cobros, deudas, egresados)? ¿Cómo los generan actualmente (a mano, en Excel)?
**Por qué necesitamos saberlo:** Identifica reportes reales ya en uso para no inventarlos.
**Impacto si no se conoce:** `UNKNOWN` → Reportes irreales o faltantes.
**Respuesta:** `PENDING`

#### Q-036 — Reportes / Formato de salida
**Dominio:** Reportes — Formato.
**Pregunta:** ¿En qué formato necesitan los reportes (impresos en papel, PDF, Excel, pantalla) y es
necesario exportarlos/ imprimirlos?
**Por qué necesitamos saberlo:** Define formato y exportación de salida.
**Impacto si no se conoce:** `UNKNOWN` → Formato de salida incorrecto.
**Respuesta:** `PENDING`

#### Q-037 — Reportes / Adicionales
**Dominio:** Reportes — Necesidades.
**Pregunta:** ¿Qué información desearían consultar o imprimir que hoy no pueden obtener con facilidad?
**Por qué necesitamos saberlo:** Identifica reportes de valor real sin imponerlos como requisito.
**Impacto si no se conoce:** `UNKNOWN` → Oportunidades de mejora no detectadas.
**Respuesta:** `PENDING`

#### Q-038 — Reportes / Periodicidad y destinatarios
**Dominio:** Reportes — Periodicidad/Destinatarios.
**Pregunta:** ¿Con qué frecuencia se genera cada reporte y quiénes lo reciben o consultan (directora,
docentes, encargados, otras autoridades)?
**Por qué necesitamos saberlo:** Define frecuencia, destinatarios y permisos de los reportes.
**Impacto si no se conoce:** `UNKNOWN` → Reportes con alcance o audiencia equivocados.
**Respuesta:** `PENDING`

---

### 8. Documentos

#### Q-039 — Documentos / Qué se almacena
**Dominio:** Documentos — Contenido.
**Pregunta:** ¿Qué documentos o papeles maneja y necesita conservar la institución (matrículas, actas
de nacimiento, comprobantes de pago, comunicaciones, otras)? ¿Quiere guardarlos dentro del sistema?
**Por qué necesitamos saberlo:** Determina si el sistema almacena documentos digitales.
**Impacto si no se conoce:** `UNKNOWN` → Necesidad documental no cubierta.
**Respuesta:** `PENDING`

#### Q-040 — Documentos / Formatos
**Dominio:** Documentos — Formatos.
**Pregunta:** ¿En qué formato están esos documentos hoy (papel, foto/escaneo, PDF, Excel, Word)?
**Por qué necesitamos saberlo:** Define formatos manejables al digitalizar.
**Impacto si no se conoce:** `UNKNOWN` → Formatos no soportables.
**Respuesta:** `PENDING`

#### Q-041 — Documentos / Acceso
**Dominio:** Documentos — Acceso.
**Pregunta:** ¿Quién necesita acceder a cada tipo de documento y para qué (consulta, edición,
impresión)?
**Por qué necesitamos saberlo:** Define permisos de acceso a documentos.
**Impacto si no se conoce:** `UNKNOWN` → Acceso incorrecto a documentos sensibles.
**Respuesta:** `PENDING`

#### Q-042 — Documentos / Retención
**Dominio:** Documentos — Retención.
**Pregunta:** ¿Cuánto tiempo deben conservarse los documentos antes de que puedan eliminarse, y hay
alguna norma o práctica interna al respecto?
**Por qué necesitamos saberlo:** Define política de retención/eliminación.
**Impacto si no se conoce:** `UNKNOWN` → Retención excesiva o eliminación riesgosa.
**Respuesta:** `PENDING`

---

### 9. Datos existentes

#### Q-043 — Datos / Excel y otros archivos
**Dominio:** Datos existentes — Inventario.
**Pregunta:** ¿Qué datos se encuentran hoy en Excel u otros archivos (estudiantes, asistencia, pagos,
matrícula, otros)? Enumere los archivos y su uso.
**Por qué necesitamos saberlo:** Inventario de datos a importar o consolidar.
**Impacto si no se conoce:** `UNKNOWN` → No se sabe qué datos migrar.
**Respuesta:** `PENDING`

#### Q-044 — Datos / Calidad
**Dominio:** Datos existentes — Calidad.
**Pregunta:** En esos datos existentes, ¿hay duplicados, información incompleta o desactualizada?
¿Sabe aproximadamente cuántos registros en mal estado hay?
**Por qué necesitamos saberlo:** Define esfuerzo de limpieza y validación de datos.
**Impacto si no se conoce:** `UNKNOWN` → Importación de datos corruptos o duplicados.
**Respuesta:** `PENDING`

#### Q-045 — Datos / Fuente oficial
**Dominio:** Datos existentes — Fuente oficial.
**Pregunta:** ¿Cuál es la fuente oficial de los datos de los estudiantes (el archivo más confiable y
actualizado) que debe usarse como base para el sistema?
**Por qué necesitamos saberlo:** Identifica la fuente de verdad para la migración.
**Impacto si no se conoce:** `UNKNOWN` → Migración desde una fuente incorrecta.
**Respuesta:** `PENDING`

---

### 10. Usuarios

#### Nota sobre consolidación
**Nota:** La antigua Q-046 ("quién usará V1") se consolidó con Q-003 (ver `Revision History`).
Q-003 y Q-048 cubren quién usa el sistema y qué actividades le corresponden a cada persona.

#### Q-047 — Usuarios / Futuros
**Dominio:** Usuarios — Versiones futuras.
**Prioridad:** MEDIUM
**Pregunta:** Más adelante, ¿cree que alguna otra persona podría necesitar usar el sistema, además de
quienes lo usan desde el inicio? Si es así, ¿quiénes serían y para qué tareas?
**Por qué necesitamos saberlo:** Anticipa si el sistema podría requerir más roles o más usuarios en el
futuro, sin comprometer el alcance de V1.
**Impacto si no se conoce:** `UNKNOWN` → Arquitectura o roles incorrectos si el uso futuro crece.
**Respuesta:** `PENDING`

#### Q-048 — Usuarios / Responsabilidades
**Dominio:** Usuarios — Responsabilidades.
**Pregunta:** Para cada persona que use el sistema, ¿qué actividades de las ya mencionadas les
corresponden (registro de asistencia, cobros, matrícula, reportes, respaldos)?
**Por qué necesitamos saberlo:** Asigna responsabilidades y permisos por rol.
**Impacto si no se conoce:** `UNKNOWN` → Permisos y responsabilidades ambiguos.
**Respuesta:** `PENDING`

---

### 11. Seguridad

#### Q-049 — Seguridad / Acceso físico
**Dominio:** Seguridad — Acceso físico.
**Pregunta:** ¿Quién tiene acceso físico a la computadora donde se ejecutará el sistema y a los
archivos/registros? ¿Hay personas externas o no autorizadas cerca?
**Por qué necesitamos saberlo:** Define el nivel de control de acceso necesario.
**Impacto si no se conoce:** `UNKNOWN` → Datos sensibles expuestos a accesos no autorizados.
**Respuesta:** `PENDING`

#### Q-050 — Seguridad / Credenciales
**Dominio:** Seguridad — Credenciales.
**Pregunta:** ¿Cómo manejan hoy el acceso a los registros (cada usuario con sus credenciales, una
cuenta compartida, archivos sin protección)? ¿Saben si prefieren que cada persona tenga su propio
acceso o usan un acceso compartido?
**Por qué necesitamos saberlo:** Define el modelo de autenticación y roles.
**Impacto si no se conoce:** `UNKNOWN` → Autenticación insuficiente o sobre-diseñada.
**Respuesta:** `PENDING`

#### Q-051 — Seguridad / Confidencial
**Dominio:** Seguridad — Información confidencial.
**Pregunta:** ¿Qué información del sistema considera confidencial o sensible y que no debe ver
cualquier usuario (salud, datos personales, historial de pagos, calificaciones, otro)?
**Por qué necesitamos saberlo:** Identifica datos a proteger y permisos restringidos.
**Impacto si no se conoce:** `UNKNOWN` → Divulgación de información sensible.
**Respuesta:** `PENDING`

#### Q-052 — Seguridad / Auditoría
**Dominio:** Seguridad — Auditoría.
**Pregunta:** ¿Requieren registrar quién hizo cada cambio importante (por ejemplo, quién modificó o
eliminó un pago o un dato), o basta con que quede el dato actualizado?
**Por qué necesitamos saberlo:** Define si se necesita registro de auditoría.
**Impacto si no se conoce:** `UNKNOWN` → Falta de trazabilidad ante errores o disputas.
**Respuesta:** `PENDING`

#### Q-053 — Seguridad / Recuperación
**Dominio:** Seguridad — Necesidades de recuperación.
**Pregunta:** Si se perdiera la información, ¿qué tan grave sería y cuánto tiempo aceptable tomaría
recuperarla (por ejemplo, perder un día, un mes, el año completo)?
**Por qué necesitamos saberlo:** Define el nivel crítico de los datos y la política de respaldo.
**Impacto si no se conoce:** `UNKNOWN` → Riesgo de pérdida de datos críticos no mitigado.
**Respuesta:** `PENDING`

#### Q-077 — Seguridad / Confidencialidad de datos (GAP-003)
**Dominio:** Seguridad — Confidencialidad de datos.
**Prioridad:** HIGH
**Pregunta:** ¿Qué información de estudiantes y encargados considera confidencial (por ejemplo, salud,
dirección, datos de pagos, otra) y a qué personas les está permitido verla?
**Por qué necesitamos saberlo:** Complementa Q-051 y Q-041 para delimitar qué información se protege y
quién puede accederla.
**Impacto si no se conoce:** `UNKNOWN` → Datos confidenciales accesibles a personal no autorizado.
**Respuesta:** `PENDING`

#### Q-078 — Seguridad / Políticas institucionales (GAP-003)
**Dominio:** Seguridad — Políticas institucionales.
**Prioridad:** HIGH
**Pregunta:** ¿Existen políticas o normas internas de la institución sobre cómo guardar o compartir la
información de los estudiantes? Si existen, ¿puede describirlas o compartirlas?
**Por qué necesitamos saberlo:** Identifica políticas existentes que el sistema debe respetar.
**Impacto si no se conoce:** `UNKNOWN` → El sistema puede incumplir políticas internas.
**Respuesta:** `PENDING`

#### Q-079 — Seguridad / Obligaciones de protección de datos (GAP-003)
**Dominio:** Seguridad — Obligaciones de protección de datos.
**Prioridad:** HIGH
**Pregunta:** ¿La institución tiene alguna obligación o procedimiento de protección de datos que ya
aplique (por ejemplo, autorizaciones firmadas por los encargados, avisos de privacidad, o límites
sobre quién puede ver los datos)?
**Por qué necesitamos saberlo:** Detecta obligaciones y procedimientos existentes sobre datos; no se
inventan obligaciones legales.
**Impacto si no se conoce:** `UNKNOWN` → Incumplimiento de obligaciones existentes.
**Respuesta:** `PENDING`

#### Q-080 — Seguridad / Acceso autorizado (GAP-003)
**Dominio:** Seguridad — Acceso autorizado.
**Prioridad:** HIGH
**Pregunta:** ¿Quién está autorizado a acceder a la información de los estudiantes y encargados, y
quién no? ¿Hay datos que solo deba ver la directora, por ejemplo?
**Por qué necesitamos saberlo:** Define los límites de acceso por persona/rol (complementa Q-041 y
Q-048).
**Impacto si no se conoce:** `UNKNOWN` → Accesos incorrectos a información sensible.
**Respuesta:** `PENDING`

#### Q-081 — Seguridad / Restricciones y validación legal (GAP-003)
**Dominio:** Seguridad — Restricciones y validación legal.
**Prioridad:** HIGH
**Pregunta:** ¿Existen restricciones que el sistema deba respetar sobre cómo se guardan o comparten
estos datos? Si la institución no está segura de si existen obligaciones legales, indíquelo claramente.
**Por qué necesitamos saberlo:** Determina restricciones aplicables. Si no pueden confirmarse las
obligaciones, se requerirá validación legal externa; este documento no brinda asesoría legal.
`EXTERNAL_VALIDATION_REQUIRED` si la institución no puede confirmar sus obligaciones legales.
**Impacto si no se conoce:** `UNKNOWN` → Incumplimiento normativo no detectado.
**Respuesta:** `PENDING`

---

### 12. Backup y Restore

#### Q-054 — Backups / Qué respaldar
**Dominio:** Backup — Contenido.
**Pregunta:** ¿Qué información considera irremplazable y que debe estar respaldada (datos de
estudiantes, pagos, asistencia, documentos)?
**Por qué necesitamos saberlo:** Define el contenido mínimo del respaldo.
**Impacto si no se conoce:** `UNKNOWN` → Respaldos incompletos.
**Respuesta:** `PENDING`

#### Q-055 — Backups / Frecuencia
**Dominio:** Backup — Frecuencia.
**Pregunta:** ¿Con qué frecuencia desearían respaldar (diaria, semanal, mensual) considerando cuántos
datos nuevos registran al día?
**Por qué necesitamos saberlo:** Define la frecuencia de respaldo adecuada.
**Impacto si no se conoce:** `UNKNOWN` → Respaldos con frecuencia inadecuada.
**Respuesta:** `PENDING`

#### Q-056 — Backups / Destinos
**Dominio:** Backup — Destinos.
**Pregunta:** ¿Qué destinos de respaldo hay disponibles (una memoria USB, otro disco, un servicio de
nube, otra computadora)? ¿Puede almacenarse el respaldo fuera del equipo principal?
**Por qué necesitamos saberlo:** Determina dónde/con qué se guardan los respaldos.
**Impacto si no se conoce:** `UNKNOWN` → Respaldos en el mismo equipo, inútiles ante fallo.
**Respuesta:** `PENDING`

#### Q-057 — Backups / Responsable
**Dominio:** Backup — Responsable.
**Pregunta:** ¿Qué persona sería responsable de verificar que los respaldos se realicen y estén al día?
**Por qué necesitamos saberlo:** Asigna la responsabilidad operativa de respaldos.
**Impacto si no se conoce:** `UNKNOWN` → Ningún respaldo realizado en la práctica.
**Respuesta:** `PENDING`

#### Q-058 — Backups / Restauración
**Dominio:** Backup — Recuperación ante fallo.
**Pregunta:** Si el sistema fallara o se perdiera un dato, ¿qué esperan poder hacer de inmediato para
recuperar la información? ¿Quién realizaría esa recuperación?
**Por qué necesitamos saberlo:** Define el procedimiento esperado de restauración.
**Impacto si no se conoce:** `UNKNOWN` → Incapacidad de recuperación ante fallo.
**Respuesta:** `PENDING`

#### Q-059 — Backups / Protocolo ante fallo
**Dominio:** Backup — Protocolo.
**Pregunta:** ¿Qué haría la institución hoy si la computadora con sus datos se dañara o perdiera?
¿Existe algún plan o procedimiento ante ese incidente?
**Por qué necesitamos saberlo:** Identifica la brecha actual de continuidad de datos.
**Impacto si no se conoce:** `UNKNOWN` → Pérdida total sin plan de recuperación.
**Respuesta:** `PENDING`

---

### 13. Infraestructura

#### Q-060 — Infraestructura / Computadora y SO
**Dominio:** Infraestructura — Hardware.
**Pregunta:** ¿Con qué computadora cuenta la institución para ejecutar el sistema, y qué sistema
operativo tiene (Windows, macOS, Linux)? ¿Cuántos usuarios la usarían a la vez?
**Por qué necesitamos saberlo:** Define compatibilidad y requisitos de instalación.
**Impacto si no se conoce:** `UNKNOWN` → Instalación incompatible con el equipo real.
**Respuesta:** `PENDING`

#### Q-061 — Infraestructura / Conectividad
**Dominio:** Infraestructura — Conectividad.
**Pregunta:** ¿Tiene la institución acceso a internet? ¿Con qué frecuencia o en qué momentos está
disponible? Cuando no hay internet, ¿qué hace actualmente con su información para no perderla?
**Por qué necesitamos saberlo:** Determina la disponibilidad de conexión y cómo afecta el trabajo
diario; la decisión sobre si funcionar sin conexión es interna, no debe inducirse al responder.
**Impacto si no se conoce:** `UNKNOWN` → Dependencia de internet no validada puede dejar el sistema
inoperante.
**Respuesta:** `PENDING`

#### Q-062 — Infraestructura / Restricciones
**Dominio:** Infraestructura — Restricciones técnicas.
**Pregunta:** ¿Existen restricciones técnicas o de seguridad (por ejemplo, políticas de la escuela o
de una entidad reguladora) sobre qué programas pueden instalarse o cómo se guardan los datos de
estudiantes?
**Por qué necesitamos saberlo:** Determina limitaciones de instalación y almacenamiento.
**Impacto si no se conoce:** `UNKNOWN` → Solución que infringe restricciones existentes.
**Respuesta:** `PENDING`

#### Q-063 — Infraestructura / Acceso físico
**Dominio:** Infraestructura — Acceso físico.
**Pregunta:** ¿El equipo se encuentra en la institución o en la casa de alguien? ¿Quién lo resguarda
y en qué horario se usa?
**Por qué necesitamos saberlo:** Confirma el despliegue on-premise y sus condiciones.
**Impacto si no se conoce:** `UNKNOWN` → Suposición de despliegue local sin validar.
**Respuesta:** `PENDING`

---

### 14. Operación y mantenimiento

> **Nota:** la antigua Q-065 ("solicitudes de cambio") fue retirada por bajo valor para el discovery
> (ver `Revision History`). El rol de solicitar cambios y la aprobación quedan cubiertos por Q-070
> (aprobación) y Q-085 (patrocinador).

#### Q-064 — Operación / Administrador
**Dominio:** Operación — Administración.
**Pregunta:** ¿Qué persona administrará el sistema a diario (mantener datos al día, crear usuarios,
corregir errores)?
**Por qué necesitamos saberlo:** Define responsabilidad administrativa y de soporte.
**Impacto si no se conoce:** `UNKNOWN` → Sistema sin administración ni datos al día.
**Respuesta:** `PENDING`

#### Q-066 — Operación / Continuidad del desarrollador
**Dominio:** Operación — Continuidad.
**Pregunta:** Si el desarrollador original no estuviera disponible, ¿cómo podría la institución
seguir actualizando o reparando el sistema? ¿Existe alguien que dé soporte técnico?
**Por qué necesitamos saberlo:** Define estrategia de handover y mantenibilidad.
**Impacto si no se conoce:** `UNKNOWN` → Sistema insostenible sin el desarrollador original.
**Respuesta:** `PENDING`

#### Q-067 — Operación / Actualizaciones
**Dominio:** Operación — Actualizaciones.
**Pregunta:** ¿Qué entienden por "actualizar el sistema" (corregir errores, sumar funciones, pasar de
año lectivo) y con qué frecuencia lo esperan?
**Por qué necesitamos saberlo:** Define el alcance y cadencia de las actualizaciones.
**Impacto si no se conoce:** `UNKNOWN` → Expectativas de actualización inciertas.
**Respuesta:** `PENDING`

---

### Alcance, calidad y cierre (transversales)

#### Q-068 — Alcance / Datos en V1
**Dominio:** Alcance / Datos existentes.
**Pregunta:** Para la primera versión, ¿partirá el sistema desde cero (registrando estudiantes nuevos)
o debe incluir información ya existente (por ejemplo, la matrícula del año en curso)?
**Por qué necesitamos saberlo:** Define qué datos requiere V1 y si hay migración.
**Impacto si no se conoce:** `UNKNOWN` → V1 sin los datos que la institución espera usar de inmediato.
**Respuesta:** `PENDING`

#### Q-069 — Alcance / Prioridad de V1
**Dominio:** Alcance / Prioridades.
**Pregunta:** De las funciones (estudiantes, matrícula, asistencia, pagos, reportes, respaldos,
documentos), ¿cuál considera indispensable desde el primer día y cuál podría esperar?
**Por qué necesitamos saberlo:** Define la prioridad y alcance del MVP/V1.
**Impacto si no se conoce:** `UNKNOWN` → V1 con prioridades incorrectas respecto a lo que se necesita.
**Respuesta:** `PENDING`

#### Q-070 — Alcance / Documento maestro
**Dominio:** Alcance / Gobernanza.
**Pregunta:** ¿Existe un documento oficial o maestro del proyecto más allá de la visión breve
(`docs/Vision.md`), o este documento puede servir como fuente definitiva? ¿Quién lo aprueba o valida?
**Por qué necesitamos saberlo:** Confirma cuál es la fuente de verdad y el responsable de aprobación.
**Impacto si no se conoce:** `UNKNOWN` → Ambigüedad sobre qué fuente define el proyecto.
**Respuesta:** `PENDING`

#### Q-082 — Alcance / Funcionamiento correcto (GAP-004)
**Dominio:** Alcance — Calidad / Aceptación.
**Prioridad:** MEDIUM
**Pregunta:** ¿Cómo sabrían que el sistema funciona correctamente y está listo para usarse
normalmente? ¿Qué resultados esperan ver en su día a día?
**Por qué necesitamos saberlo:** El Discovery Audit registra como desconocidos los criterios de
aceptación; revela qué significa "funciona bien" para la institución.
**Impacto si no se conoce:** `UNKNOWN` → No hay forma de saber si V1 es aceptable.
**Respuesta:** `PENDING`

#### Q-083 — Alcance / Procesos críticos y errores (GAP-004)
**Dominio:** Alcance — Procesos críticos.
**Prioridad:** MEDIUM
**Pregunta:** ¿Qué procesos consideran críticos y qué errores serían inaceptables en el uso diario
(por ejemplo, perder un pago, no registrar asistencia, equivocar datos de un estudiante)?
**Por qué necesitamos saberlo:** Identifica procesos críticos y errores a evitar en V1, sin convertirlos
en pruebas todavía.
**Impacto si no se conoce:** `UNKNOWN` → Se podrían descuidar procesos críticos.
**Respuesta:** `PENDING`

#### Q-084 — Alcance / Condiciones mínimas de V1 (GAP-004)
**Dominio:** Alcance — Condiciones de aceptación.
**Prioridad:** MEDIUM
**Pregunta:** ¿Qué condiciones mínimas deberían cumplirse para que consideren aceptable la primera
versión del sistema (por ejemplo, poder registrar estudiantes, registrar asistencia, cobrar y ver
reportes básicos)?
**Por qué necesitamos saberlo:** Define el umbral de aceptación de V1 desde la perspectiva institucional.
**Impacto si no se conoce:** `UNKNOWN` → V1 podría cerrarse sin cumplir expectativas mínimas.
**Respuesta:** `PENDING`

#### Q-085 — Alcance / Patrocinador institucional (GAP-005)
**Dominio:** Alcance — Gobernanza / Patrocinador.
**Prioridad:** LOW
**Pregunta:** ¿Quién es la persona responsable o patrocinadora del proyecto por parte de la
institución, con autoridad para validar las decisiones y aceptar la entrega del sistema?
**Por qué necesitamos saberlo:** El Discovery Audit requiere identificar al responsable que valida
decisiones y acepta la entrega (GAP-005).
**Impacto si no se conoce:** `UNKNOWN` → Sin un responsable definido no es posible validar decisiones
ni aceptar la entrega.
**Respuesta:** `PENDING`

---

## 8. Evidence Required

Evidencia útil cuando corresponda. El encargado de responder debería adjuntarla o permitir su
referencia sin exponer datos reales de menores (idealmente anonimizados).

- **Excel:** una copia anónima / ejemplo de la hoja de estudiantes (y de asistencia/pagos si existen),
  mostrando las columnas usadas (relacionado con Q-007, Q-043).
- **Formularios:** los formularios de inscripción/matrícula actuales (Q-017).
- **Recibos:** una copia (anonimizada) de un recibo o constancia de pago emitido (Q-032).
- **Reportes:** copias de los listados/reportes que generan hoy (Q-035).
- **Documentos:** ejemplos del tipo de documentos que se guardan (Q-039, Q-040, Q-042).
- **Capturas:** capturas de pantalla de los archivos o del sistema actual si lo hubiera (Q-043).
- **Procedimientos actuales:** descripción escrita si existe de cómo se realizan matrícula, cobros y
  asistencia (Q-004, Q-015).
- **Asignaturas/plan de estudios:** listado de grados y, si aplica, de asignaturas por grado
  (Q-071–Q-073; GAP-001).
- **Descuentos/becas:** documento o registro de descuentos/becas otorgados, si existe
  (Q-074–Q-076; GAP-002).
- **Autorización/consentimiento de datos:** cualquier formulario de autorización o aviso de privacidad
  firmado al inscribir (Q-077–Q-081; GAP-003).
- **Políticas/procedimientos de datos:** políticas internas de manejo, retención o privacidad
  (Q-078, Q-079; GAP-003).
- **Definición de "funciona correctamente":** evidencias o ejemplos de resultados esperados para
  validar la aceptación de V1 (Q-082–Q-084; GAP-004).

> Nota: no se requiere ni se debe compartir información personal identificable de estudiantes para
> responder este cuestionario. Un ejemplo anónimo (nombres ficticios en una fila de ejemplo) es
> suficiente para definir la estructura.

---

## 9. Discovery Completion Criteria

Se considera **terminado** el Discovery institucional cuando se cumplan todas las condiciones:

1. **Todas las preguntas en las secciones 3 (Critical) y 4 (High Priority) tienen respuesta** no
   `PENDING`, registrada por la institución.
2. **Las preguntas 5 (Medium) y 6 (Low)** tienen respuesta o una razón explícita de "no aplica" o "no
   se sabe" declarada.
3. **Se ha identificado a la persona/institución responsable** que respondió y validó cada dominio
   (registrada en el documento).
4. **La evidencia de la sección 8** ha sido adjuntada o anonimizada para los dominios con datos
   existentes, matrícula, pagos, reportes, asignaturas, descuentos y privacidad de datos.
5. **No queda ninguna clase de información clasificada como `UNKNOWN` en los dominios críticos**
   (institución, estudiantes, matrícula, encargados, asistencia, pagos, reportes, datos existentes,
   usuarios, seguridad, backup, infraestructura, operación) que impida el diseño.
6. **Se han resuelto los GAPs del Discovery Validation:** asignaturas (GAP-001, Q-071–Q-073),
   descuentos/becas (GAP-002, Q-074–Q-076), privacidad/cumplimiento (GAP-003, Q-077–Q-081),
   criterios de aceptación (GAP-004, Q-082–Q-084) y patrocinador (GAP-005, Q-085), con respuesta o
   razón válida de "no aplica".
7. **Se ha confirmado la fuente de verdad del proyecto** (documento maestro / visión) y el responsable
   de aprobación (Q-070), y se ha identificado al patrocinador institucional (Q-085).
8. **Se ha definido el alcance y prioridad de V1** (Q-068, Q-069) y las condiciones mínimas de
   aceptación (Q-084).
9. El resultado puede responder las cinco preguntas del criterio de calidad:
   - ¿Qué sabemos? — Los procesos, datos y reglas institucionales confirmados.
   - ¿Qué no sabemos? — Se redujo al mínimo documentado (declarado "no aplica" o "no se sabe").
   - ¿Qué estamos suponiendo? — Todas las inferencias previas quedaron validadas o desmentidas.
   - ¿Qué debemos preguntarle a la institución? — Nada pendiente en dominios críticos.
   - ¿Qué decisiones debemos tomar? — Las decisiones quedaron tomadas o con recomendación clara.

10. **El Discovery institucional ha sido revisado y aprobado** como completo por el responsable del
    proyecto antes de autorizar el avance a la fase Foundation.

> Ninguna de estas condiciones se cumple en el estado actual: todas las respuestas permanecen
> `PENDING` y los dominios críticos siguen `UNKNOWN` hasta que la institución responda.

---

## 10. Revision History

Registro de los cambios aplicados en esta revisión (corrección según
`docs/00-foundation/discovery-validation.md`).

### Preguntas corregidas (identificación / etiquetas)
- **Q-063:** Corregidas las referencias y etiquetas en las secciones de prioridad (3 y 4). Ahora se
  describe correctamente como "Infraestructura / Acceso físico" (ubicación del equipo y despliegue).
  El contenido conceptual no cambió. Resuelve: inconsistencia de identificación señalada por la
  auditoría.
- **Q-068:** Corregidas las referencias y etiquetas en la sección 6 (era etiquetada como
  "Expectativas de actualización"). Ahora se identifica correctamente como "Alcance / Datos en V1";
  la actualización del sistema queda cubierta por Q-067. El contenido conceptual no cambió. Resuelve:
  inconsistencia de identificación señalada por la auditoría.
- Se corrigieron además las referencias incorrectas de otras preguntas en las secciones de prioridad
  (Q-008, Q-010, Q-016, Q-017, Q-018, Q-022, Q-028, Q-030, Q-031, Q-033, Q-047, Q-048, Q-051, Q-062,
  Q-069, Q-070) para que cada etiqueta coincida con el contenido real de su ID.

### Corrección de trazabilidad (sección 4 — etiquetas de Alta prioridad)
- Se corrigió el desplazamiento de etiquetas de la sección 4 (High Priority Questions): cada `Q-XX`
  ahora describe el contenido real de la pregunta que identifica, restableciendo la correspondencia
  `ID mostrado → contenido de la pregunta`.
- **13 IDs afectados:** Q-011, Q-012, Q-013, Q-014, Q-015, Q-019, Q-020, Q-021, Q-023, Q-024, Q-025,
  Q-026, Q-027.
- **Sin cambios de contenido:** no se reformuló, agregó ni eliminó ninguna pregunta; no se alteraron
  prioridades, dominios, respuestas ni requisitos. Solo se corrigieron las etiquetas descriptivas de la
  lista de Alta prioridad.
- La corrección se realizó para restaurar la trazabilidad, conforme a la tabla de correspondencia de la
  sección 5 de `docs/00-foundation/discovery-validation.md`. Las respuestas permanecen `PENDING`.

### Preguntas reformuladas
- **Q-004:** Reformulada para ser una vista general breve del orden de los procesos; el detalle de
  cada proceso se delega a sus preguntas específicas (Q-015, Q-023, Q-031, Q-035). Resuelve:
  "demasiado amplia" de la auditoría.
- **Q-007:** Reformulada para preguntar únicamente por la existencia y campos de la planilla; la
  solicitud del ejemplo anónimo se movió a la sección 8 (Evidence Required). Resuelve: "mezcla
  pregunta con solicitud de evidencia".
- **Q-047:** Reformulada para eliminar la inducción ("¿Se anticipa una necesidad futura...?").
  Resuelve: "inducción leve".
- **Q-061:** Reformulada para eliminar la solución implícita ("debe funcionar sin conexión"); ahora
  pregunta por disponibilidad de internet y su efecto real. Resuelve: "solución técnica implícita".
- **Q-050:** Ajuste menor de redacción para reducir inducción (uso de "¿Saben si prefieren...?").
  Resuelve: mejora de neutralidad.

### Preguntas consolidadas
- **Q-046 (eliminada como pregunta independiente):** Consolidada con Q-003 (quién usa el sistema,
  incluida V1). Su cobertura (quiénes usan V1) se absorbió en Q-003, y las responsabilidades por
  persona quedan en Q-048. No se perdió información; el cambio se registra para trazabilidad.
  Resuelve: `DUPLICATE` (Q-046) de la auditoría.

### Preguntas eliminadas
- **Q-065 (eliminada):** Evaluada como de bajo valor para decisiones de dominio, alcance, seguridad,
  arquitectura, datos u operación (canal/formato de solicitudes de cambio es propio de la fase de
  operación/handover). Se verificó que ninguna otra pregunta depende de ella; la aprobación queda en
  Q-070 y el patrocinio en Q-085. Resuelve: `LOW_VALUE` (Q-065) de la auditoría.

### Nuevas preguntas (para resolver GAPs del Discovery Validation)
- **Q-071, Q-072, Q-073** — Asignaturas y su relación con grados/secciones. Resuelven: **GAP-001**.
- **Q-074, Q-075, Q-076** — Descuentos, becas/exoneraciones y sus reglas de pago. Resuelven:
  **GAP-002**.
- **Q-077, Q-078, Q-079, Q-080, Q-081** — Confidencialidad, políticas, obligaciones de protección de
  datos, acceso autorizado y restricciones. Resuelven: **GAP-003**. Q-081 incluye el marcador
  `EXTERNAL_VALIDATION_REQUIRED` si la institución no puede confirmar sus obligaciones legales.
- **Q-082, Q-083, Q-084** — Criterios de aceptación y condiciones para considerar correcta y aceptable
  la V1. Resuelven: **GAP-004**.
- **Q-085** — Identificación del patrocinador institucional. Resuelve: **GAP-005**.

### Notas de trazabilidad
- Todas las respuestas permanecen `PENDING`; no se respondió ninguna pregunta.
- El contenido conceptual de las preguntas no vacías se conservó salvo cuando era necesario corregir
  la inconsistencia o la calidad señaladas por la auditoría.
- `docs/00-foundation/discovery-validation.md` NO fue modificado; se conserva como evidencia de la
  auditoría previa.

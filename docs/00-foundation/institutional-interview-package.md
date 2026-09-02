# Institutional Interview Package — Sistema de Gestión Escolar

> PIPELINE 00.4 — Paquete de entrevista institucional.
> Instrumento de apoyo para dialogar con el personal de la institución y obtener respuestas reales a
> las preguntas del cuestionario de Discovery.
> Este documento NO reemplaza a `docs/00-foundation/institutional-discovery.md`, que sigue siendo la
> **fuente de verdad**. Cada pregunta conserva su ID original y su prioridad; ninguna ha sido respondida.
> Este documento NO diseña soluciones, arquitectura, base de datos o requisitos.

---

## Cómo usar este paquete

- Se organiza en **14 sesiones lógicas** para conducir la entrevista por temas afines.
- Cada pregunta indica: dominio, prioridad, la pregunta tal como está formulada en el cuestionario,
  por qué se hace y un ejemplo del **tipo de información** que buscamos (el ejemplo es solo para
  aclarar el alcance; **no** es una respuesta sugerida ni introduce reglas).
- Responda en sus propias palabras; si una pregunta no aplica o no se sabe la respuesta, indíquelo.
- Registre la respuesta, la evidencia disponible, quién la proporcionó y la fecha.
- Prioridad: **CRITICAL** y **HIGH** deben responderse primero.
- Todas las respuestas permanecen en `PENDING` hasta que la institución las conteste.

---

# Sesión 1 — Institución y usuarios

### Q-001

**Dominio:** Institución — Contexto operativo.

**Prioridad:** CRITICAL

**Pregunta:** ¿Cuál es el nombre oficial de la institución, su nivel educativo (por ejemplo, inicial, primaria, secundaria, mixto) y cuántas sedes o campus tiene?

**Por qué necesitamos saberlo:** Para dimensionar el alcance del sistema y conocer el contexto en el que operará.

**Ejemplo de respuesta esperada:** Se busca una descripción breve del lugar y su entorno educativo: qué nivel(es) atiende y si opera en uno o varios sitios. El ejemplo sirve para aclarar que la respuesta puede ser sencilla (por ejemplo, indicar un nivel y la cantidad de sedes), y cada institución debe describir su propia realidad; no se asume ningún nivel ni número de sedes.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING` — útil: documentación general de la institución si existe.

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-002

**Dominio:** Institución — Personal y dimensión.

**Prioridad:** HIGH

**Pregunta:** ¿Cuántos estudiantes tiene aproximadamente la institución y cuántas personas participan en la gestión (directora, docentes, secretaría, administración, otros)?

**Por qué necesitamos saberlo:** Determina la escala de datos, el número probable de usuarios y la complejidad de la gestión diaria.

**Ejemplo de respuesta esperada:** Se busca una estimación cuantitativa razonable (no un conteo exacto): volumen aproximado de estudiantes y de personas que colaboran en la gestión, junto con sus roles aproximados. El ejemplo solo aclara que basta una cifra aproximada y una idea de cuántas personas intervienen; no indica cifras concretas esperadas.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-003

**Dominio:** Institución — Personal involucrado.

**Prioridad:** CRITICAL

**Pregunta:** ¿Quién usará el sistema (incluida la primera versión)? ¿Solo la directora, o también docentes, secretaría, personal administrativo u otros? Indique quién realizará cada tarea.

**Por qué necesitamos saberlo:** Define los roles y permisos del sistema y qué actividades necesita soportar; consolida la información de quién usa el sistema y quién lo hará en V1.

**Ejemplo de respuesta esperada:** Se busca una lista de las personas/cargos que usarán la herramienta y, de cada una, qué tarea le corresponde (por ejemplo, quién registra, quién cobra, quién consulta). El ejemplo aclara que se esperan roles y tareas concretas; no presupone quiénes son ni qué hacen.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-004

**Dominio:** Institución — Procesos de negocio.

**Prioridad:** CRITICAL

**Pregunta:** En general, ¿en qué orden se realizan durante el año la matrícula, el registro de asistencia, los cobros de pagos y la generación de reportes? Solo necesita darme una visión general; más adelante preguntaré el detalle de cada proceso.

**Por qué necesitamos saberlo:** Confirma el orden y la secuencia de los procesos sin pedir un flujo extenso que ya se aborda en las preguntas específicas.

**Ejemplo de respuesta esperada:** Se busca un orden aproximado de los grandes momentos del año (por ejemplo, cuál ocurre antes, cuál después), sin entrar en detalle. El ejemplo aclara que basta una secuencia general; no se asume un orden concreto.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-005

**Dominio:** Institución — Ciclo académico.

**Prioridad:** HIGH

**Pregunta:** ¿Cuáles son las fechas del ciclo académico? ¿En qué fechas inicia y termina el ciclo, cuántos periodos/meses tiene el año escolar, y hay fechas clave (inicio de clases, vacaciones, cierre)?

**Por qué necesitamos saberlo:** El ciclo afecta matrícula, asistencia, cobros y reportes.

**Ejemplo de respuesta esperada:** Se busca el calendario escolar real: cuándo empieza y termina, cuántos momentos/periodos hay y si existen fechas importantes. El ejemplo aclara el tipo de dato (fechas/periodos) que se desea; no supone un calendario concreto.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING` — útil: calendario escolar o cronograma anual si existe.

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-047

**Dominio:** Usuarios — Versiones futuras.

**Prioridad:** MEDIUM

**Pregunta:** Más adelante, ¿cree que alguna otra persona podría necesitar usar el sistema, además de quienes lo usan desde el inicio? Si es así, ¿quiénes serían y para qué tareas?

**Por qué necesitamos saberlo:** Anticipa si el sistema podría requerir más roles o más usuarios en el futuro, sin comprometer el alcance de V1.

**Ejemplo de respuesta esperada:** Se busca saber si existe una posible ampliación futura de usuarios y, de haberla, quiénes y para qué. El ejemplo aclara que la pregunta es prospectiva y opcional; no implica que deba haber más usuarios.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-048

**Dominio:** Usuarios — Responsabilidades.

**Prioridad:** MEDIUM

**Pregunta:** Para cada persona que use el sistema, ¿qué actividades de las ya mencionadas les corresponden (registro de asistencia, cobros, matrícula, reportes, respaldos)?

**Por qué necesitamos saberlo:** Asigna responsabilidades y permisos por rol.

**Ejemplo de respuesta esperada:** Se busca asignar, a cada persona/cargo, las actividades que le competen (quién hace cada cosa). El ejemplo aclara que se espera un reparto de tareas real; no asume cuál persona hace qué.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

# Sesión 2 — Estudiantes

### Q-006

**Dominio:** Estudiantes / Datos existentes.

**Prioridad:** CRITICAL

**Pregunta:** ¿Existen actualmente registros de estudiantes en algún formato (Excel, papeles, otro sistema)? ¿Cuántos y en qué forma se guardan?

**Por qué necesitamos saberlo:** Determina si V1 debe importar datos o partir de cero, y condiciona la migración.

**Ejemplo de respuesta esperada:** Se busca saber si hay información previa registrada, en qué formato y en qué cantidad aproximada. El ejemplo aclara que se espera un dato de existencia/formato/volumen; no se asume que existan registros.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING` — útil: un listado o inventario de los registros existentes.

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-007

**Dominio:** Estudiantes / Datos existentes.

**Prioridad:** CRITICAL

**Pregunta:** ¿Existe una hoja, planilla o archivo donde actualmente se registren los estudiantes (por ejemplo, un documento de Excel o un cuaderno)? Si existe, ¿qué datos incluye por estudiante (por ejemplo, nombre, documento, grado, contacto)?

**Por qué necesitamos saberlo:** Determina la estructura de datos existente que el sistema deberá conservar o importar.

**Ejemplo de respuesta esperada:** Se busca conocer, si existe, qué campos se anotan por estudiante en la planilla actual. El ejemplo aclara que se espera una enumeración de columnas/campos; no se asume qué contiene la planilla.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING` — útil: una copia anónima/ejemplo de la hoja (ver paquete, sección de evidencia).

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-008

**Dominio:** Estudiantes — Identificación.

**Prioridad:** CRITICAL

**Pregunta:** ¿Qué documento o campo sirve para identificar de forma única a un estudiante (por ejemplo, un número de identidad, un código interno, o el nombre completo)? ¿Existe algún caso de dos estudiantes con el mismo nombre?

**Por qué necesitamos saberlo:** Define la clave de identidad y cómo evitar duplicados.

**Ejemplo de respuesta esperada:** Se busca saber qué dato distingue a un estudiante de otro y si conviven nombres iguales. El ejemplo aclara que se espera un campo identificador y una constatación de casos ambiguos; no impone cuál debe ser ese campo.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-009

**Dominio:** Estudiantes — Datos personales.

**Prioridad:** HIGH

**Pregunta:** ¿Qué datos personales de un estudiante registran actualmente (por ejemplo, nombre, fecha de nacimiento, dirección, contacto, otro) y cuáles consideran obligatorios para matricularlo?

**Por qué necesitamos saberlo:** Define exactamente los campos del estudiante y cuáles son requeridos.

**Ejemplo de respuesta esperada:** Se busca una lista de los datos que se guardan de cada estudiante y cuáles son imprescindibles al matricular. El ejemplo aclara el tipo de información (lista de campos + cuáles obligatorios); no determina qué campos debe haber.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING` — útil: formulario de inscripción actual si existe.

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-010

**Dominio:** Estudiantes — Estados del estudiante.

**Prioridad:** CRITICAL

**Pregunta:** ¿Qué estados atraviesa un estudiante a lo largo de su tiempo en la institución (por ejemplo, activo, retirado, egresado, trasladado, de baja)? ¿Quién decide y registra cada estado?

**Por qué necesitamos saberlo:** Define estados de ciclo de vida y transiciones de datos.

**Ejemplo de respuesta esperada:** Se busca saber qué situaciones describe la institución para un estudiante a lo largo del tiempo y quién las determina. El ejemplo aclara que se esperan estados y responsable de cada uno; no fija qué estados deben existir.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-011

**Dominio:** Estudiantes — Historial.

**Prioridad:** HIGH

**Pregunta:** ¿Qué información histórica de un estudiante debe conservarse pese a haber terminado su paso por la institución (por ejemplo, ciclo cursado, estado, fechas)?

**Por qué necesitamos saberlo:** Determina qué mantener tras la baja/egreso y la retención de datos.

**Ejemplo de respuesta esperada:** Se busca saber qué datos de un estudiante que ya no asiste conviene conservar. El ejemplo aclara el tipo de dato (histórico) que se desea precisar; no indica qué conservar.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-012

**Dominio:** Estudiantes — Altas y bajas.

**Prioridad:** HIGH

**Pregunta:** ¿Cómo se da de alta a un estudiante nuevo y cómo se da de baja a uno que se retira? ¿Quién lo autoriza y qué datos deben registrarse en ese momento?

**Por qué necesitamos saberlo:** Define los flujos de alta/baja y quién puede ejecutarlos.

**Ejemplo de respuesta esperada:** Se busca describir cómo entra y sale un estudiante de la institución y quién lo aprueba. El ejemplo aclara que se esperan pasos y responsable; no presume un procedimiento.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING` — útil: procedimientos o formatos de alta/baja si existen.

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-013

**Dominio:** Estudiantes — Correcciones de información.

**Prioridad:** HIGH

**Pregunta:** ¿Con qué frecuencia corrigen o actualizan los datos de un estudiante (por ejemplo, dirección, teléfono, nombre mal escrito) y quién autoriza la corrección?

**Por qué necesitamos saberlo:** Define si se requiere control/auditoría al editar datos.

**Ejemplo de respuesta esperada:** Se busca saber qué tan seguido se actualiza la información y quién puede hacerlo. El ejemplo aclara que se esperan frecuencia y responsable; no supone cuán frecuente es ni quién autoriza.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-014

**Dominio:** Estudiantes / Documentos.

**Prioridad:** HIGH

**Pregunta:** ¿Qué documentos o papeles de un estudiante deben conservarse (por ejemplo, acta de nacimiento, comprobante de pago, formulario de inscripción, otros) y dónde se guardan hoy?

**Por qué necesitamos saberlo:** Determina si el sistema debe almacenar documentos y en qué formato.

**Ejemplo de respuesta esperada:** Se busca una lista de los papeles que se guardan por estudiante y dónde. El ejemplo aclara el tipo de información (tipos de documento + ubicación); no prescribe qué documentos debe haber.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

# Sesión 3 — Matrícula

### Q-015

**Dominio:** Matrícula — Proceso actual.

**Prioridad:** HIGH

**Pregunta:** ¿Cuál es el proceso actual de matrícula? ¿Con qué periodicidad se realiza (una vez al año, por periodo, continua) y en qué fechas?

**Por qué necesitamos saberlo:** Define el flujo y el calendario de matrícula.

**Ejemplo de respuesta esperada:** Se busca describir cómo se matricula hoy y en qué momentos del año. El ejemplo aclara que se esperan pasos y periodicidad; no asume un proceso ni un calendario.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING` — útil: procedimiento o formulario de matrícula si existe.

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-016

**Dominio:** Matrícula — Grados/Secciones.

**Prioridad:** CRITICAL

**Pregunta:** ¿Cuáles son los grados y secciones que existen (por ejemplo, grados A/B/C, niveles) y cómo se asigna un estudiante a un grado/sección?

**Por qué necesitamos saberlo:** Define la estructura académica usada en matrícula, asistencia y reportes.

**Ejemplo de respuesta esperada:** Se busca conocer la organización académica (qué grados/secciones hay) y el criterio para ubicar a un estudiante. El ejemplo aclara el tipo de información (estructura + asignación); no define qué grados existen.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING` — útil: listado de grados/secciones actual si existe.

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-017

**Dominio:** Matrícula — Documentación.

**Prioridad:** CRITICAL

**Pregunta:** ¿Qué documentos se exigen al matricular a un estudiante y qué debe comprobarse antes de aceptar la matrícula?

**Por qué necesitamos saberlo:** Define requisitos de validación de la matrícula.

**Ejemplo de respuesta esperada:** Se busca saber qué papeles se piden al matricular y qué se verifica. El ejemplo aclara el tipo de información (requisitos documentales); no impone qué debe exigirse.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING` — útil: formularios de inscripción/matrícula actuales.

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-018

**Dominio:** Matrícula — Reingresos/Traslados.

**Prioridad:** CRITICAL

**Pregunta:** ¿Cómo manejan los reingresos (un estudiante que vuelve) y los traslados (entrada o salida hacia otra institución)? ¿Se conserva su historial?

**Por qué necesitamos saberlo:** Define flujos especiales y continuidad del historial.

**Ejemplo de respuesta esperada:** Se busca describir cómo se trata a un estudiante que regresa o se traslada, y si se guarda su historia. El ejemplo aclara que se esperan esos casos y su manejo; no supone cómo se hacen.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-019

**Dominio:** Matrícula — Históricos.

**Prioridad:** HIGH

**Pregunta:** ¿Necesitan conservar el historial de matrículas de años anteriores de cada estudiante y consultarlo? ¿Por cuánto tiempo?

**Por qué necesitamos saberlo:** Define persistencia de históricos de matrícula.

**Ejemplo de respuesta esperada:** Se busca saber si se conserva el historial de matrícula por estudiante y por cuánto tiempo. El ejemplo aclara el tipo de dato (histórico + retención); no indica cuánto tiempo conservar.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-071

**Dominio:** Matrícula — Asignaturas.

**Prioridad:** HIGH

**Pregunta:** ¿Existen asignaturas o materias específicas que se enseñen en la institución? Si es así, ¿puede enumerarlas y, en la medida que corresponda, indicar a qué grado o sección pertenece cada una?

**Por qué necesitamos saberlo:** Registra como desconocido el registro de asignaturas y la organización académica; no se asume que todas las instituciones manejan las mismas asignaturas.

**Ejemplo de respuesta esperada:** Se busca saber si la institución trabaja con asignaturas definidas y, de ser así, cuáles y en qué grados. El ejemplo aclara que la respuesta puede ser "no aplica" si no se usan asignaturas; no asume que existan.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING` — útil: listado de asignaturas/plan de estudios por grado si existe.

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-072

**Dominio:** Matrícula — Asignaturas.

**Prioridad:** HIGH

**Pregunta:** ¿El sistema debe registrar las asignaturas de cada grado/sección, o solo basta con registrar el grado y la sección de cada estudiante?

**Por qué necesitamos saberlo:** Define si las asignaturas forman parte del modelo de datos, sin presuponer que son necesarias.

**Ejemplo de respuesta esperada:** Se busca saber qué nivel de detalle se necesita guardar: si basta el grado/sección o si además se requiere el detalle por asignatura. El ejemplo aclara que se espera una preferencia sobre el nivel de registro; no decide por la institución.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-073

**Dominio:** Matrícula — Asignaturas.

**Prioridad:** HIGH

**Pregunta:** La asistencia y los reportes, ¿se organizan por asignatura, por grado/sección, o por ambos?

**Por qué necesitamos saberlo:** Determina el nivel de detalle de asistencia y reportes.

**Ejemplo de respuesta esperada:** Se busca saber cómo deben agruparse la asistencia y los reportes (por grado, por asignatura, o ambos). El ejemplo aclara el tipo de decisión solicitada; no elige por la institución.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

# Sesión 4 — Encargados

### Q-020

**Dominio:** Encargados — Relación estudiante-encargado.

**Prioridad:** HIGH

**Pregunta:** ¿Quién es el encargado o responsable de cada estudiante (padre, madre, tutor, otro)? ¿Un estudiante puede tener más de un encargado?

**Por qué necesitamos saberlo:** Define si se modelan uno o varios encargados por estudiante.

**Ejemplo de respuesta esperada:** Se busca saber quién responde por cada estudiante y si puede haber más de un responsable. El ejemplo aclara el tipo de información (figura responsable + cantidad); no asume quién ni cuántos.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-021

**Dominio:** Encargados — Datos registrados.

**Prioridad:** HIGH

**Pregunta:** ¿Qué datos registran de cada encargado (por ejemplo, nombre, teléfono, correo, dirección, parentesco)? ¿Cuáles son obligatorios?

**Por qué necesitamos saberlo:** Define campos y requisitos del encargado.

**Ejemplo de respuesta esperada:** Se busca una lista de los datos que se guardan de cada encargado y cuáles son imprescindibles. El ejemplo aclara el tipo de información (campos + obligatoriedad); no determina qué campos debe haber.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING` — útil: formulario de inscripción actual si lo incluye.

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-022

**Dominio:** Encargados — Responsabilidades.

**Prioridad:** CRITICAL

**Pregunta:** ¿Qué responsabilidades tiene el encargado ante la institución (por ejemplo, pagos, asistencia, comunicaciones, retiro del estudiante)? ¿Debe dársele acceso al sistema o solo a datos?

**Por qué necesitamos saberlo:** Determina si el encargado interactúa con el sistema.

**Ejemplo de respuesta esperada:** Se busca saber qué papel juega el encargado y si necesita ver/consultar algo en el sistema. El ejemplo aclara el tipo de información (rol del encargado + necesidad de acceso); no decide si el encargado debe tener acceso.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

# Sesión 5 — Asistencia

### Q-023

**Dominio:** Asistencia — Registro.

**Prioridad:** HIGH

**Pregunta:** ¿Quién registra la asistencia y en qué momento del día se hace (entrada, cada clase, fin de jornada)? ¿Es por estudiante o por grupo?

**Por qué necesitamos saberlo:** Define quién usa la función de asistencia y cuándo.

**Ejemplo de respuesta esperada:** Se busca saber quién anota la asistencia, en qué momento y si se registra por cada estudiante o por grupo. El ejemplo aclara el tipo de información (responsable, momento, granularidad); no asume cómo se hace.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-024

**Dominio:** Asistencia — Estados.

**Prioridad:** HIGH

**Pregunta:** ¿Qué estados de asistencia usan (presente, ausente, tardanza, permiso, justificado, otro)? ¿Cómo se representa a un estudiante que no asiste?

**Por qué necesitamos saberlo:** Define el conjunto de estados de asistencia.

**Ejemplo de respuesta esperada:** Se busca saber qué situaciones de asistencia maneja la institución y cómo se marca la falta. El ejemplo aclara que se espera una lista de estados; no fija qué estados deben existir.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-025

**Dominio:** Asistencia — Reglas de negocio.

**Prioridad:** HIGH

**Pregunta:** ¿Qué reglas aplican a la asistencia (llegada tardía a partir de cuántos minutos, límite de faltas, cómo se justifica una falta y quién autoriza la justificación)?

**Por qué necesitamos saberlo:** Define lógica de negocio de asistencia.

**Ejemplo de respuesta esperada:** Se busca conocer las reglas internas que miden tardes, faltas y justificaciones, y quién las autoriza. El ejemplo aclara el tipo de información (reglas y responsable); no introduce reglas ni supone cuáles existen.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-026

**Dominio:** Asistencia — Correcciones.

**Prioridad:** HIGH

**Pregunta:** ¿Con qué frecuencia necesitan corregir o modificar una asistencia registrada por error y quién autoriza la corrección?

**Por qué necesitamos saberlo:** Define si se requiere edición controlada de asistencia.

**Ejemplo de respuesta esperada:** Se busca saber qué tan seguido se arregla una asistencia anotada mal y quién puede hacerlo. El ejemplo aclara el tipo de información (frecuencia y autoridad); no supone cuán frecuente es.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-027

**Dominio:** Asistencia — Reportes.

**Prioridad:** HIGH

**Pregunta:** ¿Qué reportes de asistencia necesitan (por ejemplo, resumen mensual por estudiante, por grupo, total de faltas) y quién los usa?

**Por qué necesitamos saberlo:** Define reportes de asistencia necesarios.

**Ejemplo de respuesta esperada:** Se busca saber qué resúmenes/listados de asistencia se requieren y quién los consulta. El ejemplo aclara el tipo de información (contenido del reporte + audiencia); no define qué reportes debe haber.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

# Sesión 6 — Pagos

### Q-028

**Dominio:** Pagos — Conceptos cobrados.

**Prioridad:** CRITICAL

**Pregunta:** ¿Qué conceptos se cobran a los estudiantes (por ejemplo, matrícula, mensualidad, cuotas, uniformes, otros) y en qué moneda?

**Por qué necesitamos saberlo:** Define los conceptos de cobro y la moneda del sistema.

**Ejemplo de respuesta esperada:** Se busca conocer qué cosas se cobran y en qué moneda. El ejemplo aclara el tipo de información (conceptos + moneda); no determina qué conceptos ni qué moneda.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING` — útil: tabla de aranceles/cobros si existe.

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-029

**Dominio:** Pagos — Periodicidad.

**Prioridad:** HIGH

**Pregunta:** ¿Con qué periodicidad se cobra cada concepto (mensual, trimestral, anual, único)? ¿Hay fechas límite de pago?

**Por qué necesitamos saberlo:** Define la periodicidad y los vencimientos de cobros.

**Ejemplo de respuesta esperada:** Se busca saber cada cuánto se cobra cada cosa y si hay fechas tope. El ejemplo aclara el tipo de información (frecuencia + vencimientos); no define periodicidades.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-030

**Dominio:** Pagos — Pagos parciales/Saldos.

**Prioridad:** CRITICAL

**Pregunta:** ¿Permiten pagos parciales de un concepto, abonos, o solo pagos completos? ¿Cómo manejan los saldos o deudas pendientes de un estudiante?

**Por qué necesitamos saberlo:** Define el manejo de abonos y saldos.

**Ejemplo de respuesta esperada:** Se busca saber si se aceptan abonos o pagos a plazos y cómo se registra lo que queda pendiente. El ejemplo aclara el tipo de información (modalidad de pago + tratamiento de la deuda); no asume si existen abonos.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-031

**Dominio:** Pagos — Forma de pago.

**Prioridad:** HIGH

**Pregunta:** ¿Cómo se reciben los pagos hoy (efectivo, transferencia, tarjeta, otro) y quién los recibe y registra?

**Por qué necesitamos saberlo:** Define cómo se ingresa y registra el pago.

**Ejemplo de respuesta esperada:** Se busca saber en qué modalidad se recibe el dinero y quién lo recibe/apunta. El ejemplo aclara el tipo de información (medios + responsable); no supone qué modalidad se usa.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-032

**Dominio:** Pagos — Recibos.

**Prioridad:** HIGH

**Pregunta:** ¿Emiten recibos, comprobantes o constancias de pago a los encargados? ¿Con qué formato (papel, digital) y qué datos deben tener?

**Por qué necesitamos saberlo:** Define la emisión de recibos y sus campos.

**Ejemplo de respuesta esperada:** Se busca saber si se entrega un comprobante de pago, en qué formato y qué lleva. El ejemplo aclara el tipo de información (si emiten recibo + formato + datos); no supone que se emitan recibos.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING` — útil: copia (anonimizada) de un recibo/constancia emitido.

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-033

**Dominio:** Pagos — Anulaciones.

**Prioridad:** CRITICAL

**Pregunta:** ¿Cómo manejan una anulación o corrección de un pago registrado por error, y quién lo autoriza?

**Por qué necesitamos saberlo:** Define el control de anulaciones de pagos.

**Ejemplo de respuesta esperada:** Se busca saber cómo se corrige un pago anotado mal y quién puede hacerlo. El ejemplo aclara el tipo de información (procedimiento + autoridad); no supone un procedimiento concreto.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-034

**Dominio:** Pagos — Historial.

**Prioridad:** HIGH

**Pregunta:** ¿Qué historial de pagos de un estudiante debe conservarse y por cuánto tiempo (por ejemplo, todos los años o solo el ciclo actual)?

**Por qué necesitamos saberlo:** Define retención y consulta del historial de pagos.

**Ejemplo de respuesta esperada:** Se busca saber qué historial de pagos se conserva y por cuánto tiempo. El ejemplo aclara el tipo de información (alcance + retención); no indica cuánto conservar.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-074

**Dominio:** Pagos — Descuentos.

**Prioridad:** HIGH

**Pregunta:** ¿Otorgan descuentos en los pagos a algunos estudiantes (por ejemplo, un porcentaje menor, un monto fijo, o solo sobre ciertos conceptos)?

**Por qué necesitamos saberlo:** Cita "descuentos" como decisión pendiente del modelo de pagos; no se asume que existan.

**Ejemplo de respuesta esperada:** Se busca saber si se aplican rebajas a algunos estudiantes y de qué tipo. El ejemplo aclara que la respuesta puede ser "no aplica" si no existen descuentos; no asume que los haya ni de qué tipo.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING` — útil: registro o documento de descuentos si existe.

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-075

**Dominio:** Pagos — Becas y exoneraciones.

**Prioridad:** HIGH

**Pregunta:** ¿Otorgan becas o exoneraciones de pago (total o parcial) a algunos estudiantes? ¿Cómo se deciden y quién las autoriza?

**Por qué necesitamos saberlo:** Define si existen becas/exoneraciones y su autorización, para modelar el saldo correctamente.

**Ejemplo de respuesta esperada:** Se busca saber si hay becas o exoneraciones y cómo se deciden. El ejemplo aclara que la respuesta puede ser "no aplica" si no existen; no asume que existan.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING` — útil: registro o documento de becas si existe.

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-076

**Dominio:** Pagos — Reglas de descuentos.

**Prioridad:** HIGH

**Pregunta:** Si se aplica un descuento, beca o exoneración, ¿qué reglas se siguen (por ejemplo, un solo descuento a la vez, sobre qué monto, y cómo afecta el saldo final que debe pagar el estudiante)?

**Por qué necesitamos saberlo:** Captura las reglas de negocio de los descuentos sin diseñar la solución.

**Ejemplo de respuesta esperada:** Se busca conocer las reglas internas cuando se aplica una rebaja o exoneración y cómo afecta lo que queda por pagar. El ejemplo aclara el tipo de información (reglas de aplicación), solo si existen; no introduce reglas.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

# Sesión 7 — Reportes

### Q-035

**Dominio:** Reportes — Uso actual.

**Prioridad:** HIGH

**Pregunta:** ¿Qué listados o reportes produce la institución hoy (por ejemplo, listas de estudiantes, reportes de asistencia, cobros, deudas, egresados)? ¿Cómo los generan actualmente (a mano, en Excel)?

**Por qué necesitamos saberlo:** Identifica reportes reales ya en uso para no inventarlos.

**Ejemplo de respuesta esperada:** Se busca enumerar qué listados se producen hoy y con qué medio. El ejemplo aclara el tipo de información (contenido + forma de generación); no presume qué reportes existen.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING` — útil: copias de los reportes/listados que generan hoy.

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-036

**Dominio:** Reportes — Formato.

**Prioridad:** HIGH

**Pregunta:** ¿En qué formato necesitan los reportes (impresos en papel, PDF, Excel, pantalla) y es necesario exportarlos/imprimirlos?

**Por qué necesitamos saberlo:** Define formato y exportación de salida.

**Ejemplo de respuesta esperada:** Se busca saber en qué presentación conviene recibir cada reporte y si se debe poder imprimir/exportar. El ejemplo aclara el tipo de información (formato/exportación); no fija un formato.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-037

**Dominio:** Reportes — Necesidades.

**Prioridad:** HIGH

**Pregunta:** ¿Qué información desearían consultar o imprimir que hoy no pueden obtener con facilidad?

**Por qué necesitamos saberlo:** Identifica reportes de valor real sin imponerlos como requisito.

**Ejemplo de respuesta esperada:** Se busca conocer datos que hoy cuesta obtener y que sería útil revisar. El ejemplo aclara que es una consulta de necesidades abiertas; no determina qué reportes se añadirán.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-038

**Dominio:** Reportes — Periodicidad/Destinatarios.

**Prioridad:** HIGH

**Pregunta:** ¿Con qué frecuencia se genera cada reporte y quiénes lo reciben o consultan (directora, docentes, encargados, otras autoridades)?

**Por qué necesitamos saberlo:** Define frecuencia, destinatarios y permisos de los reportes.

**Ejemplo de respuesta esperada:** Se busca saber con qué regularidad se produce cada reporte y quién lo usa. El ejemplo aclara el tipo de información (frecuencia + audiencia); no supone quién consume cada reporte.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

# Sesión 8 — Documentos

### Q-039

**Dominio:** Documentos — Contenido.

**Prioridad:** HIGH

**Pregunta:** ¿Qué documentos o papeles maneja y necesita conservar la institución (matrículas, actas de nacimiento, comprobantes de pago, comunicaciones, otras)? ¿Quiere guardarlos dentro del sistema?

**Por qué necesitamos saberlo:** Determina si el sistema almacena documentos digitales.

**Ejemplo de respuesta esperada:** Se busca enumerar qué papeles se manejan y si convendría guardarlos en el sistema. El ejemplo aclara el tipo de información (tipos de documento + preferencia); no decide si se guardan en el sistema.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING` — útil: ejemplos de los tipos de documentos que se guardan.

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-040

**Dominio:** Documentos — Formatos.

**Prioridad:** HIGH

**Pregunta:** ¿En qué formato están esos documentos hoy (papel, foto/escaneo, PDF, Excel, Word)?

**Por qué necesitamos saberlo:** Define formatos manejables al digitalizar.

**Ejemplo de respuesta esperada:** Se busca saber en qué presentación existen hoy esos papeles. El ejemplo aclara el tipo de información (formato físico/digital); no supone qué formatos se usan.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-041

**Dominio:** Documentos — Acceso.

**Prioridad:** HIGH

**Pregunta:** ¿Quién necesita acceder a cada tipo de documento y para qué (consulta, edición, impresión)?

**Por qué necesitamos saberlo:** Define permisos de acceso a documentos.

**Ejemplo de respuesta esperada:** Se busca saber quién consulta o modifica cada tipo de documento. El ejemplo aclara el tipo de información (persona + acción); no decide permisos.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-042

**Dominio:** Documentos — Retención.

**Prioridad:** HIGH

**Pregunta:** ¿Cuánto tiempo deben conservarse los documentos antes de que puedan eliminarse, y hay alguna norma o práctica interna al respecto?

**Por qué necesitamos saberlo:** Define política de retención/eliminación.

**Ejemplo de respuesta esperada:** Se busca saber cuánto tiempo se guarda cada documento y si hay una práctica al respecto. El ejemplo aclara el tipo de información (plazo + norma); no fija plazos.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

# Sesión 9 — Datos existentes

### Q-043

**Dominio:** Datos existentes — Inventario.

**Prioridad:** HIGH

**Pregunta:** ¿Qué datos se encuentran hoy en Excel u otros archivos (estudiantes, asistencia, pagos, matrícula, otros)? Enumere los archivos y su uso.

**Por qué necesitamos saberlo:** Inventario de datos a importar o consolidar.

**Ejemplo de respuesta esperada:** Se busca una relación de los archivos existentes y para qué se usan. El ejemplo aclara el tipo de información (inventario de archivos + uso); no supone qué archivos existen.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING` — útil: capturas o listado de los archivos existentes.

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-044

**Dominio:** Datos existentes — Calidad.

**Prioridad:** MEDIUM

**Pregunta:** En esos datos existentes, ¿hay duplicados, información incompleta o desactualizada? ¿Sabe aproximadamente cuántos registros en mal estado hay?

**Por qué necesitamos saberlo:** Define esfuerzo de limpieza y validación de datos.

**Ejemplo de respuesta esperada:** Se busca saber si los datos previos tienen errores o repeticiones y en qué medida. El ejemplo aclara el tipo de información (estado/calidad de los datos); no asume que haya errores.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-045

**Dominio:** Datos existentes — Fuente oficial.

**Prioridad:** MEDIUM

**Pregunta:** ¿Cuál es la fuente oficial de los datos de los estudiantes (el archivo más confiable y actualizado) que debe usarse como base para el sistema?

**Por qué necesitamos saberlo:** Identifica la fuente de verdad para la migración.

**Ejemplo de respuesta esperada:** Se busca saber cuál de los registros existentes es el más confiable y al día. El ejemplo aclara el tipo de información (fuente de referencia); no supone cuál es.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

# Sesión 10 — Seguridad y privacidad

### Q-049

**Dominio:** Seguridad — Acceso físico.

**Prioridad:** HIGH

**Pregunta:** ¿Quién tiene acceso físico a la computadora donde se ejecutará el sistema y a los archivos/registros? ¿Hay personas externas o no autorizadas cerca?

**Por qué necesitamos saberlo:** Define el nivel de control de acceso necesario.

**Ejemplo de respuesta esperada:** Se busca saber quién puede llegar físicamente al equipo y a los papeles. El ejemplo aclara el tipo de información (personas + entorno); no asume un nivel de riesgo.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-050

**Dominio:** Seguridad — Credenciales.

**Prioridad:** HIGH

**Pregunta:** ¿Cómo manejan hoy el acceso a los registros (cada usuario con sus credenciales, una cuenta compartida, archivos sin protección)? ¿Saben si prefieren que cada persona tenga su propio acceso o usan un acceso compartido?

**Por qué necesitamos saberlo:** Define el modelo de autenticación y roles.

**Ejemplo de respuesta esperada:** Se busca saber cómo se controla hoy el acceso y qué preferiría la institución. El ejemplo aclara el tipo de información (práctica actual + preferencia); no decide el modelo de acceso.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-051

**Dominio:** Seguridad — Información confidencial.

**Prioridad:** CRITICAL

**Pregunta:** ¿Qué información del sistema considera confidencial o sensible y que no debe ver cualquier usuario (salud, datos personales, historial de pagos, calificaciones, otro)?

**Por qué necesitamos saberlo:** Identifica datos a proteger y permisos restringidos.

**Ejemplo de respuesta esperada:** Se busca saber qué datos considera sensibles la institución y quiénes no deberían verlos. El ejemplo aclara el tipo de información (categorías de datos + restricción); no define qué debe ser confidencial.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-052

**Dominio:** Seguridad — Auditoría.

**Prioridad:** HIGH

**Pregunta:** ¿Requieren registrar quién hizo cada cambio importante (por ejemplo, quién modificó o eliminó un pago o un dato), o basta con que quede el dato actualizado?

**Por qué necesitamos saberlo:** Define si se necesita registro de auditoría.

**Ejemplo de respuesta esperada:** Se busca saber si importa dejar constancia de quién hizo cada cambio o si basta ver el valor final. El ejemplo aclara el tipo de decisión solicitada; no elige por la institución.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-053

**Dominio:** Seguridad — Necesidades de recuperación.

**Prioridad:** HIGH

**Pregunta:** Si se perdiera la información, ¿qué tan grave sería y cuánto tiempo aceptable tomaría recuperarla (por ejemplo, perder un día, un mes, el año completo)?

**Por qué necesitamos saberlo:** Define el nivel crítico de los datos y la política de respaldo.

**Ejemplo de respuesta esperada:** Se busca saber cuánta información podría tolerarse perder y en cuánto tiempo habría que recuperarla. El ejemplo aclara el tipo de dato (tolerancia a pérdida); no fija tolerancias.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-077

**Dominio:** Seguridad — Confidencialidad de datos.

**Prioridad:** HIGH

**Pregunta:** ¿Qué información de estudiantes y encargados considera confidencial (por ejemplo, salud, dirección, datos de pagos, otra) y a qué personas les está permitido verla?

**Por qué necesitamos saberlo:** Complementa Q-051 y Q-041 para delimitar qué información se protege y quién puede accederla.

**Ejemplo de respuesta esperada:** Se busca delimitar qué datos se resguardan y quiénes pueden consultarlos. El ejemplo aclara el tipo de información (dato + quién lo ve); no determina restricciones.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-078

**Dominio:** Seguridad — Políticas institucionales.

**Prioridad:** HIGH

**Pregunta:** ¿Existen políticas o normas internas de la institución sobre cómo guardar o compartir la información de los estudiantes? Si existen, ¿puede describirlas o compartirlas?

**Por qué necesitamos saberlo:** Identifica políticas existentes que el sistema debe respetar.

**Ejemplo de respuesta esperada:** Se busca saber si hay normas internas de manejo de datos. El ejemplo aclara que la respuesta puede ser "no aplica" si no existen; no asume que existan.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING` — útil: políticas/procedimientos escritos de datos si existen.

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-079

**Dominio:** Seguridad — Obligaciones de protección de datos.

**Prioridad:** HIGH

**Pregunta:** ¿La institución tiene alguna obligación o procedimiento de protección de datos que ya aplique (por ejemplo, autorizaciones firmadas por los encargados, avisos de privacidad, o límites sobre quién puede ver los datos)?

**Por qué necesitamos saberlo:** Detecta obligaciones y procedimientos existentes sobre datos; no se inventan obligaciones legales.

**Ejemplo de respuesta esperada:** Se busca saber si ya existen autorizaciones o procedimientos sobre los datos. El ejemplo aclara que la respuesta puede ser "no aplica" si no existen; no se asume obligación alguna.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING` — útil: autorizaciones/avisos de privacidad firmados si existen.

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-080

**Dominio:** Seguridad — Acceso autorizado.

**Prioridad:** HIGH

**Pregunta:** ¿Quién está autorizado a acceder a la información de los estudiantes y encargados, y quién no? ¿Hay datos que solo deba ver la directora, por ejemplo?

**Por qué necesitamos saberlo:** Define los límites de acceso por persona/rol.

**Ejemplo de respuesta esperada:** Se busca saber quién puede ver cada tipo de información y quién no. El ejemplo aclara el tipo de información (límites de acceso); no decide quién accede.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-081

**Dominio:** Seguridad — Restricciones y validación legal.

**Prioridad:** HIGH

**Pregunta:** ¿Existen restricciones que el sistema deba respetar sobre cómo se guardan o comparten estos datos? Si la institución no está segura de si existen obligaciones legales, indíquelo claramente.

**Por qué necesitamos saberlo:** Determina restricciones aplicables. Si no pueden confirmarse las obligaciones, se requerirá validación legal externa; este documento no brinda asesoría legal.

**Ejemplo de respuesta esperada:** Se busca saber si hay restricciones que respetar y si existe certeza sobre obligaciones legales. El ejemplo aclara que es válido responder "no se sabe"; este documento no asume obligaciones legales.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

# Sesión 11 — Backup y recuperación

### Q-054

**Dominio:** Backup — Contenido.

**Prioridad:** HIGH

**Pregunta:** ¿Qué información considera irremplazable y que debe estar respaldada (datos de estudiantes, pagos, asistencia, documentos)?

**Por qué necesitamos saberlo:** Define el contenido mínimo del respaldo.

**Ejemplo de respuesta esperada:** Se busca saber qué datos conviene conservar ante una pérdida. El ejemplo aclara el tipo de información (qué respaldar); no determina qué datos.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-055

**Dominio:** Backup — Frecuencia.

**Prioridad:** HIGH

**Pregunta:** ¿Con qué frecuencia desearían respaldar (diaria, semanal, mensual) considerando cuántos datos nuevos registran al día?

**Por qué necesitamos saberlo:** Define la frecuencia de respaldo adecuada.

**Ejemplo de respuesta esperada:** Se busca saber cada cuánto conviene guardar una copia, según cuánta información nueva se anota. El ejemplo aclara el tipo de información (frecuencia); no fija la frecuencia.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-056

**Dominio:** Backup — Destinos.

**Prioridad:** MEDIUM

**Pregunta:** ¿Qué destinos de respaldo hay disponibles (una memoria USB, otro disco, un servicio de nube, otra computadora)? ¿Puede almacenarse el respaldo fuera del equipo principal?

**Por qué necesitamos saberlo:** Determina dónde/con qué se guardan los respaldos.

**Ejemplo de respuesta esperada:** Se busca saber con qué lugares o dispositivos se cuenta para guardar copias. El ejemplo aclara el tipo de información (destinos disponibles); no supone qué destinos hay.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-057

**Dominio:** Backup — Responsable.

**Prioridad:** MEDIUM

**Pregunta:** ¿Qué persona sería responsable de verificar que los respaldos se realicen y estén al día?

**Por qué necesitamos saberlo:** Asigna la responsabilidad operativa de respaldos.

**Ejemplo de respuesta esperada:** Se busca identificar a la persona que cuidaría que las copias estén al día. El ejemplo aclara el tipo de información (responsable); no asume quién es.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-058

**Dominio:** Backup — Recuperación ante fallo.

**Prioridad:** MEDIUM

**Pregunta:** Si el sistema fallara o se perdiera un dato, ¿qué esperan poder hacer de inmediato para recuperar la información? ¿Quién realizaría esa recuperación?

**Por qué necesitamos saberlo:** Define el procedimiento esperado de restauración.

**Ejemplo de respuesta esperada:** Se busca saber qué se espera poder hacer ante una falla y quién la resolvería. El ejemplo aclara el tipo de información (expectativa de recuperación + responsable); no define un procedimiento.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-059

**Dominio:** Backup — Protocolo.

**Prioridad:** HIGH

**Pregunta:** ¿Qué haría la institución hoy si la computadora con sus datos se dañara o perdiera? ¿Existe algún plan o procedimiento ante ese incidente?

**Por qué necesitamos saberlo:** Identifica la brecha actual de continuidad de datos.

**Ejemplo de respuesta esperada:** Se busca saber qué se hace hoy ante un fallo del equipo y si hay un plan. El ejemplo aclara que la respuesta puede ser "no hay plan"; no asume que exista uno.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

# Sesión 12 — Infraestructura

### Q-060

**Dominio:** Infraestructura — Hardware.

**Prioridad:** HIGH

**Pregunta:** ¿Con qué computadora cuenta la institución para ejecutar el sistema, y qué sistema operativo tiene (Windows, macOS, Linux)? ¿Cuántos usuarios la usarían a la vez?

**Por qué necesitamos saberlo:** Define compatibilidad y requisitos de instalación.

**Ejemplo de respuesta esperada:** Se busca conocer el equipo y su sistema operativo, y cuántas personas lo usarían al mismo tiempo. El ejemplo aclara el tipo de información (hardware + SO + usuarios simultáneos); no asume ningún equipo.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-061

**Dominio:** Infraestructura — Conectividad.

**Prioridad:** HIGH

**Pregunta:** ¿Tiene la institución acceso a internet? ¿Con qué frecuencia o en qué momentos está disponible? Cuando no hay internet, ¿qué hace actualmente con su información para no perderla?

**Por qué necesitamos saberlo:** Determina la disponibilidad de conexión y cómo afecta el trabajo diario; la decisión sobre si funcionar sin conexión es interna, no debe inducirse al responder.

**Ejemplo de respuesta esperada:** Se busca saber si hay conexión, con qué regularidad, y cómo se trabaja cuando no la hay. El ejemplo aclara el tipo de información (disponibilidad de red + práctica actual); no sugiere soluciones ni modo de operación.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-062

**Dominio:** Infraestructura — Restricciones técnicas.

**Prioridad:** MEDIUM

**Pregunta:** ¿Existen restricciones técnicas o de seguridad (por ejemplo, políticas de la escuela o de una entidad reguladora) sobre qué programas pueden instalarse o cómo se guardan los datos de estudiantes?

**Por qué necesitamos saberlo:** Determina limitaciones de instalación y almacenamiento.

**Ejemplo de respuesta esperada:** Se busca saber si hay reglas sobre qué se puede instalar o cómo guardar datos. El ejemplo aclara que la respuesta puede ser "no hay restricciones"; no asume que existan.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-063

**Dominio:** Infraestructura — Acceso físico.

**Prioridad:** CRITICAL

**Pregunta:** ¿El equipo se encuentra en la institución o en la casa de alguien? ¿Quién lo resguarda y en qué horario se usa?

**Por qué necesitamos saberlo:** Confirma el despliegue on-premise y sus condiciones.

**Ejemplo de respuesta esperada:** Se busca saber dónde está el equipo, quién lo cuida y cuándo se usa. El ejemplo aclara el tipo de información (ubicación + custodia + uso); no supone dónde está.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

# Sesión 13 — Operación y mantenimiento

### Q-064

**Dominio:** Operación — Administración.

**Prioridad:** MEDIUM

**Pregunta:** ¿Qué persona administrará el sistema a diario (mantener datos al día, crear usuarios, corregir errores)?

**Por qué necesitamos saberlo:** Define responsabilidad administrativa y de soporte.

**Ejemplo de respuesta esperada:** Se busca identificar a la persona que mantendría el sistema al día. El ejemplo aclara el tipo de información (rol administrativo); no asume quién es.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-066

**Dominio:** Operación — Continuidad.

**Prioridad:** LOW

**Pregunta:** Si el desarrollador original no estuviera disponible, ¿cómo podría la institución seguir actualizando o reparando el sistema? ¿Existe alguien que dé soporte técnico?

**Por qué necesitamos saberlo:** Define estrategia de handover y mantenibilidad.

**Ejemplo de respuesta esperada:** Se busca saber cómo se mantendría el sistema sin el desarrollador original. El ejemplo aclara que la respuesta puede ser que aún no se ha pensado; no asume un plan.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-067

**Dominio:** Operación — Actualizaciones.

**Prioridad:** LOW

**Pregunta:** ¿Qué entienden por "actualizar el sistema" (corregir errores, sumar funciones, pasar de año lectivo) y con qué frecuencia lo esperan?

**Por qué necesitamos saberlo:** Define el alcance y cadencia de las actualizaciones.

**Ejemplo de respuesta esperada:** Se busca saber qué espera la institución cuando menciona "actualizar" y con qué ritmo. El ejemplo aclara el tipo de información (definición + frecuencia); no define el alcance de las actualizaciones.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

# Sesión 14 — Alcance V1 y criterios de aceptación

### Q-068

**Dominio:** Alcance / Datos existentes.

**Prioridad:** CRITICAL

**Pregunta:** Para la primera versión, ¿partirá el sistema desde cero (registrando estudiantes nuevos) o debe incluir información ya existente (por ejemplo, la matrícula del año en curso)?

**Por qué necesitamos saberlo:** Define qué datos requiere V1 y si hay migración.

**Ejemplo de respuesta esperada:** Se busca saber si la primera versión debe arrancar con datos ya existentes o en blanco. El ejemplo aclara el tipo de decisión solicitada; no elige por la institución.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-069

**Dominio:** Alcance / Prioridades.

**Prioridad:** HIGH

**Pregunta:** De las funciones (estudiantes, matrícula, asistencia, pagos, reportes, respaldos, documentos), ¿cuál considera indispensable desde el primer día y cuál podría esperar?

**Por qué necesitamos saberlo:** Define la prioridad y alcance del MVP/V1.

**Ejemplo de respuesta esperada:** Se busca conocer qué funciones se necesitan primero y cuáles pueden esperar. El ejemplo aclara el tipo de decisión solicitada; no define qué va primero.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-070

**Dominio:** Alcance / Gobernanza.

**Prioridad:** CRITICAL

**Pregunta:** ¿Existe un documento oficial o maestro del proyecto más allá de la visión breve (docs/Vision.md), o este documento puede servir como fuente definitiva? ¿Quién lo aprueba o valida?

**Por qué necesitamos saberlo:** Confirma cuál es la fuente de verdad y el responsable de aprobación.

**Ejemplo de respuesta esperada:** Se busca saber si hay un documento maestro del proyecto y quién lo aprueba. El ejemplo aclara el tipo de información (fuente de verdad + aprobador); no asume que exista un documento.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING` — útil: documento maestro del proyecto si existe.

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-082

**Dominio:** Alcance — Calidad / Aceptación.

**Prioridad:** MEDIUM

**Pregunta:** ¿Cómo sabrían que el sistema funciona correctamente y está listo para usarse normalmente? ¿Qué resultados esperan ver en su día a día?

**Por qué necesitamos saberlo:** Registra como desconocidos los criterios de aceptación; revela qué significa "funciona bien" para la institución.

**Ejemplo de respuesta esperada:** Se busca saber qué resultados diarios le dirían a la institución que el sistema sirve. El ejemplo aclara el tipo de información (señales de buen funcionamiento); no define criterios.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-083

**Dominio:** Alcance — Procesos críticos.

**Prioridad:** MEDIUM

**Pregunta:** ¿Qué procesos consideran críticos y qué errores serían inaceptables en el uso diario (por ejemplo, perder un pago, no registrar asistencia, equivocar datos de un estudiante)?

**Por qué necesitamos saberlo:** Identifica procesos críticos y errores a evitar en V1, sin convertirlos en pruebas todavía.

**Ejemplo de respuesta esperada:** Se busca saber qué es lo más importante de no fallar en el uso diario. El ejemplo aclara el tipo de información (procesos críticos); los ejemplos del enunciado son ilustrativos, no se asumen.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-084

**Dominio:** Alcance — Condiciones de aceptación.

**Prioridad:** MEDIUM

**Pregunta:** ¿Qué condiciones mínimas deberían cumplirse para que consideren aceptable la primera versión del sistema (por ejemplo, poder registrar estudiantes, registrar asistencia, cobrar y ver reportes básicos)?

**Por qué necesitamos saberlo:** Define el umbral de aceptación de V1 desde la perspectiva institucional.

**Ejemplo de respuesta esperada:** Se busca saber qué debería poder hacer la primera versión para aceptarse. El ejemplo aclara el tipo de información (condiciones mínimas); los ejemplos son ilustrativos, no se asumen como requisito.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

### Q-085

**Dominio:** Alcance — Gobernanza / Patrocinador.

**Prioridad:** LOW

**Pregunta:** ¿Quién es la persona responsable o patrocinadora del proyecto por parte de la institución, con autoridad para validar las decisiones y aceptar la entrega del sistema?

**Por qué necesitamos saberlo:** Requiere identificar al responsable que valida decisiones y acepta la entrega.

**Ejemplo de respuesta esperada:** Se busca identificar a la persona autorizada en la institución para aprobar decisiones y la entrega. El ejemplo aclara el tipo de información (rol/patrocinador); no asume quién es.

**Respuesta institucional:** `PENDING`

**Evidencia disponible:** `PENDING`

**Respondido por:** `PENDING`

**Fecha:** `PENDING`

---

## Notas de cierre

- Este paquete contiene las **83 preguntas activas** (Q-001…Q-085, excepto Q-046 y Q-065, retiradas).
- **IDS retirados no reutilizados:** Q-046 (consolidada en Q-003/Q-048) y Q-065 (bajo valor); no aparecen en este documento.
- Cada pregunta conserva su **ID original**, su **dominio** y su **prioridad** sin cambios.
- Todas las respuestas permanecen en `PENDING` hasta que la institución las responda.
- La fuente de verdad sigue siendo `docs/00-foundation/institutional-discovery.md`. Este paquete se usa
  solo como instrumento de entrevista; no reemplaza ni modifica el cuestionario maestro.
- No se ha introducido ningún requisito, solución, arquitectura, base de datos ni tecnología.
- No se emite `FOUNDATION READY`; el proyecto continúa en Discovery hasta completar el diálogo
  institucional y resolver las preguntas pendientes.

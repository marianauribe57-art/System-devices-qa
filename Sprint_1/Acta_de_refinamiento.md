# Acta de refinamiento · Sprint 1 · Grupo 3

> **PARCIAL** – contiene las preguntas de HU-010. Cada responsable agrega las de su HU en su propia rama.

[Volver al índice](../README.md)

| Campo | Valor |
|---|---|
| Fecha | ___ |
| Participantes | Mariana Uribe Muñoz, Davier, Diego, Ismael · Product Owner: instructor Carlos Navia |
| Objetivo | Aclarar las dudas que afectan el diseño antes de comprometer cada HU (DoR, punto 4) |

> **Regla (guía EV05, Fase 2):** no convertir una suposición en requisito. Mientras el PO no responda, cada pregunta lleva una **interpretación provisional** con la que se diseña, y queda registrada.

## HU-010 Consultar el listado de usuarios · Responsable: Mariana Uribe Muñoz

| ID | Pregunta para el Product Owner | Por qué importa (origen) | Interpretación provisional | Respuesta del PO |
|---|---|---|---|---|
| PA-01 | ¿Qué valores tiene el filtro **estado**? La ficha no los enumera. | CA-HU-010-01 · regla 29 | Se usan «activa» (HU-001 crea cuentas activas) y un segundo valor distinto, que se confirma antes de ejecutar. | ___ |
| PA-02 | ¿Rol y estado son **obligatorios** para consultar, o existe una opción «todos»? | CA-HU-010-01 habla de seleccionar «un rol y un estado» | Se prueba siempre con un rol y un estado seleccionados. La opción «todos» queda fuera hasta que se defina. | ___ |
| PA-03 | ¿Cambiar el **orden** (campo o sentido) ejecuta la consulta de inmediato, o también requiere pulsar el botón? | La regla 30 habla de filtros; CA-HU-010-02 no menciona el botón | Se verifica solo el resultado ordenado. No se afirma si el cambio de orden genera o no una solicitud. | ___ |
| PA-04 | ¿Qué **columnas** muestra el listado (nombre, correo, rol, estado, fecha de alta)? | La ficha menciona nombre, fecha de alta, rol y estado, pero no lista columnas | Se verifican rol, estado, nombre y fecha de alta, porque los usan filtros y orden. | ___ |
| PA-05 | ¿Cómo se **destaca** la cuenta actual? ¿Tiene un texto o indicador que lea el lector de pantalla? | CA-HU-010-03 · RNF-004 | Se acepta cualquier marca visible que la distinga de las demás filas; para RNF-004 se verifica que el lector la anuncie. | ___ |
| PA-06 | El límite de **30 consultas por minuto**, ¿se cuenta por sesión, por persona o en total? ¿Cuentan las consultas rechazadas o las de la recarga (CA-06)? | CA-HU-010-07 · RNF-006 | Se cuenta en total, desde una sola sesión, en un minuto sin otras consultas. | ___ |
| PA-07 | ¿Qué **mensaje** informa el exceso de consultas? | CA-HU-010-07 dice «informa la situación» sin el texto | No se inventa el texto: se verifica que exista un aviso de rechazo y que no se muestren resultados nuevos. | ___ |
| PA-08 | Al ordenar por **nombre**, ¿cómo se ordenan las tildes, las mayúsculas y los nombres repetidos? | CA-HU-010-02 | Los datos de prueba usan nombres sin empates ni tildes al inicio. | ___ |

## HU-011 Crear usuarios desde el servicio · Responsable: Davier

| ID | Pregunta para el Product Owner | Por qué importa (origen) | Interpretación provisional | Respuesta del PO |
|---|---|---|---|---|
| PA-01 | | | | |

## HU-012 Actualizar usuarios desde el servicio · Responsable: Davier

| ID | Pregunta para el Product Owner | Por qué importa (origen) | Interpretación provisional | Respuesta del PO |
|---|---|---|---|---|
| PA-01 | | | | |

## HU-013 Eliminar usuarios sin préstamos · Responsable: Ismael

| ID | Pregunta para el Product Owner | Por qué importa (origen) | Interpretación provisional | Respuesta del PO |
|---|---|---|---|---|
| PA-01 | | | | |

## HU-022 Consultar el historial de un usuario · Responsable: Diego

| ID | Pregunta para el Product Owner | Por qué importa (origen) | Interpretación provisional | Respuesta del PO |
|---|---|---|---|---|
| PA-01 | | | | |

## HU-024 Consultar Mis préstamos · Responsable: Diego

| ID | Pregunta para el Product Owner | Por qué importa (origen) | Interpretación provisional | Respuesta del PO |
|---|---|---|---|---|
| PA-01 | | | | |

## Decisiones del refinamiento

| N.º | Decisión | HU | Registrada por |
|---:|---|---|---|
| 1 | | | |

# Mapa de riesgos · Grupo 3

> **BORRADOR – pendiente de validación del equipo**

[Volver al índice](../README.md)

Cada riesgo sale de una regla, un CA o un RNF de las fichas. La **prioridad** de todas las HU del grupo es **Alta** según sus fichas. El **impacto** se apoya en la ficha. La **probabilidad** es una **estimación propuesta** (las fichas no la indican), con su razón en la última columna, para que el equipo la confirme o la ajuste.

**Escala:** Impacto y Probabilidad de 1 (bajo) a 5 (alto) · **Severidad = Impacto × Probabilidad**
**Nivel:** 🔴 Crítico (15–25) · 🟠 Alto (8–14) · 🟡 Medio (1–7)

| ID | Riesgo | Origen en la ficha | HU afectadas | Impacto | Prob. | Severidad | Nivel | Prioridad | Razón de la probabilidad propuesta |
|---|---|---|---|:-:|:-:|:-:|:-:|---|---|
| R-04 | Se elimina un usuario que solo tiene préstamos devueltos (historial) | RN-006 · CA-HU-013-03 · RNF-003 | HU-013 | 5 | 4 | 20 | 🔴 | Alta | Es fácil confundir «sin préstamos activos» con «sin historial»; la guía EV05 usa este caso como ejemplo de lectura |
| R-02 | Se consultan datos protegidos sin sesión vigente (o con sesión inválida) | RNF-002 / CC-003 · CA-HU-010-04 · CA-HU-024-04 | HU-010, HU-024 | 5 | 3 | 15 | 🔴 | Alta | RNF-002 advierte que ocultar la opción del menú no sustituye la comprobación en el servicio |
| R-03 | Se crea o asigna un correo que ya usa otra cuenta | RN-001 · CA-HU-011-02 · CA-HU-012-03 | HU-011, HU-012 | 4 | 3 | 12 | 🟠 | Alta | La validación suele existir al crear, pero puede faltar al actualizar el correo de otra cuenta |
| R-06 | Una actualización parcial borra campos que no se enviaron | CA-HU-012-02 | HU-012 | 4 | 3 | 12 | 🟠 | Alta | Actualización completa y parcial se confunden con facilidad en un mismo servicio |
| R-01 | Se muestran contraseñas legibles en listados, respuestas o almacenamiento | RNF-001 / CC-001 | HU-010, HU-011, HU-012 | 5 | 2 | 10 | 🟠 | Alta | Es un requisito explícito, pero una respuesta del servicio puede incluir el campo sin querer |
| R-07 | Se mezclan préstamos de otra persona o de otra sesión | CA-HU-022-02 · CA-HU-024-02 | HU-022, HU-024 | 5 | 2 | 10 | 🟠 | Alta | Ocurre al cambiar de usuario consultado o al compartir equipo entre dos sesiones |
| R-08 | Un fallo de consulta se presenta como lista vacía (o al revés) | CA-HU-010-05 · CA-HU-022-05 · CA-HU-024-05 · RF-029 | HU-010, HU-022, HU-024 | 3 | 3 | 9 | 🟠 | Alta | Tres fichas lo piden explícitamente; es un error común en pantallas de listados |
| R-09 | El límite de 30 consultas de usuarios por minuto no se aplica o rechaza antes de tiempo | RNF-006 / CC-011–012 · CA-HU-010-07 | HU-010 | 3 | 3 | 9 | 🟠 | Alta | El conteo por minuto tiene detalles sin definir en la ficha (ver PA-06 del acta) |
| R-05 | Una solicitud rechazada modifica registros existentes | CA-HU-011-02 · CA-HU-012-04/05/06 · CA-HU-013-02/04 · RNF-003 | HU-011, HU-012, HU-013 | 4 | 2 | 8 | 🟠 | Alta | Los rechazos validan antes de guardar; el riesgo está en validaciones hechas a medias |
| R-11 | Las fechas se muestran en hora universal como si fueran locales | RNF-007 / CC-013 | HU-010, HU-022, HU-024 | 2 | 4 | 8 | 🟠 | Alta | La conversión de zona horaria se omite con frecuencia; RNF-007 lo advierte en su restricción |
| R-10 | Los filtros del listado se pierden al recargar, abrir el enlace o usar Atrás | CA-HU-010-06 · RF-027 | HU-010 | 2 | 3 | 6 | 🟡 | Alta | Depende de otra historia (HU-027) que debe estar integrada |
| R-13 | La consulta pública del historial exige sesión o se confunde con Mis préstamos | CA-HU-022-04 · regla 21 de HU-022 | HU-022, HU-024 | 3 | 2 | 6 | 🟡 | Alta | Las dos consultas muestran préstamos de una persona y pueden compartir lógica |
| R-12 | La respuesta del servicio no permite identificar la atención (identificador, versión, tiempo) | RNF-008 / CC-014 | HU-011, HU-012, HU-013 | 2 | 2 | 4 | 🟡 | Alta | Es un requisito transversal que suele resolverse una sola vez para todo el servicio |

> La tabla está ordenada de mayor a menor severidad: los riesgos 🔴 son los que se prueban primero.

## Resumen por HU

| HU | Riesgos | Riesgo más alto |
|---|---|---|
| HU-010 | R-01, R-02, R-08, R-09, R-10, R-11 | R-02 🔴 |
| HU-011 | R-01, R-03, R-05, R-12 | R-03 🟠 |
| HU-012 | R-01, R-03, R-05, R-06, R-12 | R-03 · R-06 🟠 |
| HU-013 | R-04, R-05, R-12 | R-04 🔴 |
| HU-022 | R-07, R-08, R-11, R-13 | R-07 🟠 |
| HU-024 | R-02, R-07, R-08, R-11, R-13 | R-02 🔴 |

## Para validar en equipo

- [ ] Confirmar o ajustar la probabilidad propuesta y el impacto de cada riesgo.
- [ ] Agregar los riesgos que cada responsable encuentre al analizar su HU.

# System-devices-qa · Grupo 3 «Usuarios e historial personal»

Repositorio de diseño de pruebas por historia de usuario del proyecto **Device Systems**.
Evidencia **GA-220501096-05-EV05 – Diseño de pruebas por historia de usuario con Scrum** · Competencia 220501096 *Pruebas de Software y SCRUM* · Ficha 3229209 · Instructor Carlos Navia.

| Enlace | Dónde |
|---|---|
| GitHub Project (tablero) | [System-devices-qa · Grupo 3 · Sprint 1](https://github.com/users/marianauribe57-art/projects/4) |
| Fichas de las HU | `Historias_de_Usuario_Device_Systems.pdf` (Classroom de la evidencia EV05) |
| Guía para integrantes | [GUIA_EQUIPO.md](GUIA_EQUIPO.md) |
| Organización del equipo | [00_Organizacion](00_Organizacion/) |
| Planificación del Sprint 1 | [Sprint_1](Sprint_1/) |

**Revisión cruzada (guía EV05):** al Grupo 3 lo revisa el **Grupo 2**; el Grupo 3 revisa las HU del **Grupo 4**.

## Índice de historias de usuario

| HU | Nombre | Módulo de origen | Responsable | Revisor (Grupo 2) | Carpeta | Issue |
|---|---|---|---|---|---|---|
| HU-010 | Consultar el listado de usuarios | Usuarios e inventario (`USR`) | Mariana Uribe Muñoz | Pendiente | [Proceso_Pruebas_HU-010](02_Usuarios_e_inventario/Proceso_Pruebas_HU-010_Consultar_el_listado_de_usuarios/) | [#1](https://github.com/marianauribe57-art/System-devices-qa/issues/1) |
| HU-011 | Crear usuarios desde el servicio | Usuarios e inventario (`USR`) | Davier Andrés Quinto Bejarano (líder) | Pendiente | [Proceso_Pruebas_HU-011](02_Usuarios_e_inventario/Proceso_Pruebas_HU-011_Crear_usuarios_desde_el_servicio/) | [#2](https://github.com/marianauribe57-art/System-devices-qa/issues/2) |
| HU-012 | Actualizar usuarios desde el servicio | Usuarios e inventario (`USR`) | Davier Andrés Quinto Bejarano (líder) | Pendiente | [Proceso_Pruebas_HU-012](02_Usuarios_e_inventario/Proceso_Pruebas_HU-012_Actualizar_usuarios_desde_el_servicio/) | [#3](https://github.com/marianauribe57-art/System-devices-qa/issues/3) |
| HU-013 | Eliminar usuarios sin préstamos | Usuarios e inventario (`USR`) | Ismael Mira Correa | Pendiente | [Proceso_Pruebas_HU-013](02_Usuarios_e_inventario/Proceso_Pruebas_HU-013_Eliminar_usuarios_sin_prestamos/) | [#4](https://github.com/marianauribe57-art/System-devices-qa/issues/4) |
| HU-022 | Consultar el historial de un usuario | Préstamos y experiencia (`PRE`) | Diego Andrés Rojas Quintero | Pendiente | [Proceso_Pruebas_HU-022](03_Prestamos_y_experiencia/Proceso_Pruebas_HU-022_Consultar_el_historial_de_un_usuario/) | [#5](https://github.com/marianauribe57-art/System-devices-qa/issues/5) |
| HU-024 | Consultar Mis préstamos | Préstamos y experiencia (`PRE`) | Diego Andrés Rojas Quintero | Pendiente | [Proceso_Pruebas_HU-024](03_Prestamos_y_experiencia/Proceso_Pruebas_HU-024_Consultar_Mis_prestamos/) | [#6](https://github.com/marianauribe57-art/System-devices-qa/issues/6) |

> Las carpetas de módulo siguen las tres secciones del PDF de fichas: *Acceso y sesión · Usuarios e inventario · Préstamos y experiencia*. HU-022 y HU-024 pertenecen a Préstamos (HU-018 a HU-024).

## Estructura

```text
System-devices-qa/
├── README.md                     ← este índice
├── GUIA_EQUIPO.md                ← paso a paso para cada integrante
├── 00_Organizacion/              ← ficha, asignación, riesgos, tipos, alcance, DoR, DoD
├── Sprint_1/                     ← acta, estimaciones, capacidad, Sprint Backlog
├── 02_Usuarios_e_inventario/     ← HU-010, HU-011, HU-012, HU-013
└── 03_Prestamos_y_experiencia/   ← HU-022, HU-024
```

## Reglas del repositorio

- Cada HU se publica en su propia rama `qa/hu-0XX` y entra a `main` solo mediante Pull Request revisada.
- Solo datos y cuentas **ficticias**: nada de Excel, identificaciones, notas, credenciales ni datos reales.
- Mientras no exista una corrida real, los casos quedan en **«No ejecutado»**. No se inventan capturas, defectos ni resultados.

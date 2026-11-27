# Alcance de pruebas · Grupo 3 · Sprint 1

> **BORRADOR – pendiente de validación del equipo**

[Volver al índice](../README.md)

## Objetivo de diseño del Sprint (propuesta)

Diseñar un banco de pruebas trazable (CA → escenario → caso → dato → script) para las 6 HU del Grupo 3, revisado por el Grupo 2 e integrado en `main`.

## Dentro del alcance

| Elemento | Detalle |
|---|---|
| Historias | HU-010, HU-011, HU-012, HU-013, HU-022, HU-024 |
| Criterios | Todos los CA de cada ficha, con su identificador original |
| Condiciones de calidad | Solo los RNF que la ficha de cada HU declara como aplicables (ver [Matriz de tipos](Matriz_tipos_de_prueba.md)) |
| Artefactos | Preparación (1.1–1.4) e Implementación (2.1–2.7) de la plantilla |
| Revisión | Revisión por pares del Grupo 2 (2.7) y revisión de las HU del Grupo 4 |

## Fuera del alcance

| Elemento | Razón (fuente) |
|---|---|
| Ejecución real de los casos | El diseño no exige una instalación funcional de Device Systems (guía, Ambiente requerido). Se marca «No ejecutado». |
| Fases 03 Ejecución y 04 Evaluación | Se conservan con la plantilla para continuar el Tema 6 (guía, Fase 5) |
| Paginación del listado de usuarios | Regla 31 de HU-010 |
| Pantallas web administrativas para crear, actualizar o eliminar usuarios | Reglas de HU-011, HU-012, HU-013 |
| Aprobación excepcional para eliminar usuarios con historial | Regla 22 de HU-013 |
| HU de otros grupos | Solo se usan como dependencia o precondición (por ejemplo, HU-002, HU-027, HU-029) |
| Datos reales, cuentas reales o credenciales | Guía EV05, Fase 1 |
| Pruebas de carga o rendimiento distintas del límite de 30 consultas/min | No aparecen en las fichas del grupo |

## Para validar en equipo

- [ ] Confirmar el objetivo de diseño del Sprint.
- [ ] Comparar el alcance con la capacidad (ver [Capacidad_QA](../Sprint_1/Capacidad_QA.md)). Si no alcanza, las HU restantes quedan en el backlog (regla de carga de la guía).

# Matriz de tipos de prueba por módulo · Grupo 3

> **BORRADOR – pendiente de validación del equipo**

[Volver al índice](../README.md)

## 1. Tipo de acceso según la ficha

La guía pide distinguir **pantallas, servicios y consultas públicas o restringidas**.

| HU | Módulo | Cómo se usa | Acceso | Fuente |
|---|---|---|---|---|
| HU-010 | Usuarios (`USR`) | Pantalla web «Usuarios» | Restringido: exige sesión vigente | Ficha HU-010 · RNF-002 |
| HU-011 | Usuarios (`USR`) | Solo servicio, sin pantallas web | Ficha y RNF-002 no definen una restricción de rol | Ficha HU-011 · RNF-002 (restricciones) |
| HU-012 | Usuarios (`USR`) | Solo servicio, sin pantallas web | Ficha y RNF-002 no definen una restricción de rol | Ficha HU-012 · RNF-002 (restricciones) |
| HU-013 | Usuarios (`USR`) | Solo servicio, sin pantallas web | Ficha y RNF-002 no definen una restricción de rol | Ficha HU-013 · RNF-002 (restricciones) |
| HU-022 | Préstamos (`PRE`) | Pantalla relacionada o consulta del servicio | Público: no exige iniciar sesión | Ficha HU-022 · CA-HU-022-04 |
| HU-024 | Préstamos (`PRE`) | Pantalla web «Mis préstamos» | Restringido: identidad de la sesión | Ficha HU-024 · RNF-002 |

## 2. Tipos de prueba que aplican

✅ = aplica según la ficha · — = no aplica

| Tipo de prueba | RNF | HU-010 | HU-011 | HU-012 | HU-013 | HU-022 | HU-024 |
|---|---|:-:|:-:|:-:|:-:|:-:|:-:|
| Funcional · caja negra (CA de la ficha) | — | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Confidencialidad de contraseñas | RNF-001 | ✅ | ✅ | ✅ | — | — | — |
| Permisos (sesión y rol) | RNF-002 | ✅ | — | — | — | — | ✅ |
| Conservación y consistencia de datos | RNF-003 | — | ✅ | ✅ | ✅ | ✅ | ✅ |
| Accesibilidad (teclado, lector de pantalla) | RNF-004 | ✅ | — | — | — | — | — |
| Adaptación a pantallas (computador y móvil) | RNF-005 | ✅ | — | — | — | ✅ | ✅ |
| Límites de uso | RNF-006 | ✅ (30/min) | — | — | — | — | — |
| Presentación de fechas | RNF-007 | ✅ | — | — | — | ✅ | ✅ |
| Seguimiento de operaciones | RNF-008 | — | ✅ | ✅ | ✅ | — | — |

> Los ✅ siguen las «Condiciones de calidad aplicables» de cada ficha. La guía pide **no** asignar los ocho RNF a todas las HU.
> RNF-004 y RNF-005 no aplican a HU-011, HU-012 y HU-013 porque la ficha del RNF indica que no se crean pantallas para esas capacidades del servicio.

## 3. Nivel y enfoque

| Elemento | Decisión propuesta |
|---|---|
| Nivel | Sistema y aceptación (se prueba contra los CA de la ficha) |
| Enfoque | Caja negra: se diseña desde el comportamiento especificado, sin acceso al código |
| Ejecución | Scripts manuales. La guía no exige una instalación funcional de Device Systems |
| Herramientas posibles al ejecutar | Navegador con herramientas de desarrollador (pantallas) · Postman (servicio) · lector de pantalla (RNF-004) |

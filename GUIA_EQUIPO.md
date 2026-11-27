# Guía para el equipo · cómo subir tu HU

[Volver al índice](README.md)

La calificación es **individual**: cada persona diseña **solo su HU**, en **su propia rama**, y la publica con **su propia Pull Request (PR)**. Así el instructor puede ver qué hizo cada uno.

| Integrante | Tu HU | Tu rama | Tu carpeta |
|---|---|---|---|
| Davier Andrés Quinto Bejarano | HU-011 | `qa/hu-011` | `02_Usuarios_e_inventario/Proceso_Pruebas_HU-011_Crear_usuarios_desde_el_servicio/` |
| Davier Andrés Quinto Bejarano | HU-012 | `qa/hu-012` | `02_Usuarios_e_inventario/Proceso_Pruebas_HU-012_Actualizar_usuarios_desde_el_servicio/` |
| Ismael Mira Correa | HU-013 | `qa/hu-013` | `02_Usuarios_e_inventario/Proceso_Pruebas_HU-013_Eliminar_usuarios_sin_prestamos/` |
| Diego Andrés Rojas Quintero | HU-022 | `qa/hu-022` | `03_Prestamos_y_experiencia/Proceso_Pruebas_HU-022_Consultar_el_historial_de_un_usuario/` |
| Diego Andrés Rojas Quintero | HU-024 | `qa/hu-024` | `03_Prestamos_y_experiencia/Proceso_Pruebas_HU-024_Consultar_Mis_prestamos/` |
| Mariana | HU-010 | `qa/hu-010` | `02_Usuarios_e_inventario/Proceso_Pruebas_HU-010_Consultar_el_listado_de_usuarios/` |

> Si tienes **dos HU** (Davier y Diego), haces todo **dos veces**: una rama y una PR por cada HU. No mezcles las dos HU en la misma rama.

En los pasos uso **HU-011** como ejemplo. Cámbialo por tu número.

---

## Paso 1 · Aceptar la invitación

1. Revisa el correo de tu cuenta de GitHub o entra a <https://github.com/notifications>.
2. Abre la invitación a **System-devices-qa** y pulsa **Accept invitation**.

## Paso 2 · Clonar el repositorio (descargarlo a tu computador)

Abre **Git Bash** en la carpeta donde guardas tus proyectos y ejecuta:

```bash
git clone https://github.com/marianauribe57-art/System-devices-qa.git
cd System-devices-qa
```

| Comando | Qué hace |
|---|---|
| `git clone <url>` | Copia el repositorio de GitHub a tu computador |
| `cd System-devices-qa` | Entra a la carpeta que se acaba de crear |

## Paso 3 · Crear TU rama

```bash
git checkout main
git pull
git checkout -b qa/hu-011
```

| Comando | Qué hace |
|---|---|
| `git checkout main` | Se ubica en la rama principal |
| `git pull` | Trae los últimos cambios de GitHub, para empezar desde la versión más reciente |
| `git checkout -b qa/hu-011` | Crea tu rama y se pasa a ella (`-b` = crear) |

Para comprobar en qué rama estás: `git branch` (la tuya aparece con `*`).

## Paso 4 · Trabajar SOLO en tu carpeta

1. Abre **tu** carpeta de la tabla de arriba. Ya tiene la plantilla copiada, con el número de tu HU puesto.
2. Llena los archivos `01_Preparacion` (1.1 a 1.4) y `02_Implementacion` (2.1 a 2.6) usando **solo la ficha de tu HU** (PDF de fichas en Classroom).
3. Crea tus casos copiando `_Plantilla_Caso.md` y tus scripts copiando `_Plantilla_Script.md` (ver `00_Nomenclatura.md`).
   - El caso **no** lleva «CP» → `USR-CRE-001.md`
   - El script **sí** lleva «SCR» → `SCR-USR-CRE-001.md`
4. `2.7 Revisión`, `03_Ejecucion` y `04_Evaluacion` se dejan con la plantilla. En ejecución todo dice **«No ejecutado»**.

**Códigos de módulo** (igual que el ejemplo de HU-001): `USR` = Usuarios (HU-010 a 013) · `PRE` = Préstamos (HU-022, 024).

## Paso 5 · Agregar tu parte a los archivos del Sprint

| Archivo | Qué haces |
|---|---|
| `Sprint_1/Estimacion_QA_HU-0XX.md` | **Lo creas tú.** Copia `Estimacion_QA_HU-010.md` como guía de formato y escribe **tus** tareas y horas |
| `Sprint_1/Acta_de_refinamiento.md` | Escribe tus preguntas para el PO **solo en la sección de tu HU** |
| `Sprint_1/Capacidad_QA.md` | Llena **solo tu fila** con tus horas reales |

> Edita solo tu sección o tu fila. Si todos cambian la misma línea, GitHub marca un conflicto.

## Paso 6 · Guardar y subir tus cambios

```bash
git status
git add .
git commit -m "HU-011: diseño de pruebas (preparación e implementación)"
git push -u origin qa/hu-011
```

| Comando | Qué hace |
|---|---|
| `git status` | Muestra qué archivos cambiaste. Revisa que solo aparezcan tu carpeta y tus partes de `Sprint_1` |
| `git add .` | Prepara todos los cambios para guardarlos |
| `git commit -m "..."` | Guarda una «foto» de tus cambios con un mensaje |
| `git push -u origin qa/hu-011` | Sube tu rama a GitHub (`-u` la deja conectada para la próxima vez) |

Si después haces más cambios, basta con `git add .`, `git commit -m "..."` y `git push`.

## Paso 7 · Abrir tu Pull Request hacia `main`

1. Entra al repositorio en GitHub. Aparece un aviso amarillo **Compare & pull request**: púlsalo.
2. Revisa que diga **base: `main`** ← **compare: `qa/hu-011`**.
3. Título: `[HU-011] Diseñar pruebas: Crear usuarios desde el servicio`
4. En la descripción pega esto y complétalo:

```markdown
## HU-011 Crear usuarios desde el servicio

- Issue: #___
- Carpeta: 02_Usuarios_e_inventario/Proceso_Pruebas_HU-011_Crear_usuarios_desde_el_servicio/
- Matriz: .../02_Implementacion/2.2_Matriz_de_trazabilidad.md
- CA cubiertos: CA-HU-011-01, CA-HU-011-02, ... (todos los de la ficha)
- RNF cubiertos: RNF-___
- Autor: @tu-usuario
- Revisor (designado por el Grupo 2): @usuario-revisor
- Estado de ejecución: No ejecutado
```

5. En **Reviewers** agrega a la persona que designó el Grupo 2.
6. Pulsa **Create pull request**.
7. En el tablero ([GitHub Project](https://github.com/users/marianauribe57-art/projects/4)), mueve tu tarea a **«En revisión»**.

## Paso 8 · Atender la revisión

- El revisor deja observaciones en la PR y en `2.7_Revision_por_pares.md`.
- Corriges en **tu misma rama** y haces `git add .`, `git commit -m "HU-011: ajustes de la revisión"` y `git push`. La PR se actualiza sola.
- **No** fusiones tu PR antes de que el revisor la apruebe.

---

## ❌ Lo que NO se debe hacer

| No hagas esto | Por qué |
|---|---|
| Editar la carpeta de la HU de otra persona | La calificación es individual y se pierde la autoría |
| Hacer `git push` directo a `main` | Todo entra por PR revisada (guía EV05, Fase 6) |
| Subir datos reales: Excel del grupo, documentos, notas, correos o contraseñas reales | La guía lo prohíbe; usa solo datos ficticios |
| Inventar URL, códigos de respuesta o textos de error que la ficha no dice | Regla de la guía (Fase 4): anótalo como pregunta para el PO |
| Marcar casos como «Pasó» sin una corrida real | Se deja «No ejecutado» |
| Copiar los datos o resultados del ejemplo de HU-001 | El ejemplo es solo para ver la estructura |
| Mover una tarea a «Hecho» para ocultar un bloqueo | Se registra la causa y quién puede resolverlo |

## ¿Algo salió mal?

| Problema | Qué hacer |
|---|---|
| `git push` dice *rejected* | Ejecuta `git pull origin qa/hu-011` y vuelve a hacer `git push` |
| Trabajaste en `main` sin querer (y aún no hiciste commit) | Ejecuta `git checkout -b qa/hu-011`: tus cambios pasan a la rama nueva |
| La PR muestra conflictos en `Sprint_1/` | Avisa en el grupo antes de resolverlo; probablemente alguien editó la misma fila |

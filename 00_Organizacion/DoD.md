# Definition of Done (DoD) · diseño de pruebas por HU

> **BORRADOR – pendiente de validación del equipo**

[Volver al índice](../README.md)

Una tarea de diseño pasa a **«Hecho»** en el tablero solo si cumple todos los puntos (guía EV05, Fases 2 y 6). La DoD **no** equivale a los criterios de aceptación de la HU.

| N.º | Criterio | Fuente | Cómo se comprueba |
|---:|---|---|---|
| 1 | **Cobertura trazable:** cada CA y cada RNF pertinente tiene escenario, caso, dato y script en la matriz 2.2 | Guía · Fase 2 y Fase 4 | Tabla de cobertura de 2.2 sin «Sin cubrir» |
| 2 | **Scripts reproducibles:** otra persona puede preparar el dato, hacer los pasos y distinguir el resultado correcto | Guía · Fase 4 y Fase 5 | Recorrido de escritorio del revisor |
| 3 | **Revisión ajena resuelta:** las observaciones del revisor están corregidas o justificadas | Guía · Fase 5 | 2.7 y la PR con la resolución |
| 4 | **Archivos integrados:** la PR de la HU está fusionada en `main` | Guía · Fase 6 | PR en estado *Merged* |
| 5 | **Enlaces accesibles:** el índice, la issue y la carpeta abren sin pedir permisos | Guía · Fase 6 y Entrega | Prueba con una cuenta sin permisos de edición |
| 6 | **Sin resultados inventados:** los casos sin corrida dicen «No ejecutado» | Guía · Fase 5 | 2.2 y 3.2 |
| 7 | **Nomenclatura respetada:** el caso no lleva «CP»; el script lleva «SCR»; mismo consecutivo | Guía · Fase 4 | 00_Nomenclatura.md |
| 8 | **Solo datos ficticios** | Guía · Fase 1 | Revisión de 2.3 (.md y .csv) |

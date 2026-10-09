# Auditoría inicial de proyectos · 9 de octubre de 2026

## Alcance y límites

Esta revisión leyó metadatos del repositorio y archivos de entrada/README de cinco proyectos prioritarios. No es una auditoría completa de todas las páginas, enlaces, scripts, permisos ni despliegues. No se modificaron esos cinco proyectos. La revisión no certifica exactitud factual de sus contenidos ni funcionamiento visual en navegadores reales.

## Clasificación operativa propuesta

| Proyecto | Rol según documentación/entrada revisada | Estado operativo recomendado | Primera prioridad |
|---|---|---|---|
| OCARINA-WILD | Atlas visual de fauna y flora local | **CONGELADO: solo cambios expresamente autorizados** | Comprobar imágenes reales, carga de datos, consola y vista móvil sin modificar nada |
| OCARINA-CLIMATICA | Observatorio local con fuentes, ingesta y validación | **ACTIVO / sensible a datos** | Verificar flujo de datos, fecha de actualización, procedencia y tratamiento de fallos de fuentes |
| Chañar HUB | Guía útil para resolver necesidades locales | **ACTIVO / información crítica** | Verificar números, teléfonos, direcciones, horarios y fecha/fuente de comprobación |
| VECINDAD | Sistema educativo ciudadano basado en normas y evidencia | **ACTIVO / contenido jurídico sensible** | Inventariar documentos primarios y distinguir verificado, pendiente e interpretación |
| VILLA-PELON-GAME | Juego histórico-territorial, núcleo V4 protegido | **CONGELADO: preservar contratos y progresión** | Pruebas de regresión del recorrido, guardado y controles antes de cualquier extensión |

## Hallazgos comprobados

- Los cinco repositorios revisados son públicos y usan la rama main.
- OCARINA-WILD tiene un index.html autónomo con estilos integrados; no se debe tocar para esta auditoría.
- OCARINA CLIMÁTICA documenta una arquitectura de fuente → ingestor → adaptador → validación → observatorio → reporte → interfaz. Debe verificarse contra los archivos y ejecuciones reales antes de dar por sano el flujo.
- Chañar HUB documenta una interfaz deliberadamente pequeña y advierte que los datos sensibles necesitan fuente y fecha de comprobación.
- VECINDAD documenta reglas de evidencia y una arquitectura estática sin backend.
- VILLA-PELON-GAME declara protegida su base V4 y establece como regla identificar causa, corregir causa, probar y congelar. Respetar ese contrato.

## Riesgos a resolver en orden

1. **Datos y afirmaciones:** información local desactualizada o sin fuente clara.
2. **Medios:** imágenes rotas, faltantes, mal atribuidas o sin permiso/licencia clara.
3. **Regresión:** un cambio visual rompe navegación, guardado o controles.
4. **Publicación:** enlaces y recursos que funcionan en local pero fallan en GitHub Pages por rutas, mayúsculas o dependencias.
5. **Mantenibilidad:** ausencia de inventario uniforme, instrucciones de prueba y registro de cambios.

## Protocolo seguro para la siguiente ronda

- No tocar repositorios congelados ni proyectos fuera del alcance aprobado.
- Leer primero README, árbol de archivos, configuración de Pages/Actions disponible y entradas principales.
- Ejecutar verificaciones estáticas y pruebas de enlaces cuando la infraestructura lo permita.
- Para datos externos, guardar fuente, fecha, unidad, ubicación, método y estado de verificación.
- Para cada especie de WILD: fotografía representativa real antes de publicar la ficha, nombre, fuente y licencia/atribución.
- Para cada cambio: registrar objetivo, archivos, pruebas, resultado y posibilidad de reversión.
- No incorporar backend, servicios pagos ni nuevas dependencias sin una necesidad demostrada.

## Próxima secuencia recomendada

1. Terminar inventario de los 25 repositorios visibles y clasificarlos como activo, congelado, experimental o pendiente de decisión.
2. Auditar la cadena de datos de OCARINA CLIMÁTICA sin editarla.
3. Preparar un comprobador estático reutilizable para rutas locales, recursos referenciados, imágenes declaradas y metadatos básicos.
4. Ejecutar primero el comprobador en una copia o rama de prueba, nunca directamente sobre proyectos congelados.
5. Priorizar correcciones por impacto real; no rediseñar ni migrar proyectos por moda tecnológica.

## Registro

- Fecha: 2026-10-09
- Repositorios inspeccionados en esta ronda: OCARINA-WILD, OCARINA-CLIMATICA, chanar-hub, vecindad y VILLA-PELON-GAME.
- Cambios hechos en esos repositorios: ninguno.
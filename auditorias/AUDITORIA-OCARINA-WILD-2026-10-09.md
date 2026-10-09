# Auditoría estática de OCARINA WILD · 9 de octubre de 2026

## Alcance

Se leyeron index.html, data.js y app.js de la rama main. No se modificó ningún archivo de OCARINA WILD. Esta revisión inspecciona datos y código; no comprueba la respuesta HTTP de cada fotografía ni sustituye una revisión visual en navegador.

## Resultados estáticos comprobados

- El atlas contiene 39 fichas de especies.
- Las 39 fichas contienen un campo de fotografía y una fuente fotográfica.
- Las 39 fichas incluyen los campos de evidencia que exige la puerta fotográfica del renderizador, y el campo audit está marcado como verified-live.
- Las 39 fichas declaran el estado de licencia como “verificación pendiente”. La propia política del proyecto aclara correctamente que una fuente no equivale a permiso de reutilización.
- La interfaz construye las tarjetas desde data.js y carga las imágenes en forma diferida (loading="lazy"). Por eso, buscar etiquetas img en index.html no alcanza para revisar las fotografías: las imágenes se generan dinámicamente desde JavaScript.
- En app.js no se encontró un manejador explícito de error de carga de imagen (onerror) ni una comprobación automática de que la imagen haya cargado correctamente.

## Interpretación

**La puerta de metadatos existe, pero no demuestra por sí sola que las 39 fotografías carguen en el navegador, representen correctamente la especie, estén bien encuadradas o puedan reutilizarse legalmente.** El nombre verified-live debe interpretarse como un valor de datos ya existente, no como resultado de una prueba HTTP realizada durante esta auditoría.

## Recomendaciones sin intervención directa

1. Mantener el proyecto congelado: no cambiar estructura ni funcionamiento sin autorización explícita.
2. Hacer una comprobación de carga de las 39 imágenes en un entorno de prueba, registrando código HTTP, redirecciones y resultado final; no dar por cargada una foto solo porque el campo contiene una URL.
3. Auditar visualmente cada foto: organismo/planta viva, ejemplar completo y reconocible, luz y encuadre adecuados, contexto natural y ausencia de imágenes prohibidas por la política editorial.
4. Resolver atribución y licencia individualmente antes de redistribuir imágenes. Mientras la licencia esté pendiente, mostrar ese estado con honestidad.
5. Solo si se autoriza una mejora de diseño, considerar un estado de error elegante para imágenes que fallen, sin eliminar fichas ni sustituir automáticamente la foto por una imagen engañosa.

## Registro

- Rama revisada: main.
- Archivos leídos: index.html, data.js, app.js.
- Cambios hechos en OCARINA WILD: ninguno.
- Siguiente paso seguro: preparar una verificación de imágenes aislada, sin publicar ni alterar el proyecto congelado.
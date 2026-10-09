# Estándar de calidad Ocarina 1.0

Este estándar sirve para páginas web, mapas históricos, videojuegos, libros digitales, documentos, ilustraciones y producciones audiovisuales. Adaptar la lista al formato; no exigir a todos los proyectos la misma tecnología.

## 1. Propósito y público
- ¿Qué necesidad concreta resuelve?
- ¿Para quién está hecho y en qué contexto lo usará?
- ¿Qué debería poder hacer o comprender una persona en el primer minuto?
- ¿Qué queda fuera del alcance?

## 2. Veracidad y curaduría
- Separar hechos documentados, interpretaciones, testimonios, hipótesis y ficción.
- Guardar título de la fuente, institución/autor, enlace o referencia, fecha de consulta y dato que respalda.
- En historia local, priorizar documentos primarios y fuentes institucionales cuando existan; contrastar afirmaciones importantes.
- En ciencia y naturaleza, indicar nombre común/científico cuando corresponda, distribución y límites de la evidencia.
- No usar “oficial”, “confirmado” o “verificado” sin evidencia suficiente.
- Revisar ortografía, fechas, nombres propios, topónimos, unidades y consistencia interna.

## 3. Derechos y atribución
- Registrar autoría y licencia de fotos, mapas, tipografías, música, video, ilustraciones y textos.
- No asumir que una imagen encontrada en internet es reutilizable.
- Conservar créditos visibles y enlaces requeridos por la licencia.
- Evitar datos personales innecesarios y obtener permiso antes de publicar material sensible.

## 4. Diseño y experiencia
- Diseñar primero para móvil; verificar también escritorio y tamaños intermedios.
- Una acción principal clara por pantalla o sección.
- Jerarquía visual evidente; texto breve y escaneable, con contenido profundo detrás de puertas claras.
- Contraste suficiente, foco de teclado visible, botones legibles y controles utilizables sin precisión extrema.
- Evitar superposiciones, scroll horizontal accidental, popups invasivos y enlaces que sorprendan.
- Imágenes relevantes, bien encuadradas, optimizadas y con texto alternativo útil.
- Mantener identidad visual coherente sin sacrificar legibilidad.

## 5. Calidad técnica
- Comprobar consola y errores visibles en el navegador cuando sea posible.
- Verificar enlaces, imágenes, rutas relativas, navegación, formularios y estados vacíos.
- Confirmar que no haya secretos, tokens, claves API ni datos privados en archivos públicos.
- Probar recarga, vuelta atrás, conexión lenta y ausencia de datos externos.
- Evitar dependencias innecesarias y documentar las que sean críticas.
- No incorporar backend, base de datos ni servicios pagos sin una necesidad demostrada.

## 6. Seguridad y preservación
- Revisar el estado inicial antes de editar.
- Hacer un cambio acotado por commit y explicar el motivo.
- No borrar ni reemplazar archivos desconocidos sin inspeccionarlos.
- Mantener una vía de recuperación: historial Git, copia o versión etiquetada.
- Proteger proyectos congelados; los cambios autorizados deben respetar su alcance.
- No desplegar ni sincronizar cambios con otros proyectos sin autorización expresa.

## 7. Cierre de trabajo
Cada tarea debe indicar:
- Qué se cambió.
- Archivos afectados.
- Qué pruebas se ejecutaron y su resultado.
- Qué no se pudo probar.
- Riesgos o pendientes.
- Cómo revertir el cambio.

## Criterio de salida
Una pieza no está “terminada” solo porque abre. Debe cumplir su propósito, ser comprensible, mostrar información fiable, funcionar en los dispositivos objetivo y tener derechos/atribuciones revisados.
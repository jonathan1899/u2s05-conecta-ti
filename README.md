# Conecta TI 2026 · Kit de inicio U2S05

Sitio de un evento ficticio de tecnología. El HTML ya está completo y la hoja de estilos ya tiene colores, tipografía y bordes. **Lo que falta es la maquetación responsiva**, y eso es lo que vas a construir en esta sesión.

## Estructura

```
conecta-ti/
├── index.html          <- NO necesitas modificarlo (salvo el paso 1 del tutorial)
├── css/
│   └── estilos.css     <- aquí trabajas, en el bloque 6 al final del archivo
├── capturas/           <- aquí guardas tus 3 capturas de evidencia
└── README.md           <- aquí respondes la bitácora (al final de este archivo)
```

## Cómo abrirlo

- **En Codespaces:** sube la carpeta a un repositorio nuevo llamado `u2s05-conecta-ti`, abre el Codespace y ejecuta en la terminal `php -S localhost:8000`. Abre el puerto 8000 en el navegador.
- **Sin Codespaces:** abre `index.html` directamente en Chrome o Edge. Funciona igual porque es HTML y CSS puro.

## Anchos de prueba (DevTools, modo dispositivo)

| Vista | Ancho | Nombre de la captura |
|---|---|---|
| Celular | 375 px | `capturas/movil-375.png` |
| Tableta | 768 px | `capturas/tableta-768.png` |
| Escritorio | 1280 px | `capturas/escritorio-1280.png` |

Para tomar captura de página completa en DevTools: `Ctrl + Shift + P` (en Mac `Cmd + Shift + P`), escribe `screenshot` y elige **Capture full size screenshot**.

## Bitácora (responde aquí, 2 a 4 líneas por pregunta)

1. **¿Por qué el sitio original se veía diminuto o con barra horizontal en el celular? Menciona las dos causas que corregiste.**

   _Tu respuesta:_El sitio tenía un contenedor con un ancho fijo de 1100 px, por lo que no se adaptaba a las pantallas pequeñas. También necesitaba la etiqueta meta viewport para ajustarse correctamente al ancho del dispositivo. Corregí ambos problemas haciendo que el contenedor fuera flexible y agregando dicha etiqueta.

2. **¿En qué parte del sitio elegiste Flexbox y en cuál Grid? Explica el criterio que usaste (una dimensión vs. dos dimensiones).**

   _Tu respuesta:_Utilicé Flexbox en el encabezado, el menú y los bloques de horarios, porque necesitaba acomodar elementos en una dirección, ya fuera en filas o columnas. Utilicé Grid en las tarjetas de ponentes, la portada, la agenda, los patrocinadores y el pie de página, porque necesitaba organizar elementos en filas y columnas.

3. **¿Qué hace exactamente `repeat(auto-fit, minmax(240px, 1fr))`? Explícalo como si se lo contaras a un compañero que faltó.**

   _Tu respuesta:_Esta instrucción permite crear automáticamente tantas columnas como quepan en el espacio disponible. Cada columna tendrá un mínimo de 240 px y podrá crecer para ocupar el espacio restante. Así, las tarjetas se acomodan automáticamente dependiendo del tamaño de la pantalla.

4. **¿Qué fue lo que más te costó y cómo lo resolviste? (qué recurso usaste: tutorial, hoja de referencia, checklist de errores, laboratorio, un compañero)**

   _Tu respuesta:_Lo que más me costó fue conseguir que todas las secciones se acomodaran correctamente en los diferentes tamaños de pantalla. Lo resolví modificando las reglas de CSS y realizando pruebas con las herramientas de desarrollador de Chrome, utilizando distintos anchos de pantalla para comprobar los resultados.

---
*Conecta TI 2026 es un evento ficticio creado con fines didácticos. Prof. Alonso · Tecnologías de Información*

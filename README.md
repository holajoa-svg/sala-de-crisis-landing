# Sala de crisis — página de presentación

Página única y estática que presenta el prototipo «Sala de crisis» y lleva al
asistente. Forma parte del Trabajo Fin de Máster de Joanna Cristina Jiménez
Martínez (Máster Universitario en Tecnologías en Marketing y Comunicación
Política, Universidade de Santiago de Compostela).

No lleva servidor, ni analítica, ni recoge dato alguno. El único enlace de
salida es el GPT «Sala de crisis v8.1».

## Estructura

    index.html   la página entera, con sus estilos dentro
    img/         logotipos, extintor e iconos, del diseño original

## Tipografías

- **Alfarn** (Adobe Fonts, proyecto web `qdp3oii`) en los rótulos de sección.
  El dominio donde se publique tiene que estar dado de alta en el proyecto web
  de Adobe Fonts, o cargará la sustituta.
- **Barlow Semi Condensed** en titulares y cifras, y **Exo 2** en el texto,
  ambas de Google Fonts.

## Notas de construcción

- El extintor viene en escala de grises y toma el rojo del fondo mediante
  `mix-blend-mode: luminosity`.
- El logotipo del pie va incrustado en el HTML, no como imagen, porque su SVG
  lleva el texto vivo en Alfarn y un SVG externo no puede cargar tipografías.
- Abierta con doble clic la tipografía Alfarn no carga, porque no hay dominio.
  Hay que servirla: `python3 -m http.server 8777`.

## Pendiente

- El botón «Conocer la investigación» está retirado hasta que haya un destino.
- El pie todavía no identifica el trabajo ni a la autora.

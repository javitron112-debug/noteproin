# Editor Web Multi-Formato PRO
Un procesador de textos robusto y completamente autocontenido en un solo archivo HTML. No requiere servidor, base de datos ni instalación. Funciona directamente en el navegador y permite alternar fluidamente entre un editor visual (WYSIWYG) y código Markdown puro.

## 🚀 Características Principales
100% Local y Privado: Todo el procesamiento y almacenamiento se realiza en tu navegador. Ningún dato viaja a servidores externos.

Modo Dual: Escribe visualmente (estilo Word) o cambia al "Modo Código" para editar directamente la sintaxis Markdown.

Auto-guardado Ininterrumpido: Tu progreso se guarda automáticamente en el localStorage del navegador cada vez que pausas la escritura.

Exportación a PDF: Genera documentos PDF con tamaño estándar A4. Soporta inserción de saltos de página personalizados (Ctrl/Cmd + Click o desde el menú).

Gestión de Archivos .md: Abre archivos Markdown desde tu equipo o descarga tu trabajo en formato .md.

Modo Oscuro Integrado: Cambia entre tema claro y oscuro para reducir la fatiga visual. (Los PDF siempre se exportan con fondo blanco para impresión).

Drag & Drop de Imágenes: Arrastra imágenes directamente al lienzo. Las imágenes se pueden redimensionar arrastrando desde su esquina inferior derecha.

Formato para LinkedIn: Convierte el texto seleccionado a fuentes Unicode "Negrita" compatibles con plataformas como LinkedIn que no soportan Markdown de forma nativa.

Selector de Emojis: Panel de emojis moderno e integrado.

## 🛠️ Tecnologías y Librerías
El proyecto está construido con HTML, JavaScript Vanilla y CSS, apoyándose en las siguientes librerías cargadas vía CDN:

Tailwind CSS - Para el diseño responsivo y la interfaz de usuario.

FontAwesome - Para la iconografía de la barra de herramientas.

html2pdf.js - Motor de conversión de HTML a PDF.

Marked.js - Parseador superrápido para renderizar Markdown a HTML.

Turndown - Conversor de HTML de vuelta a sintaxis Markdown.

Turndown GFM Plugin - Extensión para soportar tablas y otras características de GitHub Flavored Markdown.

emoji-picker-element - Web component ligero para la selección de emojis.

## 💻 Instalación y Uso
No hay proceso de instalación.

Descarga el archivo editor.html.

Haz doble clic sobre él para abrirlo en cualquier navegador web moderno (Chrome, Firefox, Safari, Edge).

Empieza a escribir.

## ⚠️ Limitaciones Técnicas Conocidas
Dado que esta aplicación es un experimento "Serverless" (sin backend) concentrado en un único archivo, existen limitaciones físicas impuestas por los navegadores:

Límite de Almacenamiento (Imágenes): Las imágenes arrastradas se convierten a código Base64 para poder existir en el archivo. El auto-guardado usa localStorage, que tiene un límite estricto de ~5MB por dominio. Si insertas imágenes de muy alta resolución, alcanzarás este límite, el documento dejará de auto-guardarse y el sistema te alertará.

Edición de Tablas: Puedes insertar una tabla básica (2x2) y escribir en ella de forma visual. Sin embargo, para añadir nuevas columnas o filas de forma compleja, deberás pasar al modo Markdown.

Formateador LinkedIn (Accesibilidad): La herramienta "Negrita LN" usa caracteres matemáticos Unicode. Su uso excesivo puede ser perjudicial para usuarios que utilizan lectores de pantalla, por lo que se recomienda usarlo con moderación solo para títulos o palabras clave.

## 🤝 Contribución
Siéntete libre de bifurcar (fork) este proyecto y adaptar el código a tus necesidades. Al ser un archivo plano, es ideal para experimentar con las APIs nativas del navegador (document.execCommand, manipulación de la API Selection, etc.).

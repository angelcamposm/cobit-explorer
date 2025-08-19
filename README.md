Explorador Interactivo de COBIT 2019
Este proyecto es una Single Page Application (SPA) interactiva y responsive diseñada para explorar de manera visual e intuitiva el marco de gobierno y gestión de I&T COBIT® 2019. La aplicación transforma el denso contenido del marco en una experiencia de usuario fluida y fácil de navegar, ideal para profesionales, estudiantes y cualquier persona interesada en el gobierno de TI.

✨ Características Principales
Navegación Fluida en una Sola Página: Todo el contenido está estructurado en una única página con desplazamiento suave. La barra de navegación fija permite saltar fácilmente entre secciones.

Totalmente Bilingüe (ES/EN): Soporte completo para español e inglés. El idioma se puede cambiar al instante con un selector de botones intuitivo.

Diseño Responsive: La interfaz se adapta perfectamente a cualquier tamaño de pantalla, desde ordenadores de escritorio hasta dispositivos móviles.

Visualización de Datos: Incluye un gráfico de anillo interactivo (creado con Chart.js) para mostrar la distribución de los 40 objetivos de COBIT en sus 5 dominios.

Contenido Interactivo:

Línea de Tiempo Evolutiva: Muestra la historia de COBIT de forma visual.

Explorador de Objetivos: Permite filtrar los 40 objetivos por dominio y ver el propósito de cada uno en una ventana modal.

Secciones Desplegables: Los principios y la cascada de metas se presentan en acordeones para una lectura más limpia.

Cero Dependencias Externas: Funciona directamente en el navegador sin necesidad de instalación, build steps o un servidor web.

🚀 Tecnologías Utilizadas
Este proyecto está construido con tecnologías web estándar para garantizar la máxima compatibilidad y simplicidad:

HTML5: Para la estructura semántica del contenido.

Tailwind CSS: Para un diseño de interfaz de usuario moderno, responsive y basado en utilidades, cargado a través de CDN.

JavaScript (Vanilla): Para toda la lógica de interactividad, incluyendo:

Gestión del estado del idioma.

Manipulación del DOM para actualizar el contenido dinámicamente.

Control de la navegación por scroll (Intersection Observer).

Manejo de eventos para todos los elementos interactivos.

Chart.js: Para la creación del gráfico de anillo, cargado a través de CDN.

💻 Cómo Utilizarlo
Simplemente descarga el archivo index.html y ábrelo en tu navegador web preferido.

# Clona el repositorio (opcional)
git clone https://github.com/tu-usuario/cobit-explorer.git

# Navega al directorio
cd cobit-explorer

# Abre el archivo index.html en tu navegador

¡Y eso es todo! No se requiere ninguna instalación ni configuración adicional.

📂 Estructura del Código
El proyecto está contenido en un único archivo index.html para una portabilidad máxima. Su estructura interna es la siguiente:

<head>: Contiene los metadatos, los enlaces a las CDNs de Tailwind CSS y Chart.js, y los estilos CSS personalizados.

<header>: La barra de navegación superior fija con los enlaces a las secciones y el selector de idioma.

<main>: El contenedor principal con las diferentes secciones del contenido (<section>), cada una con su propio ID para la navegación.

<footer>: Un pie de página simple.

<script>: Todo el código JavaScript se encuentra al final del <body>.

i18nData: Un objeto JSON que contiene todas las traducciones en español e inglés.

Funciones de Inicialización (init...): Un conjunto de funciones que se encargan de renderizar cada componente interactivo (la línea de tiempo, los acordeones, el gráfico, etc.).

Lógica de Traducción (translatePage): La función principal que actualiza todo el contenido visible según el idioma seleccionado.

Manejadores de Eventos: El código que gestiona los clics, el scroll y otras interacciones del usuario.

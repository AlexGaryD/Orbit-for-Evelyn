🍏 Proyecto: Firmamento Especial para Evelyn

Este proyecto es una experiencia web interactiva y personalizada diseñada como un regalo de cumpleaños digital. Combina animaciones inmersivas, elementos multimedia y una interfaz de usuario premium para crear un "refugio digital" que celebra un momento especial.

🚀 Características Principales
Experiencia inmersiva: Comienza con un sobre interactivo que, al abrirse, despliega una secuencia de comandos simulada con efectos visuales tipo "CRT".

Narrativa multimedia: Un viaje a través de diferentes vistas que combinan mensajes emotivos con un diseño minimalista y oscuro (dark mode).

Galería dinámica: Incluye un carrusel de recuerdos con efectos 3D (Swiper.js) y un sistema de lightbox para visualizar detalles.

Estética premium: Uso intensivo de Tailwind CSS, animaciones personalizadas (Keyframes), degradados en texto y tipografía elegante (Poppins).

Música de fondo: Sistema integrado para la reproducción de audio, permitiendo acompañar la lectura con música.

🛠 Tecnologías Utilizadas

Frontend: HTML5, CSS3 (con animaciones personalizadas), JavaScript (ES6+).

Estilizado: Tailwind CSS (vía CDN para prototipado rápido).

Interactividad: Swiper.js para el carrusel de fotos 3D.

Iconografía: Font Awesome.

Fuentes: Google Fonts (Poppins).

Efectos visuales: Canvas API para simulaciones de fuegos artificiales y manipulación del DOM para efectos de partículas.

⚙️ Estructura del Proyecto
index.html: El archivo raíz que contiene toda la lógica de vistas, estilos y scripts.

assets/: Carpeta contenedora de recursos visuales (imágenes, iconos, etc.).

recuerdos/: Carpeta dedicada al almacenamiento de los fragmentos fotográficos del proyecto.

💡 Detalles Técnicos Relevantes

Aislamiento de Navegación: Se implementó una lógica de navegación secuencial y táctil (touch events) con aislamiento crítico para que el carrusel de fotos no interfiera con el scroll de la página principal.

Optimización: Uso de backdrop-filter para efectos de vidrio (glassmorphism) y manejo de opacidad para transiciones fluidas entre secciones.

Flicker Effect: Animación tipo CRT para la consola de inicio, mejorando la sensación de un sistema de "override" exclusivo.

Responsividad: Diseño totalmente adaptable a dispositivos móviles, optimizando la experiencia de usuario táctil.

🎨 Inspiración

Este proyecto fue creado con el objetivo de convertir un día común en una experiencia memorable, utilizando el código como un medio de expresión creativa y afectiva.  Nota: Este proyecto es una pieza de desarrollo frontend orientada a la experiencia de usuario, priorizando la fluidez de las animaciones y la carga de activos multimedia de manera eficiente.

🚀 Deployment y Flujo de Cambios

La producción se despliega automáticamente en Vercel desde la rama `Main`. Para que un cambio aparezca en el link de producción, ese cambio debe llegar a `Main`.

Flujo de trabajo:

1. Edita el proyecto en v0. Cada cambio se guarda en una rama `v0/*`.
2. Crea un Pull Request hacia `Main` (botón "Create PR" en v0, arriba a la derecha).
3. El PR se fusiona automáticamente a `Main` gracias al workflow de auto-merge.
4. Vercel detecta el nuevo commit en `Main` y despliega a producción en 1-2 minutos.
5. Refresca el link de producción con `Ctrl+Shift+R` para limpiar la caché y ver los cambios.

⚙️ Auto-merge automático

El archivo `.github/workflows/auto-merge-v0.yml` fusiona automáticamente cualquier PR que venga de una rama `v0/*` hacia `Main`. Esto evita tener que hacer el merge manual cada vez.

Si un PR no se fusiona solo:
- Verifica en GitHub que GitHub Actions esté habilitado: `Settings → Actions → General` y permite la ejecución de workflows.
- Asegúrate de que el PR apunte a la rama base `Main`.

⚠️ Importante: Si haces un cambio y el link de producción no lo refleja, casi siempre es porque el cambio quedó en una rama `v0/*` sin fusionar a `Main`. Crea/fusiona el PR hacia `Main` y espera el redeploy de Vercel.

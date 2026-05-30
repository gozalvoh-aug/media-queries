# media-queries
⚡ Electric Cards
Catálogo web de vehículos eléctricos con diseño oscuro, layout responsive y navegación lateral fija.

Descripción
Electric Cards es una página web estática que presenta un catálogo de productos de vehículos eléctricos organizados en tarjetas. El diseño utiliza una paleta oscura con acentos cian eléctrico, tipografía tecnológica y un layout de dos columnas que mantiene la navegación siempre visible mientras el usuario navega por el catálogo.

Estructura del proyecto
electric-cards/
│
├── index.html
├── README.md
└── assets/
    ├── css/
    │   └── style.css
    └── img/
        ├── 1.jpeg
        ├── 2.jpeg
        ├── 3.jpeg
        ├── 4.jpeg
        ├── 5.jpeg
        ├── 6.jpeg
        ├── 7.jpeg
        └── 8.jpeg

Layout
El diseño se basa en CSS Grid con una columna lateral izquierda fija de 250px y una columna derecha fluida.
┌──────────┬──────────────────────────────┐
│          │  aside  (filtros)            │
│  nav     ├──────────────────────────────┤
│  75vh    │  main   (tarjetas)           │
│          │                              │
├──────────┤                              │
│  footer  │                              │
│  25vh    │  (footer fijo, no se mueve)  │
└──────────┴──────────────────────────────┘
ElementoComportamientonavColumna izquierda, sticky, altura 75vhfooterposition: fixed en la parte inferior izquierda, altura 25vh, siempre visibleasideColumna derecha superior — barra de filtros y ordenamientomainColumna derecha inferior — grilla de tarjetas de productos

Responsive — Media Queries
BreakpointComportamiento> 992pxLayout de 2 columnas. Cards en 4 columnas577px – 992pxLayout de 2 columnas. Cards en 3 columnas≤ 576pxLayout de 1 columna. Nav horizontal con menú hamburguesa. Footer estático al final

Tecnologías

HTML5 semántico
CSS3 (Grid, Flexbox, Custom Properties, Media Queries)
Google Fonts — Exo 2 + DM Sans
Material Symbols — ícono electric_car
Font Awesome 6 — íconos de redes sociales


Paleta de colores
VariableColorUso--bg#0d0f14Fondo general--surface#161a24Nav, aside, footer--card-bg#1c2130Tarjetas de producto--accent#00e5ffCian eléctrico — énfasis principal--accent2#ff3d6bRojo eléctrico — hover de botones--text#e8ecf4Texto principal--muted#6b7896Texto secundario

Tipografía

Exo 2 — títulos, marca, botones. Estilo tecnológico y futurista.
DM Sans — cuerpo de texto, etiquetas, párrafos. Legible y moderno.


Cómo usar

Clona o descarga el repositorio.
Agrega tus imágenes en assets/img/ con los nombres 1.jpeg a 8.jpeg.
Abre index.html directamente en el navegador — no requiere servidor ni instalación.

bash# Opcionalmente, con un servidor local:
npx serve .
# o
python -m http.server 8000

Posibles mejoras

Activar el menú hamburguesa con JavaScript en mobile.
Conectar el <select> de ordenamiento a lógica de filtrado dinámico.
Añadir animaciones de entrada a las tarjetas con Intersection Observer.
Integrar un backend o JSON para cargar los productos de forma dinámica.


Licencia
Proyecto de uso educativo. Libre para modificar y distribuir.

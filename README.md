# Landing Page - Estilo E-commerce
 

## Paso a Paso de la Construcción

### Paso 1: Estructura Base del Proyecto
Se crearon los archivos fundamentales:
- `index.html` - Estructura HTML del sitio
- `styles.css` - Estilos CSS
- `README.md` - Documentación

### Paso 2: Reset CSS y Estilos Base
Primero se estableció un reset CSS para normalizar los estilos entre navegadores:
```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
```
Se definió la tipografía base (Arial) y el color de fondo de la página (`#eaeded`).

### Paso 3: Header Principal
Se construyó el header en dos partes:

#### 3.1 Barra Principal (`#131921`)
- **Logo/Nombre**: Texto blanco y negrita a la izquierda
- **Barra de búsqueda**: Input blanco con botón naranja (`#febd69`)
- **Navegación derecha**: Enlaces "Cuentas y Listas", "Devoluciones", "Carrito"

```html
<div class="header-main">
    <div class="logo">...</div>
    <div class="search-bar">...</div>
    <nav class="nav-links">...</nav>
</div>
```

#### 3.2 Sub-navegación (`#232f3e`)
Barra secundaria con enlaces como "Ofertas", "Servicio al Cliente", etc.

### Paso 4: Contenedor Principal
Se definió el contenedor central con ancho fijo y centrado:
```css
.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 15px;
}
```

### Paso 5: Grilla de Productos
Se implementó CSS Grid para organizar las tarjetas de productos:
```css
.product-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 20px;
}
```

### Paso 6: Tarjetas de Producto
Cada tarjeta incluye:
- **Imagen placeholder**: Fondo gris claro (`#f0f0f0`)
- **Título**: Color azul marino (`#007185`)
- **Precio**: Símbolo de moneda pequeño, precio en negro
- **Botón**: Degradado amarillo (`#ffd814`) con bordes redondeados

```css
.product-card {
    background-color: #ffffff;
    border: 1px solid #ddd;
    border-radius: 4px;
}
```

### Paso 7: Footer
Se construyó en tres secciones:

#### 7.1 Botón "Volver Arriba" (`#37475a`)
```html
<div class="back-to-top">
    <a href="#">Volver arriba</a>
</div>
```

#### 7.2 Sección de Enlaces (`#232f3e`)
4 columnas organizadas con CSS Grid:
- Conócenos
- Gana dinero con nosotros
- Métodos de pago
- ¿Necesitas ayuda?

#### 7.3 Copyright (`#131921`)
Barra inferior con texto centrado.

### Paso 8: Responsive Design
Se añadieron media queries para adaptabilidad:
- **992px**: 3 columnas de productos
- **768px**: 2 columnas, reorganización del header
- **480px**: 1 columna, footer vertical

---

## Paleta de Colores Utilizada

| Elemento | Color Hex |
|----------|-----------|
| Header principal | `#131921` |
| Sub-navegación | `#232f3e` |
| Fondo página | `#eaeded` |
| Tarjetas producto | `#ffffff` |
| Botón búsqueda | `#febd69` |
| Títulos producto | `#007185` |
| Botón carrito | `#ffd814` |
| Footer "volver arriba" | `#37475a` |

---

## Estructura de Archivos

```
LandingPage/
├── index.html      # Estructura HTML
├── styles.css      # Estilos CSS
└── README.md       # Documentación
```

---

## Cómo Usar

1. Abre el archivo `index.html` en cualquier navegador moderno
2. Los estilos se cargarán automáticamente desde `styles.css`
3. Para personalizar, modifica los colores y contenido según necesites

---

## Tecnologías Utilizadas

- HTML5
- CSS3 (Flexbox, Grid, Variables)
- Responsive Design

---

## Documentación de Etiquetas HTML

A continuación se documenta cada etiqueta HTML utilizada en el proyecto:

### Etiquetas de Estructura del Documento

| Etiqueta | Descripción | Uso en el proyecto |
|----------|-------------|-------------------|
| `<!DOCTYPE html>` | Declaración que indica al navegador que el documento es HTML5 | Primera línea del documento |
| `<html>` | Elemento raíz que contiene todo el documento HTML | Envuelve todo el contenido, con `lang="es"` para indicar idioma español |
| `<head>` | Contenedor de metadatos del documento (no visible) | Contiene meta tags, título y enlace a CSS |
| `<body>` | Contenedor del contenido visible de la página | Envuelve header, main y footer |

### Etiquetas de Metadatos (dentro de `<head>`)

| Etiqueta | Descripción | Uso en el proyecto |
|----------|-------------|-------------------|
| `<meta>` | Define metadatos sobre el documento HTML | `charset="UTF-8"` para codificación de caracteres, `viewport` para responsive |
| `<title>` | Define el título de la página (aparece en la pestaña del navegador) | "Mi Tienda - Landing Page" |
| `<link>` | Enlaza recursos externos al documento | Conecta el archivo `styles.css` |

### Etiquetas Semánticas de Sección

| Etiqueta | Descripción | Uso en el proyecto |
|----------|-------------|-------------------|
| `<header>` | Representa el encabezado del documento o sección | Contiene la navegación principal y logo |
| `<nav>` | Define un conjunto de enlaces de navegación | Menú principal y sub-navegación |
| `<main>` | Contenido principal único del documento | Grilla de productos destacados |
| `<footer>` | Pie de página del documento o sección | Enlaces, copyright y "volver arriba" |

### Etiquetas de Contenedor (División)

| Etiqueta | Descripción | Uso en el proyecto |
|----------|-------------|-------------------|
| `<div>` | Contenedor genérico para agrupar elementos | Múltiples usos: `.container`, `.product-card`, `.search-bar`, etc. |

### Etiquetas de Encabezado

| Etiqueta | Descripción | Uso en el proyecto |
|----------|-------------|-------------------|
| `<h2>` | Encabezado de nivel 2 | Título "Productos Destacados" |
| `<h3>` | Encabezado de nivel 3 | Títulos de cada producto |
| `<h4>` | Encabezado de nivel 4 | Títulos de columnas en el footer |

### Etiquetas de Texto

| Etiqueta | Descripción | Uso en el proyecto |
|----------|-------------|-------------------|
| `<p>` | Define un párrafo de texto | Texto de copyright en el footer |
| `<span>` | Contenedor en línea para texto | Precios, iconos de carrito, líneas de navegación |
| `<a>` | Define un hipervínculo | Enlaces de navegación, productos, footer |

### Etiquetas de Lista

| Etiqueta | Descripción | Uso en el proyecto |
|----------|-------------|-------------------|
| `<ul>` | Lista desordenada (sin numeración) | Listas de enlaces en las columnas del footer |
| `<li>` | Elemento de lista | Cada enlace dentro de las listas del footer |

### Etiquetas de Formulario

| Etiqueta | Descripción | Uso en el proyecto |
|----------|-------------|-------------------|
| `<input>` | Campo de entrada de datos | Barra de búsqueda (`type="text"`) |
| `<button>` | Botón clickeable | Botón de búsqueda 🔍, botones "Agregar al carrito" |

### Comentarios HTML

| Sintaxis | Descripción | Uso en el proyecto |
|----------|-------------|-------------------|
| `<!-- texto -->` | Comentario (no visible en el navegador) | Separadores de secciones: `<!-- HEADER PRINCIPAL -->`, `<!-- Producto 1 -->`, etc. |

---

## Atributos HTML Importantes

| Atributo | Descripción | Ejemplo |
|----------|-------------|---------|
| `class` | Asigna una o más clases CSS al elemento | `class="product-card"` |
| `href` | URL de destino para enlaces | `href="#"` (enlace vacío) |
| `type` | Tipo de input o botón | `type="text"` |
| `placeholder` | Texto de ayuda en inputs | `placeholder="Buscar productos..."` |
| `lang` | Idioma del contenido | `lang="es"` |
| `charset` | Codificación de caracteres | `charset="UTF-8"` |
| `rel` | Relación del recurso enlazado | `rel="stylesheet"` |

---

## Características

- Header sticky (se mantiene fijo al hacer scroll)
- Diseño responsivo para móviles, tablets y desktop
- Efectos hover en botones y enlaces
- Grilla de productos adaptable
- Footer con múltiples columnas de enlaces

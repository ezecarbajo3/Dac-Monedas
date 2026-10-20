# Dac Monedas 🪙

Catálogo y tienda online de monedas de colección e inversión argentinas y del mundo, con diseño de alta numismática y la identidad cromática **Azul y Oro** del Club Atlético Boca Juniors.

Sitio estático de alto rendimiento en HTML5, CSS3 y JavaScript moderno (Vanilla JS), sin dependencias pesadas ni frameworks de compilación.

---

## 🌟 Características y Funcionalidades

- **Doble Vista Fluida (Landing & Catálogo)**:
  - **Portada / Landing (`data-view="landing"`)**: Pantalla de bienvenida con presentación, buscador de categorías destacadas (Inversión, Argentinas, Mundiales, Económicas, Insumos, Varios), marquesina de novedades en tiempo real y modal interactivo de novedades.
  - **Catálogo Interactivo (`data-view="catalog"`)**: Grilla responsiva de piezas con carga optimizada de imágenes (WebP y fallback JPEG), efecto flip de anverso/reverso, vista de estado (*Sin Circular*, *Excelente*, *Muy Bueno*, *Vendido*, *A pedido*) y navegación fluida sin recarga de página.
- **Identidad Boca Juniors (Azul y Oro)**:
  - Paleta *Azul Xeneize* (`#001C58`, fondos azul noche profundos con gradientes radiales elegantes).
  - Acentos *Oro Xeneize* (`#FCB813`, dorado vibrante para monogramas, botones, bordes, ribbons e insignias).
  - Efecto lumínico de halo dorado dinámico (`glow.js`) que acompaña con suavidad los movimientos del puntero en GPU.
- **Carrito de Compras & Checkout Completo (`cart.js`)**:
  - Drawer deslizante interactivo con persistencia local en `localStorage`.
  - Selector de entregas (Punto de encuentro en Parque Rivadavia o envíos a domicilio/sucursal).
  - Medios de pago por transferencia / depósito bancario (datos bancarios y alias configurable).
  - Generación automática de comprobantes y despacho ágil por WhatsApp o FormSubmit.
- **Switch Multidivisa en Vivo (USD / ARS)**:
  - Alternador flotante e instantáneo de moneda entre Dólares y Pesos Argentinos con cotización actualizada y redondeo comercial inteligente.
- **Ficha de Detalle Individual (`detalle.html`)**:
  - Zoom de alta resolución, especificaciones técnicas completas (país, metal, año, peso, diámetro, tirada, catálogo KM/CJ), botón de consulta directa por WhatsApp y carrusel de piezas relacionadas.
- **Cumplimiento Legal y Confianza**:
  - Páginas de Envíos y Devoluciones, Términos y Condiciones, Privacidad y Botón de Arrepentimiento conforme a la normativa argentina.

---

## 📂 Estructura del Proyecto

```text
dac-monedas/
├── index.html                  # Página principal (Portada y Catálogo)
├── detalle.html                # Ficha de detalle de producto
├── envios-y-devoluciones.html   # Información de envíos y garantías
├── terminos.html               # Términos y condiciones
├── privacidad.html             # Política de privacidad
├── arrepentimiento.html        # Formulario legal de arrepentimiento
├── gracias.html                # Confirmación de pedido
├── styles.css                  # Estilos únicos del sitio (Azul y Oro)
├── common.js                   # Lógica compartida, divisas y helpers
├── script.js                   # Controlador del catálogo y filtros
├── cart.js                     # Carrito de compras y checkout
├── glow.js                     # Animación del halo del puntero
├── coins.json                  # Catálogo de monedas de muestra
├── config.json                 # Parámetros del vendedor y de marca
├── .nojekyll                   # Compatibilidad con GitHub Pages
└── images/                     # Fotos de monedas y recursos gráficos
    ├── og-image.png            # Isologo oficial Dac Monedas
    └── thumbs/                 # Miniaturas WebP optimizadas
```

---

## 🚀 Despliegue Local o en GitHub Pages

Al tratarse de un sitio estático, puede servirse con cualquier servidor web HTTP o alojarse directamente en **GitHub Pages**:

```bash
# Servir localmente con Python
python3 -m http.server 8000
```

Accedé a `http://localhost:8000` en tu navegador.

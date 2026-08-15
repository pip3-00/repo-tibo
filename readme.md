# Página de ventas — TikTok Monetización (versión gris)

DEMO:https://pip3-00.github.io/repo-tibo/

Landing page tipo funnel inspirada en el video de referencia, adaptada a una
paleta en escala de grises (grafito/steel) en lugar de morado/negro.

## Archivos del proyecto

```
pagina-tiktok-gris/
├── index.html                    # Página principal (funnel de ventas)
├── styles.css                    # Estilos de index.html
├── index-sin-css.html            # Solo HTML de la página principal, sin estilos
├── politica-de-privacidad.html   # Página legal (autocontenida, con su propio CSS)
└── README.md                     # Este archivo
```

## Cómo usarlo

1. Descarga toda la carpeta `pagina-tiktok-gris/` completa — `index.html`
   necesita a `styles.css` en la misma ubicación para verse bien.
2. Ábrelo localmente haciendo doble clic en `index.html`, o súbelo tal cual
   a tu hosting / Systeme.io / donde vayas a publicar la página.
3. `politica-de-privacidad.html` no depende de ningún otro archivo — puedes
   subirla sola si lo necesitas.

## Qué debes personalizar antes de publicar

**En `index.html`:**
- `TuMarcaDigital` y `tudominio.systeme.io` → nombre y dominio reales
- Textos de la sección hero, dolor, precios y testimonios → tu copy real
- Precios `$29` / `$117` → tus precios reales
- Los `href="#"` de los botones → tu link real de WhatsApp o checkout
- Las estadísticas del `proof-card` y los `tcard` (testimonios) → capturas
  o cifras reales; ahora mismo son de ejemplo

**En `politica-de-privacidad.html`:**
- `hola@tudominio.com` → tu correo real
- `+1 (___) ___-____` → tu número de WhatsApp
- Nombre y dominio del negocio (igual que en `index.html`)
- Revisa que los proveedores mencionados (PayPal, Systeme.io, WhatsApp)
  coincidan con los que realmente usas

## Paleta de colores

Definida como variables CSS al inicio de `styles.css`:

| Variable | Color | Uso |
|---|---|---|
| `--graphite-950` | `#111113` | Fondos más oscuros (hero, CTA final) |
| `--graphite-900` | `#18181b` | Tarjetas de precio |
| `--graphite-800` | `#232327` | Bordes, acentos oscuros |
| `--graphite-700` | `#33333a` | Bordes secundarios |
| `--graphite-500` | `#6b6b74` | Texto secundario |
| `--graphite-300` | `#a8a8b0` | Texto sobre fondo oscuro |
| `--steel-100` | `#e7e7ea` | Acento claro, botones, destacados |
| `--paper` | `#f3f2f0` | Fondo general de secciones claras |
| `--paper-card` | `#ffffff` | Fondo de tarjetas |

Para ajustar el tono de gris de toda la página, cambia estos valores en un
solo lugar y se propaga a todos los elementos.

## Estructura de `index.html`

1. **Topbar** — simula la barra del navegador/app del video de referencia
2. **Hero** — titular, badge y tarjeta de prueba social (gráfico)
3. **Pain** — pregunta de dolor + tarjeta con el problema/solución
4. **Pricing** — dos opciones de precio, una destacada como "más completo"
5. **Results** — testimonios en scroll horizontal
6. **Final CTA** — último empujón con los dos botones de compra
7. **Footer** — enlaces a políticas y condiciones

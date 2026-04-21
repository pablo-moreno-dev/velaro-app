# Velaro — Landing Page

Landing oficial de **Velaro** · Descubre tu estilo · +60 marcas · 40.000 prendas

---

## 📁 Estructura del proyecto

```
velaro-landing/
├── index.html                  ← La landing (HTML + CSS + JS en un solo archivo)
├── images/
│   ├── logo.png                ← Logo V (nav, footer, favicon, CTA)
│   ├── hero-screen.jpg         ← Mockup iPhone del hero (pantalla Colección)
│   ├── feature-swipe.jpg       ← Mockup Feature 01 (swipe con ♥ ✕)
│   ├── feature-buscar.jpg      ← Mockup Feature 02 (búsqueda visual)
│   ├── feature-marcas.jpg      ← Mockup Feature 03 (favoritos)
│   └── feature-ficha.jpg       ← Mockup bonus (ficha de producto)
└── README.md
```

---

## 🚀 Subir a GitHub Pages

### 1. Crea el repositorio
1. Entra en [github.com/new](https://github.com/new)
2. Nombre: `velaro-landing`
3. Marca **Public**
4. Crea el repositorio

### 2. Sube los archivos (incluida la carpeta images)

**Truco importante** — para subir una carpeta en GitHub:

1. En tu repo vacío, click en **"uploading an existing file"**
2. **Arrastra directamente la carpeta `images/`** (no los archivos sueltos) desde tu explorador a la zona de upload
3. GitHub mantiene la estructura automáticamente
4. Arrastra también `index.html` y `README.md`
5. Commit changes

### 3. Activa GitHub Pages
1. **Settings → Pages**
2. En **Source**: branch `main`, folder `/ (root)`
3. Save

En 1-2 minutos tu landing estará en:
```
https://TU-USUARIO.github.io/velaro-landing/
```

### 4. (Opcional) Dominio propio

Si tienes `velaro.app` u otro dominio:
1. **Settings → Pages → Custom domain** → introduce el dominio
2. En tu proveedor DNS, crea un CNAME apuntando a `TU-USUARIO.github.io`
3. Activa **Enforce HTTPS**

---

## 🎨 Personalización

Todo el estilo está en el `<style>` al principio de `index.html`. Variables principales:

```css
:root {
  --bg: #ffffff;          /* fondo */
  --bg-soft: #f5f3ef;     /* fondo cálido */
  --ink: #0a0a0a;         /* negro tinta */
  --muted: #8a8680;       /* gris cálido */
  --line: #e8e6e0;        /* líneas */
}
```

### Cambiar textos
Busca los comentarios `<!-- ==================== NOMBRE ==================== -->` en el HTML.

### Cambiar enlace de Google Play
Busca `play.google.com/store/apps/details?id=com.velaro.app` (3 apariciones).

### Cambiar marcas del ticker
Sección `<!-- ==================== MARQUEE ==================== -->` — edita la lista (aparece duplicada por el loop continuo, edita ambas).

### Reemplazar imágenes
Simplemente sustituye cualquier archivo en `/images/` manteniendo el mismo nombre.

---

## 🛠 Stack

- HTML5 + CSS puro + JS vanilla
- Fuentes: **Playfair Display** (serif) + **Inter Tight** (sans)
- Cero dependencias, cero build, cero npm
- 100% responsive
- Imágenes optimizadas (total <1 MB)
- Respeta `prefers-reduced-motion`

---

## 📝 Licencia

© 2026 Velaro. Todos los derechos reservados.

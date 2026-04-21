# Velaro — Landing Page

Landing oficial de **Velaro** · Descubre tu estilo · +60 marcas · 40.000 prendas

---

## 📁 Estructura del proyecto

```
velaro-landing/
├── index.html          ← La landing completa (HTML + CSS + JS en un solo archivo)
├── images/
│   ├── logo.png         ← Logo V (nav, footer, favicon, CTA)
│   ├── hero.png         ← Portada editorial del hero
│   ├── feature-swipe.png    ← Feature 01
│   ├── feature-buscar.png   ← Feature 02
│   └── feature-marcas.png   ← Feature 03
└── README.md
```

---

## 🚀 Subir a GitHub Pages (paso a paso)

### 1. Crear el repositorio

1. Entra en [github.com/new](https://github.com/new)
2. Nombre sugerido: `velaro-landing`
3. Marca **Public** (GitHub Pages gratis requiere repo público)
4. **NO** marques "Add a README" (ya lo tenemos)
5. Click en **Create repository**

### 2. Subir los archivos

**Opción A — Interfaz web (más fácil):**

1. En tu nuevo repo vacío, click en **"uploading an existing file"**
2. Arrastra **index.html**, la carpeta **images/** completa, y **README.md**
3. Escribe un commit message: `Initial commit`
4. Click en **Commit changes**

**Opción B — Con Git (terminal):**

```bash
cd velaro-landing
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/velaro-landing.git
git push -u origin main
```

### 3. Activar GitHub Pages

1. En tu repo, ve a **Settings** (pestaña superior)
2. En el menú izquierdo, busca **Pages**
3. En **Source**, selecciona:
   - Branch: `main`
   - Folder: `/ (root)`
4. Click en **Save**
5. Espera 1-2 minutos

Tu landing estará online en:
```
https://TU-USUARIO.github.io/velaro-landing/
```

### 4. (Opcional) Dominio personalizado

Si tienes `velaro.app` o similar:

1. **Settings → Pages → Custom domain** → introduce tu dominio
2. En tu proveedor de DNS, crea un registro **CNAME** apuntando a `TU-USUARIO.github.io`
3. Activa **Enforce HTTPS** (tras 10-20 min cuando valide el dominio)

---

## 🎨 Cómo personalizar

Todo el estilo está en el `<style>` al principio de `index.html`. Las variables clave:

```css
:root {
  --bg: #ffffff;          /* fondo principal */
  --bg-soft: #f5f3ef;     /* fondo cálido (feature visuals) */
  --ink: #0a0a0a;         /* negro tinta */
  --muted: #8a8680;       /* gris cálido */
  --line: #e8e6e0;        /* líneas divisorias */
}
```

### Cambiar textos

Cada sección está marcada con comentarios HTML como:
```html
<!-- ==================== HERO ==================== -->
```

Los más importantes:
- **Hero**: busca `Descubre / tu / estilo.`
- **Strap (banda negra)**: las tres cifras clave (60, 40.000, 1 gesto)
- **Features**: títulos `Desliza y explora`, `Haz una foto...`, `Un armario infinito`
- **CTA final**: `Tu próximo fondo de armario...`

### Cambiar marcas del ticker

Busca `<!-- ==================== MARQUEE ==================== -->`. Duplica la lista (aparece dos veces para que el loop sea continuo sin saltos).

### Cambiar el enlace de Google Play

Búsqueda global de `play.google.com/store/apps/details?id=com.velaro.app` (aparece 3 veces: nav, hero, CTA final).

### Reemplazar imágenes

Sustituye cualquier archivo en `/images/` manteniendo **el mismo nombre** y la landing seguirá funcionando.

---

## 🛠 Stack

- HTML5 + CSS puro + JS vanilla
- Fuentes: **Playfair Display** (serif editorial) + **Inter Tight** (sans)
- **Cero dependencias de build** · Cero npm · Cero bundler
- 100% responsive
- Animaciones respetan `prefers-reduced-motion`

---

## 📝 Licencia

© 2026 Velaro. Todos los derechos reservados.

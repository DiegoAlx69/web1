# Level Music — Landing Page

Landing page para una escuela de guitarra en Lima con formulario de reservas, animaciones de scroll y diseño oscuro minimalista.

---

## Demo

🔗 [levelmusic.vercel.app](https://levelmusic.vercel.app/)

---

## Tecnologías

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Formspree](https://img.shields.io/badge/Formspree-ED5B4F?style=flat&logo=formspree&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat&logo=vercel&logoColor=white)

---

## Características

- **Hero con imagen de fondo** — foto en escala de grises con gradiente oscuro para legibilidad del texto
- **Contadores animados** — los precios suben solos con easing al hacer scroll hasta la sección de planes, activándose una sola vez via `IntersectionObserver`
- **Formulario conectado a Formspree** — envío sin recarga, validación client-side, estado de carga y mensaje de confirmación con fade
- **FAQ con acordeón** — JavaScript nativo, sin librerías
- **Scroll reveal** — las secciones aparecen con transición suave al entrar al viewport
- **Responsive completo** — nav con hamburger animado, grids que se apilan en mobile
- **SEO y Open Graph** — meta tags completas incluyendo Twitter Card y og:image personalizado a 1200×630

---

## Estructura del proyecto

```
/
├── index.html        # Página principal (todo en un solo archivo)
├── guitar2.jpg       # Imagen de fondo del Hero
├── mastil.jpg        # Imagen del bento de currículo
└── og-image.jpg      # Imagen para compartir en redes (1200×630)
```

---

## Cómo ejecutar localmente

No requiere dependencias ni build step. Tailwind se carga vía CDN.

1. Clona el repositorio:
   ```bash
   git clone https://github.com/tu-usuario/level-music.git
   cd level-music
   ```

2. Abre `index.html` directamente en el navegador, o usa Live Server si tienes VS Code:
   ```bash
   # Con la extensión Live Server instalada
   code .
   # Clic derecho sobre index.html → "Open with Live Server"
   ```

3. Para que el formulario funcione, reemplaza `TU-ENDPOINT` en el script de `index.html` con tu ID real de [Formspree](https://formspree.io):
   ```js
   fetch('https://formspree.io/f/TU-ENDPOINT', { ... })
   ```

---

## Despliegue

El proyecto está desplegado en Vercel directamente desde este repositorio. Cualquier push a `main` genera un nuevo deployment automático.

Para conectar tu propio repositorio a Vercel:

1. Importa el repo en [vercel.com/new](https://vercel.com/new)
2. No necesitas configurar nada — Vercel detecta que es un sitio estático
3. El deployment queda listo en menos de un minuto

---

## Licencia

MIT

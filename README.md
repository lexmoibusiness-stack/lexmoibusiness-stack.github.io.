# Lex Portfolio

Portfolio personal de Moisés Acevedo Avendaño. Arquitecto de Sistemas IA, Operaciones y Automatización. Builder.

Sitio en producción: https://lexmoibusiness-stack.github.io/Lex-Portfolio/

---

## Preview

> Screenshot del portfolio en producción

El sitio es una single-page application estática de 10 secciones que presenta servicios, proyectos propios, casos públicos y canales de contacto.

---

## Stack

Sitio estático sin build step. Sin frameworks, sin bundler, sin dependencias npm.

- HTML5 semántico
- CSS3 puro (sin Tailwind, sin preprocesadores)
- Tipografías servidas desde Google Fonts:
  - Cormorant Garamond (display / titulares)
  - Syne (acentos)
  - DM Mono (números, código, etiquetas técnicas)
- Calendly inline widget embebido en la sección de contacto
- Hosting: GitHub Pages

---

## Estructura del portfolio

El archivo `index.html` contiene 10 secciones en orden de scroll:

1. Hero con posicionamiento y CTA principal
2. Propuesta de valor
3. Servicios
4. Proyectos propios (Lex Consultor Agents, Lector Lex, Player's Stats)
5. Casos públicos validados
6. Apariciones en medios y publicaciones
7. Vertical dealers automotriz
8. Ventajas competitivas
9. Stack técnico y herramientas
10. Contacto con widget Calendly

Toda la maquetación, estilos y contenido viven en archivos planos en la raíz del repo.

---

## Correr localmente

El sitio no requiere compilación. Hay tres formas de levantarlo:

### Opción 1: abrir el HTML directamente

```bash
# Desde el repo clonado
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

Funciona para revisar contenido. Algunos navegadores bloquean ciertas features cuando el origen es `file://`; para una vista 1:1 con producción usar las opciones 2 o 3.

### Opción 2: Python (built-in)

```bash
python -m http.server 8000
# Abrir http://localhost:8000
```

### Opción 3: npx serve

```bash
npx serve .
# Abrir la URL que imprime en consola
```

---

## Deployment

El despliegue se hace por GitHub Pages desde la rama por defecto del repo. Cualquier push a la rama principal publica el sitio en pocos segundos.

Configuración: Settings, Pages, Source: rama principal, carpeta raíz.

URL pública: https://lexmoibusiness-stack.github.io/Lex-Portfolio/

---

## Contacto

El CTA principal del hero y la sección final del sitio incluyen el widget de Calendly para agendar una llamada. Toda la información de contacto vigente vive en el portfolio en producción.

Para colaboraciones o consultas técnicas, usar el formulario y el calendario integrados en la página.

- **Email:** lex.moi.business@gmail.com
- **WhatsApp:** +58 424 292 19 42
- **Calendly:** https://calendly.com/lex-moi-business/30min

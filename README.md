# LC Abogados Corp. — Sitio web editorial

Sitio web completo de la firma LC Abogados Corp., desarrollado según la **Ficha de identidad y dirección visual v2.0**.

Dirección creativa: minimalismo de alto impacto inspirado en estudios de arquitectura contemporánea (fotografía de gran formato, tipografía protagonista, composición asimétrica, ritmo editorial).

---

## Estructura del proyecto

```
lc-abogados-site/
├── index.html              # Inicio
├── servicios.html          # Servicios (7 áreas)
├── estudio.html            # Nuestro estudio
├── experiencia.html        # Experiencia y testimonios
├── conocimiento.html       # Artículos, FAQ, actualizaciones
├── contacto.html           # Formulario y datos de contacto
├── css/
│   └── styles.css          # Sistema de diseño completo
├── js/
│   └── main.js             # Navegación, reveal, form, FAQ
├── images/                 # (vacío — usar URLs temporales o archivos locales)
└── README.md
```

---

## Cómo visualizar el sitio

### Opción 1 — Abrir directamente
Abre `index.html` en un navegador moderno (Chrome, Firefox, Safari, Edge).

### Opción 2 — Servidor local (recomendado)
Desde la carpeta del proyecto:

```bash
# Python
python3 -m http.server 8080

# o Node (si tienes npx)
npx serve .
```

Luego visita `http://localhost:8080`.

---

## Sistema visual aplicado

| Elemento | Valor |
|----------|--------|
| **Azul institucional profundo** | `#172B40` |
| **Grafito** | `#20272C` |
| **Azul pizarra** | `#536B78` |
| **Blanco cálido** | `#F3F2EE` |
| **Gris mineral** | `#DCE3E3` |
| **Cobre apagado** | `#A87959` |
| **Titulares** | Manrope (Google Fonts) |
| **Cuerpo** | Source Sans 3 (Google Fonts) |

### Composición
- Hero a pantalla completa (~100 vh) con fotografía de fondo, titular grande a la izquierda y texto lateral a la derecha.
- Secciones alternadas (oscuro / claro / mineral).
- Retícula asimétrica y tipografía de gran escala.
- Sin tarjetas genéricas redondeadas, sin sombras pesadas, sin glassmorphism.
- Animaciones discretas con respeto a `prefers-reduced-motion`.

---

## Contenido y validaciones pendientes

**No se ha inventado información institucional.** Todo dato no confirmado aparece como:

`[INFORMACIÓN POR VALIDAR]` o marcadores equivalentes.

### Lista de validaciones necesarias (según ficha v2.0)

1. Servicios prioritarios, vigentes y rentables.
2. Segmentos de clientes prioritarios.
3. Diferenciales reales frente a otros estudios.
4. Nombres, cargos, especialidades y credenciales del equipo.
5. Años de experiencia y cifras institucionales.
6. Testimonios y autorización para nombres/logotipos.
7. Teléfonos, WhatsApp, correos, dirección y horarios.
8. Fotografías reales de equipo, oficina y reuniones.
9. Redes sociales oficiales y enlaces funcionales.
10. Aprobación del tono y del concepto de comunicación.

### Imágenes
Las fotografías actuales son de Unsplash (arquitectura e interiores profesionales) y están marcadas como **temporales**. Deben reemplazarse por material autorizado de LC Abogados o por recursos licenciados correctamente. No se presentan como proyectos, oficinas o equipo de la firma.

---

## Edición de contenidos

| Qué editar | Dónde |
|------------|--------|
| Textos del hero y mensajes principales | `index.html` |
| Listado y descripciones de servicios | `servicios.html` |
| Presentación del estudio y equipo | `estudio.html` |
| Testimonios y casos | `experiencia.html` |
| Artículos y FAQ | `conocimiento.html` |
| Datos de contacto y formulario | `contacto.html` |
| Colores, tipografía, espaciados | `css/styles.css` (`:root`) |
| Comportamiento (menú, form, animaciones) | `js/main.js` |

Para sustituir imágenes temporales:
1. Descarga o prepara archivos optimizados (WebP/AVIF preferible).
2. Colócalos en `images/`.
3. Actualiza los `src` de las etiquetas `<img>` y elimina las notas “Imagen temporal”.

---

## Formulario de contacto

El formulario valida campos en el cliente y muestra un mensaje de éxito simulado.  
**Para producción** conectar a un endpoint real (Formspree, Netlify Forms, API propia, etc.) y actualizar el manejador en `js/main.js`.

WhatsApp: sustituir el marcador por un enlace del tipo  
`https://wa.me/XXXXXXXXXXX?text=Hola%2C%20quisiera%20orientación...`

---

## SEO y accesibilidad

- Títulos y meta descriptions por página.
- Estructura semántica (`header`, `main`, `nav`, `section`, `footer`).
- Contraste revisado sobre fondos oscuros y claros.
- Navegación por teclado y estados focus.
- `prefers-reduced-motion` respetado.
- Etiquetas en formulario y mensajes de estado.

---

## Próximos pasos recomendados

1. Validar con LC Abogados todos los datos marcados.
2. Sustituir imágenes temporales por material autorizado.
3. Completar perfiles del equipo y testimonios reales.
4. Conectar formulario y WhatsApp.
5. Publicar aviso de privacidad y términos.
6. (Opcional) Migrar a Next.js/React si se requiere CMS o internacionalización.

---

**Dirección creativa y desarrollo:** alineados a la Ficha de identidad v2.0 · LC Abogados Corp.

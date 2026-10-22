# Andrés Sabogal — Lengua · Literatura · Educación

Sitio web estático, responsive y editorial para la marca académica del profesor Andrés Sabogal. Estética basada en negro, carbón, grises y beige, con collage de papel, tipografía literaria y fotografías de referencia.

## Abrir la web

1. Descomprime el ZIP.
2. Abre `index.html` en tu navegador. Recomendado: extensión Live Server de VS Code o `python -m http.server 8000` y visita `http://localhost:8000`.
3. Si tienes internet, las fotos editoriales se cargarán desde Unsplash. Sin internet se muestra un gráfico de reemplazo; **las fotos no están incluidas físicamente en el ZIP**.

## Estructura

```text
andres-sabogal/
├── index.html                   Página principal
├── privacidad.html              Aviso provisional de privacidad
├── assets/
│   ├── css/styles.css           Diseño, colores y responsive
│   ├── js/config.js             Contacto, foto del profesor, imágenes
│   ├── js/data.js               Cursos, programas, precios y temarios
│   ├── js/app.js                Interacciones y formularios
│   └── img/
│       └── foto-pendiente.svg   Reemplazo si no carga una imagen
├── docs/
│   ├── PERSONALIZACION.md       Guía de cambios
│   └── LANZAMIENTO.md           Pendientes legales y comerciales
└── README.md
```

## Lo que ya funciona

- Menú responsive, navegación por secciones y botones.
- Filtros por área de formación.
- Fichas de cursos en ventanas con temario, duración, modalidad y precio sugerido.
- Selección de un curso que lo lleva al formulario con ese programa elegido.
- Formulario validado que prepara un mensaje de WhatsApp o correo (cuando se configure un contacto real).
- Tarjetas de programas, biblioteca informativa, secciones de clases particulares y comunidad.
- Imágenes editoriales remotas con respaldo visual local.
- Enlaces de contacto configurables.

## Lo que NO hace todavía

Este sitio **no es un LMS**: no crea cuentas, no almacena estudiantes, no tiene panel administrativo, no cobra, no envía correos automáticamente, no comprueba cupos y no emite certificados. No se anuncia lo contrario. Para esas funciones se necesita un backend o integración segura con un proveedor externo. La página de privacidad es un borrador y debe sustituirse antes de una operación comercial real.

## Contacto y fotografías

En `assets/js/config.js` completa `whatsapp` (57 + número colombiano, sin espacios) y/o `email`. Para la foto de Andrés, copia su fotografía real a `assets/img/andres-sabogal.jpg`. Para cambiar una foto editorial, añade el archivo a `assets/img/` y reemplaza la URL correspondiente en `config.js` por `assets/img/nombre.jpg`.

## Cursos y precios

Edita `assets/js/data.js`. Todos los precios, duraciones y programas son **propuestas comerciales**, no información confirmada por el profesor. Evita publicar títulos académicos sin verificar. Las inscripciones requieren confirmación humana.

## Publicar en GitHub + Vercel

1. Crea un repositorio nuevo en GitHub y sube el **contenido** de la carpeta `andres-sabogal` (con `index.html` en la raíz).
2. En Vercel, `Add New → Project`, importa el repositorio.
3. Framework Preset: `Other`; no se necesita comando de compilación; Output Directory: `.`.
4. Publica y prueba botones, imágenes y formulario en móvil.
5. Antes de aceptar estudiantes, completa los puntos de `docs/LANZAMIENTO.md`.

## Créditos

Fuentes: Google Fonts (DM Sans, DM Mono, Playfair Display). Fotografías de referencia cargadas desde Unsplash (sujetas a disponibilidad, atribución y términos del proveedor). No se incluyen fotos ni retratos generados del profesor.

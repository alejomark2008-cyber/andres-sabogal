# Personalización rápida

## Cambiar colores

En `assets/css/styles.css`, al inicio, edita las variables de `:root`:

- `--black`: fondo negro.
- `--char`, `--char2`: superficies oscuras.
- `--paper`, `--cream`: fondos y textos claros.
- `--beige`: botones, acentos y detalles.

## Agregar fotografía real del profesor

1. Guarda una fotografía autorizada como `assets/img/andres-sabogal.jpg`.
2. Procura una imagen vertical, bien iluminada, de al menos 1000 × 1200 px.
3. No uses fotografías inventadas o retratos sintéticos como si fueran del profesor.
4. La página mostrará automáticamente la fotografía si existe.

## Cambiar fotos de cursos

El sitio trae URLs de fotos editoriales de Unsplash (requieren conexión). Para independizarte de servicios externos, guarda fotografías reales con autorización en `assets/img/` y modifica el objeto `photos` en `assets/js/config.js`.

Ejemplo: `literature: 'assets/img/literatura.jpg'`.

## Editar datos y programas

En `assets/js/data.js`, cada curso tiene `id`, `name`, `tag`, `type`, `duration`, `frequency`, `format`, `price`, `image`, `description`, `topics` y `audience`.

- `price: null` indica «Consultar disponibilidad».
- `type: 'programa'` lo ubica en la sección de programas; `type: 'curso'` o `'taller'` en el catálogo de cursos.
- `image` debe corresponder a una clave del objeto `photos` de `config.js`.
- Los nombres de `tag` permiten filtrar los cursos. Usa una categoría existente.

## Ajustar la biografía

Busca `Hola, soy` en `index.html` y reemplaza la biografía provisional por información confirmada: título profesional, posgrados reales, años de experiencia y publicaciones si las tiene.

## Contacto e inscripción

Configura al menos un método de contacto en `assets/js/config.js`. El formulario abre WhatsApp con un mensaje redactado o prepara un correo; el estudiante debe enviarlo. Si no hay contacto, intenta copiar el texto al portapapeles. No almacena datos.

## Biblioteca y comunidad

Los botones muestran información provisional. Para subir PDF, recursos, clases grabadas, eventos o publicaciones reales hay que agregar los archivos y enlaces, respetando derechos de autor. Para crear cuentas o una biblioteca privada se requiere desarrollo adicional.

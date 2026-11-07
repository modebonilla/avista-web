# Sitio web AVISTA

Sitio de una sola página, sin dependencias ni instalación. Funciona directo en **GitHub Pages**.

## Estructura
```
index.html        ← todo el sitio (textos, estilos y funciones)
assets/img/       ← fotografías
assets/logos/     ← logotipos de AVISTA y de clientes
```

## Publicar en GitHub Pages (5 minutos)
1. Entra a github.com → **New repository** → nómbralo, por ejemplo, `avista-web` → **Create repository**.
2. Haz clic en **uploading an existing file** y arrastra **el contenido** de esta carpeta (index.html, README.md y la carpeta assets).
3. Haz clic en **Commit changes**.
4. Ve a **Settings → Pages**. En *Branch* elige `main` y carpeta `/ (root)` → **Save**.
5. En 1–2 minutos el sitio estará en `https://TU-USUARIO.github.io/avista-web/`.

### Dominio propio (opcional)
En **Settings → Pages → Custom domain** escribe, por ejemplo, `avista.mx` y configura en tu proveedor de dominio un registro CNAME hacia `TU-USUARIO.github.io`.

## Agregar datos de contacto
Abre `index.html` (en GitHub: clic en el archivo → ícono del lápiz) y busca este bloque al inicio:

```js
const CONTACTO = {
  whatsapp: "",   // solo números con clave de país, ej. "522281234567"
  correo: "",
  telefono: ""
};
```

Llena los datos y guarda (**Commit changes**). Automáticamente:
- aparecen las tarjetas de WhatsApp, correo y teléfono en la sección de contacto;
- se activa el formulario, que abre WhatsApp (o el correo) con el mensaje del cliente ya escrito.

Mientras estén vacíos, el formulario permanece oculto para no mostrar un botón que no envía nada.

## Cambiar fotos
Reemplaza los archivos de `assets/img/` por fotografías reales con el mismo nombre (truck.jpg, van.jpg, etc.). Se recomiendan JPG de máximo 1800 px de ancho.

# Operación MK Ultra — Invitación

Invitación interactiva estilo memorando clasificado, con medalla deslizante
para descifrar el mensaje y recuadros tachados que se raspan para revelar
fecha, hora, zona y demás datos.

## Uso local

npm install
npm run dev

Abre la URL que muestra la terminal (por defecto http://localhost:5173).

## Generar la versión final para publicar

npm run build

Esto crea la carpeta `dist/` con el sitio ya listo (un solo `index.html`
autocontenido, sin dependencias externas salvo la tipografía de Google Fonts).

## Publicarlo (elige una opción)

### Opción A — Netlify (la más simple, sin cuenta técnica)
1. Ejecuta `npm run build`.
2. Entra a https://app.netlify.com/drop
3. Arrastra la carpeta `dist` completa a esa página.
4. Netlify te da un link público al instante (algo como
   `nombre-al-azar.netlify.app`). Puedes cambiar el nombre del subdominio
   en Site settings → Change site name.

### Opción B — Vercel
1. Crea una cuenta en https://vercel.com (puedes usar tu GitHub).
2. Sube este proyecto a un repositorio de GitHub.
3. En Vercel, "Add New Project" → importa el repo → Deploy.
   Vercel detecta Vite automáticamente.

### Opción C — GitHub Pages
1. Sube el proyecto a un repositorio de GitHub.
2. Instala el paquete de despliegue:
   npm install -D gh-pages
3. Agrega a package.json en "scripts":
   "deploy": "vite build && gh-pages -d dist"
4. Ejecuta: npm run deploy
5. Activa GitHub Pages en el repo (Settings → Pages → rama gh-pages).

Para todas las opciones, una vez publicado obtienes un link que puedes
enviar directo por WhatsApp a los equipos convocados.

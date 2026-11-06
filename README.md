# Mi línea de la semana

Página estática (un solo `index.html`, sin dependencias ni build) para llevar tus tareas diarias, metas y premios.

## Subirla a GitHub

1. Creá un repositorio nuevo en github.com (por ejemplo `linea-semana`), vacío y sin README.
2. En esta carpeta, en la terminal:

```bash
git init
git add .
git commit -m "Primera versión"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/linea-semana.git
git push -u origin main
```

## Publicarla en Vercel

1. Entrá a vercel.com e iniciá sesión con tu cuenta de GitHub.
2. Add New, Project, elegí el repositorio `linea-semana` e Import.
3. Dejá todo por defecto (Framework: Other, sin build command) y tocá Deploy.
4. Vercel te da un link tipo `linea-semana.vercel.app`. Abrilo desde el celular y agregalo a la pantalla de inicio.

Cada vez que hagas `git push`, Vercel vuelve a publicar solo.

## Importante: dónde se guarda tu progreso

El progreso se guarda en el `localStorage` del navegador, es decir, **solo en el dispositivo y navegador donde lo usás**. Si lo abrís en el celular y en la compu, cada uno tiene su propio progreso, y si borrás los datos del navegador se pierde.
Usalo siempre desde el mismo dispositivo. Si más adelante querés sincronizar entre dispositivos, se puede sumar una base de datos (por ejemplo Vercel KV o Supabase).

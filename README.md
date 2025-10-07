Mini Centro - Sitio estático

Este repositorio contiene una versión estática inicial del sitio "Mini Centro de Datos Didácticos" inspirada en un diseño limpio y elegante similar a páginas de producto.

Archivos principales:
- `index.html` — Página principal (HTML semántico).
- `styles.css` — Estilos CSS con diseño responsive.
- `assets/` — Carpeta para imágenes y recursos.

Cómo ver localmente:

Abrir `index.html` directamente en el navegador o usar un servidor simple (recomendado):

```powershell
# desde la carpeta del proyecto
python -m http.server 8000
# luego abrir http://localhost:8000 en tu navegador
```

Siguientes pasos recomendados:
- Reemplazar imágenes por versiones optimizadas y propias en `assets/`.
- Ajustar textos y enlaces a tu contenido final.
- Desplegar en GitHub Pages o Netlify para publicar.

Si quieres, puedo:
- Ajustar el diseño para seguir más fielmente la estética de Apple (tipografías, espaciado fino, animaciones suaves).
- Crear variantes de color y soporte para modo oscuro.
- Preparar el despliegue automático en GitHub Pages.

Despliegue a GitHub Pages (pasos rápidos desde PowerShell)

1) Crea un repositorio en GitHub (puede ser público). Supongamos que lo llamas `mini-centro`.

2) Desde la carpeta del proyecto en tu PC (PowerShell):

```powershell
# inicializa git (si no lo tienes)
git init
git add .
git commit -m "Initial site"
# reemplaza <TU_USUARIO> y <NOMBRE_REPO> por tus datos
git remote add origin https://github.com/<TU_USUARIO>/<NOMBRE_REPO>.git
git branch -M main
git push -u origin main
```

3) El workflow incluido (`.github/workflows/gh-pages.yml`) desplegará automáticamente el contenido a GitHub Pages cuando hagas push a `main`. GitHub Pages generará una URL con el formato:

- Para repositorios personales/organización: `https://<TU_USUARIO>.github.io/<NOMBRE_REPO>/`

4) Notas y permisos:

- Asegúrate de que el repositorio en GitHub tenga habilitado Pages (en Settings → Pages, si no aparece el sitio, espera unos minutos tras el primer deploy).
- Si quieres, puedo preparar además un workflow para publicar desde una rama `gh-pages` concreta o añadir un `CNAME` si tienes un dominio propio.

Si quieres, puedo ejecutar los pasos que generan el repositorio remoto (crear repo, push) por ti —pero necesitaría acceso a tus credenciales o un token; por seguridad, prefiero darte los comandos y guiarte. ¿Quieres que te muestre exactamente los comandos listos para pegar en PowerShell con tu usuario y repo ya puestos? 

# 💖 Página Romántica para GitHub Pages

## 📝 Descripción
Una hermosa página web con dos pantallas:
1. **index.html**: Pregunta romántica con un botón
2. **princesa.html**: Marco elegante para mostrar la foto de tu novia

## 🚀 Cómo usar GitHub Pages (Guía paso a paso)

### Opción 1: Subir directamente desde el navegador (más fácil)

1. **Crea un repositorio en GitHub**
   - Ve a https://github.com y haz login
   - Click en el botón verde "New" (o "Nuevo")
   - Nombre del repositorio: `mensaje-princesa` (o el que quieras)
   - Marca como "Public" (público)
   - Click en "Create repository"

2. **Sube los archivos**
   - En la página del repositorio nuevo, click en "uploading an existing file"
   - Arrastra los archivos: `index.html` y `princesa.html`
   - Si tienes la foto de tu novia, súbela también (por ejemplo: `foto.jpg`)
   - Click en "Commit changes"

3. **Activa GitHub Pages**
   - Ve a "Settings" (Configuración) del repositorio
   - En el menú lateral, busca "Pages"
   - En "Source", selecciona "main" branch
   - Click en "Save"
   - ¡Espera 1-2 minutos!

4. **Accede a tu página**
   - Tu página estará en: `https://TU-USUARIO.github.io/mensaje-princesa/`
   - GitHub te mostrará la URL exacta en la sección Pages

### Opción 2: Usando Git (si ya lo tienes instalado)

```bash
# 1. Crea una carpeta para tu proyecto
mkdir mensaje-princesa
cd mensaje-princesa

# 2. Copia los archivos index.html y princesa.html a esta carpeta

# 3. Inicializa git
git init
git add .
git commit -m "Mi mensaje romántico"

# 4. Crea el repositorio en GitHub (desde el navegador)
# Luego conecta tu carpeta local:
git remote add origin https://github.com/TU-USUARIO/mensaje-princesa.git
git branch -M main
git push -u origin main

# 5. Activa GitHub Pages desde Settings > Pages (como en la Opción 1)
```

## 📸 Para agregar la foto de tu novia

### Método 1: Editar directamente en GitHub
1. Sube la foto al repositorio (por ejemplo: `foto.jpg`)
2. Click en `princesa.html` para editarlo
3. Click en el ícono del lápiz (Edit)
4. Busca esta línea:
   ```html
   <div class="photo-placeholder">
   ```
5. Reemplázala con:
   ```html
   <img src="foto.jpg" alt="Mi Princesa" class="photo">
   ```
6. Guarda los cambios (Commit changes)

### Método 2: Editar en tu computadora
1. Abre `princesa.html` con cualquier editor de texto
2. Encuentra el comentario que dice:
   ```html
   <!-- To use a real image, comment out the div above and uncomment this:
   ```
3. Sigue las instrucciones ahí (comenta el placeholder, descomenta el img)
4. Asegúrate que el nombre del archivo en `src="foto.jpg"` coincida con tu foto
5. Guarda y sube los cambios a GitHub

## 🎨 Personalización

### Cambiar colores
Edita las variables CSS al inicio de cada archivo:
```css
:root {
    --rose-petal: #ffc9d9;    /* Rosa suave */
    --deep-rose: #ff85a8;     /* Rosa intenso */
    --soft-cream: #fff8f5;    /* Crema */
    --gold-accent: #d4af37;   /* Dorado */
}
```

### Cambiar el mensaje
En `princesa.html`, busca:
```html
<p class="message">
    La princesa más hermosa del mundo ✨
</p>
```
Y cámbialo por el mensaje que quieras.

## ❓ Preguntas Frecuentes

**P: ¿Cuánto tarda en aparecer mi página?**
R: Normalmente 1-2 minutos después de activar GitHub Pages. Si no aparece, revisa Settings > Pages.

**P: ¿Puedo usar un dominio personalizado?**
R: Sí, en Settings > Pages > Custom domain puedes agregar tu propio dominio.

**P: ¿Es gratis?**
R: Totalmente gratis con GitHub Pages.

**P: ¿Puedo hacerlo privado?**
R: El repositorio puede ser privado, pero GitHub Pages de repositorios privados requiere GitHub Pro.

**P: La imagen no se ve**
R: Asegúrate de que el nombre del archivo sea exactamente igual (mayúsculas/minúsculas importan).

## 💡 Tips

- Usa imágenes en formato JPG o PNG
- Para mejor resultado, usa una foto cuadrada (mismo ancho y alto)
- Puedes probar la página localmente abriendo `index.html` en tu navegador antes de subirla
- Si quieres hacer cambios, edita los archivos y súbelos de nuevo

## 🛠️ Solución de problemas

1. **La página muestra código**: Asegúrate de que los archivos se llamen exactamente `index.html` y `princesa.html`
2. **No aparece nada**: Verifica que GitHub Pages esté activado en Settings
3. **Error 404**: Espera unos minutos más, GitHub Pages puede tardar en actualizar

---

¡Disfruta tu página romántica! 💝

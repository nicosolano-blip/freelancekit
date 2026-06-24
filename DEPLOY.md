# Deploy FreelanceKit a Vercel en 5 minutos

## Requisitos
- Cuenta en [GitHub](https://github.com) (gratis)
- Cuenta en [Vercel](https://vercel.com) (gratis)

## Paso 1: Crear repo en GitHub

```bash
# En la carpeta del proyecto
cd C:\Users\nicos\Documents\Claude\Downloads-Page-Market-Analysis

git init
git add .
git commit -m "Initial commit: FreelanceKit - 39 herramientas para LATAM"

# Crear repo en GitHub.com, copiar URL
git remote add origin https://github.com/TU_USER/freelancekit
git push -u origin main
```

## Paso 2: Deploy en Vercel

1. Ir a https://vercel.com/dashboard
2. Click en **"Add New..." → "Project"**
3. Buscar y seleccionar el repo `freelancekit`
4. **IMPORTANTE:**
   - Build Command: **dejar vacío**
   - Install Command: **dejar vacío**
   - Output Directory: **dejar vacío** (usa `.` por defecto)
5. Click **"Deploy"**

✅ **En 30 segundos estará online** en `freelancekit-xxx.vercel.app`

## Paso 3: Personalizar dominio (Opcional)

1. En Vercel, ir a **Deployments**
2. Click en el dominio → **Domains**
3. Opción A: **Agregar dominio propio** (si tienes)
4. Opción B: **Usar dominio gratuito `.vercel.app`**

## Paso 4: Activar Google Analytics (Opcional)

1. En `index.html`, buscar `gtag('config', 'G-XXXXX');`
2. Crear proyecto en [Google Analytics 4](https://analytics.google.com)
3. Copiar ID (formato: `G-XXXXXXXXXX`)
4. Reemplazar en el código
5. Descomentar la línea de script:
   ```html
   <script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXX"></script>
   ```
6. Commit y push
7. Vercel automáticamente redeploya en <1 min

## Comandos Git para futuros cambios

```bash
# Hacer cambios
# Editar archivos...

# Commit y push
git add .
git commit -m "Mejora: [descripción]"
git push origin main

# Vercel automáticamente redeploya ✅
```

## Monitoreo

- **Uptime:** Vercel proporciona 99.99%
- **CDN global:** Automático
- **HTTPS:** Automático
- **Logs:** En Vercel dashboard → Deployments → Logs

## Solucionar problemas

### El deploy falla
- Revisar logs en Vercel: **Deployments → Failed → Logs**
- Revisar que todos los archivos `.html` estén en la carpeta raíz

### El sitio ve blanco
- Limpiar caché: `Ctrl+Shift+Del`
- Ir a Vercel dashboard y hacer redeploy manual

### Búsqueda no funciona
- Esperar a que se complete el deploy (5-10 seg)
- En Chrome, abrir DevTools (F12) → Console para ver errores

---

**Costo: $0 / mes** ✅
**Tiempo de deploy: <1 minuto** ✅
**Uptime: 99.99%** ✅

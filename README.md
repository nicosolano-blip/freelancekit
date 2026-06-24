# FreelanceKit — 39 Herramientas para LATAM

**39 calculadoras, simuladores y generadores de PDFs** para freelancers, constructores, empleadores y emprendedores. Sin registro, sin instalación, offline.

## 🚀 Stack

- **Frontend:** HTML5 + CSS3 vanilla (sin frameworks)
- **Hosting:** Vercel (static site)
- **Analytics:** Google Analytics (opcional)
- **Pagos:** Lemon Squeezy (integración futura)

## 📦 Contenido

### Categorías (7)
1. **Freelancers & Autónomos** (6 tools) — tarifa hora, cotizaciones, contratos, tracker de horas
2. **Construcción & Oficios** (6 tools) — cálculo de materiales, presupuestos, electricidad
3. **Recursos Humanos** (4 tools) — costo de empleado, liquidación, indemnización
4. **Eventos & Vida Cotidiana** (5 tools) — mudanzas, viajes, mascotas, dietas
5. **Finanzas Personales** (6 tools) — ahorro, deuda, inversión, jubilación
6. **Salud & Bienestar** (4 tools) — IMC, calorías, hidratación, ayuno
7. **Pequeños Negocios** (8 tools) — margen, ROAS, CAC/LTV, flujo de caja

### Herramientas Gratis (7)
- ✅ Tarifa Hora
- ✅ Ladrillos & Cemento
- ✅ Costo Real de Empleado
- ✅ Costo por Persona en Eventos
- ✅ Meta de Ahorro
- ✅ IMC y Peso Ideal
- ✅ Punto de Equilibrio

## 🛠 Desarrollo Local

No hay build step. Simplemente abrir `index.html` en el navegador.

```bash
# Opción 1: Abrir directo
open index.html

# Opción 2: Con servidor local (para testing)
python -m http.server 8000
# o
npx http-server
```

## 🌐 Deploy a Vercel

### Opción A: Via GitHub (Recomendado)

1. Pushear código a GitHub
   ```bash
   git init
   git add .
   git commit -m "Initial commit: FreelanceKit"
   git remote add origin https://github.com/tu-user/freelancekit
   git push -u origin main
   ```

2. Ir a [Vercel](https://vercel.com/import)
3. Conectar repo de GitHub
4. **No necesita build command** (dejar en blanco)
5. Vercel automáticamente sirve `index.html`

### Opción B: Direct Deploy (Sin GitHub)

```bash
npm install -g vercel
vercel
```

Seguir las instrucciones interactivas.

### Configuración (vercel.json)

```json
{
  "buildCommand": "",
  "installCommand": "",
  "framework": "static",
  "outputDirectory": "."
}
```

## 📊 Google Analytics (Opcional)

Para activar tracking:

1. Crear proyecto en [Google Analytics 4](https://analytics.google.com)
2. Copiar el ID (formato: `G-XXXXXXXXXX`)
3. En `index.html`, reemplazar:
   ```javascript
   gtag('config', 'G-XXXXX'); // → tu ID real
   ```
4. Descommentar la línea de Google Analytics script

## 🔒 Seguridad

✅ **Todo corre localmente** — ningún dato sale del navegador del usuario
✅ **No hay backend** — no hay base de datos que hackear
✅ **No hay registro** — no hay credenciales almacenadas
✅ **HTTPS automático** — Vercel lo proporciona gratis

## 💰 Roadmap

- [ ] Integración con Lemon Squeezy para pagos
- [ ] Landing con CTA mejorada
- [ ] Dark mode
- [ ] Exportar resultados a PDF (algunas herramientas ya lo hacen)
- [ ] Traducción a EN/PT

## 📄 Licencia

Privado. Uso exclusivo de FreelanceKit.

---

**Deploy:** Vercel | **Mantenimiento:** 0 USD/mes | **Uptime:** 99.9%

# 🚀 Quick Start — Implementar tu nuevo README

---

## ⚡ Paso 1: Preparar el repositorio

Tu nuevo README debe ir en un repositorio especial de GitHub con tu **username**:

```bash
# Crear o navegar al repo
mkdir ~/Ltomxd
cd ~/Ltomxd

# Si no existe, inicializar git
git init
git remote add origin https://github.com/Ltomxd/Ltomxd.git

# Si ya existe, actualizar
cd ~/Ltomxd
git pull origin main
```

---

## 📝 Paso 2: Reemplazar el README

```bash
# Opción A: Copiar el archivo directamente
cp /ruta/a/README.md ~/Ltomxd/README.md

# Opción B: Crear desde cero y copiar contenido
touch ~/Ltomxd/README.md
# Luego pega el contenido de README.md
```

---

## ✏️ Paso 3: Personalizar (IMPORTANTE)

Abre `README.md` y reemplaza:

```markdown
# CAMBIOS OBLIGATORIOS:

1. Reemplaza "Ltomxd" en todos los links por tu username correcto
2. Actualiza emails a: velasquez8014@gmail.com
3. Actualiza LinkedIn: https://linkedin.com/in/ftoml
4. Actualiza HackTheBox: https://app.hackthebox.com/profile/1767382
5. Actualiza Portfolio: https://portafolio-nextjs.lirictom209.workers.dev/

# CAMBIOS OPCIONALES (pero recomendados):

- Actualiza tabla de "Featured Projects" con tus proyectos reales
- Agrega secciones de Certifications si tienes
- Personaliza "Professional Services" según tus ofertas
- Cambia colores primarios si prefieres otro esquema
```

---

## 🎨 Paso 4: Personalizar Colores (Opcional)

Los colores principales están en varios lugares:

**Color Principal (Lime):** `#9FEF00`
**Color Secundario (Cyan):** `#0ff3ff`
**Color Terciario (Blue):** `#00A1F1`

### Para cambiar esquema de colores globalmente:

1. Abre `README.md`
2. Usa Ctrl+H (Find & Replace)
3. Busca: `9FEF00` → Reemplaza con tu color (sin #)
4. Busca: `0ff3ff` → Reemplaza con tu color
5. Busca: `00A1F1` → Reemplaza con tu color

---

## ✅ Verificación Pre-Push

Antes de hacer commit, verifica:

```markdown
☑️ Links a LinkedIn funcionan
☑️ Links a HackTheBox funcionan
☑️ Links a Portfolio funcionan
☑️ Email es correcto
☑️ Tabla de proyectos está actualizada
☑️ Nombres personales/usernames son correctos
☑️ No hay URLs rotas (verifica en raw.githubusercontent.com)
☑️ Emojis se ven correctamente
☑️ Las imágenes carguen (badges, stats)
```

---

## 🚀 Paso 5: Hacer Push a GitHub

```bash
# Navega al directorio
cd ~/Ltomxd

# Agrega cambios
git add README.md

# Commit
git commit -m "🎨 feat: Nuevo README profesional con arquitectura moderna

- Header wave dinámico con Capsule Render
- GitHub stats y streak automáticos
- Tablas de proyectos y competencias
- Secciones de servicios profesionales
- Esquema de colores consistente (Lima/Cyan/Blue)"

# Push
git push origin main
```

---

## 📊 Paso 6: Verificar en GitHub

1. Navega a **github.com/Ltomxd/Ltomxd**
2. Verifica que el README cargue correctamente
3. Prueba todos los links
4. Espera ~1 minuto para que GitHub actualice la vista previa

**Resultado esperado:**
- ✅ Header wave colorido con tu nombre
- ✅ Badges de perfil views, LinkedIn, HackTheBox, Email
- ✅ Secciones bien organizadas
- ✅ Tablas formateadas correctamente
- ✅ Stats de GitHub actualizados automáticamente

---

## 🔧 Paso 7: Configuración Adicional (Opcional)

### Agregar Snake Animation (GitHub Actions)

Crea `.github/workflows/snake.yml`:

```yaml
name: Generate snake animation

on:
  schedule:
    - cron: "0 0 * * 0"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk@v3
        with:
          github_user_name: Ltomxd
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark
      - uses: crazy-max/ghaction-github-pages@v3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

Luego agrega a README (antes del footer):

```markdown
[![GitHub Contribution Snake](https://raw.githubusercontent.com/Ltomxd/Ltomxd/output/github-contribution-grid-snake-dark.svg)](https://raw.githubusercontent.com/Ltomxd/Ltomxd/output/github-contribution-grid-snake-dark.svg)
```

### Agregar WakaTime Stats (Opcional)

1. Instala WakaTime en VS Code
2. Conecta con tu cuenta GitHub
3. Agrega a README:

```markdown
[![WakaTime Stats](https://github-readme-stats.vercel.app/api/wakatime?username=ltomxd&theme=dark&layout=compact)](https://wakatime.com/@ltomxd)
```

---

## 📋 Checklist de Implementación

```
PREPARACIÓN:
☐ Clonar/navegar a ~/Ltomxd
☐ Crear README.md vacío si no existe

PERSONALIZACIÓN:
☐ Copiar contenido del nuevo README.md
☐ Reemplazar todos los usernames (Ltomxd)
☐ Reemplazar emails y links
☐ Actualizar tabla de proyectos
☐ Verificar colores y emojis

VERIFICACIÓN:
☐ Verificar todos los links localmente
☐ Verificar que no hay placeholder text
☐ Verificar formato markdown
☐ Revisar en VS Code markdown preview

DESPLIEGUE:
☐ git add README.md
☐ git commit con mensaje descriptivo
☐ git push origin main
☐ Verificar en github.com/Ltomxd/Ltomxd

POST-DESPLIEGUE:
☐ Esperar ~2 minutos a que cargue en GitHub
☐ Probar todos los links
☐ Verificar que badges cargan correctamente
☐ Compartir con reclutadores/colegas
```

---

## 🆘 Troubleshooting

### **Problema: Las imágenes/badges no cargan**

**Solución:**
- Espera 5 minutos (GitHub cachea recursos)
- Verifica conexión internet
- Hard refresh: Ctrl+Shift+R
- Verifica que las URLs sean HTTPS

### **Problema: Los links no funcionan**

**Solución:**
- Verifica que no tengas espacios en URLs
- Usa URL encoding para espacios: `%20`
- Verifica que links sean públicos (no requieren login)

### **Problema: El markdown no se ve bien**

**Solución:**
- Verifica indentation (usa espacios, no tabs)
- Cierra todas las secciones correctamente
- Valida markdown en: https://www.markdownlint.com/

### **Problema: Los emojis no aparecen**

**Solución:**
- Verifica encoding UTF-8 en tu editor
- Algunos navegadores/SO antiguos no soportan emojis nuevos
- Usa emojis clásicos si es necesario

### **Problema: GitHub dice "file not found"**

**Solución:**
- Verifica que el repo sea público
- El archivo debe llamarse exactamente `README.md` (mayúsculas)
- Debe estar en la raíz del repositorio (no en carpetas)

---

## 📞 Contacto & Soporte

Si tienes preguntas durante la implementación:

1. **Revisa la documentación:** `README_CUSTOMIZATION.md`
2. **Consulta snippets:** `README_SNIPPETS.md`
3. **Valida markdown:** https://www.markdownlint.com/
4. **Prueba badges:** https://shields.io

---

## 🎉 ¡Listo!

Tu nuevo README profesional está activo. Ahora:

✅ Tu perfil destaca entre reclutadores
✅ Tus proyectos están bien organizados
✅ Tus habilidades son claras y verificables
✅ Tu marca personal es consistente

**Mantén actualizado:**
- Tabla de proyectos (cada 3 meses)
- Links a portfolios (si cambian)
- Competencias técnicas (según aprendas nuevas)
- Stats de GitHub (automático)

---

**Éxito en tu carrera, TOM 🦝**

*Build it. Break it. Secure it.*


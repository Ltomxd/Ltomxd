# 🎨 README Customization Guide for Tom's GitHub Profile

Este documento contiene **instrucciones y snippets** para personalizar y actualizar dinámicamente tu README.

---

## 📋 Elementos Dinámicos Implementados

### 1. **Header Wave (Capsule Render)**
El banner superior con degradado se genera vía Capsule Render. Puedes modificarlo:

```markdown
![Capsule Render - Header](https://capsule-render.vercel.app/api?type=waving&color=0:050409,25:0ff3ff,50:00a1f1,75:02845c,100:9fef00&height=280&section=header&text=Franklyn%20Velásquez&fontSize=64&fontColor=ffffff&fontAlignY=38&fontAlign=50&desc=Pentester%20|%20Red%20Team%20|%20Full%20Stack%20Dev&descAlignY=58&descSize=18&descFontColor=9fef00&stroke=9fef00&strokeWidth=1)
```

**Parámetros ajustables:**
- `color=0:050409,25:0ff3ff...` → Gradiente de colores (hex)
- `text=Tu%20Titulo` → Título principal
- `desc=Tu%20Descripción` → Descripción
- `fontSize=64` → Tamaño del texto
- `descFontColor=9fef00` → Color de la descripción

---

### 2. **GitHub Stats (con tema oscuro)**

```markdown
[![GitHub Stats](https://github-readme-stats-eight-theta.vercel.app/api?username=Ltomxd&show_icons=true&theme=algolia&include_all_commits=true&count_private=true&hide_border=true&title_color=9FEF00&icon_color=00A1F1&text_color=FFFFFF&bg_color=0D1117)](https://github.com/Ltomxd)
```

**Para cambiar el usuario:** Reemplaza `Ltomxd` por tu username.

---

### 3. **GitHub Streak Stats**

```markdown
[![GitHub Streak](https://streak-stats.demolab.com/?user=Ltomxd&theme=dark&hide_border=true&background=0D1117&ring=9FEF00&fire=FF6633&currStreakLabel=9FEF00&sideLabels=9FEF00&dates=FFFFFF&stroke=9FEF00)](https://git.io/streak-stats)
```

---

### 4. **Top Languages**

```markdown
[![Top Languages](https://github-readme-stats-eight-theta.vercel.app/api/top-langs/?username=Ltomxd&layout=compact&langs_count=8&theme=algolia&hide_border=true&title_color=9FEF00&text_color=FFFFFF&bg_color=0D1117)](https://github.com/Ltomxd)
```

---

## 🎨 Paleta de Colores Recomendada (TOM)

```yaml
Primary Colors:
  - Accent Green: #9FEF00 (Lime neon - principal)
  - Cyan: #0ff3ff (Cian brillante)
  - Blue: #00A1F1 (Azul profesional)
  - Dark Green: #02845c (Verde oscuro - contraste)
  - Black: #0D1117 (Fondo oscuro)

Highlights:
  - Orange/Fire: #FF6633 (Para énfasis)
  - White: #FFFFFF (Texto claro)
```

---

## 🔧 Personalización por Sección

### **A. Actualizar proyectos destacados**

En la tabla "Featured Projects", añade/modifica filas:

```markdown
| **Nombre Proyecto** | **Tipo** | **Stack** | **Descripción** |
|:---|:---:|:---|:---|
| 🔐 Nombre Real | Categoría | Tech1 · Tech2 · Tech3 | Breve descripción del impacto |
```

### **B. Añadir nuevas secciones**

Puedes agregar:
- **🎓 Certifications** (OSCP, CEH, Security+, etc.)
- **🏆 Awards & Recognition** (GitHub Achievements, HackTheBox ranks)
- **📚 Articles & Writeups** (Blog posts, security writeups)
- **🔐 Security Findings** (CVEs, Bug Bounties)

Ejemplo:

```markdown
## 🏆 Security Achievements

- 🎯 **HackTheBox Rank:** Pro Hacker (Level XXX)
- 🔴 **CVE Findings:** CVE-2024-XXXXX, CVE-2024-YYYYY
- 🚩 **CTF Championships:** [Event Name] - 1st Place
- 💰 **Bug Bounties:** $X,XXX total bounty earnings
```

### **C. Footer Wave (Capsule Render)**

```markdown
[![Capsule Render - Footer](https://capsule-render.vercel.app/api?type=waving&color=0:020409,25:050f24,50:0a2540,75:02845c,100:00ff9d&height=140&section=footer&text=Build%20it.%20Break%20it.%20Secure%20it.&fontSize=15&fontColor=00ff9d&fontAlignY=68&reversal=true)]
```

---

## 🚀 Instrucciones de Implementación

### **Step 1: Reemplaza tu README actual**

```bash
# Navega a tu directorio de GitHub profile
cd ~/Ltomxd

# Backup de tu README actual (opcional)
cp README.md README.md.bak

# Copia el nuevo README
cp ~/nuevo-README.md README.md

# Commit y push
git add README.md
git commit -m "🎨 refactor: Modernizar perfil GitHub con arquitectura profesional"
git push origin main
```

### **Step 2: Mantén los datos actualizados**

Revisa y actualiza regularmente:
- **GitHub Stats** → Se actualizan automáticamente
- **Streak** → En tiempo real
- **Proyectos** → Actualiza la tabla cuando completes o inicies nuevos
- **Skill Icons** → Usa [skillicons.dev](https://skillicons.dev) para agregar más tecnologías

### **Step 3: Añade badges personalizados**

Crea badges únicos para tus proyectos usando [shields.io](https://shields.io):

```markdown
[![Version](https://img.shields.io/badge/version-1.0.0-9FEF00?style=for-the-badge)](https://github.com/Ltomxd/proyecto)
[![Security](https://img.shields.io/badge/security-CRITICAL-FF6633?style=for-the-badge)](https://github.com/Ltomxd/proyecto)
[![Status](https://img.shields.io/badge/status-PRODUCTION-00ff9d?style=for-the-badge)](https://github.com/Ltomxd/proyecto)
```

---

## 🎯 Advanced Customizations

### **Typing Animation (Readme Typing SVG)**

Para agregar animación de escritura en cualquier sección:

```markdown
![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=18&pause=1000&color=9FEF00&background=0D1117&center=true&vCenter=true&width=750&lines=Security+Engineer;Pentester;Full+Stack+Developer)
```

### **GitHub Contribution Graph**

```markdown
![GitHub Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=Ltomxd&bg_color=0D1117&color=9FEF00&line=00A1F1&point=9FEF00&area=true&area_color=9FEF0033&hide_border=true&radius=8)
```

### **Snake Animation (GitHub Contribution Snake)**

Requiere workflow de GitHub Actions. Agrega este archivo:

`.github/workflows/snake.yml`:

```yaml
name: Generate snake animation

on:
  schedule:
    - cron: "0 0 * * 0" # Weekly
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

---

## 🔐 Security Best Practices para tu README

✅ **DO:**
- Enlaza a portfolios públicos
- Muestra tus proyectos reales
- Usa HTTPS en todos los links
- Mantén contacto profesional

❌ **DON'T:**
- No publiques credenciales o keys
- No enlaces a datos sensibles de clientes
- No expongas rutas internas de sistemas
- No hagas mención de vulnerabilidades no parcheadas

---

## 📊 Métricas que Deberías Monitorear

| Métrica | Herramienta | URL |
|:---|:---|:---|
| **GitHub Activity** | GitHub Insights | `github.com/Ltomxd?tab=overview` |
| **HackTheBox Progress** | HackTheBox | `app.hackthebox.com/profile/1767382` |
| **Profile Views** | Komarev | Generado automáticamente |
| **Contribution Streak** | Streak Stats | Actualizado diariamente |

---

## 🎬 Próximos Pasos

1. ✅ Personaliza colores según tu brand
2. ✅ Actualiza tabla de proyectos
3. ✅ Agrega secciones de certificaciones/awards
4. ✅ Implementa snake animation workflow
5. ✅ Configura Google Analytics (opcional)

---

## 📝 Notas Finales

- Este README está diseñado para ser **dinámico y escalable**
- Todos los badges y gráficos se **actualizan automáticamente**
- Personaliza colores y contenido según necesites
- Mantén el README **fresco y relevante** con tus proyectos actuales

**TOM** 🦝 · Hecho en El Salvador 🇸🇻


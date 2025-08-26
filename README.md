# Whitestack Technology Radar

Este repositorio contiene el **Technology Radar de Whitestack**, diseñado para guiar la adopción, evaluación y exploración de tecnologías abiertas aplicadas a nubes privadas.

El radar se construyó siguiendo el modelo de **Zalando Tech Radar** y contiene tecnologías clasificadas en **cuadrantes** y **anillos**:

- **Cuadrantes**: Languages & Frameworks, Tools, Platforms, Techniques.
- **Anillos**: Adopt, Trial, Assess, Hold.

---

## 🚀 Ver el Radar Online

El radar está disponible en **GitHub Pages**:  
👉 https://sergio-tarazona.github.io/tech-radar/

---

## 📂 Estructura del Repositorio

- `index.html` → Página principal del radar.  
- `radar.json` → Dataset con la lista extendida de tecnologías.  

---

## 🔄 Cómo actualizar el radar

1. Edita `radar.json` para añadir, mover o eliminar tecnologías.  
   - Cada entrada tiene:
     ```json
     {
       "quadrant": 0,
       "ring": 1,
       "label": "Kubernetes Operators",
       "active": true,
       "moved": 0
     }
     ```
   - `quadrant`: 0–3 (Languages & Frameworks, Tools, Platforms, Techniques).  
   - `ring`: 0–3 (Adopt, Trial, Assess, Hold).  
   - `label`: nombre de la tecnología.  
   - `moved`: -1 (baja), 0 (sin cambios), 1 (sube).  

2. Haz commit y push:
   ```bash
   git add radar.json
   git commit -m "Update radar entries"
   git push origin main

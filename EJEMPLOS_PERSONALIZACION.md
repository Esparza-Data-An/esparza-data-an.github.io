# 📝 EJEMPLOS: Cómo personalizar cada sección

Este documento te muestra EJEMPLOS REALES de cómo llenar cada parte del portafolio.

---

## EJEMPLO 1: Personalizar _config.yml

### ❌ ANTES (Genérico)
```yaml
title: "Esparza Data Analytics"
description: "Analista de Datos • Antropólogo | Transformando datos en insights"
```

### ✅ DESPUÉS (Personalizado)
```yaml
title: "Abraham Esparza - Analista de Datos"
description: "Analista de Datos con visión antropológica | Python • SQL • Tableau"

author:
  name: "Abraham Esparza López"
  email: "abraham.esparza@email.com"

social:
  github: "esparzadataan"
  linkedin: "abraham-esparza-12345"
  twitter: "abraham_data"
```

---

## EJEMPLO 2: Personalizar index.md (Home)

### ❌ ANTES (Genérico)
```markdown
# ¡Hola! 👋

Soy **Analista de Datos** y **Antropólogo**...
```

### ✅ DESPUÉS (Concreto)
```markdown
# ¡Hola! 👋 Soy Abraham Esparza

Soy **Analista de Datos** y **Antropólogo** con 3+ años de experiencia 
transformando datos complejos en decisiones accionables.

He trabajado con startups fintech y organizaciones de investigación, 
aplicando rigor estadístico con empatía por el comportamiento humano.

## 🎯 Mi enfoque

- Combino **análisis cuantitativo** con **pensamiento crítico**
- Comunico hallazgos complejos de forma clara y accionable
- Entiendo contextos culturales e históricos detrás de los datos
```

---

## EJEMPLO 3: Personalizar about.md

### Sección de Habilidades

#### ❌ ANTES
```markdown
### Lenguajes de Programación
- **Python** - Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
```

#### ✅ DESPUÉS
```markdown
### Lenguajes de Programación
- **Python** - Experto en Pandas, NumPy; Scikit-learn para modelos; 
  Matplotlib/Seaborn/Plotly para visualizaciones avanzadas
- **SQL** - Queries complejas en PostgreSQL y MySQL; optimización de 
  performance; stored procedures
- **R** - Análisis estadístico avanzado, ggplot2 para visualización
```

### Sección de Experiencia

#### ❌ ANTES
```markdown
**Analista de Datos**  
[Empresa], [Período]
- Describir proyectos y logros
```

#### ✅ DESPUÉS
```markdown
**Senior Analyst - Datos & Insights**  
Fintech Startup XYZ, Enero 2023 - Presente
- Lideré análisis de 500k+ transacciones para identificar patrones de 
  fraude (reducción del 40% en incidentes)
- Desarrollé dashboard interactivo en Tableau usado por 50+ ejecutivos 
  diarios
- Mentoricé a 2 analistas junior en metodología de análisis

**Analista de Datos**  
Instituto de Investigación ABC, Junio 2021 - Diciembre 2022
- Procesé datos cualitativos y cuantitativos de estudios etnográficos
- Creé reportes automáticos que redujeron tiempo de análisis 60%
```

---

## EJEMPLO 4: Personalizar projects.md

### ❌ ANTES (Demasiado genérico)
```markdown
## Proyecto 1: [Tu Primer Proyecto]

**Descripción:** Breve descripción de qué se analiza y por qué es interesante.

**Tecnologías:** Python, Pandas, Tableau
```

### ✅ DESPUÉS (Concreto y atractivo)
```markdown
## Proyecto 1: Análisis de Churn de Clientes en SaaS

**Descripción:** Identificación de patrones de retención en plataforma 
de software. Utilizando datos de 10k+ usuarios activos, descubrí que 
el 85% del churn ocurría en primeras 2 semanas, permitiendo enfocar 
estrategia de onboarding.

**Tecnologías:** Python, Pandas, Scikit-learn, Plotly, SQL  
**Duración:** Octubre - Noviembre 2024

**Objetivos:**
- Predecir qué usuarios podrían abandonar el producto
- Identificar factores comunes en usuarios que se quedan
- Cuantificar impacto financiero del churn

**Insights principales:**
- 📉 Usuarios con sesiones <5min primeros 7 días tienen 95% probabilidad 
  de churn
- 📊 Usuarios con contacto con soporte dentro de 48h tienen 60% más 
  retención
- 💡 Sector público retiene 30% más que sector privado

**Metodología:**
- EDA completo de 15+ variables
- Análisis de cohortes por fecha
- Modelo de clasificación (Random Forest, AUC 0.87)
- Simulación de impacto financiero

📖 **[Ver análisis completo (Jupyter Notebook)](./analisis_churn_saas.ipynb)**
```

### Otro ejemplo:

```markdown
## Proyecto 2: Etnografía Digital - Patrones de Comportamiento en Redes Sociales

**Descripción:** Estudio cuantitativo de 50k+ posts en comunidad online 
para entender dinámicas de pertenencia y construcción de identidad. 
Integración de métodos antropológicos con análisis de textos (NLP).

**Tecnologías:** Python, NLTK, Pandas, Matplotlib, Excel  
**Duración:** Febrero - Abril 2024

**Objetivos:**
- Mapear redes de influencia dentro de comunidad
- Identificar rituales y códigos compartidos
- Analizar cómo la comunidad construye significado compartido

**Insights principales:**
- 🔗 Existen 3 subcomunidades distintas basadas en lenguaje e intereses
- 📣 "Influencers" son figuras de confianza, no famosos
- 🎭 60% de posts incluyen código in-group o referencias culturales

📖 **[Ver análisis completo (Jupyter Notebook)](./etnografia_digital_redes.ipynb)**
```

---

## EJEMPLO 5: Estructura de un Proyecto en projects.md

**Estructura recomendada:**

```markdown
## Proyecto: [Título específico y atractivo]

**Descripción:** 2-3 líneas sobre QUÉ hiciste y POR QUÉ importa

**Tecnologías:** [Lista de herramientas usadas]  
**Duración:** [Mes/Año - Mes/Año]

**Objetivos:**
- Objetivo 1 (cuantificable)
- Objetivo 2 (cuantificable)
- Objetivo 3 (cuantificable)

**Insights principales:**
- 🔍 Insight 1 con número
- 📊 Insight 2 con número
- 💡 Insight 3 con conclusión

📖 **[Ver análisis completo](./nombre_notebook.ipynb)**
```

---

## EJEMPLO 6: Editar _config.yml

```yaml
# Configuración Jekyll para GitHub Pages
theme: jekyll-theme-cayman

# Información del sitio
title: "Abraham Esparza - Data & Insights"
description: "Analista de Datos | Antropólogo Aplicado | Python • SQL • Tableau"
url: "https://esparzadataan.github.io"

# Autor (PERSONAL)
author:
  name: "Abraham Esparza López"
  email: "abraham.esparza@gmail.com"

# Redes sociales (PERSONALIZA)
social:
  github: "esparzadataan"
  linkedin: "abraham-esparza-lopez-123456"
  twitter: "abraham_data"
  email: "abraham.esparza@gmail.com"

# Configuración técnica
markdown: kramdown
highlighter: rouge
plugins:
  - jekyll-feed
  - jekyll-seo-tag

# Exclusiones
exclude:
  - .gitignore
  - Gemfile
  - Gemfile.lock
  - README.md
  - GUIA_CONSTRUCCION.md
  - PASOS_SIGUIENTES.md
```

---

## ✅ CHECKLIST DE PERSONALIZACIÓN

- [ ] Cambié `title` en _config.yml
- [ ] Cambié `author.name` con mi nombre completo
- [ ] Cambié `author.email` con mi email real
- [ ] Cambié `social.github` con mi usuario
- [ ] Cambié `social.linkedin` con mi perfil
- [ ] Actualicé `index.md` con saludo personal
- [ ] Escribí biografía en `about.md` (2-3 párrafos reales)
- [ ] Completa `about.md` con educación real
- [ ] Completa `about.md` con experiencia real
- [ ] Actualicé `projects.md` con mis 3 mejores proyectos
- [ ] Cada proyecto tiene objetivo específico y resultados
- [ ] Cada proyecto linkea a un notebook real en `/projects`

---

## 🎯 PRINCIPIOS PARA ESCRIBIR BIEN

### Sé específico, no genérico
❌ "Trabajé con datos"  
✅ "Analicé 500k transacciones y reduje el fraude 40%"

### Usa números
❌ "Hice un análisis grande"  
✅ "Procesé 15+ variables de 10,000+ clientes"

### Muestra impacto
❌ "Creé un dashboard"  
✅ "Dashboard usado por 50+ ejecutivos para decisiones diarias"

### Sé honesto
❌ "Experto en todo"  
✅ "Profundo en Python/SQL; aprendiendo Machine Learning"

---

**¡Ahora personaliza y publica! 🚀**

# 🎓 GUÍA EDUCATIVA: Construyendo tu Portafolio en GitHub Pages
## Para Analista de Datos + Antropólogo

---

## PARTE 1: ENTENDIENDO LA ARQUITECTURA

### 1.1 ¿Qué es GitHub Pages?

**Concepto:** GitHub Pages es un servicio gratuito de GitHub que convierte tu repositorio en un sitio web.

**¿Por qué lo usamos?**
- ✅ **Gratis** - No pagas por hosting
- ✅ **Profesional** - Dominio profesional (esparzadataan.github.io)
- ✅ **Integrado con Git** - Los cambios se actualizan con un simple push
- ✅ **Perfecto para portafolios** - Es exactamente para esto

**¿Cómo funciona?**
```
Tu código local → Git push → GitHub → GitHub Pages → Tu sitio en línea
```

---

## PARTE 2: OPCIONES DE TECNOLOGÍA

### 2.1 Comparación de opciones

| Opción | Complejidad | Flexibilidad | Ideal para |
|--------|------------|--------------|-----------|
| **HTML/CSS/JS puro** | Media | Alta | Total control, aprender web |
| **Jekyll** | Baja | Media | GitHub Pages nativo (recomendado) |
| **Hugo** | Media | Alta | Rendimiento extremo |
| **React/Next.js** | Alta | Muy Alta | Aplicaciones complejas |

### 2.2 Mi recomendación para ti: Jekyll

**¿Por qué Jekyll?**
1. **Nativo en GitHub Pages** - Funciona directamente sin configuración extra
2. **Perfecto para portfolios** - Diseñado para blogs y sitios estáticos
3. **Temas profesionales** - Existen temas gratis y hermosos
4. **Bajo mantenimiento** - No necesitas servidor
5. **Markdown friendly** - Escribes en Markdown (que ya conoces de Jupyter)

**¿Qué es Jekyll?**
- Un generador de sitios estáticos
- Transforma archivos Markdown → Sitios HTML profesionales
- Tiene temas listos para usar

---

## PARTE 3: ESTRUCTURA LÓGICA DE UN PORTAFOLIO EFECTIVO

### 3.1 Componentes que un reclutador espera

```
📱 Sitio del Portafolio
├── 🏠 INICIO (Home)
│   ├── Tu nombre y título
│   ├── Frase de impacto (2-3 líneas)
│   ├── Foto profesional (opcional)
│   └── Botones de contacto/redes
│
├── 👨‍💼 SOBRE MÍ (About)
│   ├── Quién eres (breve historia)
│   ├── Habilidades
│   ├── Experiencia destacada
│   └── Educación
│
├── 📊 PROYECTOS (Portfolio/Projects)
│   ├── Proyecto 1 (con Jupyter Notebook)
│   │   ├── Descripción
│   │   ├── Tecnologías usadas
│   │   └── Link a Jupyter Notebook
│   ├── Proyecto 2
│   ├── Proyecto 3
│   └── etc.
│
├── 📝 BLOG/ARTÍCULOS (opcional)
│   ├── Análisis de datos
│   ├── Insights antropológicos
│   └── Learnings
│
└── 📧 CONTACTO
    ├── Email
    ├── LinkedIn
    ├── GitHub
    └── Formulario de contacto
```

### 3.2 ¿Por qué esta estructura?

**Para el reclutador:**
- Necesita encontrar rápidamente quién eres
- Quiere ver tus mejores proyectos INMEDIATAMENTE
- Busca habilidades técnicas
- Quiere contactarte fácilmente

**Tiempo promedio:** Los reclutadores ven tu portafolio 30-60 segundos. ⏱️

---

## PARTE 4: LÓGICA DE LOS JUPYTER NOTEBOOKS EN TU PORTAFOLIO

### 4.1 ¿Cómo integrar Notebooks?

**Opción A: Mostrar en línea (recomendada)**
```
Tu portafolio Jekyll → Link a Notebook → GitHub renderiza el .ipynb
```

**Ventajas:**
- Los reclutadores ven el código y resultados
- GitHub renderiza Notebooks automáticamente
- No necesitas configuración extra

**Ejemplo URL:**
```
https://github.com/esparzadataan/esparzadataan.github.io/blob/main/projects/analisis_ventas.ipynb
```

**Opción B: Convertir a HTML**
```
Notebook (.ipynb) → nbconvert → HTML → Incluir en sitio
```

Más complejo, pero tienes control total.

### 4.2 Estructura de carpetas para proyectos

```
EsparzaDataAn.github.io/
├── index.html (o index.md para Jekyll)
├── assets/
│   ├── css/
│   └── images/
├── projects/
│   ├── proyecto_1.ipynb
│   ├── proyecto_2.ipynb
│   └── proyecto_3.ipynb
├── _posts/ (para blog, si usas Jekyll)
│   ├── 2026-01-22-mi-primer-articulo.md
│   └── etc.
└── _config.yml (configuración Jekyll)
```

---

## PARTE 5: PLAN DE IMPLEMENTACIÓN (Paso a paso)

### Fase 1: Preparación (30 minutos)
1. **Elegir tema Jekyll** - Seleccionar un tema profesional
2. **Crear estructura de carpetas** - Organizar archivos
3. **Escribir contenido** - Sobre ti, habilidades, proyectos

### Fase 2: Crear la página (1-2 horas)
1. **Configurar Jekyll** - _config.yml
2. **Crear Home** - index.md
3. **Crear About** - about.md
4. **Crear Projects** - projects.md con links a Notebooks
5. **Crear navegación** - Menú principal

### Fase 3: Vincular Jupyter Notebooks (30 minutos)
1. **Subir Notebooks** a carpeta `/projects`
2. **Crear links** en tu página Projects
3. **Organizar con descripciones**

### Fase 4: Deploy (5 minutos)
1. **Git add, commit, push** → Listo
2. **GitHub Pages se actualiza automáticamente**

### Fase 5: Mejoras posteriores (continuo)
1. Agregar más proyectos
2. Escribir artículos en el blog
3. Actualizar habilidades

---

## PARTE 6: DECISIONES DE DISEÑO IMPORTANTES

### 6.1 Colores y estética
- **Profesional pero moderno** - Azules, grises, blancos
- **Contraste claro** - Fácil de leer
- **Sin distracciones** - El foco en tu contenido
- **Responsive** - Se vea bien en móvil (¡Los reclutadores usan móvil!)

### 6.2 Contenido para reclutadores
- **Foto profesional** (no obligatorio, pero +10 puntos)
- **Resumen ejecutivo** - 3-4 líneas sobre quién eres
- **Habilidades técnicas claras**
  - Python, SQL, Tableau, Power BI
  - Análisis cuantitativo
  - Investigación antropológica
- **Proyectos destacados** (máximo 3-5 al inicio)
- **Call to action** - "¡Contacta conmigo!" bien visible

### 6.3 Keywords para SEO (para que te encuentren)
- "Analista de datos"
- "Antropología aplicada"
- "Python análisis"
- "Tu nombre"

---

## PARTE 7: HERRAMIENTAS Y RECURSOS

### Para crear el sitio:
- **Jekyll** - Generador de sitios estáticos
- **GitHub Pages** - Hosting gratuito
- **Markdown** - Lenguaje de escritura
- **Git** - Control de versiones (ya lo tienes)

### Temas Jekyll recomendados:
1. **Minimal** - Limpio y profesional
2. **Hacker** - Moderno para tech
3. **Cayman** - Hermoso y simple
4. **Architect** - Profesional y elegante

### Para convertir Notebooks (si los necesitas en HTML):
```bash
jupyter nbconvert --to html tu_notebook.ipynb
```

---

## PARTE 8: TIMELINE REALISTA

| Fase | Tiempo | Incluye |
|------|--------|---------|
| Planificación | 30 min | Elegir tema, estructurar contenido |
| Desarrollo | 2-3 horas | Crear sitio, escribir sobre ti |
| Integración Notebooks | 1 hora | Subir y linkar tus proyectos |
| Testing y pulido | 1 hora | Ver en móvil, links, ortografía |
| **Total** | **5-6 horas** | Sitio completamente funcional |

---

## PRÓXIMOS PASOS

1. **Paso 1: Responder** - ¿Quieres usar Jekyll o prefieres HTML/CSS puro?
2. **Paso 2: Elegir tema** - Te muestro opciones visuales
3. **Paso 3: Escribir contenido** - Empezamos con tu biografía
4. **Paso 4: Construir** - Creamos el sitio paso a paso
5. **Paso 5: Publicar** - Tu portafolio en línea en 5 minutos

---

## RESUMEN CONCEPTUAL

### La fórmula del portafolio efectivo:
```
Identidad Clara + Proyectos Viables + Fácil Contacto = Oportunidades
```

### Lo que importa a reclutadores (en orden):
1. **Proyectos reales** - ¿Qué has hecho?
2. **Habilidades técnicas** - ¿Qué sabes?
3. **Comunicación** - ¿Cómo lo explicas?
4. **Facilidad de contacto** - ¿Dónde te encuentro?

---

**¿Preguntas sobre alguna sección?** ¿Listos para comenzar?

# ProzAI — Levantamiento Inteligente de Procesos Empresariales

<div align="center">

![ProzAI Logo](https://img.shields.io/badge/ProzAI-v5.0-2563eb?style=for-the-badge&labelColor=0f1117)
![MIEDE 2.0](https://img.shields.io/badge/MIEDE%202.0-Aligned-16a34a?style=for-the-badge&labelColor=0f1117)
![Sin API Key](https://img.shields.io/badge/Sin%20API%20Key-100%25%20Local-d97706?style=for-the-badge&labelColor=0f1117)
![License](https://img.shields.io/badge/License-MIT-6366f1?style=for-the-badge&labelColor=0f1117)

**Herramienta de levantamiento, documentación y optimización de procesos empresariales**  
**100% standalone · Sin servidor · Sin API Key · Abre en cualquier navegador**

*by [Transformación ExO](https://transformacionexo.com) — Juan Carlos Alzate García*

</div>

---

## ¿Qué es ProzAI?

ProzAI es una aplicación web completa (un solo archivo HTML) que permite a empresas **levantar, documentar, analizar y optimizar** sus procesos operativos aplicando las mejores metodologías globales:

- **BPMN 2.0** — Notación estándar de modelado de procesos
- **Lean Manufacturing** — Detección automática de los 8 desperdicios
- **Six Sigma DMAIC** — Análisis de causa raíz estructurado
- **MIEDE 2.0** — Marco de Evolución Digital Empresarial (70% Personas · 25% Metodología · 5% Tecnología)

El análisis se ejecuta localmente mediante un **motor de reglas** — sin necesidad de API Key, sin conexión a internet, sin datos que salgan del navegador del usuario.

---

## Características principales

| Funcionalidad | Descripción |
|---|---|
| **Formulario guiado 4 pasos** | Contexto → Participantes → Flujo AS-IS → Métricas |
| **Roles ilimitados** | Agrega todos los actores necesarios (swim lanes BPMN) |
| **Diagrama visual AS-IS** | Render automático del proceso con clasificación por tipo |
| **Análisis Lean 8 desperdicios** | Detección automática por patrones de lenguaje |
| **Proceso optimizado TO-BE** | Generado algorítmicamente eliminando desperdicios |
| **DMAIC completo** | Define → Mide → Analiza → Mejora → Controla |
| **KPIs comparativos** | Proyecciones antes vs. después con benchmarks sectoriales |
| **Hoja de ruta MIEDE 2.0** | Acciones 70/25/5 priorizadas para implementación |
| **Madurez digital** | Score en 4 dimensiones con ruta de evolución |
| **Multi-proceso** | Almacena y gestiona múltiples procesos en localStorage |
| **100% offline** | Sin servidor, sin API, sin dependencias externas en runtime |

---

## Demo rápido

```
1. Abre index.html en tu navegador
2. Haz clic en "+ Nuevo proceso"
3. Completa los 4 pasos del formulario
4. Haz clic en "Ver diagrama del proceso"
5. Haz clic en "Generar análisis completo"
```

**No necesitas instalar nada. No necesitas configurar nada.**

---

## Cómo usar

### Opción A — Uso directo (más simple)
```bash
# Clona el repositorio
git clone https://github.com/TU_USUARIO/prozai.git

# Abre el archivo en tu navegador
open index.html
# o en Windows:
start index.html
```

### Opción B — GitHub Pages (publicar online)
1. Haz fork de este repositorio
2. Ve a **Settings → Pages**
3. En *Source*, selecciona `main` branch y carpeta `/root`
4. GitHub publicará la app en `https://TU_USUARIO.github.io/prozai`

### Opción C — Servidor local
```bash
# Con Python
python -m http.server 8080

# Con Node.js
npx serve .

# Con VS Code: instala la extensión Live Server
```

---

## Estructura del repositorio

```
prozai/
├── index.html          # Aplicación completa (único archivo necesario)
├── README.md           # Esta documentación
├── LICENSE             # Licencia MIT
└── .gitignore          # Archivos ignorados por Git
```

> **Nota:** Toda la aplicación vive en `index.html`. Es un archivo autocontenido — puedes copiarlo, enviarlo por email o compartirlo sin necesidad de ningún otro archivo.

---

## Metodologías aplicadas

### BPMN 2.0
El motor clasifica automáticamente cada paso del proceso según su tipo:
- **Inicio / Fin** — Eventos de inicio y cierre del proceso
- **Actividad** — Tareas ejecutadas por un rol
- **Decisión** — Puntos de bifurcación del flujo
- **Espera** — Tiempos muertos y demoras
- **Error/Reproceso** — Pasos con fallas identificadas

### Lean — 8 Desperdicios (TIMWOODS)
| # | Desperdicio | Detección |
|---|---|---|
| 1 | Sobreproducción | Generación de más de lo requerido |
| 2 | Espera | Tiempos muertos, aprobaciones pendientes |
| 3 | Transporte | Movimiento innecesario de información |
| 4 | Sobreprocesamiento | Pasos duplicados o innecesarios |
| 5 | Inventario | Trabajo acumulado sin procesar |
| 6 | Movimiento | Búsqueda de información o personas |
| 7 | Defectos | Errores, rechazos y reprocesos |
| 8 | Talento | Conocimiento no documentado, dependencias |

### DMAIC — Six Sigma
Análisis estructurado en 5 fases generado con los datos del proceso:
- **Define** — Enunciado del problema con impacto cuantificado
- **Measure** — Métricas baseline del proceso actual
- **Analyze** — Causas raíz identificadas en el flujo
- **Improve** — Soluciones concretas por causa raíz
- **Control** — Mecanismos de sostenimiento de la mejora

### MIEDE 2.0 — Marco Integral de Evolución Digital Empresarial
Evalúa la madurez digital del proceso en 4 dimensiones (score 1-5):
- **Personas** — Capacidades, cultura y gestión del cambio
- **Metodología** — Estandarización y mejora continua
- **Tecnología** — Sistemas, automatización e integración
- **Datos / IA** — Analítica, toma de decisiones e inteligencia artificial

La hoja de ruta de implementación sigue la distribución **70% Personas · 25% Metodología · 5% Tecnología**.

---

## Almacenamiento de datos

ProzAI guarda todos los procesos en `localStorage` del navegador:
- ✅ Los datos **nunca salen de tu dispositivo**
- ✅ No hay servidor, no hay base de datos externa
- ✅ Los procesos persisten entre sesiones
- ✅ Puedes eliminar los datos desde el botón "Eliminar" en cada proceso

> Para **exportar** un proceso, usa la función de impresión del navegador (`Ctrl+P`) para generar un PDF del análisis completo.

---

## Sectores cubiertos

Agroindustria · Construcción e Inmobiliaria · Manufactura · Retail y Distribución · Servicios Financieros · Salud · Tecnología · Educación · Logística y Transporte · Consultoría y Servicios · Gobierno y Sector Público

---

## Requisitos

| Requisito | Detalle |
|---|---|
| Navegador | Chrome 80+, Firefox 75+, Safari 13+, Edge 80+ |
| Servidor | No requerido |
| Internet | Solo para cargar las fuentes tipográficas (Google Fonts) |
| API Key | No requerida |
| Instalación | No requerida |

> Si usas sin internet, la aplicación funciona igual pero con fuentes del sistema.

---

## Roadmap

- [ ] Exportación a PDF integrada
- [ ] Exportación de diagrama BPMN en formato `.bpmn` / `.xml`
- [ ] Modo comparación entre dos versiones del mismo proceso
- [ ] Versión con análisis IA vía API (opcional, para usuarios con API Key)
- [ ] Plantillas de procesos por sector
- [ ] Importación/exportación de procesos en JSON

---

## Contribuir

Las contribuciones son bienvenidas. Para contribuir:

1. Haz fork del repositorio
2. Crea una rama: `git checkout -b feature/nueva-funcionalidad`
3. Commitea tus cambios: `git commit -m 'feat: descripcion del cambio'`
4. Push a la rama: `git push origin feature/nueva-funcionalidad`
5. Abre un Pull Request

---

## Acerca del autor

**Juan Carlos Alzate García**  
Founder & CEO — Transformación ExO  
Certified ExO Coach · ExO Mindset Award LatAm  
30+ años de experiencia en transformación digital empresarial

- 🌐 [transformacionexo.com](https://transformacionexo.com)
- 💼 [LinkedIn](https://linkedin.com/in/jcalzateg)
- 📧 jcalzate@transformacionexo.com

---

## Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo [LICENSE](LICENSE) para más detalles.

```
MIT License — Copyright (c) 2025 Juan Carlos Alzate García / Transformación ExO
```

---

<div align="center">

**ProzAI** · Transformación ExO · MIEDE 2.0  
*Levantamiento inteligente de procesos empresariales*

</div>

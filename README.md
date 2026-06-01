<!-- HEADER BANNER -->
<div align="center">

```
██╗   ██╗███████╗██╗  ██╗██╗ ██████╗██╗     ███████╗    ██╗ ██████╗
██║   ██║██╔════╝██║  ██║██║██╔════╝██║     ██╔════╝    ██║██╔═══██╗
██║   ██║█████╗  ███████║██║██║     ██║     █████╗      ██║██║   ██║
╚██╗ ██╔╝██╔══╝  ██╔══██║██║██║     ██║     ██╔══╝      ██║██║▄▄ ██║
 ╚████╔╝ ███████╗██║  ██║██║╚██████╗███████╗███████╗    ██║╚██████╔╝
  ╚═══╝  ╚══════╝╚═╝  ╚═╝╚═╝ ╚═════╝╚══════╝╚══════╝    ╚═╝ ╚══▀▀═╝
```

### 🚗 Vehicle Market Intelligence · End-to-End Data Analysis Project

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/TU_USUARIO/vehicle-market-analysis/blob/main/vehicle_sales_analysis.ipynb)
&nbsp;
![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?style=flat&logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-Interactive-3F4F75?style=flat&logo=plotly&logoColor=white)
![API](https://img.shields.io/badge/API-NHTSA%20%E2%80%94%20Free-success?style=flat)
![License](https://img.shields.io/badge/License-MIT-lightgrey?style=flat)

*¿Qué pasa cuando consumes datos reales de una API oficial del gobierno y los conviertes en inteligencia de mercado accionable?*

</div>

---

## 🧭 La Historia Detrás del Proyecto

Todo proyecto de datos nace de una pregunta incómoda.

La mía fue esta: **el mercado automotriz lleva décadas siendo dominado por las mismas marcas… pero algo está cambiando silenciosamente**. Los vehículos eléctricos no son una tendencia marginal ni una moda de Silicon Valley. Son una disrupción estructural. Y los datos lo confirman, si sabes dónde buscar.

Este proyecto nació de querer responder eso con datos reales, no con opinión. Usando la **API pública NHTSA** del gobierno de EE.UU. —completamente gratuita, sin clave— construí un pipeline que extrae el catálogo oficial de fabricantes y modelos, lo combina con datos de ventas calibrados con tendencias reales del mercado, y lo convierte en 7 visualizaciones interactivas que cuentan la historia completa.

El resultado: **un dashboard de inteligencia de mercado que cualquier analista, gerente o inversor puede reproducir en minutos desde Google Colab.**

---

## 📖 El Arco Narrativo — 5 Actos

```
ACT I          ACT II         ACT III        ACT IV         ACT V
  │               │               │               │               │
  ▼               ▼               ▼               ▼               ▼
¿Quién          ¿Cómo          ¿Electric       ¿Cuándo         ¿Dónde
domina          llegamos        o               vender          está la
el mercado?     hasta acá?      Gasoline?       más?            oportunidad?
  │               │               │               │               │
Treemap         Área           Barras          Heatmap         Bubble
Market          Temporal       Apiladas        Estacional      Precio vs
Share           2020–2024      Drive Type      por Mes         Volumen
```

Cada visualización es una pregunta de negocio. Cada insight, una decisión posible.

---

## 🎯 Business Questions

| # | La pregunta real | Lo que el dato revela |
|---|---|---|
| 1 | ¿Quién realmente mueve el dinero? | Toyota y Ford dominan volumen, pero el segmento Luxury genera más revenue por unidad |
| 2 | ¿El mercado creció o se contrajo? | COVID generó un dip en 2020–2021; la recuperación fue más fuerte de lo esperado |
| 3 | ¿EV es hype o realidad? | Los eléctricos crecen **4× más rápido** que el mercado total |
| 4 | ¿Cuándo se vende más? | Nov–Dic y Jul–Ago son picos. Enero–Febrero, el valle más profundo |
| 5 | ¿Precio alto mata volumen? | No siempre. Tesla rompe esa correlación completamente |
| 6 | ¿Cuáles son los Top 5 mes a mes? | Toyota mantiene liderazgo constante; Tesla escala sin pausa |
| 7 | ¿Cómo se estructura el mercado completo? | Mass Market domina en unidades; EV/Tech en tasa de crecimiento |

---

## 📊 Las 7 Visualizaciones

<table>
<tr>
<td width="50%">

**🗺️ Chart 1 — Market Treemap**
```
Segmento > Fabricante > Revenue
Tipo: Treemap jerárquico
Interacción: Click para zoom
```
Responde: ¿quién tiene el mayor pedazo del pastel y en qué categoría?

</td>
<td width="50%">

**📈 Chart 2 — Área Temporal**
```
Ventas anuales por fabricante (2020-2024)
Tipo: Área apilada
Interacción: Toggle por marca
```
Responde: ¿cómo cambió el liderazgo a lo largo del tiempo?

</td>
</tr>
<tr>
<td>

**⚡ Chart 3 — EV vs ICE**
```
Unidades y Revenue por Drive Type
Tipo: Barras agrupadas (dual panel)
Interacción: Hover para comparar
```
Responde: ¿está la revolución eléctrica en los datos?

</td>
<td>

**📅 Chart 4 — Heatmap Estacional**
```
Ventas mensuales por año (matriz)
Tipo: Heatmap RdYlGn
Interacción: Hover con valores exactos
```
Responde: ¿qué meses son oro y cuáles son trampa?

</td>
</tr>
<tr>
<td>

**💰 Chart 5 — Bubble Scatter**
```
Precio × Volumen × Revenue
Tipo: Bubble Chart (3 variables)
Interacción: Zoom + hover
```
Responde: ¿existe correlación entre precio y ventas?

</td>
<td>

**📊 Chart 6 — Series Temporales**
```
Top 5 fabricantes mes a mes
Tipo: Líneas + anotaciones
Interacción: Zoom, pan, unify hover
```
Responde: ¿cuál fue el impacto real del COVID en ventas?

</td>
</tr>
<tr>
<td colspan="2" align="center">

**🌐 Chart 7 — Sunburst Full Drill**
```
Segmento > Fabricante > Propulsión
Tipo: Sunburst jerárquico
Interacción: Drill-down click
```
Responde: ¿cómo se descompone el 100% del mercado hasta el nivel de propulsión?

</td>
</tr>
</table>

---

## 🌐 API Utilizada — NHTSA vPIC

> **National Highway Traffic Safety Administration** — Vehicle Product Information Catalog  
> Fuente oficial del gobierno de los Estados Unidos. Gratis, sin clave, sin límite.

```
Base URL:  https://vpic.nhtsa.dot.gov/api/vehicles/
```

| Endpoint | Uso en el proyecto |
|---|---|
| `getallmakes` | Obtener los ~11,000 fabricantes registrados |
| `getmodelsformake/{make}` | Catálogo de modelos por marca |
| `getvehicletypesformake/{make}` | Clasificación de tipo (Sedan, SUV, etc.) |
| `getmakesforvehicletype/Electric` | Todos los fabricantes con EV registrado |

```python
# Así de simple. Sin API key. Sin token. Sin signup.
import requests
r = requests.get('https://vpic.nhtsa.dot.gov/api/vehicles/getallmakes?format=json')
makes = r.json()['Results']   # → lista con ~11,000 fabricantes
```

---

## 🧪 Metodología — Datos Sintéticos + API Real

El proyecto combina dos fuentes con propósitos distintos:

```
┌─────────────────────────────────────────────────────────────────┐
│                     PIPELINE DE DATOS                           │
│                                                                 │
│  NHTSA API (real)          Datos Sintéticos                     │
│  ──────────────            ────────────────                     │
│  ✅ Fabricantes            ✅ Volumen de ventas                 │
│  ✅ Modelos exactos        ✅ Precios promedio                  │
│  ✅ Tipos de vehículo      ✅ Tendencias temporales             │
│  ✅ ~11,000 marcas         ✅ Estacionalidad                    │
│         │                        │                              │
│         └──────────┬─────────────┘                              │
│                    ▼                                            │
│            Dataset Integrado                                    │
│            ─────────────────                                    │
│            📦 ~180,000 registros                                │
│            📅 2020 – 2024                                       │
│            🏭 15 fabricantes, 80+ modelos                       │
│            💰 $2.3T USD en revenue simulado                     │
└─────────────────────────────────────────────────────────────────┘
```

**¿Por qué datos sintéticos?** Los datos reales de ventas automotrices están detrás de paywalls de $5,000+/año (IHS Markit, Cox Automotive). Generar datos sintéticos con distribuciones estadísticas calibradas es una práctica estándar en portfolios de data science. Las distribuciones se basan en informes públicos de Cox Automotive, Statista y el Bureau of Economic Analysis.

---

## 🚀 Quick Start

### ▶ Opción 1 — Google Colab (sin instalar nada)

1. Click en el badge **Open in Colab** al inicio del README
2. En Colab: `Runtime → Run All`
3. Los 7 gráficos aparecen inline, interactivos

### 💻 Opción 2 — Local

```bash
# 1. Clonar el repo
git clone https://github.com/TU_USUARIO/vehicle-market-analysis.git
cd vehicle-market-analysis

# 2. Instalar dependencias
pip install -r requirements.txt

# 3. Abrir el notebook
jupyter notebook vehicle_sales_analysis.ipynb
```

### 📦 requirements.txt

```
requests>=2.31.0
pandas>=2.0.0
numpy>=1.24.0
plotly>=5.18.0
kaleido>=0.2.1
```

---

## 📁 Estructura del Repo

```
vehicle-market-analysis/
│
├── 📓 vehicle_sales_analysis.ipynb    ← Notebook principal (ejecutar este)
├── 📄 README.md                       ← Este archivo
├── 📋 requirements.txt                ← Dependencias Python
│
└── 📊 outputs/                        ← Generados al ejecutar el notebook
    ├── vehicle_sales_dataset.csv      ← Dataset completo (~180k filas)
    ├── make_summary.csv               ← KPIs por fabricante
    ├── chart_treemap.html             ← Gráfico 1 (interactivo)
    ├── chart_area_annual.html         ← Gráfico 2
    ├── chart_ev_vs_ice.html           ← Gráfico 3
    ├── chart_heatmap_seasonal.html    ← Gráfico 4
    ├── chart_scatter_price_volume.html← Gráfico 5
    ├── chart_monthly_top5.html        ← Gráfico 6
    └── chart_sunburst.html            ← Gráfico 7
```

---

## 🔬 Stack Técnico

| Herramienta | Rol en el proyecto | Por qué esta elección |
|---|---|---|
| **Python 3.10+** | Lenguaje base | Ecosistema de datos más completo |
| **Pandas 2.x** | ETL y transformaciones | GroupBy, pivot, merge eficientes |
| **NumPy** | Generación de datos sintéticos | Distribuciones estadísticas realistas |
| **Plotly 5.x** | Visualizaciones interactivas | HTML exportable, hover nativo, drill-down |
| **Requests** | Consumo API REST | Simple, sin dependencias extra |
| **NHTSA vPIC API** | Fuente de datos real | Oficial, gratis, actualizada |

---

## 🏆 Key Findings

```
┌──────────────────────────────────────────────────────────────────┐
│                    RESUMEN EJECUTIVO                             │
├──────────────────────────────────────────────────────────────────┤
│                                                                  │
│  🥇  Toyota lidera en volumen, pero Ford en revenue por pickup   │
│                                                                  │
│  ⚡  EV creció +310% entre 2020 y 2024 en unidades              │
│                                                                  │
│  📅  Noviembre y Diciembre = +12% sobre la media mensual        │
│                                                                  │
│  💎  Luxury genera 2.3× más revenue por unidad que Mass Market  │
│                                                                  │
│  🚀  Tesla rompe la correlación precio-volumen: precio alto      │
│      y crecimiento exponencial coexisten                         │
│                                                                  │
│  🔁  COVID generó el dip más profundo en Feb-Abr 2020;          │
│      la recuperación superó niveles pre-pandemia en 2022        │
│                                                                  │
└──────────────────────────────────────────────────────────────────┘
```

---

## 💡 Próximos Pasos (Roadmap)

- [ ] Integrar precios reales de CarGurus API (free tier)
- [ ] Agregar predicción de ventas con Prophet (Facebook)
- [ ] Dashboard en Streamlit con filtros dinámicos
- [ ] Análisis de sentimiento de reviews de modelos (web scraping)
- [ ] Comparativa por región geográfica (EV adoption por estado)

---


<div align="center">

*Hecho con curiosidad, datos públicos y demasiado café.*

**[⭐ Starneá el repo si te fue útil]** · **[🔗 Conectá en LinkedIn](https://linkedin.com/in/davidardizzonedev)**

</div>

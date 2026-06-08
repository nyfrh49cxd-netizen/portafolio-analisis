# 📈 Análisis Financiero — Sector Defensa Global
## Lockheed Martin vs Northrop Grumman vs BAE Systems (2022-2026)

---

## 🎯 Objetivo
Analizar el desempeño financiero y accionario de las tres principales 
empresas de defensa del mundo, correlacionando sus resultados con 
eventos geopolíticos clave como la invasión rusa a Ucrania (Feb 2022) 
y el conflicto en Gaza (Oct 2023).

---

## 🔍 Metodología
1. Extracción automatizada de estados financieros via API yfinance
2. Conversión multidivisa GBP→USD usando tipo de cambio promedio histórico
3. Cálculo de métricas financieras clave (YoY Growth, Margen Neto)
4. Análisis de rendimiento accionario normalizado a base 100
5. Dashboard interactivo en Looker Data Studio

---

## 💡 Hallazgos Principales

### Compresión de márgenes — Lockheed Martin
| Año | Ingresos (USD M) | Margen Neto |
|---|---|---|
| 2022 | $65,984 | 8.69% |
| 2023 | $67,571 | 10.24% |
| 2024 | $71,043 | 7.51% |
| 2025 | $75,048 | 6.69% |

### Rendimiento accionario 2022-2026
| Empresa | Rendimiento |
|---|---|
| BAE Systems | +265% |
| Lockheed Martin | +65% |
| Northrop Grumman | +52% |

### Conclusión estratégica
BAE Systems se benefició de un **cambio estructural permanente** en el 
gasto europeo de defensa post-invasión a Ucrania, mientras LMT y NOC 
muestran volatilidad cíclica ligada a conflictos específicos.

---

## 🛠️ Herramientas
- Python 3.13
- yfinance — extracción de datos financieros
- Pandas — limpieza y transformación
- Matplotlib — visualizaciones
- Looker Data Studio — dashboard interactivo

---

## 📁 Archivos
- `defensa_analysis.ipynb` — Notebook principal
- `data/metricas_defensa.csv` — Métricas financieras consolidadas
- `data/precios_defensa_largo.csv` — Precios accionarios normalizados

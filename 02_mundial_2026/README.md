# ⚽ Modelo Predictivo — ADN del Campeón Mundial 2026

---

## 🎯 Objetivo
Construir un modelo predictivo basado en el perfil etario histórico 
de los 10 últimos campeones mundiales para identificar qué selección 
del Mundial 2026 tiene el ADN más cercano al campeón ideal.

---

## 🔍 Metodología
1. Web scraping de plantillas oficiales de 10 mundiales (Wikipedia)
2. Cálculo de edad exacta al momento del torneo
3. Construcción del perfil ideal por posición (4 posiciones)
4. Scraping de las 48 selecciones confirmadas para 2026
5. Modelo de distancia al perfil ideal
6. Score final ponderado: 60% perfil edad + 40% Índice Potencial Revelación

---

## 💡 Hallazgos Principales

### ADN del Campeón Mundial Histórico
| Posición | Edad Ideal |
|---|---|
| Portero | 29.27 años |
| Defensa | 27.55 años |
| Delantero | 26.97 años |
| Mediocampista | 26.40 años |

### Score Final — Favoritos Mundial 2026
| Selección | Score Final |
|---|---|
| Francia | 86.18/100 |
| Inglaterra | 81.69/100 |
| España | 81.16/100 |
| Portugal | 72.36/100 |
| Alemania | 60.93/100 |
| Argentina | 55.82/100 |
| Brasil | 34.84/100 |

### Conclusión
Francia lidera entre los favoritos con el perfil etario más cercano 
al ADN histórico del campeón. Brasil ocupa el último lugar (#48) 
entre las 48 selecciones — el perfil más alejado del ideal.

---

## 🛠️ Herramientas
- Python 3.13
- BeautifulSoup — web scraping
- Pandas — análisis y transformación
- Matplotlib / Seaborn — visualizaciones
- NumPy — cálculos estadísticos

---

## 📁 Archivos
- `mundial_prediccion.ipynb` — Notebook principal
- `data/edad_por_posicion.csv` — Perfil histórico por posición
- `data/edad_2026_por_posicion.csv` — Perfil 48 selecciones 2026

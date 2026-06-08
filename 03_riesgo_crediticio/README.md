# 💳 Modelo de Riesgo Crediticio — Random Forest

---

## 🎯 Objetivo
Construir un modelo de clasificación binaria para predecir 
riesgo de impago crediticio, optimizando el umbral de decisión 
según el apetito de riesgo institucional.

---

## 🔍 Metodología
1. Carga y exploración del German Credit Dataset (1,000 clientes)
2. Feature engineering — One-Hot Encoding de 13 variables categóricas
3. División train/test 80/20
4. Entrenamiento Random Forest con 100 árboles
5. Optimización de umbral de decisión (0.50 → 0.30)
6. Evaluación con matriz de confusión y reporte de clasificación

---

## 💡 Hallazgos Principales

### Mejora del modelo con ajuste de umbral
| Umbral | Recall Mal Cliente | Precision |
|---|---|---|
| 0.50 (default) | 34% | 77% |
| 0.30 (optimizado) | 69% | 62% |

### Top 5 Variables más Predictivas
| Variable | Relevancia |
|---|---|
| Monto solicitado | #1 |
| Edad | #2 |
| Duración del crédito | #3 |
| Estado de cuenta | #4 |
| Tasa de cuota | #5 |

### Conclusión estratégica
El umbral óptimo varía según el tipo de institución:
- **Banco conservador** → umbral 0.25 (maximiza detección de riesgo)
- **Banco estándar** → umbral 0.30 (balance riesgo/negocio)
- **Fintech agresiva** → umbral 0.40 (maximiza aprobaciones)

---

## 🛠️ Herramientas
- Python 3.13
- Scikit-learn — Random Forest, métricas
- Pandas — procesamiento de datos
- Seaborn — matriz de confusión
- NumPy — cálculos estadísticos

---

## 📁 Archivos
- `riesgo_crediticio.ipynb` — Notebook principal
- `data/german_credit.csv` — Dataset original

# Data

Esta carpeta contiene los datasets utilizados por el proyecto Research_01_QQQ_Regimes.

---

# Archivos

## qqq_part1_dataset.csv

Dataset principal generado en la Parte 1 del proyecto.

Incluye:

- Datos históricos semanales de QQQ.
- Variables de precio y volatilidad.
- Métricas de drawdown.
- Indicadores de tendencia.
- Variables derivadas utilizadas en el análisis de regímenes de mercado.
- Embeddings UMAP.
- Etiquetas de clusters obtenidas mediante HDBSCAN.
- Variables auxiliares utilizadas en los experimentos posteriores.

Uso:

- Parte 2 — Poder predictivo de factores estructurales.
- Parte 3 — Validación económica y construcción de estrategias.
- Apéndices metodológicos.

---

## qqq_part2_validation_dataset.csv

Dataset enriquecido generado durante la Parte 2 del proyecto.

Incluye:

- Factores seleccionados durante la validación estadística.
- Variables con evidencia predictiva significativa.
- Scores de régimen desarrollados durante la investigación.
- Señales asociadas al Universo A (DD + ATR).
- Señales asociadas al Universo B (Bull Regime).
- Variables utilizadas para backtesting y validación económica.
- Scores y componentes empleados en la construcción de estrategias.

Uso:

- Parte 3 — Validación económica de señales.
- Construcción de campeones y ensembles.
- Estudios de robustez.
- Sensitivity testing.
- Rolling backtests.
- Análisis de operabilidad.

---

# Nota

Estos datasets corresponden a versiones de investigación utilizadas para reproducir los resultados documentados en el repositorio.

Cada etapa del proyecto genera nuevas variables y estructuras derivadas, por lo que se recomienda utilizar el dataset correspondiente a la fase del análisis que se desea reproducir.

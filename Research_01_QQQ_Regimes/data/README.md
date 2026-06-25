# Data

Esta carpeta contiene los datasets y artefactos utilizados por el proyecto **Research_01_QQQ_Regimes**.

En ella se almacenan tanto los datasets generados durante las distintas etapas de investigación como los artefactos operativos persistidos que permiten reproducir exactamente el estado del pipeline sin recalcular resultados previamente validados.

---

# Contenido

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

**Uso**

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

**Uso**

- Parte 3 — Validación económica de señales.
- Construcción de campeones y ensembles.
- Estudios de robustez.
- Sensitivity testing.
- Rolling backtests.
- Análisis de operabilidad.

---

## qqq_p4_cache/

Carpeta de persistencia del **estado operativo** generada por la Parte 3.5.

Su objetivo es almacenar una versión congelada del universo operativo para que las etapas posteriores del proyecto trabajen exactamente sobre el mismo estado, sin reconstruir señales ni recalcular información previamente validada.

Esta carpeta es creada y administrada automáticamente por el pipeline.

Contiene artefactos como:

- `live_df.pkl`
- `or_trades.pkl`
- `or_panels.pkl`
- `metadata.pkl`
- `MANIFEST.json`
- `model_artifacts.joblib` *(cuando la Parte 1 incorpore su persistencia definitiva)*

Estos archivos representan el estado operativo sellado del proyecto y son utilizados por las etapas posteriores para garantizar consistencia y reproducibilidad.

---

# Nota

Los datasets y artefactos contenidos en esta carpeta corresponden a versiones utilizadas para reproducir los resultados documentados en este repositorio.

Cada etapa del proyecto genera nuevos productos de datos, por lo que se recomienda utilizar el artefacto correspondiente a la fase del pipeline que se desea reproducir.

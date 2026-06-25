# Research 01 — Regímenes de Mercado en QQQ

## Objetivo

Investigar si los regímenes de mercado, sus probabilidades pronosticadas y variables derivadas de tendencia, volatilidad y estructura contienen información predictiva útil para evaluar retornos futuros en QQQ.

---

## Parte 1 — Descubrimiento y Forecast de Regímenes

### Metodología

* Reducción de dimensionalidad mediante UMAP
* Clustering mediante HDBSCAN
* Construcción de meta-estados de mercado
* Forecast supervisado con XGBoost
* Calibración de probabilidades
* Análisis de transiciones de régimen
* Construcción de signatures
* Backtesting y validación

### Hallazgos principales

* Los regímenes contienen información económica relevante.
* El forecast mostró capacidad predictiva estadística.
* Forecast ≠ Alpha: la capacidad predictiva no se tradujo directamente en rentabilidad operativa.
* Las señales de persistencia mostraron más utilidad que las señales de transición.
* El mejor baseline operativo surgió de estructuras simples de tendencia y momentum.

**Estado:** ✅ Completado

---

## Parte 2 — Investigación de Factores y State Scores

### Metodología

* Análisis Spearman de factores individuales
* Optimización de horizonte predictivo
* Construcción de rankings y quintiles
* Mapas de estados de mercado
* Event Studies
* Backtesting de señales
* Construcción de scores compuestos
* Optimización de pesos mediante grid search

### Hallazgos principales

* Los factores más informativos fueron ATR relativo, tendencia y drawdown.
* Las combinaciones de factores mostraron más información que los factores individuales.
* Los estados de mercado permitieron identificar contextos con retornos futuros diferenciados.
* Los Event Studies mostraron que las transiciones de entrada contienen más información que las semanas consecutivas dentro del mismo estado.
* Los scores compuestos mejoraron sustancialmente la capacidad de ranking respecto a factores individuales.

**Estado:** ✅ Completado

---

## Parte 3 — Validación Cuantitativa y Campeón Final

### Metodología

* Bootstrap y validación temporal
* Ranking y leaderboard de factores
* Backtesting de estrategias
* Ensambles AND y OR
* Robustness Grid y Rolling Backtests
* Bootstrap de trades, Monte Carlo y Leave-One-Out

### Hallazgos principales

* DD+ATR fue el factor compuesto más robusto del Universo A y State Score Opt el mejor candidato del Universo B.
* Los ensambles AND y OR mostraron perfiles operativos distintos y complementarios.
* El AND Champion destacó por su menor riesgo y mayor estabilidad, mientras que el OR Champion entregó mayor cobertura y retorno absoluto.
* La validación final aportó evidencia favorable para el AND Champion, considerando la limitación del reducido número de trades.
* Se definieron dos estrategias candidatas para la etapa operativa del proyecto.

**Estado:** ✅ Completado

---

## Parte 3.5 — Construcción del Dataset Operativo

### Metodología

* Integración de los resultados validados de las Partes 1 y 2.
* Construcción del universo operativo a partir de las señales seleccionadas durante la investigación.
* Generación de las operaciones correspondientes a los campeones OR y AND.
* Construcción de paneles individuales por operación.
* Validación de integridad y consistencia de los resultados.
* Persistencia del dataset operativo para las etapas posteriores del proyecto.

### Hallazgos principales

* Se consolidó un único dataset operativo a partir de los resultados obtenidos durante la investigación.
* Las señales validadas pudieron transformarse en un conjunto consistente de operaciones individuales.
* Se estableció una estructura estandarizada para organizar las operaciones, paneles y metadata generada.
* El proceso garantiza coherencia entre el universo operativo y los resultados derivados de la investigación.

**Estado:** ✅ Completado

---

## Estructura del Proyecto

* **QQQ_Regime_Research.ipynb**

  * Parte 1: Regímenes y Forecast

* **QQQ_Regime_Research_Parte 2.ipynb**

  * Parte 2: Factores, Estados y Scores

* **QQQ_Regime_Research_Parte 3.ipynb**

  * Parte 3: Validación Cuantitativa y Campeón Final

* **QQQ_Regime_Research_Parte 3_5.ipynb**

  * Parte 3.5: Construcción del Dataset Operativo

---

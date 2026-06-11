Reproducibilidad de Regímenes de Mercado
Objetivo
Investigar la estabilidad y reproducibilidad de los regímenes de mercado obtenidos mediante UMAP + HDBSCAN sobre datos semanales de QQQ.

Motivación
Durante el desarrollo del proyecto principal de regímenes de mercado surgieron diferencias relevantes en la cantidad y estructura de clusters obtenidos al repetir el pipeline bajo distintas condiciones.

Este experimento busca determinar si dichas diferencias corresponden a:

Variabilidad propia de UMAP.
Sensibilidad de HDBSCAN.
Dependencia de semillas aleatorias.
Cambios reales en la geometría del embedding.
Fenómenos de bifurcación o fusión de clusters.
Preguntas de investigación
¿Qué tan reproducibles son los clusters generados por UMAP + HDBSCAN?
¿Existen regiones estables del embedding que persisten entre ejecuciones?
¿Qué parámetros generan mayor estabilidad estructural?
¿Los cambios observados corresponden a ruido o a bifurcaciones legítimas de la estructura del mercado?
Contenido
Experimentos de sensibilidad de UMAP.
Experimentos de sensibilidad de HDBSCAN.
Comparación de embeddings.
Análisis de estabilidad de clusters.
Estudio de bifurcaciones de regímenes.
Relación con otros proyectos
Este estudio funciona como apéndice metodológico del proyecto:

Research 01 — QQQ Market Regimes

Su propósito es evaluar la robustez de la metodología utilizada para construir los estados de mercado.

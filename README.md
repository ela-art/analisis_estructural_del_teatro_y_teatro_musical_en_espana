Análisis del Teatro Musical en España (2010–2025) Descripción del proyecto

Este proyecto realiza un análisis integral del teatro musical en España entre 2010 y 2025, combinando diversas fuentes públicas y datos propios. El objetivo es comprender la evolución del sector, su estructura productiva, la distribución geográfica de los musicales, los patrones de duración y el comportamiento de las obras activas frente a las finalizadas.

Objetivos del análisis

Construir un dataset maestro unificado sobre musicales estrenados en España entre 2010 y 2025.

Detectar tendencias de producción y evolución anual del número de estrenos.

Identificar principales productoras y su peso real en el mercado.

Analizar la centralización geográfica del teatro musical.

Estudiar los patrones de duración de los espectáculos y factores asociados.

Comparar la duración entre musicales activos e inactivos.

Integrar datasets complementarios como hábitos de consumo y precios de entradas para futuros análisis.

Estructura del repositorio

Carpeta: Data/
Contiene todos los archivos de datos utilizados en este proyecto:

Archivo Descripción maestro_musicales.csv Dataset principal que integra musicales, productoras, ciudades, años de inicio/fin, duración y estado activo. musicales_limpio.csv Versión depurada del listado original de musicales antes de la integración final. musicales_listado.xlsx Listado base en formato Excel utilizado como fuente inicial. precios_musicales_limpio_definitivo.csv Dataset final sobre precios de entradas de musicales actuales. precios_musicales_limpio_final.csv Variación previa del dataset de precios. teatro_musical_habitos_2011_2025_limpio.csv Dataset limpio sobre hábitos de consumo y asistencia al teatro musical. teatro_musical_habitos.csv Versión sin depurar previa del dataset de hábitos. 2. Carpeta: Notebooks/

Incluye los cuadernos Jupyter de exploración y análisis:

Notebook Contenido eda_maestro_musicales.ipynb EDA completo del dataset maestro. Limpieza final, descriptivos, visualizaciones clave y conclusiones. eda_musicales_limpio.ipynb Análisis intermedio del dataset previo a la construcción del maestro. eda_precio_musicales_limpio_definitivo.ipynb Exploración y validación de precios de entradas. eda_teatro_musical_habitos.ipynb Análisis del dataset de hábitos de consumo y tendencias del público. maestro_musicales.ipynb Notebook utilizado para la consolidación de todas las fuentes y generación del CSV maestro. Metodología

Recolección y consolidación de datos mediante fuentes públicas, plataformas de teatro musical y contenido verificado.

Limpieza exhaustiva:

Normalización de nombres (p. ej. SOM → ATG Entertainment).

Corrección de inconsistencias ortográficas y formato.

Eliminación de duplicados por clave compuesta.

Conversión correcta de tipos (ej. activa a booleano).

EDA estructurado:

Descriptivos numéricos y categóricos.

Análisis temporal de estrenos.

Ranking de productoras.

Distribución geográfica por ciudad.

Análisis de duración y comportamiento por estado activo.

Visualización:

Histogramas, barplots, boxplots, violin plots y series temporales.

Interpretación orientada a insights accionables.

Hallazgos clave

Tendencia creciente en el número de musicales estrenados, especialmente entre 2021 y 2024, consolidando el crecimiento post-pandemia.

El mercado presenta una alta concentración: Let’s Go Company, ATG Entertainment y Stage Entertainment dominan la producción nacional.

Madrid es el epicentro absoluto del teatro musical español, acumulando más de 50 musicales entre 2011 y 2025; Barcelona queda en segundo plano.

La duración de los musicales se estandariza en torno a los 140 minutos, con variabilidad moderada y picos entre 130–160 minutos.

La duración no determina que un musical siga activo; no existen diferencias relevantes entre obras activas e inactivas.

El dataset final queda completamente limpio, unificado y preparado para análisis posteriores, dashboards o modelos predictivos.

Tecnologías utilizadas

Python (pandas, numpy, matplotlib, seaborn)

Jupyter Notebook

Excel / CSV

VS Code

Git & GitHub

Próximos pasos

Integración del dataset de precios de entradas para analizar accesibilidad económica.

Modelado de tendencias de asistencia combinando hábitos + estrenos + productoras.

Construcción de un dashboard interactivo en Power BI o Tableau.

Segmentación de musicales por tipología, target y modelo de explotación.

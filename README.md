

# Contexto del Proyecto
El proyecto se centra en proporcionar insights sobre el comportamiento del sector de telecomunicaciones a nivel nacional en Argentina. Se exploran variables como el acceso a internet por cada 100 habitantes, por cada 100 hogares, velocidades de conexión, y otros servicios relacionados.


# Estructura del Repositorio
- Datasets/: Carpeta que contiene los archivos de datos utilizados en el análisis.
- InformeEDA/: Carpeta que contiene los scripts de Python utilizados para realizar el análisis.
- README.md: Este archivo, que proporciona una guía sobre el proyecto y el análisis realizado.

# Análisis Exploratorio de Datos (EDA) - Proyecto de Telecomunicaciones en Argentina
Se documenta el proceso de Análisis Exploratorio de Datos (EDA) realizado para analizar el acceso a internet y otros servicios de comunicación en diferentes provincias de Argentina. El análisis se llevó a cabo utilizando múltiples hojas de datos provenientes de un conjunto de datos de telecomunicaciones.

# Pasos y Decisiones Tomadas en el EDA
## 1. Carga y Preparación de Datos
Se utilizaron archivos de Excel que contenían múltiples hojas de datos relacionadas con diferentes aspectos de las telecomunicaciones.
Cada hoja de datos se cargó utilizando pandas para su exploración y análisis.
## 2. Análisis de Cada Hoja de Datos
### Hoja de Datos: Acc_vel_loc_sinrangos
- Descripción: Análisis de velocidades de conexión por localidad y provincia.
- Acciones Tomadas: Se identificaron valores faltantes y se decidió interpretarlos como áreas donde no se ha adquirido el servicio de internet específico. Se detectaron valores atípicos explicados por el tamaño poblacional de ciertas provincias.
### Hoja de Datos: Accesos_tecnologia_localidad
- Descripción: Análisis del acceso a diferentes tecnologías de comunicación por localidad.
- Acciones Tomadas: Se observaron pocos valores atípicos que se consideraron normales dada la infraestructura tecnológica regional.
### Hoja de Datos: Dial-BAf
- Descripción: Análisis del uso de conexiones de dial-up frente a banda ancha fija.
- Acciones Tomadas: Se encontraron valores nulos en la columna 'dial up' que se interpretaron como 0 debido a la falta de registro explícito. Se consideraron los valores atípicos como normales en el contexto del predominio de la banda ancha fija.
### Hoja de Datos: Penetración-poblacion
- Descripción: Análisis de la penetración de servicios de internet por cada 100 habitantes.
- Acciones Tomadas: Se observaron valores atípicos relacionados con la variabilidad en el acceso a servicios según la provincia.
### Hoja de Datos: Penetracion-hogares
- Descripción: Análisis de la penetración de servicios de internet por cada 100 hogares.
- Acciones Tomadas: Se detectaron pocos valores atípicos que no mostraron una variabilidad extrema significativa.
### Hoja de Datos: Accesos por velocidad
- Descripción: Análisis del acceso a servicios de internet según diferentes rangos de velocidad.
- Acciones Tomadas: Se encontraron valores faltantes y valores negativos, indicando errores de digitación que requirieron corrección. Se identificaron datos mal etiquetados que se ajustaron para reflejar correctamente el año y trimestre.
### Hoja de Datos: Ingresos
- Descripción: Análisis de los ingresos asociados a los servicios de telecomunicaciones.
- Acciones Tomadas: Se observaron ingresos atípicos que se relacionaron con provincias donde se presenta un mayor acceso a servicios de internet.
## 3. Visualización y Conclusiones
- Se utilizó matplotlib y seaborn para visualizar gráficamente los datos, incluyendo diagramas de caja, mapas de calor y gráficos de barras.
- Se realizaron conclusiones detalladas sobre cada hoja de datos, destacando observaciones importantes sobre valores faltantes, atípicos, duplicados y tendencias.
## Resultados y Recomendaciones
Los resultados del EDA proporcionan una comprensión profunda del estado actual de los servicios de telecomunicaciones en diferentes regiones de Argentina. Esto servirá como base para futuros análisis y decisiones estratégicas en la mejora y expansión de la infraestructura de comunicaciones.cs


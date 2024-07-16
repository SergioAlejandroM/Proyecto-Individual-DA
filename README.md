

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

# Reporte de Análisis del Dashboard
## Introducción
Este reporte detalla el análisis realizado sobre el sector de telecomunicaciones en Argentina, enfocado principalmente en el acceso a internet. El análisis se llevó a cabo mediante la creación de un dashboard interactivo en Power BI, el cual permite explorar los datos en detalle y evaluar los principales indicadores de rendimiento (KPIs) propuestos.

## Analisis exploratorio de datos (EDA)
Antes de la creación del dashboard, se realizó un análisis exploratorio de datos (EDA) para comprender mejor la estructura de los datos y las relaciones entre las variables. Este proceso incluyó:

- Búsqueda de valores faltantes: Identificación y tratamiento de valores nulos en el conjunto de datos.
- Registros duplicados: Identificación y eliminación de registros duplicados para asegurar la integridad de los datos.
- Correcion de sintaxis: Identificación y transformacion de datos que impedian la carga del dataset generando error.

## Descripción del Dashboard
El dashboard interactivo desarrollado en Power BI incluye varias visualizaciones clave que permiten analizar el comportamiento del sector de telecomunicaciones en Argentina. Las principales secciones del dashboard son:

1. Acceso a Internet por Provincia
Esta sección muestra la tasa de acceso a internet por cada 100 hogares en cada provincia, permitiendo comparar la penetración del servicio en diferentes regiones. Los usuarios pueden filtrar los datos por año y trimestre para observar tendencias temporales.

2. Comparación de Tecnologias
Aquí se presenta una comparación entre los diferentes tecnologias. Los gráficos permiten identificar patrones de uso y preferencias entre los usuarios.

3. KPI de Acceso a Internet
El KPI principal propuesto es el aumento del 2% en el acceso a internet por cada 100 hogares para el próximo trimestre. La fórmula utilizada para calcular este KPI es:

<div align="center">
  <img src="https://latex.codecogs.com/svg.latex?\color{white}\text{KPI}=\left(\frac{\text{Nuevo%20acceso}-\text{Acceso%20actual}}{\text{Acceso%20actual}}\right)\times%20100" />
</div>

    En el análisis realizado, el KPI resultó ser de 1.75%, indicando que el aumento en el acceso a internet no alcanzó el objetivo del 2%.

4. Tendencias Temporales
Gráficos de líneas que muestran la evolución del acceso a internet a lo largo del tiempo. Estos gráficos ayudan a identificar tendencias y patrones estacionales.

## Análisis y Conclusiones
- Acceso a Internet: Se observó que el acceso a internet ha tenido un crecimiento constante en la mayoría de las provincias, aunque no se alcanzó el objetivo del 2% de aumento trimestral, con un KPI de 1.75%. Esto sugiere la necesidad de estrategias adicionales para impulsar el acceso en las áreas menos servidas.
Comparación de Tecnologias:  Cable Modem sigue siendo la tecnologia más utilizada, seguida por Fibra optica. El Cable Modem ha mostrado una tendencia decreciente a diferencia de Fibre Optica.
- Oportunidades de Crecimiento: Provincias con menor uso de Fibra Optica representan oportunidades de expansión para la empresa. Estrategias focalizadas en estas regiones podrían contribuir a mejorar el KPI en futuros trimestres.
## Recomendaciones
- Estrategias de Expansión: Desarrollar campañas de promoción y subsidios en provincias con baja disponibilidad de Fibra Optica para incrementar la adopción del servicio.
- Mejora de Infraestructura: Invertir en infraestructura para mejorar la calidad y velocidad del servicio de internet, lo cual podría aumentar la satisfacción del cliente y la tasa de adopción.
- Monitoreo Continuo: Continuar monitoreando los KPIs y ajustar las estrategias en función de los resultados obtenidos para asegurar el cumplimiento de los objetivos de crecimiento.

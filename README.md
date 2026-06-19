# Proyecto: Análisis de Clientes ConnectaTel
## Objetivo del proyecto

Analizar el comportamiento de los clientes de ConnectaTel mediante la integración de información demográfica y de uso de los servicios de telecomunicaciones, con el fin de identificar segmentos de clientes, patrones de consumo y oportunidades de mejora para la oferta comercial de la empresa.

## Datasets utilizados
### users.csv

Contiene información de los usuarios registrados en la plataforma.

Principales variables:

- user_id
- age
- city
- plan
- reg_date
- churn_date

### usage.csv

Contiene el historial de uso de los servicios por parte de los usuarios.

Principales variables:

- id
- user_id
- type
- duration
- length
- date

## Etapas del análisis
1. Exploración inicial de datos (EDA)
- Revisión de estructura y tipos de datos.
- Identificación de valores faltantes.
- Identificación de valores inválidos y sentinels.
- Revisión de consistencia entre variables.

2. Limpieza y preparación de datos
- Conversión de variables al tipo de dato adecuado.
- Tratamiento de valores faltantes.
- Corrección de valores sentinela.
- Validación de fechas y registros inconsistentes.

3. Análisis descriptivo
- Estadísticas descriptivas de variables numéricas.
- Exploración de variables categóricas.
- Análisis de distribuciones mediante histogramas y boxplots.
- Identificación y evaluación de valores atípicos mediante el método IQR.

4. Construcción de métricas de usuario
- Agrupación de registros de uso por usuario.
- Cálculo de:
 - Cantidad de mensajes.
 - Cantidad de llamadas.
 - Total de minutos consumidos.
- Integración de métricas de uso con la información demográfica.

5. Segmentación de clientes
- Segmentación por grupos de edad.
- Segmentación por nivel de uso.
- Comparación de patrones de comportamiento entre segmentos.

6. Elaboración de conclusiones y recomendaciones
- Identificación de oportunidades comerciales.
- Detección de segmentos de interés para el negocio.
- Propuestas para optimizar la oferta de planes.

## Cómo ejecutar el notebook
**Opción 1: Google Colab**
1. Ingresar a Google Colab.
2. Seleccionar Archivo → Subir cuaderno.
3. Cargar el archivo .ipynb.
4. Subir los archivos de datos (users.csv y usage.csv) al entorno de trabajo.
5. Ejecutar las celdas en orden secuencial.

**Opción 2: Jupyter Notebook**
1. Instalar Python 3.x.
2. Instalar las dependencias requeridas:
- pip install pandas numpy matplotlib seaborn
3. Abrir Jupyter Notebook.
4. Abrir el archivo del proyecto.
5. Verificar que los archivos de datos se encuentren en la ruta correcta.
6. Ejecutar las celdas en orden.

**Guía rápida de reproducción**
1. Cargar los datasets.
2. Revisar la calidad de los datos.
3. Realizar la limpieza y transformación de variables.
4. Construir las métricas agregadas por usuario.
5. Generar las visualizaciones exploratorias.
6. Segmentar a los usuarios por edad y nivel de uso.
7. Analizar los resultados obtenidos.
8. Revisar las conclusiones y recomendaciones finales.

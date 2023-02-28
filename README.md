<p align=center><img src=https://assets.soyhenry.com/logos/LOGO-HENRY-04.png><p>

# PROYECTO INDIVIDUAL N°2 - DATA ANALYTICS

## *Desarrollado por Rodrigo Pérez Delgado para Henry´s bootcamp* 


#### Problemática:
Realizar el ciclo de vida de un proyecto de **Data Analytics**, contemplando el tratamiento y recolección de los datos. Así como la presentación de la información en un **dashboard**.



#### Rol del desarrollador:
- Data analyst

<hr> 

### Proceso de "ETL" y "EDA":

# Parte 1
- Descarga de la lista de las 500 empresas
- Limpieza de datos para su procesamiento
- Visualización de sectores
- Cantidad de empresas por sector
- Cantidad de empresas por sector por fecha de ingreso
- Porcentaje de empresas por sector por fecha de ingreso

# Conclusión 1
- El sector '**Information Technology**' cuenta con una mayor participación en el índice S&P 500 (**76** empresas). <br>
- Solo **20** empresas de este sector (74% con respecto a las 76) fueron incluidas en índice antes del año 2000.
- Tomando en cuenta lo anterior, a partir de este punto continuaremos analizando **únicamente el sector Information Technology** ya que es el sector que más empresas ha ingresado al índice en los últimos 23 años.

# Parte 2
- Creación de un df con únicamente las empresas el sector IT
- Limpieza de datos para su procesamiento
- Cantidad de empresas por subsector
- Cantidad de empresas por subsector por fecha de ingreso
- Porcentaje de empresas por subsector por fecha de ingreso

# Conclusión 2
- El subsector **'Semiconductors'** tiene una mayor participación en el sector de la Tecnología de la Información con **15 empresas**.
- Es importante destacar que este subsector tiene un balance adecuado a mi juicio, ya que dos terceras partes de las empresas han sido agregadas desde el año 2000. Lo que indica que es un subsector con un mercado en constante crecimiento.
- Sumando que, si solo contamos las empresas agregadas antes del 2000, 'Semiconductors' sigue siendo el subsector con más empresas.
- A partir de este punto, analizaremos **únicamente el subsector 'Semiconductors**'.

# Parte 3
- Creación de un df con únicamente las empresas del subsector Semiconductors
- Creación columnas para pasos finales

Realizaremos 3 pasos para seleccionar nuestro top 3 de empresas:
- Eliminaremos las 5 empresas con menor antigüedad desde su fundación
- Organizaremos las 10 empresas sobrantes por los años que tardaron en ser agregadas al índice S&P 500
- Elegiremos el **top 3**

# Conclusión 3
- Después de analizar las 15 empresas del subsector 'Semiconductors', realizamos 3 pasos para elegir nuestro top 3 de empresas: 

- Se descartaron las **5** empresas con menor antigüedad considerando el año de su fundación.
- Se reordenaron las **10** empresas sobrantes por los años que tardaron en ser agregadas al índice S&P 500. 
- Seleccionamos el **top 3** resultante:

   ---  **Intel** --- **Qualcomm** --- **Nvidia**

# Parte 4
- Instalación de la liberia yfnance.
-Descarga de la información historia de las 3 empresas seleccionadas con una periodicidad diaria desde el 2000 hasta el 2023
-Realizaremos nuestro análisis únicamente considerando el precio de cierre y volumen de las acciones en movimiento de ese dia
- Visualizamos el comportamiento del precio
- Visualizamos el comportamiento del volumen
- Revisamos la correlación que existe en el precio y volumen
-Al término de nuestro análisis podremos determinar el rendimiento de crecimiento de las 3 acciones
- Nuestra recomendación será una distribución de inversión del 50/30/20 dependiendo su rendimiento.

# Conclusión 4
- Después de analizar los gráficos visualmente podemos llegar a este orden de rendimiento:
1. Nvidia
2. Qualcomm
3. Intel

- Obtuvimos una correlación del -0.3259 entre el precio de cierre y volumen de transacciones. lo que indica una correlación negativa moderada. Esto significa que cuando los precios de cierre (Close) aumentan, es probable que el volumen de negociación (Volume) disminuya, y viceversa. Sin embargo, la correlación no implica necesariamente causalidad, por lo que es importante interpretar estos resultados con precaución.

- Nuestra recomendación de inversión se desglosa de la siguiente manera:
1. Nvidia 50%
2. Qualcomm 30%
3. Intel 20%
- Según la data, en promedio el día que conviene comprar nuestras acciones es el día Lunes. Ya que el histórico indica que es el día con el precio más bajo.

#### [Archivo Jupiter con el proceso de ETL y EDA](https://github.com/roprz/PI_2_Henry/blob/main/EDA.ipynb "ETL")


### Creación de dashboard en Power BI:
#### [Archivo PBIX con el dashboard](https://github.com/roprz/PI_2_Henry/blob/main/PI_2.pbix)
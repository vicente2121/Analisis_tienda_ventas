# Proyecto de Análisis de Ventas con Power BI

¡Bienvenido a nuestro proyecto de Análisis de Ventas con Power BI! En este repositorio, encontrarás todo lo necesario para explorar y comprender el rendimiento de ventas de una tienda a través de análisis detallados y visualizaciones informativas.

## Descripción del Proyecto

Este proyecto tiene como objetivo analizar las ventas de una tienda utilizando Power BI, centrándose en las medidas creadas para obtener insights clave sobre el rendimiento de ventas.

## Contenido del Repositorio

- **Datasets:** Contiene los archivos de origen de datos utilizados en el análisis, incluyendo hojas de cálculo con información sobre presupuestos, clientes, productos y transacciones de ventas.
- **Power BI Report:** El informe de Power BI completo que muestra visualmente el análisis de ventas, con gráficos, tablas y medidas creadas para proporcionar insights significativos.

## Imagenes del desarrollo


![2](https://github.com/vicente2121/Analisis_tienda_ventas/assets/72566296/394533bb-3685-426c-b2ab-8adf291fdb88)
![3](https://github.com/vicente2121/Analisis_tienda_ventas/assets/72566296/742d0d7b-df14-41ce-8a88-09c5e2e5af92)
![2 1](https://github.com/vicente2121/Analisis_tienda_ventas/assets/72566296/08fa6f69-90be-4afd-9754-8ffda0978b52)![4](https://github.com/vicente2121/Analisis_tienda_ventas/assets/72566296/d5c4a8f4-22c9-43e5-846c-d453331507de)
![5](https://github.com/vicente2121/Analisis_tienda_ventas/assets/72566296/abdee272-4ca0-4acb-ae92-08a04a85df05)
## Medidas Creadas en Power BI

El informe de Power BI incluye una variedad de medidas clave que proporcionan insights fundamentales sobre las ventas de la tienda. Aquí están todas las medidas utilizadas:

1. **% Q1 Ventas:** Calcula el porcentaje de ventas del primer trimestre con respecto al total de ventas.
    - Fórmula: DIVIDE([Q1 ventas],[Total ventas])

2. **% Q2 Ventas:** Calcula el porcentaje de ventas del segundo trimestre con respecto al total de ventas.
    - Fórmula: DIVIDE([Q2 ventas],[Total ventas])

3. **% Q3 Ventas:** Calcula el porcentaje de ventas del tercer trimestre con respecto al total de ventas.
    - Fórmula: DIVIDE([Q3 ventas],[Total ventas])

4. **% Q4 Ventas:** Calcula el porcentaje de ventas del cuarto trimestre con respecto al total de ventas.
    - Fórmula: DIVIDE([Q4 ventas],[Total ventas])

5. **Q1 ventas:** Calcula las ventas totales del primer trimestre.
    - Fórmula: CALCULATE([Total ventas],'Tabla calendario'[Trimestre]="Q1")

6. **Q2 ventas:** Calcula las ventas totales del segundo trimestre.
    - Fórmula: CALCULATE([Total ventas],'Tabla calendario'[Trimestre]="Q2")

7. **Q3 ventas:** Calcula las ventas totales del tercer trimestre.
    - Fórmula: CALCULATE([Total ventas],'Tabla calendario'[Trimestre]="Q3")

8. **Q4 ventas:** Calcula las ventas totales del cuarto trimestre.
    - Fórmula: CALCULATE([Total ventas],'Tabla calendario'[Trimestre]="Q4")

9. **Top 10 ubicaciones:** Calcula las ventas totales para las 10 ubicaciones principales.
    - Fórmula: CALCULATE([Total ventas], FILTER(VALUES(Dim_Cliente[Customer City]), RANKX(ALL(Dim_Cliente[Customer City]),[Total ventas],,DESC)<=10))

10. **Total Clientes:** Cuenta el número total de clientes distintos.
    - Fórmula: DISTINCTCOUNT(Tabla_Hechos[CustomerKey])

... y así sucesivamente para cada medida.

## Contribuciones

¡Las contribuciones son bienvenidas! Si tienes sugerencias de mejora, correcciones o nuevas ideas para el análisis, no dudes en abrir un problema o enviar un pull request. Trabajemos juntos para hacer que este proyecto sea aún más útil y efectivo.

## Link de desarrollo completo 
https://www.novypro.com/profile_projects/vicente-antoniomagallanes-juan

https://app.powerbi.com/view?r=eyJrIjoiNTRjYTE0YTgtMjQwMy00MWM0LTg2MzYtZmVhMTBhZWQ4YmUyIiwidCI6IjkxMTVmY2FmLWE5NGQtNDBiMS1hM2JhLWIwNjJjODA1NTVlMCIsImMiOjl9

# Análisis CityBikes NY
En este proyecto analiso la base de datos pública del servicio City Bikes de NY.


![_82c4dd6c-22e5-4e96-a4a4-3830a8d77305](https://github.com/carolina-cubillos/City_Bikes/assets/152019603/dff88289-8925-48db-a01b-d322abf77e3d)


## Temas
- [Introducción](#introducción)
- [Herramientas](#herramientas)
- [Procesamiento](#procesamiento)
- [Respondiendo preguntas de Negocio](#respondiendo-preguntas-de-negocio)
- [Resultados](#resultados)
- [Conclusiones y recomendaciones](#conclusiones-y-recomendaciones)

## Introducción
Realicé un análisis de datos 📊 donde exploré la enorme cantidad de información del sistema de bicicletas compartidas de Nueva York, proporcionada por Citybikes 🚲. 
Con más de 50 millones de registros, utilicé BigQuery para limpiar y preparar la base de datos 💻. Posteriormente, busqué insights sobre los hábitos de uso, utilizando Looker Studio y en esta misma plataforma presenté estos hallazgos de manera visualmente atractiva y fácil de entender 📊👀

## Herramientas
- SQL (Google BigQuery)
- Looker Studio (Google)

## Procesamiento
- Se identifican valores nulos a través de comandos SQL COUNT, WHERE y IS NULL.
- Se identifican duplicados a través de comandos SQL COUNT, GROUP BY, HAVING.
- Se manejan variables que no son útiles para el análisis a través de comandos SQL SELECT EXCEPT.
- Se identifican datos discrepantes en variables categóricas utilizando el comandos de manejo de string, como REGEXP.
- Se identifican datos discrepantes en variables niméricas utilizando comandos como MAX, MIN y AVG.
- Se consideran fechas de inicio y término de viaje para eliminar discrepancias
- Se comprueba y modifican tipos de datos, por ejemplo para cambiar los datos de tiempo pasando de segundos a minutos.
- Se crean nuevas variables utilizando CONCAT  y SUM.
- Se construyen tablas auxiliares utilizando WITH.
- Se unen las tablas utilizando LEFT JOIN.


  
## Respondiendo preguntas de Negocio
- ¿Cuál es el número de viajes que se realizan en promedio?
- ¿Cuál es el max. min. y promedio de la duración de un viaje?
- ¿Cuál es el número total de viajes?
- ¿Cuál es el crecimiento de viajes diarios a lo largo del tiempo?
- Muestra los viajes por género y edad




## Resultados

Se genera un dashboard que muestra de forma clara y dinámica las distintas métricas solicitadas

![image](https://github.com/carolina-cubillos/City_Bikes/assets/152019603/0ae8c323-0ec6-44e7-ac34-b9999f2095af)



## Conclusiones y recomendaciones
- La mayoría de los viajes duraban alrededor de 15 minutos ⏱️ 
- La mayoría de los usuarios son hombres 👨, siendo responsables de más del 67% de los viajes, mientras que las mujeres solo pertenecían a un 21% de los usuarios 👩. 
- Existe una disminución del uso del programa durante el primer trimestre de cada año 📉. Lo que se podría asociar a factores climáticos (Invierno en el hemisferio norte)
Estos insights pueden ayudar a mejorar el servicio y satisfacer mejor las necesidades de los usuarios en el futuro 🚀. 

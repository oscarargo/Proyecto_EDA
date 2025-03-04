### Proyecto EDA Análisis Exploratorio de Datos

# Análisis Exploratorio de Datos de Tendencias de Compras 📊

## Descripción

Este proyecto consiste en un análisis exploratorio de datos (EDA) realizado sobre un conjunto de datos de tendencias de compras de clientes cuyo objetivo es obtener información valiosa sobre el comportamiento de compra de los clientes, identificar patrones y tendencias, y proporcionar una base para la toma de decisiones informadas en estrategias de marketing y ventas.

## Objetivo principal del proyecto 🎯

El propósito de este análisis es comprender los patrones de compra de los clientes, evaluar la relación entre las características del consumidor y su comportamiento de compra, detectar oportunidades para mejorar la fidelización y aumentar las ventas. Esto permitirá a la empresa personalizar sus ofertas, mejorar la segmentación del mercado y optimizar su logística de distribución.

## Conjunto de Datos📊

El conjunto de datos utilizado en este análisis contiene información sobre:

*   **ID del Cliente:** Identificador único del cliente.
*   **Edad:** Edad del cliente.
*   **Género:** Género del cliente.
*   **Artículo Comprado:** Nombre del artículo comprado.
*   **Categoría:** Categoría del artículo comprado (Ropa, Accesorios, Calzado, etc.).
*   **Monto de Compra (USD):** Monto gastado en la compra.
*   **Ubicación:** Ubicación geográfica del cliente.
*   **Talla:** Talla del artículo comprado.
*   **Color:** Color del artículo comprado.
*   **Temporada:** Temporada en la que se realizó la compra.
*   **Calificación de la Reseña:** Calificación dada por el cliente al producto.
*   **Estado de Suscripción:** Indica si el cliente está suscrito o no.
*   **Tipo de Envío:** Método de envío utilizado.
*   **Descuento Aplicado:** Indica si se aplicó un descuento en la compra.
*   **Compras Anteriores:** Número de compras anteriores realizadas por el cliente.
*   **Método de Pago:** Método de pago utilizado.
*   **Frecuencia de Compras:** Frecuencia con la que el cliente realiza compras

## Estructura del Proyecto
```bash
--- data
----- Datos_transformados.csv     # Datos usados para el EDA
----- shopping_trends_updated.csv #Datos originales

--- Readme.md
```

## Metodología✍️

 Pasos para realizar un Análisis Exploratorio de Datos (EDA) en Google Sheets:

##### 1.Carga de datos

- Subir el archivo CSV a Google Sheets.

- Revisar que los datos han sido cargados correctamente.

##### 2.Limpieza de datos

- Renombrar columnas mal etiquetadas o genéricas.

- Manejar valores nulos y duplicados usando funciones de Google Sheets.

- Convertir formatos de datos según sea necesario (ejemplo: fechas, números).

##### 3.Análisis estadístico y visualización

- Usar funciones como PROMEDIO, MEDIANA, MODA, DESVEST para obtener estadísticas descriptivas.

- Crear tablas dinámicas para agrupar y analizar datos.

- Generar gráficos para visualizar tendencias y distribuciones.

##### 4.Exploración de relaciones

- Analizar correlaciones mediante tablas dinámicas y gráficos.

- Comparar métricas clave por género, temporada y talla.

- Evaluar el impacto de descuentos y métodos de pago en el comportamiento de compra.

##### 5.- Creación de dashboard interactivos 
 - Permiten observar los datos de manera más visual y estructurada.

## Requisitos e Instalación
Este proyecto se ha desarrollado por completo en la interfaz de google, a través de Google Sheets.
URL: https://docs.google.com/spreadsheets/d/16Xv3_cnuQT56q5JkozkNtUa7c4wBzevzI4M24GKNekg/edit?gid=1274025939#gid=1274025939

a través de Kaggle, se obtuvo la base de datos y la idea necesaria para llevar a cabo este proyecto
URL: https://www.kaggle.com/datasets/iamsouravbanerjee/customer-shopping-trends-dataset/data


## Recap Session
Sesión 1: 
- Se procede a la creación del Readme, junto a la descripción del poryecto y estructura de la base de datos utilizada
- Se crean las carpetas para crear la estructura del proyecto y mantener todos los datos en un mismo lugar

Sesión 2: 
- Se crea la hoja de cálculo de google sheets y se importa la base de datos correspondiente
- Se gestiona la información y se comienza con la limpieza y transformación de los datos, creando inicialmente una tabla de traducciones para todas las palabras en inglés.
- Se realiza la conversión de los datos en texto, fechas, números o moneda en aquellos que lo requieran (principalmente la moneda, edad y calificación de la reseña).
- Se hace una visualización de los datos y se elimina la columna Código_Promocional puesto que la información se repite respecto a Descuento  (tras analizar los datos, supone la misma información).
- Posteriormente, se procede a la creación de columnas para sustituir los términos y palabras en inglés al español ( usando funcion BUSCARV).
- Se descarga la plantilla con los datos transformados en formato CSV y se vuelve a importar sustituyendo el nombre de la hoja por Datos_Transformados y el nombre de la tabla por Datos_Compras.
- En la tabla Datos_Compras se eliminan todas las columnas que contengan las palabras en inglés dejando única y exclusivamente los datos y palabras en español.
- A partir de aquí se sientas las bases para proceder al análisis de datos y concluye la fase de transformación y limpieza de datos.

Sesión 3:

- Se realiza una revisión de las dos sesiones anteriores:
   * se ha detectado una incogruencia en la traducción "dress" en el género masculino y se sustituye "vestido" por "traje"; de la misma manera se hace con "outerwear" y se traduce como "Ropa de abrigo"
   * En el caso de la Frecuencia_Compras se observa que "Quarterly" y "every 3 months" significan lo mismo por lo que se sustituye "Cada 3 meses" por "trimestral.
   * Se hacen varias modificaciones para mantener la coherencia y el formato en cuanto al texto de la tabla, corrigiendo errores de mayúsculas o minúsculas
- En esta sesión se realiza el análisis descriptivo de los datos, analizando medias, desviaciones estándar , etcétera. Además se comienzan a realizar las primeras tablas dinámicas y gráficos para comenzar con el análisis de datos general.
- Se realizan gráficas de todos los datos categóricos de manera individual para conocer las tendencias y poder aproximarse hacia análisis posteriores más exhaustivas combinando columnas y datos.
- Los datos que presentan opciones "Sí" y " No" no son estudiados mediante gráfico debido a que la opción en Google Sheets "estadísticas de columna" nos permite analizar fácilmente esta información.
- Por otra parte, se crea una nueva hoja para realizar el cálculo de los datos numéricos ( Edad, Cantidad_Pagada, Calificación_Reseña y Compras_Anteriores)

Sesión 4:

- Tras haber estudiado individualmente todas las columnas de la base de datos, procedemos a realizar un estudio más exhaustivo combinando columnas y entrando en profundidad en el estudio de la base de datos.
- Se crea la pestaña DASHBOARD GENERAL para poder proceder a la creación del Dashboard principal en paralelo conforme se realiza el EDA
- En la hoja EDA se comienza con el estudio final de los datos. Empezamos estudiando relaciones asociadas a la Cantidad_Pagada y obteniendo los totales de ventas para el dashboard 
- Se continua realizando un mapa por ubicación y cantidad total en ventas 
- estudiamos las relaciones entre variables numéricas y categóricas que nos permiten establecer correlaciones y obtener información más detallada sobre los datos que tenemos.

Sesión 5 y 6:

- Se procede a la finalización del proyecto, tras haber realizado los estudios pertinentes y haber realizado todas las gráficas necesarias para el EDA, se procede al montaje del dashboard para la finalización del proyecto.

- El dashboard principal ( DASHBOARD GENERAL) consta:
    * un gráfico comparativo de las ventas totales por cada género( masculino o femenino)
    * Un mapa de Estados Unidos para conocer los estados dónde más se vende
    * Un gráfico de columnas mostrando las ventas totales por cada categoría 
    * Un gráfico de barras mostrando las ventas totales por cada Talla
    * Un gráfico de columnas con las ventas totales según el tipo de envío
    * Un gráfico de columnas dónde se muestra el recuento de reseñas según su calificación agrupada y por cada ítem comprado

    Además se han añadido unos filtros asociados a la talla, género, temporada y descuento que nos va a permitir tener un conocimiento exhaustivo de los patrones de compra de los clientes y así poder extraer conclusiones de cara al futuro.

- Tras realizar y terminar el dashboard se arregla el readme y se comienza a la redacción final del readme

Sesión 7

 - Se realiza un segundo dashboard de apoyo ( DASHBOARD VENTAS).
 - Este dashboard contiene información asociada única y exclusivamente a las ventas de la empresa, obteniendo datos sobre color de item comprado, tipo de compra, frecuencia, entre otros datos.
 - Además para una mejor extracción de datos se han realizado dos macros para obtener el gasto medio de compra o bien para ver los totales de ventas de cada grupo.
 - Por otra parte, se añaden varios controles de filtro para poder estudiar con detalle las ventas por ubicación, descuento, suscripción, talla y temporada.
 - Con esto se finalizaría todo el proyecto y quedaría únicamente repasar y procesar la información.

Sesión 8

 - Se hace una revisión de todas las hojas de google sheet y se procede a ordenar y adecuar el formato de la hoja del EDA. Se pulen los controles de filtro y se retocan las gráficas para permitir una mejor comprensión de los datos.
 - Se hacen modificaciones en el Readme, permitiendo dejarlo más legible y ordenado.
 - En paralelo se redacta en doc word un documento para recopilar los datos del EDA y nuevas hipótesis encontradas.
 
## Resultados y Conclusiones ( INFORME EXPLICATIVO DEL ANÁLISIS)📝
#### Hallazgos iniciales.🕵️‍♂️
   * No hay valores nulos en el conjunto de datos.
   * Estadísticas clave:
       + La edad de los clientes varía entre 18 y 70 años ( media de 44 años)
       + El gasto promedio por compra es de 59,76 dólares
       + La media de la calificación de reseñas es de 3,75
       + La talla "M" es la más vendida con un 45%, seguida de la talla "L" con un 27%.
       + La media de la calificación es bastante buena a lo largo de las categorías, habiendo casos concretos como los accesorios que presentan más ventas con calificaciones de reseña entre 4 y 5.
   * Datos Categóricos:
       + Tenemos género "Masculino" y "Femenino"
       + 4 catergorías principales ( Ropa, Ropa de abrigo, Accesorios y Calzado)
       + La región geográfica es Estados Unidos y todos los estados que conforman este país
       + Tenemos 6 opciones de pago diferentes ( Venmo,PayPal, Transferencia bancaria, Tarjeta de Crédito, Dinero en efectivo...)
       + Hay varios tipos de envío diferentes y diferentes frecuencias de compra

#### Análisis visual 

   - La categoría "Ropa" es la que mayor ventas proporciona.

   - EL top 5 ítems más comprados son : Pantalones(171 uds), Joyas(171 uds), Blusas(171uds), Camisas(169 uds) y Jersey(164uds).

   - Algunas regiones tienen ventas significativamente más altas que otras.
       Se recomienda analizar estas ubicaciones con más detalle para entender el porqué de su éxito

   - Relación entre compras previas y total de la compra actual:
       Hay correlación positiva leve que afirma que los clientes con más compras previas tienden a gastar más.

   - Ventas por Género: Es notoria que hay más compras por parte de la población masculina que de la población femenina.

   - Ventas por Temporada: se observa una relación de compras bastante equilibrada en todas las temporadas, sin haber grandísimas diferencias entre las diferentes estaciones del año.

   - Ventas por ubicación: Las zonas con más ventas son Montana e Illinois, siendo Kansas y Hawai las zonas con menos ventas. No se establecen relaciones en esta variación a excepción de Hawai dónde probablemente por tipo de envío ( Express y dia siguiente, son los mayoritarios) el cliente pudiera comprar menos. Se recomienda hacer un estudio exhaustivo de la ubicación y ver los factores, tanto de la empresa como los factores sociales y demográficos, que nos permitan entender el porqué de estas ventas.

   - Descuentos: el 57% de los clientes no usaron descuentos.

#### Identificación de patrones de compra.
   
   - el 43% de los clientes utilizaron descuentos durante sus compras.

   - El método de pago más frecuente fueron PayPal, tarjeta de crédito y dinero en efectivo siendo la transferencia bancaria el método menos usado de manera general.

   - Se observan que los patrones de compra se repiten quincenal y trimestralmente, respectivamente. Siendo las frecuencias más recurrentes entre los clientes

   - Es llamativa la baja tasa de suscripciones de clientes a la plataforma/tienda

   - Los colores verdes (verde, verde azulado, aceituna) agrupan la mayor parte de las ventas siendo una tendencia a tener en cuenta en la población.
  
#### Segmentación de clientes
  - Se propone establecer una segmentación de clientes basados en los hallazgos ( por ejemplo, Clientes de "alto valor" o VIP, "Clientes Jóvenes y urbanos", " Compradores ocasionales", "Clientes adultos", entre otros).
  - Alguna de las limitaciones que se encuentran en esta base de datos, es obtener criterios más depurados que nos permitan hacer esta segmentación de clientes para poder realizar un análisis más elaborado.
  - Habría que describir las caracterísitcas de cada segmento de clientes, definir correctamente cada segmento y de esta manera podemos analizar los datos y potenciar las ventas de cara a futuro.

#### Conclusiones y Recomendaciones

   * En general, podemos afirmar que los datos de ventas se mantienen regulares a lo largo de la estaciones del año, se observa como la tienda tiene un mayor volumen de compras por parte del género masculino y dónde la categoría más comprada es la "Ropa".

   * Generalmente, las reseñas son positivas y la mayoría superan los 3,5 puntos en todas las categorías e items comprados.

   * La impresión general es que el negocio está prosperando y presenta ventas sólidas en una variada gama de productos. La base de clientes puede mejorarse, para ello se haran posteriormente unas recomendaciones para atraer nuevos clientes. La distribución estacional nos indica un desempeño constante a lo largo de todo el año.

 ++ RECOMENDACIONES

  - Recomendación 1: Las ventas más altas se observan entre los hombres, principalmente debido a una base de clientes más grande en comparación con las mujeres. Sin embargo, las ventas promedio por cliente son casi idénticas para ambos sexos (incluso ligeramente superior para el género femenino). Para impulsar las ventas generales, recomendamos dirigirse a las clientes femeninas de manera más eficaz para equilibrar la proporción entre hombres y mujeres y aumentar la participación de la población femenina en las ventas de la empresa.

  - Recomendación 2: Las ventas son mayores en el grupo de edad de adultos, lo que indica una fuerte demanda. Para sacar provecho de esto, recomendamos centrar los esfuerzos de marketing y las promociones específicamente diseñadas para adultos, impulsando así ventas aún mayores en este grupo demográfico clave.

  - Recomendación 3: La talla mediana muestra consistentemente las mayores ventas. Para optimizar el inventario y satisfacer la demanda de los clientes, sugerimos priorizar el stock y la disponibilidad de productos de tamaño mediano, asegurando que los clientes tengan acceso a sus tamaños preferidos.

 - Recomendación 4: La categoría Ropa lidera las ventas, lo que la convierte en un área crucial para el crecimiento. Recomendamos garantizar que los niveles de existencias de prendas de vestir se mantengan altos, centrándose en los estilos populares, para satisfacer la demanda continua y maximizar las ventas.


## Próximos pasos �
Dentro de los próximos pasos que habría que hacer se recomienda:

 #### Estrategias de Expansión y Diversificación
  - Ampliación de catálogo: Explorar nuevas categorías de productos basadas en las tendencias de compra detectadas.
  - Estrategia de expansión geográfica: Analizar oportunidades en nuevos mercados o estados donde la empresa aún no tiene presencia significativa.
  - Personalización de productos: Implementar estrategias de customización de productos según las preferencias detectadas en el análisis.
#### Optimización de Estrategias de Marketing
  - Campañas dirigidas: Utilizar los datos de compras para realizar campañas más personalizadas según género, edad y ubicación.
  - Retargeting y fidelización: Implementar programas de fidelización que incentiven compras recurrentes.
  - Publicidad basada en datos: Usar la segmentación de clientes para optimizar la inversión en anuncios digitales.
####  Mejoras en Logística y Experiencia del Cliente
  - Optimización del stock: Ajustar la oferta en función de la demanda estacional y los productos más vendidos.
  - Reducción de tiempos de entrega: Evaluar nuevos proveedores o estrategias logísticas para mejorar la experiencia del cliente.
  - Mejora de la experiencia postventa: Incentivar a los clientes a dejar reseñas y mejorar el soporte al cliente.
####  Incorporación de Análisis Predictivo
  - Modelos de predicción de demanda: Implementar machine learning para prever tendencias futuras.
  - Análisis de abandono de clientes: Identificar clientes en riesgo de dejar de comprar y crear estrategias para retenerlos.
  - Optimización de precios: Evaluar estrategias de precios dinámicos según la demanda y competencia.


## Contribuciones🤝
 Las contribuciones son bienvenidas. Si deseas mejorar el proyecto, por favor 
abre un pull request o una issue

## Autores y Agradecimientos

Quería agradecer a todo el equipo de The Power por la oportunidad de aprender y poder desarrollar y crear este tipo de proyectos de iniciación en el mundo de Data & Analytics.

✒ Autores:
Óscar Arganda (https://github.com/oscarargo)








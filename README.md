# Proyecto_EDA

# Análisis Exploratorio de Datos de Tendencias de Compras 📊

## Descripción

Este proyecto consiste en un análisis exploratorio de datos (EDA) realizado sobre un conjunto de datos de tendencias de compras de clientes. El objetivo principal es obtener información valiosa sobre el comportamiento de compra de los clientes, identificar patrones y tendencias, y proporcionar una base para la toma de decisiones informadas en estrategias de marketing y ventas.

#### Objetivo Principal del Proyecto🎯🎯

El propósito de este análisis es comprender los patrones de compra de los clientes, evaluar la relación entre las características del consumidor y su comportamiento de compra, y detectar oportunidades para mejorar la fidelización y aumentar las ventas. Esto permitirá a la empresa personalizar sus ofertas, mejorar la segmentación del mercado y optimizar su logística de distribución.

## Conjunto de Datos📊

El conjunto de datos utilizado en este análisis contiene información sobre:

*   **ID_Cliente:** Identificador único del cliente.
*   **Edad:** Edad del cliente.
*   **Género:** Género del cliente.
*   **Artículo_Comprado:** Nombre del artículo comprado.
*   **Categoría:** Categoría del artículo comprado (Ropa, Accesorios, Calzado, etc.).
*   **Cantidad_Pagada (USD):** Monto gastado en la compra.
*   **Ubicación:** Ubicación geográfica del cliente.
*   **Talla:** Talla del artículo comprado.
*   **Color:** Color del artículo comprado.
*   **Temporada:** Temporada en la que se realizó la compra.
*   **Calificación_Reseña:** Calificación dada por el cliente al producto.
*   **Suscripción:** Indica si el cliente está suscrito o no.
*   **Tipo_Envío:** Método de envío utilizado.
*   **Descuento Aplicado:** Indica si se aplicó un descuento en la compra.
*   **Compras_Anteriores:** Número de compras anteriores realizadas por el cliente.
*   **Tipo_Pago:** Método de pago utilizado.
*   **Frecuencia_Compras:** Frecuencia con la que el cliente realiza compras

## Estructura del Proyecto
```bash
--- data
----- Datos_transformados.csv
----- shopping_trends_updated.csv #Datos originales

--- Readme.md
```

## Metodología/ Próximos pasos✍️✍️

 Pasos para realizar un Análisis Exploratorio de Datos (EDA) en Google Sheets:

##### 1.Carga de datos

- Subir el archivo CSV a Google Sheets.

##### 2.Revisar la estructura y verificar que los datos se hayan cargado correctamente.

- Limpieza de datos

- Renombrar columnas mal etiquetadas o genéricas.

- Manejar valores nulos y duplicados usando funciones de Google Sheets.

- Convertir formatos de datos según sea necesario (ejemplo: fechas, números).

##### 3.Análisis estadístico y visualización

- Usar funciones como PROMEDIO, MEDIANA, MODA, DESVEST para obtener estadísticas descriptivas.

- Crear tablas dinámicas para agrupar y analizar datos.

- Generar gráficos (barras, líneas, histogramas, scatter plots) para visualizar tendencias y distribuciones.

##### 4.Exploración de relaciones

- Analizar correlaciones mediante tablas dinámicas y gráficos.

- Comparar métricas clave por categoría de producto y temporada.

- Evaluar el impacto de descuentos y métodos de pago en el comportamiento de compra.

## Requisitos e Instalación
Este proyecto se ha desarrollado por completo en la interfaz de google, a través de Google Sheets.
URL: https://docs.google.com/spreadsheets/d/16Xv3_cnuQT56q5JkozkNtUa7c4wBzevzI4M24GKNekg/edit?gid=1274025939#gid=1274025939

a través de Kaggle, se obtuvo la base de datos y la idea necesaria para llevar a cabo este proyecto
URL: https://www.kaggle.com/datasets/iamsouravbanerjee/customer-shopping-trends-dataset/data

## Recap Session
Sesión 1: 
- Se procede a la creación del Readme, junto a la descripción del poryecto y estructura de la base de datos utilizada.
- Se crean las carpetas para crear la estructura del proyecto y mantener todos los datos en un mismo lugar.
- Se importa la base de datos con los datos originales "shopping_trends_updated.csv".

Sesión 2: 
- Se crea la hoja de cálculo de google sheets y se importa la base de datos correspondiente
- Se gestiona la información y se comienza con la limpieza y transformación de los datos, creando inicialmente una tabla de traducciones para todas las palabras en inglés.
- Se realiza la conversión de los datos en texto, fechas, números o moneda en aquellos que lo requieran (principalmente la moneda, edad y calificación de la reseña).
- Se hace una visualización de los datos y se elimina la columna Código_Promocional puesto que la información se repite respecto a Descuento y tras analizar los datos, supone la misma información.
- Posteriormente, se procede a la creación de columnas para sustituir los términos y palabras en inglés al español ( usando funcion BUSCARV).
- Se descarga la plantilla con los datos transformados en formato CSV y se vuelve a importar sustituyendo el nombre por Datos_Compras.
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
- Se crea la pestaña DASHBOARD para poder proceder a la creación del DASHBOARD en paralelo conforme se realiza el EDA
- En la hoja EDA se comienza con el estudio final de los datos. Empezamos estudiando relaciones asociadas a la Cantidad_Pagada y obteniendo los totales de ventas para el dashboard 
- Se continua realizando un mapa por ubicación y cantidad total en ventas 
- estudiamos las relaciones entre variables numéricas y categóricas que nos permiten establecer correlaciones y obtener información más detallada sobre los datos que tenemos.

Sesión 5:

- Se procede a la finalización del proyecto, tras haber realizado los estudios pertinentes y haber realizado todas las gráficas necesarias para el EDA, se procede al montaje del dashboard para la finalización del proyecto.

- El dashboard consta:
    * un gráfico comparativo de las ventas totales por cada género( masculino o femenino)
    * Un mapa de Estados Unidos para conocer los estados dónde más se vende
    * Un gráfico de columnas mostrando las ventas totales por cada categoría 
    * Un gráfico de barras mostrando las ventas totales por cada Talla
    * Un gráfico de columnas con las ventas totales según el tipo de envío
    * Un gráfico de columnas dónde se muestra el recuento de reseñas según su calificación agrupada y por cada ítem comprado

    Además se han añadido unos filtros asociados a la talla, género, temporada y descuento que nos va a permitir tener un conocimiento exhaustivo de los patrones de compra de los clientes y así poder extraer conclusiones de cara al futuro.

## Resultados y Conclusiones
- Conclusiones iniciales y próximos pasos.

- Identificación de patrones de compra.

- Posibles segmentaciones de clientes.

- Insights sobre descuentos, métodos de pago y frecuencia de compras.




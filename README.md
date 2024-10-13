# Recomendador de Películas

![download](https://github.com/user-attachments/assets/5b234e01-94bc-4703-9e8c-0795f67087c9)

Este proyecto es un sistema de recomendación de películas que utiliza técnicas de filtrado colaborativo y descomposición en valores singulares (SVD), en su implementacion mas avanzada, el objetivo es proporcionar recomendaciones personalizadas a los usuarios.

## Técnicas Utilizadas en la Resolución de un Ejercicio de Recomendación de Películas: Cosine Similarity y SVD para la version mejorada.

En este documento, se presentan dos técnicas empleadas en la construcción de un sistema de recomendación de películas: Cosine Similarity y Singular Value Decomposition (SVD). Ambas se utilizan para resolver problemas relacionados con la identificación de preferencias de usuarios y la recomendación de contenidos, aunque tienen enfoques distintos.

## 1. Cosine Similarity: Comparación de Similitud de Películas

### Descripción

Cosine Similarity es una técnica que mide la similitud entre dos elementos al comparar la orientación de sus vectores en un espacio multidimensional. En el contexto de un sistema de recomendación de películas, Cosine Similarity se emplea para medir qué tan similares son dos películas en función de características como género, actores, director, o incluso reseñas de usuarios.

### Aplicación en el Ejercicio

En este ejercicio de recomendación de películas:
•	Cosine Similarity se utilizó para comparar películas basándose en sus características vectorizadas, como el género o las descripciones textuales de las reseñas.

•	Dado un conjunto de películas vistas por un usuario, el sistema puede sugerir películas que sean similares en contenido o estilo a las que el usuario ya ha visto.

### Ejemplo

Si un usuario ha visto varias películas de acción, podemos representar esas películas como vectores en un espacio multidimensional, donde cada dimensión representa un género o una característica relevante. Cosine Similarity mide qué películas no vistas tienen una orientación vectorial similar a las que ya le gustaron al usuario, y se las recomienda.

### Ventajas

•	Eficiente y sencillo: Es fácil de calcular y útil en problemas donde el espacio vectorial es claro.

•	Comparación directa: Permite comparar películas directamente en función de sus características o descripciones.
 
## 2. Singular Value Decomposition (SVD): Extracción de Factores Latentes

### Descripción

SVD es una técnica de descomposición de matrices que permite reducir una matriz de datos complejos en componentes fundamentales. En los sistemas de recomendación de películas, SVD se usa para descubrir factores latentes, que son características no directamente observables que explican las preferencias del usuario. Esto es especialmente útil en sistemas de filtrado colaborativo, donde se basan las recomendaciones en las preferencias de otros usuarios con gustos similares.

### Aplicación en el Ejercicio
En este ejercicio:

•	Se utilizó SVD para descomponer una matriz de valoraciones (usuario-película) en factores latentes que representan los gustos de los usuarios y las características de las películas.

•	Al reducir la dimensionalidad de la matriz, el modelo puede descubrir patrones subyacentes en las preferencias de los usuarios, lo que permite hacer recomendaciones personalizadas basadas en gustos latentes.

### Ejemplo

Si un usuario ha calificado algunas películas, SVD puede descomponer la matriz de valoraciones y detectar que este usuario tiene una preferencia latente por las películas de ciencia ficción y aquellas con tramas complejas, incluso si no ha visto muchas películas de ese tipo directamente. El sistema recomendaría películas que coincidan con esos factores latentes.

### Ventajas

•	Descubre patrones ocultos: Identifica características latentes en los datos, lo que permite hacer recomendaciones más sofisticadas.

•	Filtrado colaborativo: Ideal para sistemas que se basan en las valoraciones de otros usuarios.
 
### Comparación de Cosine Similarity y SVD en el Ejercicio

•	Cosine Similarity es útil para comparar películas directamente a partir de sus características explícitas. Es más adecuado cuando se desea medir la similitud entre películas con atributos claros, como géneros o descripciones.

•	SVD, por otro lado, es más poderoso cuando se trabaja con grandes conjuntos de datos y se busca descubrir factores latentes que no son evidentes de forma directa. Es ideal para recomendar películas basadas en patrones complejos de valoración de usuarios.


## Archivos del Proyecto

- **recomendador_pelis.ipynb**: Notebook de Jupyter que contiene el código para cargar, limpiar y procesar los datos, así como para implementar el sistema de recomendación.
- **movies.csv**: Archivo CSV que contiene información sobre las películas, incluyendo el ID de la película, el título y los géneros.
- **ratings.csv**: Archivo CSV que contiene las calificaciones de los usuarios para las películas, incluyendo el ID del usuario, el ID de la película, la calificación y la marca de tiempo.
- **requirements.txt**: Archivo que lista las dependencias necesarias para ejecutar el proyecto.

## Instalación

Para instalar las dependencias necesarias, ejecuta el siguiente comando:

bash
pip install -r requirements.txt


## Uso

1. Abre el archivo `recomendador_pelis.ipynb` en Jupyter Notebook.
2. Ejecuta las celdas en orden para cargar los datos, limpiar los datos y generar recomendaciones.
3. Modifica el `user_id` en el ejemplo de uso para obtener recomendaciones para diferentes usuarios.

## Ejemplo de Recomendaciones

Al ejecutar el modelo, se generarán recomendaciones como las siguientes:

- Godfather, The (1972) (Crime|Drama)
- Die Hard (1988) (Action|Crime|Thriller)
- Godfather: Part II, The (1974) (Crime|Drama)

## Contribuciones

Las contribuciones son bienvenidas. Si deseas contribuir, por favor abre un issue o envía un pull request.

## Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo LICENSE para más detalles.

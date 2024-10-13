# Recomendador de Películas

Este proyecto es un sistema de recomendación de películas que utiliza técnicas de filtrado colaborativo y descomposición en valores singulares (SVD), en su implementacion mas avanzada, el objetivo es proporcionar recomendaciones personalizadas a los usuarios.

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
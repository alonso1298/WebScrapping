# WebScreapping
Scraping de Libros con Calificación Alta Este script en Python utiliza BeautifulSoup y Requests para hacer scraping de un sitio web de libros y extraer los títulos de aquellos que tienen una calificación de 4 o 5 estrellas.
## Descripción del Código:
1. URL Base Dinámica: Se define una URL base que contiene un marcador de posición para el número de página. Esta URL se utilizará para iterar sobre todas las páginas del catálogo de libros.
2. Iteración de Páginas: Se itera sobre cada página del catálogo, desde la página 1 hasta la 50. En cada iteración, se obtiene el contenido HTML de la página utilizando la librería requests y se convierte en un objeto BeautifulSoup para facilitar el análisis.
3. Selección de Datos: Se seleccionan los elementos HTML que representan los libros en la página utilizando selectores CSS. Estos elementos suelen tener una clase CSS específica, como .product_pod.
4. Filtrado por Calificación: Se comprueba si cada libro tiene una calificación de 4 o 5 estrellas. Si es así, se extrae el título del libro y se agrega a una lista de títulos con calificación alta.
5. Impresión de Resultados: Finalmente, se imprime en la consola la lista de títulos de libros que tienen una calificación de 4 o 5 estrellas.
## Uso:
Asegúrate de tener instaladas las librerías bs4 y requests.
Ejecuta el script Python en tu entorno local.
Observa la consola para ver los títulos de los libros con calificación alta.
## Nota:
Este script está diseñado para un sitio web específico y puede requerir modificaciones si se utiliza en otro sitio con una estructura HTML diferente.
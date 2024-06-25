# StarWarsApi

Aplicación en Java que permite a los usuarios consultar información sobre las películas de la saga de Star Wars a través de la API SWAPI (Star Wars API). Las principales funcionalidades del proyecto son:

Consulta de películas:
El usuario puede ingresar el número de la película que desea consultar.
La aplicación realiza una solicitud HTTP a la API SWAPI para obtener los datos de la película seleccionada.
Los datos de la película se muestran en la consola.

Manejo de excepciones:
Se utilizan bloques try-catch para capturar y manejar diferentes tipos de excepciones que pueden ocurrir durante la consulta a la API, como NumberFormatException cuando el usuario ingresa un valor no numérico.
Se define una excepción personalizada RuntimeException con un mensaje más descriptivo cuando no se encuentra la película solicitada.

Generación de archivos JSON:
Se crea una clase GeneradorDeArchivo que se encarga de guardar los datos de la película consultada en un archivo JSON.
El nombre del archivo se genera a partir del título de la película.
Se utiliza la biblioteca JsonBuilder para convertir el objeto de la película a formato JSON.
Se maneja la excepción IOException que puede ocurrir durante la escritura del archivo.

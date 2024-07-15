# LiterAlura
### Descripción del Proyecto

#### Nombre del Proyecto: Biblioteca Digital

#### Descripción General

Biblioteca Digital es una aplicación web construida utilizando Spring Boot que permite la gestión y consulta de información sobre libros y autores. La aplicación está diseñada para ofrecer funcionalidades básicas de consulta de datos de libros y autores, así como información sobre los idiomas disponibles y resultados de operaciones.

#### Estructura del Proyecto

El proyecto está organizado en varios paquetes que contienen modelos de datos, controladores y configuraciones necesarias para el funcionamiento de la aplicación. Los principales componentes del proyecto son:

1. **Modelos de Datos**: Clases que representan las entidades principales del sistema, como `Author`, `Book`, `LanguagesOptions`, y `Results`.
2. **Controladores**: Clases que manejan las solicitudes HTTP y devuelven respuestas adecuadas basadas en las operaciones solicitadas.

#### Modelos de Datos

1. **Author.java**: Representa un autor con atributos `name` y `nationality`.
2. **AuthorData.java**: Envuelve un objeto `Author`.
3. **Book.java**: Representa un libro con atributos `title`, `author` (referencia a un objeto `Author`) y `language`.
4. **BookData.java**: Envuelve un objeto `Book`.
5. **LanguagesOptions.java**: Contiene un array de strings que representan los idiomas disponibles.
6. **Results.java**: Representa los resultados de una operación con atributos `status` y `message`.
7. **ResultsData.java**: Envuelve un objeto `Results`.

#### Controladores

1. **BookController.java**: Maneja las solicitudes relacionadas con libros y autores. Los endpoints principales son:
   - `/book`: Devuelve información sobre un libro basándose en el título proporcionado.
   - `/languages`: Devuelve una lista de idiomas disponibles.
   - `/results`: Devuelve los resultados de una operación basándose en los parámetros de estado y mensaje proporcionados.

#### Funcionalidades

- **Consulta de Libros**: Permite obtener información sobre un libro específico, incluyendo su título, autor y lenguaje.
- **Idiomas Disponibles**: Proporciona una lista de idiomas en los que se pueden encontrar libros.
- **Resultados de Operaciones**: Muestra el estado y mensaje de las operaciones realizadas en la aplicación.

#### Ejecución del Proyecto

Para ejecutar la aplicación, asegúrate de tener configurado el entorno de desarrollo adecuado (JDK, Maven) y sigue los siguientes pasos:

1. Clona el repositorio del proyecto.
2. Importa el proyecto en tu IDE preferido (IntelliJ IDEA, Eclipse, etc.).
3. Ejecuta la clase principal `DemoApplication.java`.
4. Accede a los endpoints proporcionados a través de un navegador web o herramientas como Postman.

#### Ejemplo de Uso

- Obtener información de un libro: `http://localhost:8080/book?title=MiLibro`
- Listar idiomas disponibles: `http://localhost:8080/languages`
- Consultar resultados de operaciones: `http://localhost:8080/results?status=success&message=Operation completed successfully`

Este proyecto proporciona una base sólida para gestionar y consultar información relacionada con libros y autores, y puede ser expandido para incluir funcionalidades adicionales según las necesidades específicas.

Si necesitas más detalles o ayuda con alguna funcionalidad específica, no dudes en preguntar.

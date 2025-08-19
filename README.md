# Foro Hub 

## Descripción

Este proyecto es una API REST desarrollada como parte del desafío del curso "Practicando Spring Framework: Challenge Foro Hub" de Alura. El objetivo es construir un foro donde los usuarios puedan crear tópicos con sus dudas y sugerencias, permitiendo a otros responder e interactuar en la comunidad.

## Funcionalidades

-   Listar todos los tópicos existentes.
-   Crear nuevos tópicos (requiere autenticación).
-   Eliminar tópicos (requiere autenticación).
-   Autenticación de usuarios mediante JWT (JSON Web Tokens).

## Tecnologías Utilizadas

-   Java
-   SpringBoot
-   Base de datos de tu elección (MySQL, PostgreSQL, etc.)
-   JWT para la autenticación
-   Insomnia (o Postman) para probar la API

## Requisitos

-   Java Development Kit (JDK) 11 o superior  
-   Maven
-   Base de datos configurada

## Configuración

1.  Clona el repositorio:

    ```bash
    git clone [URL del repositorio]
    ```

2.  Configura la base de datos:

    -   Crea una base de datos con el nombre que prefieras.
    -   Actualiza el archivo `application.properties` (o `application.yml`) con los detalles de conexión a tu base de datos.

    ```properties
    spring.datasource.url=jdbc:mysql://localhost:3306/[nombre de la base de datos]
    spring.datasource.username=[usuario]
    spring.datasource.password=[contraseña]
    spring.jpa.hibernate.ddl-auto=update
    ```

3.  Ejecuta la aplicación:

    ```bash
    mvn spring-boot:run
    ```

## Endpoints

-   `GET /topicos`: Lista todos los tópicos.
-   `POST /topicos`: Crea un nuevo tópico (requiere JWT).
-   `DELETE /topicos/{id}`: Elimina un tópico (requiere JWT).
-   `POST /auth`: Autenticación para obtener el token JWT.



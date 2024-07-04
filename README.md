# ForoHub
ForoHub es una aplicación para gestionar tópicos (temas de discusión) utilizando Spring Boot, JPA y Flyway. Este proyecto permite autenticar usuarios y gestionar tópicos.

## __Características__

Autenticación de usuarios

Gestión de tópicos (crear, listar, actualizar y eliminar)

Documentación de la API con Swagger

## __Requisitos__

Java 17+

Maven 3+

Base de datos MySQ

IDE IntelliJ

API Insomnia


## __Instalación__

__Clonar el repositorio:__

       git clone https://github.com/AleVaz70/ForoHub.git

__Navegar al directorio del proyecto:__

      cd ForoHub

__Configurar la base de datos en application.properties:__

      spring.datasource.url=jdbc:mysql://localhost:3306/forohub

      spring.datasource.username=tuusuario

      spring.datasource.password=tucontraseña

__Ejecutar la aplicación:__

      mvn spring-boot:run


## __USO - Insomnia__

__Autenticar un usuario:__
          Realizar una petición POST a /login con los datos de autenticación:


![Screenshot_234](https://github.com/AleVaz70/ForoHub/assets/124855251/7cb3a330-1691-4b04-a524-9eda59da08eb)


__Registro de Tópicos:__
         Para registrar un nuevo tópico, envía una solicitud POST a /topicos con el siguiente cuerpo JSON:

  "titulo": "Nuevo Tópico",
  
  "mensaje": "Este es el mensaje del nuevo tópico",
  
  "fechaCreacion": "2024-07-04T10:00:00",
  
  "status": "ABIERTO",
  
  "autor": "nuevoUsuario",
  
  "curso": "BACK_END",
  
  "respuestas": "No hay respuestas"




![Screenshot_232](https://github.com/AleVaz70/ForoHub/assets/124855251/19489d78-a1ab-4b96-bf3f-cda877225874)


__Listar tópicos:__ 
      Realizar una petición GET a /topicos


![Screenshot_233](https://github.com/AleVaz70/ForoHub/assets/124855251/c096a40e-ec19-4165-a04c-b8f6f6ac7f15)


__Actualizar un tópico:__
Realizar una petición PUT a /topicos/{id} con los datos actualizados del tópico.

![Screenshot_236](https://github.com/AleVaz70/ForoHub/assets/124855251/970d0f88-49af-45d0-bded-c25f10ceac31)


__Obtener datos de un tópico:__ 
Realizar una petición GET a /topicos/{id} 

![Screenshot_235](https://github.com/AleVaz70/ForoHub/assets/124855251/5447c8ea-5038-420d-b6d3-f3c67371312d)


__Eliminar un tópico:__
Realizar una petición DELETE a /topicos/{id}

![Screenshot_237](https://github.com/AleVaz70/ForoHub/assets/124855251/dc2891bd-2909-433a-a0a4-f50d509e07d2)



## __Swagger__

Swagger proporciona una interfaz gráfica para interactuar con la API. Puedes acceder a ella en           http://localhost:8080/swagger-ui.html.


![Screenshot_238](https://github.com/AleVaz70/ForoHub/assets/124855251/eba25203-b074-41ca-9dec-80ca89b846a0) 
![Screenshot_239](https://github.com/AleVaz70/ForoHub/assets/124855251/8ad32fd5-8a1a-41df-9d17-be482ac217b2)

## __Estado del Proyecto__
Este proyecto cumple con la consigna básica y se seguirá completando próximamente con más funcionalidades y mejoras.

## __Contribuciones__
Las contribuciones son bienvenidas. Por favor, abre un issue o un pull request para discutir cualquier cambio que desees realizar.

## __Licencia__
Este proyecto está licenciado bajo la Licencia MIT.


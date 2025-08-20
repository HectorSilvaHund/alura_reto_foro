# Reto Alura Foro Hub - HSH

Hola!!
Este es mi mini-foro en **Java + Spring Boot**. No tiene frontend (todavía), pero con Insomnia/Postman se puede probar todo.

---- ¿Qué hace?
- CRUD de **tópicos**: crear, listar, ver, actualizar, borrar.
- **Login** con `/auth/login` que devuelve un **token** (Bearer).
- Con token puedes crear/editar/borrar; sin token → 401/403.
- Guarda en **PostgreSQL**.

- Tech
- IDE: Intellij
- Java 17, Spring Boot 3
- Spring Web, Security, Data JPA, Validation
- PostgreSQL
- JWT (`com.auth0:java-jwt`)

## Config (application.properties)
```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/forohub_db
spring.datasource.username=forohub_user
spring.datasource.password=forohub_pass
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
app.jwt.secret=esta_es_mi_llave_super_secreta_guardala_bien
app.jwt.expiration-min=120

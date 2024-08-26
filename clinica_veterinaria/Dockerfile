FROM openjdk:22-jdk-slim
#el comando ARG especifica en donde estara nuestro archivo jar cuando se compile la app
#por defecto la ruta en intellij IDEA es esta
# "clinica_veterinaria" viene de pom.xml -> name
# "0.0.1.jar" -> viene de la version que pusimos en el archivo pom.xml -> version
ARG JAR_FILE=target/clinica_veterinaria-0.0.1.jar
COPY ${JAR_FILE} app_veterinaria.jar
EXPOSE 8080
ENTRYPOINT ["java", "-jar", "app_veterinaria.jar"]
FROM openjdk:21-ea-slim

WORKDIR /app

COPY . .

RUN ./mvnw clean package -DskipTests

RUN ls -la /app/target/demo-0.0.1-SNAPSHOT.jar

RUN chmod +x /app/target/demo-0.0.1-SNAPSHOT.jar

CMD ["java", "-jar", "/app/target/demo-0.0.1-SNAPSHOT.jar"]

FROM amazoncorretto:17
WORKDIR /app

COPY . .
RUN ./gradlew build

ENV SPRING_PROFILES_ACTIVE=production
EXPOSE 8080

CMD ["java", "-jar", "build/libs/demo-0.0.1-SNAPSHOT.jar"]
#STAGE BUILD
FROM openjdk:8-jdk-alpine AS builder
WORKDIR /workspace/
COPY . .
RUN ./gradlew clean test
RUN ./gradlew jacocoTestReport
RUN ./gradlew build

#STAGE RUN
FROM openjdk:8-jdk-alpine
WORKDIR /app/
COPY --from=builder /workspace/build/libs/*.jar ./app.jar
CMD ["java","-jar","app.jar"]
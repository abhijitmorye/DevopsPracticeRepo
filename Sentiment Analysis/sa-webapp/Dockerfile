FROM openjdk:8-jdk-alpine
RUN mkdir -p /home/app
WORKDIR /home/app
ENV SA_LOGIC_API_URL  http://localhost:5000
EXPOSE 8080
COPY ./target/sentiment-analysis-web-0.0.1-SNAPSHOT.jar.jar home/app
CMD ["java","-jar","sentiment-analysis-web-0.0.1-SNAPSHOT.jar","--sa.logic.api.url=${SA_LOGIC_API_URL}"]

FROM eclipse-temurin:21.0.2_13-jre-alpine
LABEL maintainer="yousseftouzani2003@gmail.com"
VOLUME /main-app
ADD build/libs/internet-banking-fund-transfer-service-0.0.1-SNAPSHOT.jar app.jar
EXPOSE 8084
#COPY wait-for-it.sh wait-for-it.sh
#RUN chmod +x wait-for-it.sh
# Add bash for wait-for-it.sh
RUN apk add --no-cache bash
ENTRYPOINT ["java",  "-Dspring.profiles.active=docker","-jar", "/app.jar"]

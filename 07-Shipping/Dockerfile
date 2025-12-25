FROM maven
WORKDIR /opt/server
COPY pom.xml .
COPY src /opt/server/src
RUN mvn clean package
RUN mv /opt/server/target/shipping-1.0.jar /opt/server/shipping.jar 
# ENV are in docker compose
CMD ["java", "-jar", "shipping.jar"]

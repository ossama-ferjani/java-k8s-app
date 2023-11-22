FROM  openjdk:8-jre
ADD target/productcatalogue-0.0.1-SNAPSHOT.jar productcatalogue.jar
ADD product-catalogue.yml app-config.yml
EXPOSE 8080
ENTRYPOINT [ "executable" ]["java", "-Djava.security.egd=file:/dev/./urandom", "-jar", "productcatalogue.jar", "server", "app-config.yml"]


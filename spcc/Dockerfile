FROM chandrabhogaraju/mvn-jdk17-dind:3.9.3
RUN apt update  
RUN apt install git -y
RUN  git clone https://github.com/spring-projects/spring-petclinic.git
WORKDIR spring-petclinic
RUN mvn package
EXPOSE 8080/tcp
CMD ["java" "-jar" "spring-petclinic-3.2.0-SNAPSHOT.jar"]
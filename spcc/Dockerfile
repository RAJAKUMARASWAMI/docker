FROM chandrabhogaraju/mvn-jdk17-dind:3.9.3
LABEL name="MEDHASWI" 
RUN apt update  
RUN apt install git -y
RUN  git clone https://github.com/spring-projects/spring-petclinic.git
WORKDIR spring-petclinic
RUN mvn package
WORKDIR srv/spring-petclinic/target
EXPOSE 8080/tcp
CMD ["java","-jar","spring-petclinic-3.2.0-SNAPSHOT.jar"]

FROM amazoncorretto:11
LABEL owner="raj"
LABEL company="cotton"
WORKDIR /spring-petclinic
RUN yum update  
RUN yum install maven openjdk-17-jdk git -y
RUN  git clone https://github.com/spring-projects/spring-petclinic.git 
RUN mvn package
CMD ["java" "-jar" "spring-petclinic-3.2.0-SNAPSHOT.jar"]
EXPOSE 8080/tcp
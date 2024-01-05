FROM ubuntu
RUN yum update  
RUN yum install maven openjdk-17-jdk git -y
RUN  gtcpit clone https://github.com/spring-projects/spring-petclinic.git
WORKDIR spring-petclinic
RUN mvn package
EXPOSE 8080/tcp
CMD ["java" "-jar" "spring-petclinic-3.2.0-SNAPSHOT.jar"]
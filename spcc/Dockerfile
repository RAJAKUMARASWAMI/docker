FROM amazoncorretto:11
LABEL owner="raj"
LABEL company="cotton"
RUN sudo apt update && sudo apt install maven openjdk-17-jdk -y
RUN  git clone https://github.com/spring-projects/spring-petclinic.git /home/ubuntu
RUN cd /home/ubuntu/spring-petclinic
CMD ["mvn" "package"]
RUN cd /home/ubuntu/spring-petclinic/target
CMD ["java" "-jar" "spring-petclinic-3.2.0-SNAPSHOT.jar"]
EXPOSE 8080/tcp
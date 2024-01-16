FROM eclipse-temurin:21-jdk-alpine
VOLUME /tmp
RUN addgroup -g 1002 istory && adduser -D -u 1002 -G istory istory && chown -R istory:istory /home/istory
USER istory
WORKDIR /home/istory
COPY springbootdeveloper-0.0.1-SNAPSHOT.jar /home/istory/istory.jar
# 컨테이너가 시작될 때 실행할 명령 지정
ENTRYPOINT ["java", "-jar", "istory.jar"]

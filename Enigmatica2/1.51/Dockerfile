FROM java:8-jdk-alpine
VOLUME /minecraft
RUN wget https://minecraft.curseforge.com/projects/enigmatica2/files/2629071/download -O /minecraft/install.zip
RUN unzip /minecraft/install.zip -d /minecraft/
RUN rm -f /minecraft/install.zip
EXPOSE 25565
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar" ]

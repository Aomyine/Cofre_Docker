# Escolha a imagem base do JDK. Aqui estamos usando a imagem do OpenJDK 11.
FROM openjdk:11-jre-slim

# Define o diretório de trabalho no contêiner onde todos os comandos serão executados.
WORKDIR /app

# Copie o arquivo JAR construído para o diretório de trabalho no contêiner.
COPY target/cofre-0.0.1-SNAPSHOT.jar app.jar

# Expõe a porta 25000. Ajuste se sua aplicação utiliza outra porta.
EXPOSE 25000

# Comando para executar o aplicativo.
CMD ["java", "-jar", "app.jar"]

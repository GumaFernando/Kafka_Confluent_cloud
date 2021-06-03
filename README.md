# Cloud-native service for Apache Kafka

O Apache Kafka é uma plataforma de streaming distribuída e escalável Open Source, que através dessa plataforma é 
capaz de publicar dados para qualquer número de sistemas ou aplicativos em tempo real, sendo possível ingerir
trilhões de eventos por dia em alta velocidade.

# Proposta inicial

O intuito desse projeto, foi botar em prática o conhecimento adquirido sobre os fundamentos do Apache Kafka.
Optei por utilizar a plataforma Confluent Cloud para a realização desse projeto AFIM DE ESTUDOS.

Foi realizado a criação de uma aplicação simples em Python simulando um Producer, na qual envia os dados
contendo 3 campos: "ID","NOME","DATA", simulando uma transação qualquer, e através do Kafka faz a ingestão desses dados, e foi criado utilizando o KSQL um
Stream para capturar esses dados e fazer uma agregação em uma janela de tempo de 20 segundos para identificar os TOP2 nomes.

# Desenvolvimento

### Criação de uma aplicação em Python simulando um Producer

[!alt text](https://github.com/GumaFernando/kafka_confluent_cloud/blob/main/7.png)

### Demonstração da saída dos dados

[!alt text](https://github.com/GumaFernando/kafka_confluent_cloud/blob/main/8.png)

### Criação de um stream no tópico - "TOPIC_GUMA"

[!alt text](https://github.com/GumaFernando/kafka_confluent_cloud/blob/main/1.png)

### Realizando uma agregação dos dados em KSQL utilizando uma janela de tempo 

[!alt text](https://github.com/GumaFernando/kafka_confluent_cloud/blob/main/3.png)

### Demonstração dos resultados dos Stream 

[!alt text](https://github.com/GumaFernando/kafka_confluent_cloud/blob/main/4.png)

### Consultando Schema do stream

[!alt text](https://github.com/GumaFernando/kafka_confluent_cloud/blob/main/5.png)

### Consultando informações do Tópico

[!alt text](https://github.com/GumaFernando/kafka_confluent_cloud/blob/main/6.png)


# AWS SQS integration

Esse projeto é apenas uma demonstração, um teste de como integrar seu projeto Spring
com o serviço do SQS (Simple Queue Service) da AWS.

**IMPORTANTE**

O projeto se encontra utilizando a versão 2.7.1 do SpringFramework.

## Requisitos iniciais
- Java 11 
- Postman
- Conta AWS e configurar o projeto como descrito abaixo.

Para configurar a fila para qual será enviada a mensagem, basta definir as variáveis de ambiente:

- QUEUE_NAME : Nome da Queue.
- QUEUE_URL : Endpoint da Queue definida.
- QUEUE_REGION : Região que se encontra.
- ACCESS_KEY e SECRET_KEY : Chaves de acesso e Secret da conta IAM da AWS.



## Endpoint

#### Envio de item para a fila

```http
  POST /queue/{message}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `message` | `string` | A mensagem que será enviada para a queue |



## Referências

- https://cloud.spring.io/spring-cloud-static/spring-cloud-aws/2.0.0.RELEASE/multi/multi_spring-cloud-aws.html
- https://www.youtube.com/watch?v=q3zo3YREfJI

# RabbitMQ

## Como iniciar o RabbitMQ [(download)](https://www.rabbitmq.com/download.html)

```docker
docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3-management
```

## Teste "Hello world"

Para enviar mensagens

```bash
# usa a mensagem padrão
npm run sender
# ou digitar suas mensagens
npm run sender "uma mensagem" "outra mensagem" teste
```

Para receber as mensagens

```bash
npm run receiver
```

## Teste "Work Queues"

Execute um ou mais workers

```bash
# terminal 1
./worker.js

# terminal 2
./worker.js

# quantos outros mais quiser
```

Crie novas tarefas

```bash
./new_task.js mensagem um.
./new_task.js mensagem dois..
./new_task.js mensagem tres...
./new_task.js mensagem quatro....
# quantas outras mais quiser
```

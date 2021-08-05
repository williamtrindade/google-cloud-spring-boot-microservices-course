## Demo application
### Demo application architecture

![Image](https://i.ibb.co/9tgtrCY/image.png)

### Distributed tracing using zipkin architecture
![Image](https://i.ibb.co/g3BVx19/image.png)

### Message queuing service architecture
![Image](https://i.ibb.co/Cm13HfP/image.png)
___

## Comandos cloud shell

> Visualizar conta  
```gcloud config list account```   

> Visualizar projeto  
```gcloud config list project```   

> Definir zona  
```gcloud config set compute/zone [YOUR_ZONE]```

> Ver todas variáveis definidas  
```gcloud config list```   
_____
## Comandos Cloud SQL

> Enable Cloud SQL Administration API   
```gcloud services enable sqladmin.googleapis.com```

> Confirm that Cloud SQL Administration API is enabled   
```gcloud services list | grep sqladmin```   

> Listar as instâncias de Cloud SQL   
```gcloud sql instances list```

> Criar instância Cloud SQL   
```gcloud sql instances create guestbook --region=us-central1```   

> Criar um banco em Cloud SQL   
```gcloud sql databases create messages --instance guestbook```

> Conectar ao banco com gcloud CLI   
```gcloud sql connect guestbook```   
___
### Comandos Cloud Trace API
> Habilitar a Cloud Trace API   
```gcloud services enable cloudtrace.googleapis.com```
___ 
### Comandos Cloud Pub/Sub API
> Ative a API Cloud Pub/Sub   
```gcloud services enable pubsub.googleapis.com```

> Crie um tópico Cloud Pub/Sub   
```gcloud pubsub topics create messages```

> Crie uma inscrição Pub/Sub   
```gcloud pubsub subscriptions create messages-subscription-1 --topic=messages```

> Fazer pull das mensagens Pub/Sub   
```gcloud pubsub subscriptions pull messages-subscription-1```

____

### Comandos do App Engine
> Habilitar o App Engine no projeto
```gcloud app create --region=us-central```

___

## Comandos Maven
> Rodar aplicação spring back-end    
```./mvnw -q spring-boot:run -Dserver.port=8081```
___
## Comandos da aplicação demo
> Test   
```curl http://localhost:8081/guestbookMessages```

> Post   
```
curl -XPOST -H "content-type: application/json" \
-d '{"name": "Ray", "message": "Hello"}' \
  http://localhost:8081/guestbookMessages

```
  
> Get All   
```curl http://localhost:8081/guestbookMessages```
_____

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


# App Angular Docker
App node teste para turma de Infra III da DigitalHouse

# Dependências
 - [Node >= 17.x](https://nodejs.org)
 - [Angular 2.x](https://angular.io/) - dica: add no seu Dockerfile
 
# Dicas

## Dockerfile
```
# copie o conteudo do /src pra sua imagem

RUN  npm  install  -g  @angular/cli@13
RUN  npm  ci
CMD  ["ng",  "serve",  "--host",  "0.0.0.0"]
```
## Docker-compose
```
		build: .
		ports:
			- 4200:4200
```

# Rotas
 - http://localhost:4200/api/v1/healthcheck

# serverRest-API
Testes de API - Utilizando Postman, newman e newman-htmlextra

Teste de API Rest do manual a CI/CD
## O que é
Projeto desenvolvido afim de praticar mais testes de API, desde o manual ao CI/CD, gerar massas de testes, gerar relatorios com Newman e colocar para rodar em uma pipeline CI/CD

## Tecnologias utilizadas
- Postman versão web
- node version v18.17.1
- newman v6.2.1
- newman-reporter-html

  
## Documentações
- Doc da API: [Consulte Swagger](https://serverest.dev/#/)

## Como instalar o ambiente
- Primeiro: instale o node em seu computador [baixe aqui](https://nodejs.org/en/download)
- Segundo: realize a instalação do newman de forma global [baixe aqui a dependencia](https://www.npmjs.com/package/newman)
```
npm install -g newman
```
- Terceiro: realize a instalação da dependencia dos relatórios (opcional) [newman-reporter-html
](https://www.npmjs.com/package/newman-reporter-html)
```
npm install -g newman-reporter-html
```
## Como rodar os testes
### Pelo Postman web ou desktop
- Import a collection e o environment
- Execute os teste de forma manual ou automatizada
### Pelo newman
- Abra o console de preferência
- Execute a seguinte linha de comando para rodar os testes
```
newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli
```
- Execute os teste com relatório
```
newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli,htmlextra
```

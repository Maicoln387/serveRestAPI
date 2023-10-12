# Bootcamp 01 de testes (serveRestAPI)

Testes de API's do manual a CI/CD 
Criação de testes de api utilizando postman, newman e newman-htmlextra 

## O que é

Este repositório foi criado para o bootcamp de Testes de API Rest.

## Tecnologias utilizadas

- Postman versão web
- node version v18.16.0
- newman v6.0.0
- newman-reporter-html 

##  Documentações

- Doc. da API: [Consulte Swagger](https://serverest.dev/)

## Como instalar o ambiente

- Primeiro: instalar o node [Baixar aqui](https://nodejs.org/en/download)
- Segundo: Realizar a instalação do newman de forma global [Baixe aqui a dependência](https://www.npmjs.com/package/newman)
  ```
  npm install -g newman 
  
  ```
  
- Terceiro: Realizar a instalação das dependências do relatório (Opcional) [newman-reporter-html](https://www.npmjs.com/package/newman-reporter-html)
  ```
  npm install -g newman-reporter-html
  
  ```


## Como rodar os testes

### Pelo postman web e desktop

- Importar a collection e o environment 
- Executar os testes de forma manual ou automatizada

### Pelo newman 

- Abra o console de preferência
- Execute a seguinte linha de comando para rodar os testes
  ```
  newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli
  ```
  - Execute os testes com relatório
  ```
  newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli,htmlextra
  ```

 ### Reporter

 Se optou por rodar os testes com o report htmlextra, foi gerado um arquivo html com o resultado dos testes e para verificar as validações, abra a pasta **newman** que foi criada no local em que os arquivos de collection e environment se encontram. 

## Entre em contato: 

Email: maicoln_gs@hotmail.com 

Redes Sociais: https://linktr.ee/maicoln  

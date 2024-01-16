# Bootcamp Qualiters Club serveRestAPI
Testes de API Rest do manual à CI/CD 
Criação de testes de api utilizando postman, newman e newman-htmlextra

##O que é

Este repositório foi criado para o Bootcamp de API Rest.

## Tecnologias utilizadas 

- Postman versão web
- node version v20.11.0
- newman version 6.1.0
- newman-reporter-html

## Documentações 

- Análise Técnica/
- Doc. da API: [Consulte Swagger](https://serverest.dev/#/) 

## Como instalar o ambiente 

- Primeiro: instale o node.js no seu computador [baixe aqui](https://nodejs.org/en/download)
- Segundo: realize a instalação do newman de forma global [baixe aqui a dependência](https://www.npmjs.com/package/newman)
  ```
  npm install -g newman 
  ```
- Terceiro: realize a instalação da dependência dos relatórios (opcional) [newman-reporter-html](https://www.npmjs.com/package/newman-reporter-html)
  ```
  npm install -g newman-reporter-html
  ```

## Como rodar os testes

### Pelo Postman Web ou Desktop 
- Import a collection e o environment
- Execute os testes de forma manual ou automatizada 

### Pelo Newman  
- Abra o console de preferência
- Execute a seguinte linha de comando para rodar os testes
  ```
  newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json  -r cli
  ```
- Execute os testes com relatório
  ```
  newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json  -r cli,htmlextra
  ```

### Report 

Se você optou por rodar os testes com o report htmlextra, você gerou um arquivo html comm o resultado dos testes e para verificar as validações pode-se abrir a pasta [newman] que foi criada no local em que os arquivos da collection e environment se encontram. 


## Entre em contato 

- Email: maicoln_gs@hotmail.com 
- Redes Sociais: https://linktr.ee/maicoln

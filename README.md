# API de Banco em NodeJS 🪙

Este repositório contém uma API desenvolvida em NodeJS para simular um ambiente de banco. 
Com esta API, os usuários podem criar uma conta, realizar transações dentro de sua conta, efetuar crédito e débito em sua conta, verificar o saldo e excluir a conta.

A API não possui banco de dados vinculado e armazena dados em memória, ou seja quando ocorre a atualização você perde os dados e foi criada para fins educacionais.

## Como utilizar

1. Clone este repositório
2. Instale as dependências com `npm install`
3. Inicie o servidor com `npm run dev`
4. Acesse a API em `http://localhost:3333`

## Rotas disponíveis

- `POST /account`: Cria uma nova conta
- `GET /account`: Retorna informações sobre uma conta específica
- `GET /statement`: Retorna o extrato da conta do usuario
- `GET /statement/:date`: Retorna o extrato da conta do usuario em uma data especifica
- `GET /balance`: Retorna o saldo da conta do usuario
- `POST /deposit`: Adiciona um deposito na conta do usuario
- `POST /withdraw`: Retira um saldo da conta do usuario
- `PUT /account`: Atualiza o nome do usuario
- `DELETE /account`: Remove a conta do usuario

## Teste da API utilizando o Postman

Você pode realizar testes de requisições pré configuradas utilizando a collection carregada nesse repositório no diretório [Postman_Collection]: (Postman_Collection/API Banco.postman_collection.json)
- O endereço base da API está configurado como variavel da collection, caso você altere na API lembre-se de mudar nas configurações da collection
- Os dados utilizados são ficticios
- Lembre-se de passar o campo CPF no header das requesições, pois a API tem a obrigatóriedade de uso de uma conta "ativa"

## Dependências
- v18.15.0
- express: v4.18.2
- uuid: v9.0.0

## Informações e Contato:

- A branch main está bloqueada para alteração, caso queira modificar algo realiza a criação de uma nova branch
- Caso enfrente problemas ou queira sugerir algo pode me contata em henrikesilva.dev@gmail.com
- Se divirta!! 😉

## Licença
Este projeto está licenciado sob a licença MIT.

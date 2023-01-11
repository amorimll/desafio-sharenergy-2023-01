# Desafio Sharenergy 2023 Back End Jr.
- *Tive alguns problemas com o git e acabei perdendo os commits.*
Repositório criado para a minha aplicação do Desafio Sharenergy 2023. Contato: [gabrielmaia.amorim01@gmail.com](mailto:gabrielmaia.amorim01@gmail.com?subject=[GitHub]%20Source%20Han%20Sans), https://www.linkedin.com/in/gabriel-amorim-45935b1a3/

## Deploy e Links
- Deploy do projeto: https://sharenergy-client.vercel.app/
- Vídeo explicativo: https://youtu.be/_ezj50MCbZA

# O Projeto

![image](https://user-images.githubusercontent.com/63107417/211658343-4973c772-84cb-44fb-a8b0-bd0bfc67f999.png)

## Rodar localmente

1. Use o comando `git clone https://github.com/amorimll/desafio-sharenergy-2023-01`
2. Entre nas pastas "client" e "server", e execute o comando `npm install` em ambas as pastas.
3. Crie um arquivo .env na pasta "server", e crie as seguinte variáveis, `MONGO_URL="mongodb://localhost/sharenergy-backend"`, `JWT_SECRET="SHARENERGYSECUREPASS"` e `PORT=3001`
4. Após instaladas as depedências, execute o comando `npm run dev` em ambas as pastas, e a aplicação vai iniciar.

## Portas

Client: `localhost:3000`
Server: `localhost:3001`

## Tecnologias Usadas

### Front end:
- [![My Skills](https://skillicons.dev/icons?i=ts,react,redux,materialui)](https://skillicons.dev)
### Back end: 
- [![My Skills](https://skillicons.dev/icons?i=ts,nodejs,express)](https://skillicons.dev)
### Servidor: 
- [![My Skills](https://skillicons.dev/icons?i=mongodb)](https://skillicons.dev)

## Documentação

As rotas de customer necessitam de autenticação.

### POST `/auth/login`
  Faz o login do usuário que foi passado, se existir no banco de dados.
   ```json
    {
      "username": "desafiosharenergy",
      "password": "sh@r3n3rgy"
    }
  ```
### POST `/auth/register`
  Realiza o cadastro dos dados do usuário.
  ```json
    {
      "username": "desafiosharenergy",
      "email": "desafiosharenergy@sharenergy.com",
      "password": "sh@r3n3rgy"
    }
  ```
### POST `/customer`
  Cadastra o cliente com os dados passados no formulário.
  ```json
    {
      "name": "desafiosharenergy",
      "email": "desafiosharenergy@sharenergy.com",
      "phone": "21912341234",
      "address": "Endereço",
      "cpf": "12345678901"
    }
  ```
### GET `/customer`
  Retorna todos os clientes cadastrados no banco de dados.

### DELETE `/customers/:id`
  Deleta um cliente a partir do seu id.

### PATCH `/customers/:id`
  Atualiza o customer com os novos dados a partir do seu id.
  
  ```json
    {
      "name": "desafiosharenergy",
      "email": "desafiosharenergy@sharenergy.com",
      "phone": "21912341234",
      "address": "Endereço",
      "cpf": "12345678901"
    }
  ```


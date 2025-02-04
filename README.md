# CRUD de Usuários com Express e MongoDB

Este projeto é uma API REST dedicada ao gerenciamento de usuários, desenvolvida utilizando Node.js como tecnologia principal, o framework Express para a criação de rotas e a manipulação de requisições, além do banco de dados MongoDB para o armazenamento de informações. Ele oferece uma solução eficiente e escalável para operações relacionadas a usuários, incluindo criação, leitura, atualização e exclusão (CRUD).

## 📋 Funcionalidades

- **Listar usuários**: Retorna todos os usuários cadastrados no banco de dados.
- **Cadastrar usuários**: Permite adicionar novos usuários.
- **Atualizar usuários**: Atualiza informações de um usuário existente.
- **Excluir usuários**: Remove um usuário do banco de dados.

## 🛠️ Tecnologias Utilizadas

- [Node.js](https://nodejs.org/)
- [Express](https://expressjs.com/)
- [MongoDB](https://www.mongodb.com/)
- [Mongoose](https://mongoosejs.com/)

## 🚀 Como executar o projeto

### Pré-requisitos

- Node.js instalado
- MongoDB configurado (ou uma conexão com MongoDB Atlas)

### Instalação

1. Clone o repositório:

   ```bash
   git clone https://github.com/pauloricardors/API_de_Usuarios.git

   ```

2. Instale as depêndencias

   ```bash
    npm install
   ```

3. Configure a string de conexão do MongoDB no código: Atualize o seguinte trecho no arquivo principal para usar suas credenciais:

   ```bash
   mongoose.connect('mongodb+srv://<usuário>:<senha>@<cluster>.mongodb.net/?retryWrites=true&w=majority');
   ```

4. Inicie o servidor:

   ```bash
   npm run dev
   ```

5. A API estará disponível em http://localhost:3000.

## 📝 Rotas da API

GET /
Retorna todos os usuários cadastrados.

Exemplo de resposta:

````bash
    [
    {
    "_id": "618d1f1e3d1f1f1f1f1f1f1f",
    "nome": "João",
    "sobrenome": "Silva",
    "sexo": "Masculino",
    "idade": 25,
    "cor_pele": "Parda",
    "email": "joao.silva@example.com",
    "senha": "123456"
    }
    ]

    ```
````
## 📄 Licença

- MIT License
- Este projeto é de uso livre e pode ser modificado ou integrado em outros projetos.
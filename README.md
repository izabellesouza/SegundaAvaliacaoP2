# Projeto de Avaliação - Sistema de Mensagens

Este projeto foi desenvolvido como parte da avaliação da disciplina de TECNOLOGIA PARA FRONT-END COM LÓGICA IMPERATIVA. O professor forneceu a estrutura inicial do projeto (HTML e CSS), e coube a mim complementar com funcionalidades em JavaScript, seguindo os requisitos propostos.

---

## 📋 Funcionalidades Implementadas

### 1. Envio de Mensagens (página contato.html)

- Foi criado um script para capturar os dados do formulário de contato (nome, e-mail e mensagem).
- Esses dados são organizados em um objeto e enviados para a API por meio da função `inserirMensagem(mensagem)`, já definida no arquivo `api.js`.

### 2. Login do Administrador (página admin.html)

- Foi criada uma nova página chamada `admin.html`, com campos de e-mail e senha.
- O login é validado usando a função `validarUsuario(objLoginSenha)` também presente no arquivo `api.js`.
- Caso o login esteja correto (`email: admin@admin.com`, `senha: 1234`), o usuário é redirecionado para a página `mensagens.html`.
- Se o login estiver incorreto, é exibida uma mensagem informando que os dados estão inválidos.

### 3. Visualização das Mensagens (página mensagens.html)

- A página `mensagens.html` foi criada para exibir todas as mensagens recebidas.
- Utiliza a função `obterMensagens()` da API, que retorna um array com todas as mensagens.
- A tabela com os dados é criada dinamicamente, linha por linha, a partir das informações recebidas.


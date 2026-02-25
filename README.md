# 🚀 Minha Primeira API em PHP

Esta foi a **primeira API que desenvolvi em PHP**, criada em **2019**, durante o curso de **Desenvolvedor de Sistemas**.

O principal objetivo do projeto foi colocar em prática os conhecimentos adquiridos em sala de aula e entender, na prática, como funciona a comunicação entre cliente e servidor.

Durante o desenvolvimento, trabalhei conceitos como:

- Desenvolvimento backend
- Requisições HTTP
- Manipulação de JSON
- Integração com banco de dados MySQL
- Autenticação básica
- Estruturação de rotas com `switch case`

O projeto foi construído utilizando **PHP puro**, com foco total em aprendizado e compreensão da base da linguagem, sem utilização de frameworks.

---

# 📌 Sobre a API

A API funciona através de requisições `POST` e utiliza a **query string da URL** para definir qual ação será executada.

Exemplo:
api.php?login    ->  Logar Usuario 
api.php?cadastro ->  Cadastrar User
api.php?CRpost   ->  Criar Post 
api.php?feed     ->  Mostrar feed


Todos os dados são enviados em formato **JSON**, e todas as respostas também são retornadas em **JSON**, mantendo um padrão simples de comunicação.

---

# 🛠 Tecnologias Utilizadas

- PHP (puro)
- MySQL
- JSON
- HTTP (método POST)
- MySQLi

---

# 🔐 Sistema de Validação

Para controle básico de acesso, a API utiliza:

- Uma chave de verificação chamada `WC`, enviada nas requisições
- Um token de autenticação gerado dinamicamente com base nos dados do usuário

A geração do token é feita utilizando:

```php
md5($key . $nome . $email);

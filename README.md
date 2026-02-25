# 🚀 Minha Primeira API em PHP

Esta foi a **primeira API que desenvolvi em PHP**, criada com o objetivo principal de aprender mais sobre:

- Desenvolvimento backend
- Requisições HTTP
- Manipulação de JSON
- Integração com banco de dados MySQL
- Autenticação básica
- Estruturação de rotas

O projeto foi feito utilizando **PHP puro**, como forma de aprendizado prático.

---

# 📌 Sobre a API

A API funciona através de requisições `POST` e utiliza a **query string da URL** para definir qual ação será executada.

Todos os dados são enviados em formato **JSON** e as respostas também são retornadas em **JSON**.
---

# 🔐 Sistema de Validação

A API utiliza:

- Uma chave de verificação chamada `WC`
- Um token de autenticação gerado com:

```php
md5($key . $nome . $email);

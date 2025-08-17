📌 FórumHub
🔎 Sobre o Projeto

Este repositório contém o FórumHub, uma aplicação desenvolvida como parte do projeto final do curso de Back-End Alura + Oracle Next Education.

A proposta é criar um fórum voltado para estudantes de programação, onde usuários podem:

Criar tópicos com dúvidas ou pedidos de ajuda.

Responder perguntas abertas por outros membros.

Encerrar tópicos quando a questão for solucionada.

Todos os dados são armazenados em um banco de dados local e protegidos com autenticação e autorização via JWT, garantindo a segurança das interações.

⚙️ Como funciona

Iniciando a aplicação

O projeto é construído com Spring Boot.

Para testar as rotas, pode-se utilizar ferramentas como Insomnia, Postman ou a interface gerada pelo Swagger.

Cadastro e autenticação

O usuário deve se registrar informando:

Nome

Login (valor único)

Senha

Após o cadastro, é necessário realizar o login para receber um token JWT com validade de 2 horas.

Esse token deve ser enviado no header de todas as requisições autenticadas.

Funcionalidades principais

Criar tópicos: título, curso e mensagem.

Responder tópicos: apenas mensagem.

Listar tópicos: visualização de abertos e encerrados.

Editar conteúdos: permitido apenas para o autor do tópico ou da resposta.

Encerrar tópicos: somente o autor pode finalizar, bloqueando novas interações.

🗄️ Estrutura do Banco de Dados

O sistema utiliza MySQL como banco relacional.

As migrações são gerenciadas via Flyway.

🔐 Segurança

Autenticação com JWT.

Controle de permissões para impedir que usuários alterem conteúdos que não sejam seus.

🚀 Tecnologias utilizadas

Java 17+

Spring Boot 3+

Spring Security

Spring Data JPA

Flyway Migration

MySQL

Lombok
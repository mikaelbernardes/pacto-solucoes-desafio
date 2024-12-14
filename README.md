# Desafio Técnico - Pacto Soluções
Este repositório contém o teste técnico para a vaga de Desenvolvedor Full Stack Pleno na Pacto Soluções. O objetivo do desafio é criar uma aplicação web para recrutamento interno, com usuários Candidatos e Recrutadores (usuários Administradores). O projeto foi desenvolvido utilizando Java e Spring Boot no backend, Angular no frontend e PostgreSQL como banco de dados relacional.

## Como rodar com Docker
Instale o Docker e o Docker Compose se ainda não tiver. Você pode encontrar os passos de instalação na documentação oficial do Docker.

Após a instalação, clone este repositório com o comando:

```bash
git clone https://github.com/mikaelbernardes/pacto-solucoes-desafio.git
```
Navegue até a pasta do projeto:

```bash
cd pacto-solucoes
```

Construa a aplicação Docker com o comando:

```bash
docker-compose build
```

Após a construção, inicie os containers:

```bash
docker-compose up
```

Acesse a aplicação:

Frontend: [http://localhost:4200/login](http://localhost:4200/login)
Backend: [http://localhost:8080](http://localhost:8080)
Para acessar todos os endpoints do backend, use o Swagger: [http://localhost:8080/swagger/swagger-ui/index.html#/](http://localhost:8080/swagger/swagger-ui/index.html#/)

## Funcionalidades Requisitadas
1. Autenticação
  * Implementada com Spring Security e JWT, garantindo acesso seguro a rotas restritas.
    
2. Cadastro de Vagas e Candidatura
  * Usuários Administradores (Recrutadores) podem cadastrar vagas.
  * Usuários Candidatos podem se inscrever nas vagas, com a restrição de se candidatar apenas uma vez a cada vaga.
  * Os Recrutadores podem visualizar a lista de candidatos inscritos nas vagas que publicaram.

3. Envio de Notificações
  * Implementação de notificações para avisar tanto os candidatos quanto os recrutadores sobre a candidatura realizada. Não foi utilizado serviço de e-mail nem WebSocket.
    
4. Painel do Candidato e Avaliação de Candidatos
  * Esta funcionalidade não foi implementada devido ao tempo limitado para a realização do desafio.

### Diferenciais

  * Responsividade nas páginas, adaptando-se ao tamanho da tela.
  * Disponibilização de uma versão dockerizada para facilitar a execução do projeto.
  * Utilização de boas práticas de usabilidade, como toasts e navegação fluída.
  * A implementação de testes de código não foi realizada devido ao tempo restrito. Idealmente, a abordagem TDD seria adotada para as funcionalidades implementadas.]
### Considerações Finais
Embora não tenha tido quatro dias completos para trabalhar no projeto devido ao meu emprego atual, me dediquei ao máximo, realizando o trabalho principalmente à noite. Você pode verificar o histórico de commits tanto do frontend quanto do backend para acompanhar a evolução do projeto. Espero de coração que gostem do resultado e, caso tenham dúvidas ou queiram discutir algum ponto, estou à disposição para contato.

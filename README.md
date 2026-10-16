# Sistema de Gerenciamento de Salão de Beleza

## 1. Sobre o projeto

O Sistema de Gerenciamento de Salão de Beleza é uma aplicação web desenvolvida para facilitar a organização e o gerenciamento das informações de um salão. O sistema permite cadastrar clientes, armazenar informações capilares e registrar os atendimentos realizados, mantendo os dados organizados e acessíveis.

## 2. Funcionalidades

- **Login e logout:** controle de acesso ao sistema por meio de autenticação.
- **Cadastro de clientes:** registro, consulta, edição e exclusão de clientes.
- **Busca de clientes:** pesquisa de clientes pelo nome.
- **Fichas capilares:** armazenamento de informações sobre o cabelo, como tipo, comprimento, cor atual, procedimentos químicos e alergias.
- **Registro de atendimentos:** cadastro dos serviços realizados, incluindo data, descrição, profissional responsável e valor.
- **Histórico de atendimentos:** consulta aos serviços registrados para cada cliente.
- **Controle de sessão:** encerramento automático após 30 minutos de inatividade.

## 3. Tecnologias utilizadas

- **PHP:** desenvolvimento da lógica e do processamento das informações.
- **MySQL:** armazenamento e gerenciamento dos dados.
- **MySQLi:** conexão entre a aplicação e o banco de dados.
- **HTML:** estruturação das páginas.
- **CSS:** estilização e organização visual da interface.
- **XAMPP:** ambiente de desenvolvimento local.

## 4. Estrutura do projeto

```text
salao/
├── atendimento.php
├── clientes.php
├── config.php
├── deletar_cliente.php
├── deletar_ficha.php
├── editar_atendimento.php
├── editar_cliente.php
├── editar_ficha.php
├── fichas.php
├── historico.php
├── index.php
├── login.php
├── logout.php
├── opcoes.php
├── principal.php
├── salao_db.sql
└── css/
    └── style.css
```

## 5. Banco de dados

O sistema utiliza o banco de dados `salao_db`, composto por quatro tabelas principais:

| Tabela | Descrição |
|---|---|
| `usuarios` | Armazena os dados dos usuários autorizados. |
| `clientes` | Armazena as informações cadastrais dos clientes. |
| `fichas` | Guarda as informações capilares dos clientes. |
| `atendimentos` | Registra os serviços realizados. |

As tabelas são relacionadas para permitir que as fichas capilares e os atendimentos sejam associados aos respectivos clientes.

## 6. Segurança

O sistema possui mecanismos de segurança, como autenticação por sessão, verificação de senhas e utilização de consultas preparadas em operações de banco de dados. Também implementa criptografia para o armazenamento de CPF.

Antes de disponibilizar a aplicação publicamente, recomenda-se revisar as credenciais, proteger as chaves de criptografia, utilizar HTTPS e reforçar a proteção dos dados pessoais.

## 7. Objetivo acadêmico

O projeto tem como objetivo aplicar conhecimentos de desenvolvimento web, integração com banco de dados, operações CRUD (criação, consulta, atualização e exclusão), autenticação de usuários e organização de informações em um sistema informatizado.

## 8. Autoria

Projeto desenvolvido para fins educacionais.

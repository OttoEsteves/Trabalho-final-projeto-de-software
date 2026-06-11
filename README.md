
---

# 🪙 Gestão Hospitalar
👨‍🎓

> [!NOTE]
> Plataforma web para reconhecimento do mérito acadêmico por meio de uma moeda virtual, permitindo que professores recompensem alunos e que alunos troquem moedas por vantagens oferecidas por empresas parceiras.

<table>
  <tr>
    <td width="800px">
      <div align="justify">
        O <b>Sistema de Moeda Estudantil</b> foi desenvolvido como parte da <b>Release 1</b> de um projeto acadêmico de Engenharia de Software. A aplicação tem como objetivo criar um ambiente digital capaz de estimular o reconhecimento do mérito estudantil por meio de uma moeda virtual. Professores recebem moedas periodicamente e podem distribuí-las aos alunos como forma de reconhecimento por participação, desempenho, comportamento e engajamento acadêmico. Os alunos, por sua vez, podem acompanhar seu saldo, consultar extratos e trocar moedas por vantagens cadastradas por empresas parceiras. O sistema contempla autenticação, controle de saldo, registro de transações, resgate de benefícios, geração de cupons e notificações por e-mail, seguindo uma arquitetura baseada em <b>MVC</b> e mantendo alinhamento com os modelos UML produzidos ao longo das sprints.
      </div>
    </td>
    <td>
      <div align="center">
        <img src="https://img.icons8.com/fluency/240/coins.png" alt="Logo do Sistema de Moeda Estudantil" width="130px"/>
      </div>
    </td>
  </tr> 
</table>

---

## 🚧 Status do Projeto

![Status](https://img.shields.io/badge/Status-Concluído-success?style=for-the-badge)
![Release](https://img.shields.io/badge/Release-1.0.0-blue?style=for-the-badge)
![PUC Minas](https://img.shields.io/badge/PUC%20Minas-Engenharia%20de%20Software-007ec6?style=for-the-badge)
![MVC](https://img.shields.io/badge/Arquitetura-MVC-purple?style=for-the-badge)

![React](https://img.shields.io/badge/React-18+-007ec6?style=for-the-badge&logo=react&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-5+-007ec6?style=for-the-badge&logo=typescript&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-5+-007ec6?style=for-the-badge&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3+-007ec6?style=for-the-badge&logo=tailwindcss&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-8-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET_Core-Web_API-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Compose-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-OpenAPI-85EA2D?style=for-the-badge&logo=swagger&logoColor=black)

---

## 📚 Índice

- [Links Úteis](#-links-úteis)
- [Sobre o Projeto](#-sobre-o-projeto)
- [Funcionalidades Principais](#-funcionalidades-principais)
- [Regras de Negócio](#-regras-de-negócio)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Arquitetura](#-arquitetura)
  - [Visão Geral](#visão-geral)
  - [Camadas da Aplicação](#camadas-da-aplicação)
  - [Modelo de Domínio](#modelo-de-domínio)
  - [Fluxos Principais](#fluxos-principais)
- [Instalação e Execução](#-instalação-e-execução)
  - [Pré-requisitos](#pré-requisitos)
  - [Variáveis de Ambiente](#-variáveis-de-ambiente)
  - [Instalação de Dependências](#-instalação-de-dependências)
  - [Inicialização do Banco de Dados](#-inicialização-do-banco-de-dados-postgresql)
  - [Como Executar a Aplicação](#-como-executar-a-aplicação)
- [Endpoints da API](#-endpoints-da-api)
- [Estrutura de Pastas](#-estrutura-de-pastas)
- [Demonstração](#-demonstração)
- [Testes](#-testes)
- [Modelagem UML](#-modelagem-uml)
- [Documentações Utilizadas](#-documentações-utilizadas)
- [Autores](#-autores)
- [Contribuição](#-contribuição)
- [Licença](#-licença)

---

## 🔗 Links Úteis

* 🌐 **Aplicação Web:** [Acesse a aplicação](<link-da-demo-web>)
  > 💻 Interface web do Sistema de Moeda Estudantil.

* 📖 **Documentação da API:** [Swagger / OpenAPI](<link-do-swagger>)
  > 📚 Documentação dos endpoints, contratos de requisição e respostas da API.

* 🗂️ **Repositório GitHub:** [Acesse o repositório](<link-do-repositorio>)
  > 🧾 Código-fonte, modelos UML, versionamento das sprints e documentação técnica.

* 🧩 **Modelos UML:** [Acesse os diagramas](<link-dos-modelos>)
  > 📐 Diagramas de classes, arquitetura, casos de uso e fluxos principais do sistema.

---

## 📝 Sobre o Projeto

O **Sistema de Moeda Estudantil** é uma aplicação web desenvolvida para apoiar o reconhecimento de mérito dentro do ambiente acadêmico. A proposta é permitir que professores recompensem alunos por atitudes positivas, bom desempenho, participação em aula, colaboração com colegas e outros comportamentos relevantes para a formação acadêmica.

A moeda virtual funciona como um mecanismo simbólico e prático de incentivo. Professores recebem um saldo semestral de moedas e podem distribuí-las aos alunos mediante uma justificativa obrigatória. Os alunos acumulam moedas em suas contas e podem trocá-las por vantagens cadastradas por empresas parceiras, como descontos, produtos ou benefícios acadêmicos.

O projeto foi desenvolvido com foco em:

- Reconhecimento estudantil de forma objetiva e rastreável;
- Incentivo ao engajamento acadêmico;
- Integração entre alunos, professores, instituições e empresas parceiras;
- Controle seguro de saldo e transações;
- Transparência por meio de extratos;
- Emissão de cupons para resgate presencial;
- Notificações por e-mail para os principais eventos do sistema.

A aplicação foi construída seguindo a arquitetura **MVC**, com separação entre interface, regras de negócio, persistência e comunicação com serviços externos. O backend foi desenvolvido em **.NET 8**, o frontend em **React com TypeScript**, e o banco de dados utilizado foi o **PostgreSQL**.

---

## ✨ Funcionalidades Principais

### 👨‍🎓 Aluno

- 🔐 Cadastro e autenticação no sistema;
- 🏫 Seleção de instituição de ensino pré-cadastrada;
- 📚 Cadastro de curso, endereço e dados pessoais;
- 🪙 Recebimento de moedas enviadas por professores;
- 📩 Notificação por e-mail ao receber moedas;
- 📊 Consulta de saldo atual;
- 📜 Consulta de extrato de recebimentos e resgates;
- 🎁 Visualização de vantagens disponíveis;
- 🧾 Resgate de vantagens com geração de cupom;
- 📧 Recebimento de e-mail com código de resgate.

### 👨‍🏫 Professor

- 🔐 Autenticação no sistema;
- 🏫 Vínculo com instituição de ensino;
- 🏢 Vínculo com departamento;
- 🪙 Recebimento de saldo semestral de moedas;
- ➕ Acúmulo de moedas não utilizadas entre semestres;
- 🎯 Envio de moedas para alunos;
- 📝 Registro obrigatório do motivo do reconhecimento;
- 📊 Consulta de saldo disponível;
- 📜 Consulta de extrato de envios realizados.

### 🏢 Empresa Parceira

- 🔐 Cadastro e autenticação no sistema;
- 🎁 Cadastro de vantagens oferecidas aos alunos;
- 🖼️ Inclusão de descrição e foto do produto ou benefício;
- 🪙 Definição do custo da vantagem em moedas;
- 📧 Recebimento de e-mail quando uma vantagem é resgatada;
- 🔎 Conferência do código de cupom gerado pelo sistema.

### ⚙️ Administração e Operação

- 🏫 Instituições de ensino pré-cadastradas;
- 👨‍🏫 Professores pré-cadastrados a partir da lista enviada pela instituição;
- 🔑 Controle de acesso por perfil;
- 📜 Registro de transações;
- 🧾 Geração de cupons únicos;
- 📬 Serviço de envio de e-mails;
- 🧪 Documentação e testes de API com Swagger e Postman.

---

## 📌 Regras de Negócio

As regras de negócio implementadas garantem que o sistema funcione de forma consistente, segura e alinhada à proposta da Release 1.

| Código | Regra |
| :---: | :--- |
| RN01 | Alunos devem realizar cadastro informando nome, e-mail, CPF, RG, endereço, instituição de ensino e curso. |
| RN02 | Instituições participantes devem estar previamente cadastradas no sistema. |
| RN03 | Professores devem estar previamente cadastrados e vinculados a uma instituição e departamento. |
| RN04 | Cada professor recebe 1.000 moedas a cada semestre. |
| RN05 | O saldo de moedas do professor é acumulativo entre semestres. |
| RN06 | Professores só podem enviar moedas se possuírem saldo suficiente. |
| RN07 | Todo envio de moedas deve conter uma mensagem obrigatória com o motivo do reconhecimento. |
| RN08 | O aluno deve ser notificado por e-mail ao receber moedas. |
| RN09 | Alunos e professores podem consultar extrato e saldo da conta. |
| RN10 | Empresas parceiras podem cadastrar vantagens com descrição, foto e custo em moedas. |
| RN11 | Alunos só podem resgatar vantagens se tiverem saldo suficiente. |
| RN12 | Ao resgatar uma vantagem, o valor deve ser descontado do saldo do aluno. |
| RN13 | Cada resgate deve gerar um código único de cupom. |
| RN14 | O aluno deve receber um e-mail com o cupom de resgate. |
| RN15 | A empresa parceira deve receber um e-mail com o código para conferência. |
| RN16 | Todos os fluxos principais exigem autenticação. |

---

## 🛠 Tecnologias Utilizadas

As tecnologias foram escolhidas considerando produtividade, aderência à arquitetura MVC, facilidade de manutenção, compatibilidade com aplicações web modernas e adequação ao contexto acadêmico da disciplina.

### 💻 Front-end

* **Biblioteca principal:** React 18+
* **Linguagem:** TypeScript
* **Build Tool:** Vite
* **Estilização:** Tailwind CSS
* **Componentes de UI:** shadcn/ui
* **Roteamento:** React Router
* **Requisições HTTP:** Axios
* **Gerenciamento de estado:** Context API e hooks customizados
* **Validação de formulários:** React Hook Form / Zod
* **Ícones:** Lucide React
* **Padrão visual:** Interface responsiva baseada em dashboards, cards, tabelas e formulários

### 🖥️ Back-end

* **Linguagem/Runtime:** C# com .NET 8
* **Framework:** ASP.NET Core Web API
* **Arquitetura:** MVC com Controllers, Services, Repositories e Models
* **ORM:** Entity Framework Core
* **Autenticação:** JWT Bearer Token
* **Criptografia de senha:** BCrypt
* **Documentação da API:** Swagger / OpenAPI
* **Mapeamento de dados:** DTOs para entrada e saída de dados
* **Validações:** Data Annotations e validações em camada de serviço
* **Serviço de e-mail:** SMTP configurável por variáveis de ambiente

### 🗄️ Banco de Dados

* **SGBD:** PostgreSQL 16+
* **Migrations:** Entity Framework Core Migrations
* **Modelo:** Relacional
* **Principais tabelas:** Usuários, Alunos, Professores, Empresas Parceiras, Instituições, Cursos, Departamentos, Contas, Transações, Vantagens, Resgates e Cupons

### ⚙️ Infraestrutura & DevOps

* **Versionamento:** Git e GitHub
* **Containerização:** Docker e Docker Compose
* **Testes de API:** Postman
* **Documentação de API:** Swagger
* **Ambiente local:** Frontend, backend e banco executados separadamente ou via Docker Compose
* **Organização acadêmica:** Versionamento por sprints, com modelos UML e código final no repositório

---

## 🏗 Arquitetura

### Visão Geral

O sistema foi desenvolvido utilizando a arquitetura **MVC**, separando responsabilidades entre interface, controle de requisições, regras de negócio e persistência de dados.

```mermaid
flowchart LR
    User[Usuário Web] --> Frontend[Frontend React + TypeScript]
    Frontend --> API[ASP.NET Core Web API]
    API --> Controllers[Controllers]
    Controllers --> Services[Services]
    Services --> Repositories[Repositories]
    Repositories --> DB[(PostgreSQL)]
    Services --> Email[Serviço de E-mail SMTP]

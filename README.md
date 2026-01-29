# LedgerLy - Sistema de Core Banking Simplificado

!([https://img.shields.io/badge/Spring_Boot-3.2-green](https://www.google.com/search?q=https://img.shields.io/badge/Spring_Boot-3.2-green))
!([https://img.shields.io/badge/PostgreSQL-16-blue](https://www.google.com/search?q=https://img.shields.io/badge/PostgreSQL-16-blue))

## 📖 Sobre o Projeto

O **LedgerLy** é um motor de transações financeiras (Core Banking) focado em integridade de dados e concorrência. Diferente de gerenciadores de despesas comuns, este sistema implementa um **Ledger (Livro-Razão)** baseado em contabilidade de partida dobrada (*Double-Entry Bookkeeping*) para garantir que o dinheiro nunca seja criado ou destruído, apenas movimentado.

Este projeto foi desenvolvido para simular desafios reais de Fintechs, como:

* **Race Conditions:** Tratamento de concorrência em transferências simultâneas.
* **Idempotência:** Garantia de processamento único em redes instáveis.
* **Auditabilidade:** Rastreio completo de movimentações financeiras.

## 🚀 Tecnologias e Arquitetura

* **Linguagem:** Java 21
* **Framework:** Spring Boot 4
* **Banco de Dados:** PostgreSQL 16
* **Segurança:** Spring Security 6 + JWT (Stateless)
* **Infraestrutura:** Docker & Docker Compose
* **Testes:** JUnit 5, Mockito & Testcontainers

### Decisões Arquiteturais

O projeto segue uma arquitetura de **Monólito Modular** com **Clean Architecture** (Hexagonal). O domínio financeiro é isolado de frameworks e detalhes de infraestrutura.

* **Módulo Wallet:** Gerencia contas, saldos e histórico.
* **Módulo Auth:** Gerencia identidade e tokens JWT.

## 🛠️ Como Executar

### Pré-requisitos

* Docker & Docker Compose
* Java 21 (Opcional, caso rode via Docker)

### Passo a Passo

1. Clone o repositório:bash
git clone [https://github.com/SEU_USUARIO/ledgerly.git](https://www.google.com/search?q=https://github.com/SEU_USUARIO/ledgerly.git)
```

```


2. Suba a infraestrutura (Banco de Dados):
```bash
docker-compose up -d

```


3. Execute a aplicação:
```bash

```



./mvnw spring-boot:run

```

```

# 📊Sistema-Gestão-Empresarial
## Resumo:
Sistema web para gestão de vendas, estoque e clientes, desenvolvido como projeto integrador do curso de Análise e Desenvolvimento de Sistemas.

### 🎯 Finalidade do Projeto
Este projeto tem como objetivo desenvolver um sistema de gestão empresarial (ERP) capaz de centralizar e otimizar os principais processos administrativos de uma empresa. A plataforma permite o controle integrado de pedidos, clientes, pagamentos e relatórios, proporcionando mais eficiência, organização e tomada de decisão baseada em dados.

A proposta é oferecer uma solução prática e acessível para digitalizar operações que muitas vezes ainda são feitas de forma manual ou descentralizada.

---

### 👥 Público-Alvo
O sistema é voltado para:

- 🏬 Pequenas e médias empresas (PMEs)  
- 👨‍💼 Empreendedores e gestores  
- 🧾 Setores administrativos e financeiros  
- 📦 Negócios que precisam gerenciar pedidos e operações  

---

### 🚀 Principais Benefícios
- Centralização das informações em um único sistema  
- Redução de erros operacionais  
- Automatização de processos (pedidos, pagamentos, relatórios)  
- Melhor controle financeiro e administrativo  
- Apoio na tomada de decisões estratégicas  

---

### 💡 Visão Geral
A plataforma foi pensada para ser intuitiva, eficiente e escalável, podendo ser adaptada para diferentes tipos de negócio. Além disso, busca aplicar boas práticas de desenvolvimento, organização de código e arquitetura de sistemas, servindo também como projeto de aprendizado e portfólio.

## Infraestrutura Técnica

### 🖥️ Backend

![Java](https://img.shields.io/badge/Java-007396?logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?logo=springboot&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?logo=go&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?logo=node.js&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?logo=nestjs&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?logo=apachekafka&logoColor=white)
![gRPC](https://img.shields.io/badge/gRPC-009DFF?logo=grpc&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?logo=postgresql&logoColor=white)
![Cassandra](https://img.shields.io/badge/Cassandra-1287B1?logo=apachecassandra&logoColor=white)
![DynamoDB](https://img.shields.io/badge/DynamoDB-4053D6?logo=amazondynamodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-D92C27?logo=redis&logoColor=white)
![OpenSearch](https://img.shields.io/badge/OpenSearch-1D72F3?logo=opensearch&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?logo=kubernetes&logoColor=white)
![API Gateway](https://img.shields.io/badge/API%20Gateway-FF4F8B?logo=amazonapigateway&logoColor=white)
![KMS](https://img.shields.io/badge/KMS-FF9900?logo=amazonaws&logoColor=white)

### 🌐 Frontend Web

![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?logo=next.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-06B6D4?logo=tailwindcss&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?logo=vite&logoColor=white)

### 📱 Mobile

![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?logo=kotlin&logoColor=white)
![Swift](https://img.shields.io/badge/Swift-F05138?logo=swift&logoColor=white)

### 🗄️ Banco de Dados

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?logo=postgresql&logoColor=white)
![DynamoDB](https://img.shields.io/badge/DynamoDB-4053D6?logo=amazondynamodb&logoColor=white)
![Cassandra](https://img.shields.io/badge/Cassandra-1287B1?logo=apachecassandra&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-D92C27?logo=redis&logoColor=white)
![Elasticsearch](https://img.shields.io/badge/Elasticsearch-005571?logo=elasticsearch&logoColor=white)
![OpenSearch](https://img.shields.io/badge/OpenSearch-1D72F3?logo=opensearch&logoColor=white)

## Diagrama de Sequência 
```mermaid
sequenceDiagram
    participant U as Usuário (Funcionário/Admin)
    participant F as Frontend (Sistema Web)
    participant B as Backend (Servidor)
    participant DB as Banco de Dados
    participant API as API Externa (Pagamentos/Serviços)

    U->>F: Acessa o sistema
    F->>U: Solicita login

    U->>F: Envia usuário e senha
    F->>B: Requisição de autenticação

    B->>DB: Verifica credenciais
    DB-->>B: Retorna resultado

    B-->>F: Autenticação OK
    F-->>U: Exibe dashboard

    U->>F: Solicita cadastro de pedido
    F->>B: Envia dados do pedido

    B->>DB: Salva pedido
    DB-->>B: Confirma salvamento

    B->>API: Processa pagamento
    API-->>B: Retorna status do pagamento

    B->>DB: Atualiza status do pedido
    DB-->>B: Confirma atualização

    B-->>F: Envia confirmação
    F-->>U: Exibe pedido confirmado

    U->>F: Solicita relatório
    F->>B: Requisição de dados

    B->>DB: Busca dados financeiros
    DB-->>B: Retorna dados

    B-->>F: Envia relatório
    F-->>U: Exibe relatório
```
## Link
[Diagrama de Estado](https://raw.githubusercontent.com/LeonardoMartins08/sistema-gestao-empresarial/refs/heads/main/Engenharia%20de%20Software/diagrama-estado.md)

[Diagrama de sequência](https://raw.githubusercontent.com/LeonardoMartins08/sistema-gestao-empresarial/refs/heads/main/Engenharia%20de%20Software/Diagrama%20de%20Sequ%C3%AAncia.png)

[Caso de uso](github.com/LeonardoMartins08/sistema-gestao-empresarial/blob/main/Engenharia%20de%20Software/Caso%20de%20Uso.png?raw=true)

[Figma](https://www.figma.com/make/uHUuGhyVEp9BeUHooPYxQl/Loja-com-estoque-e-faturamento?p=f&t=ASkgMtrTasQzfoQn-0&fullscreen=1)






## 📌 Integrantes:

- Leonardo Martins
- Enzo Longo Bardo
- Mateus De Freitas Martis
- Diego Favini Giacomo


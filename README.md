# 📊sistema-gestao-empresarial
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


## 📌 Integrantes:

- Leonardo Martins
- Enzo Longo Bardo
- Mateus De Freitas Martis
- Diego Favini Giacomo


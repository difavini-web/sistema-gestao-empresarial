# Diagrama de Estados – App de Gestão Empresarial

```mermaid
stateDiagram-v2

[*] --> Login

Login --> Validando : Inserir credenciais
Validando --> Dashboard : Credenciais válidas
Validando --> Login : Credenciais inválidas

Dashboard --> CadastroProdutos
Dashboard --> ControleEstoque
Dashboard --> Vendas
Dashboard --> Relatorios
Dashboard --> Configuracoes
Dashboard --> Logout

CadastroProdutos --> Dashboard : Produto cadastrado

ControleEstoque --> Entrada
ControleEstoque --> Saida

Entrada --> ControleEstoque : Estoque atualizado

Saida --> VerificarEstoque
VerificarEstoque --> ControleEstoque : Estoque insuficiente
VerificarEstoque --> ControleEstoque : Saída realizada

Vendas --> ProcessandoVenda
ProcessandoVenda --> Vendas : Adicionar itens
ProcessandoVenda --> Dashboard : Venda finalizada

Relatorios --> Dashboard : Relatório gerado

Configuracoes --> Dashboard : Configurações salvas

Logout --> [*]

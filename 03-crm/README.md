# CRM Comercial — Portfolio Demo

Versão pública de demonstração do CRM originalmente desenvolvido com **Google Apps Script + Google Sheets**.

> **Importante:** a interface deste demo é baseada no arquivo frontend original do projeto. A proposta não é reconstruir ou simplificar o CRM, mas preservar sua estrutura, telas, componentes, navegação e comportamentos e substituir apenas a identidade da empresa e a fonte de dados indisponível por dados fictícios.

## O que foi alterado para o portfólio

- Identidade da empresa real substituída por uma identidade fictícia (**Nexa CRM**).
- Logos, URLs, e-mails e referências identificáveis da empresa original removidos/substituídos.
- Dados operacionais substituídos por registros fictícios.
- Chamadas ao backend Google Apps Script foram mantidas conceitualmente, mas recebem um **adaptador local de demonstração** para que a aplicação funcione sem a antiga planilha.
- Consulta de CNPJ, no ambiente público, utiliza dados fictícios de demonstração em vez de consultar fontes reais.

Não foram criadas telas de negócio novas para esta versão e a interface original não foi reduzida a um dashboard simplificado.

## Funcionalidades preservadas

A interface original contempla, entre outros elementos:

- Login e sessão
- Dashboard comercial
- Dashboard de clientes e negócios
- Dashboard gerencial de representantes
- KPIs e indicadores
- Funil de vendas
- Saúde do pipeline
- Propostas comerciais
- Financeiro de propostas
- Prioridades gerenciais
- Insights da carteira
- Ranking e disciplina operacional dos representantes
- Pipeline agrupado por status
- Busca e filtros
- Clientes
- Representantes
- Propostas
- SysLog / trilha de auditoria
- Perfil e alteração de senha
- Cadastro e edição de clientes
- Cadastro e edição de representantes
- Cadastro e edição de propostas
- Painel lateral de detalhes do cliente
- Visão geral do cliente
- Histórico / timeline de interações
- Tarefas
- Notas
- Próxima ação / follow-up
- Tags / segmentação
- Ações rápidas
- Atalhos de teclado
- Responsividade
- Consulta de CNPJ como fluxo de cadastro

## Arquitetura original

```text
Frontend HTML / CSS / JavaScript
              ↓
     Google Apps Script
              ↓
        Google Sheets
        ├── Representantes
        ├── Clientes
        ├── Propostas
        ├── ClienteDetalhes
        └── SysLog
```

O backend original possui funções para autenticação, representantes, clientes, propostas, detalhes do cliente, auditoria e demais operações da aplicação.

## Arquitetura desta demonstração

```text
Frontend original preservado
              ↓
       Demo Adapter
              ↓
   Dados fictícios locais
        (localStorage)
```

O adaptador reproduz, para fins de demonstração, as respostas esperadas pelas chamadas do frontend. Isso permite apresentar o sistema publicamente sem depender da antiga conta, da antiga planilha ou de uma nova base de dados.

A separação também deixa clara a arquitetura que seria utilizada novamente em produção:

```text
Frontend
   ↓
Data / Backend Adapter
   ↓
Google Apps Script
   ↓
Google Sheets
```

## Dados de demonstração

Todos os nomes, e-mails, telefones, empresas, valores, IDs, registros de auditoria e informações de CNPJ exibidos no demo são fictícios.

## Stack

- Google Apps Script — arquitetura/backend original
- Google Sheets — base operacional original
- HTML5
- CSS3
- JavaScript
- Chart.js
- Lucide Icons
- Google Workspace — ambiente original

## Portfólio

**DevDias Tech Solutions — Soluções Tecnológicas**

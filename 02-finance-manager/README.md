# Finance Manager — Portfolio Demo

Dashboard financeiro criado a partir do conceito do **Gestor Financeiro** desenvolvido originalmente em Google Apps Script.

## O que esta demo demonstra

- Dashboard executivo com KPIs
- Receitas, despesas e resultado
- Contas a receber e valores em atraso
- Fluxo financeiro por período
- Despesas por categoria
- Alertas de compromissos
- Tabela de lançamentos
- Modal para inclusão de lançamento
- Interface responsiva
- Tema visual escuro orientado a aplicações de gestão

## Arquitetura original

O sistema real foi desenvolvido para trabalhar com **Google Apps Script + Google Sheets**: a camada de interface consulta o backend Apps Script, e o backend lê/grava os dados da estrutura de planilhas utilizada pela aplicação.

## Arquitetura desta demo

A base corporativa original não está mais disponível. Por isso, esta versão utiliza um `DataProvider` local com dados fictícios.

A intenção é preservar a ideia arquitetural:

```text
Interface HTML/CSS/JS
        ↓
    DataProvider
        ↓
 ┌──────┴─────────┐
 │                │
Demo             Produção
Mock local       Apps Script
                  ↓
              Google Sheets
```

No código existe um ponto explícito para substituir o provider de demonstração por chamadas `google.script.run` em um eventual ambiente de produção.

Isso permite apresentar a interface e a experiência do sistema sem depender de uma conta ou planilha corporativa.

## Dados

Todos os registros apresentados são fictícios e foram criados exclusivamente para demonstração.

## Stack

- HTML5
- CSS3
- JavaScript
- Google Apps Script — arquitetura de integração original
- Google Sheets — fonte de dados da aplicação original
- Chart.js
- Lucide Icons

## Portfolio

**DevDias Tech Solutions — Soluções Tecnológicas**

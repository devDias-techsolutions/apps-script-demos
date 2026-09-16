# CRM Comercial — Portfolio Demo

Demonstração pública baseada no conceito do CRM originalmente desenvolvido com **Google Apps Script + Google Sheets**.

## Funcionalidades demonstradas

- Dashboard comercial
- Base de clientes
- Leads e oportunidades
- Pipeline por etapa
- Valor potencial do pipeline
- Origem dos leads
- Responsáveis comerciais
- Status de clientes
- Atividade recente
- Cadastro de cliente em modo demo
- Estrutura preparada para auditoria

O backend original possui operações para autenticação, representantes, clientes, propostas e registro de auditoria (`SysLog`). A interface original também consumia funções do Apps Script para carregar e salvar clientes. fileciteturn22file0 fileciteturn24file1 fileciteturn25file0

## Arquitetura

### Projeto original

```text
Web App
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

### Demo pública

```text
HTML / CSS / JavaScript
          ↓
     DataProvider
          ↓
      Mock local
```

A camada `DataProvider` foi criada para deixar clara a separação entre apresentação e fonte de dados. Em uma implantação real, ela pode ser substituída por chamadas ao backend Apps Script (`google.script.run`).

## Dados

Todos os nomes, contatos, valores e registros exibidos são fictícios.

## Stack

- Google Apps Script — arquitetura original
- Google Sheets — base operacional original
- HTML5 / CSS3 / JavaScript
- Lucide Icons
- Interface responsiva

## Portfólio

**DevDias Tech Solutions — Soluções Tecnológicas**

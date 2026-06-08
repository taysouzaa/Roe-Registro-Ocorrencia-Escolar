# ROE — Registro de Ocorrência Escolar

> Sistema web para digitalizar e gerenciar ocorrências escolares, com automação via n8n e integração com Google Sheets e Gmail.

![Status](https://img.shields.io/badge/status-concluído-22c55e)
![Frontend](https://img.shields.io/badge/frontend-HTML%2FCSS%2FJS-1f6feb)
![Automação](https://img.shields.io/badge/automação-n8n-FF6D00)
![License](https://img.shields.io/badge/license-MIT-green)

## Visão do Projeto

O **ROE** é um sistema desenvolvido como projeto de TCC para substituir o registro manual de ocorrências escolares por um fluxo digital completo: o coordenador preenche o formulário web, os dados são salvos no Google Sheets e uma confirmação é enviada automaticamente por e-mail.

### O que o sistema resolve

- Digitaliza o processo de registro de ocorrências, eliminando papéis.
- Automatiza notificações por e-mail para responsáveis e equipe escolar.
- Centraliza dados em planilha Google Sheets para consulta e histórico.

## O Que Foi Desenvolvido

### 1. Formulário Web de Ocorrências
- Interface HTML/CSS/JS para preenchimento de ocorrências.
- Validação client-side antes do envio.
- Envio dos dados para webhook n8n.

### 2. Automação com n8n
- Workflow n8n que recebe os dados do formulário.
- Salva automaticamente no Google Sheets.
- Dispara e-mail de notificação via Gmail API.

### 3. Integrações
- **Google Sheets:** banco de dados da aplicação.
- **Gmail API:** envio de e-mails automáticos.

## Stack Técnica

- **Frontend:** HTML5, CSS3, JavaScript (vanilla)
- **Automação:** n8n (self-hosted ou cloud)
- **Banco de dados:** Google Sheets
- **Notificações:** Gmail API

## Estrutura do Projeto

```text
.
├─ index.html       ← formulário principal
├─ style.css        ← estilos
├─ script.js        ← lógica de envio
├─ docs/            ← workflow n8n e documentação
└─ LICENSE
```

## Como Executar

1. Importe o workflow n8n da pasta `docs/`.
2. Configure as credenciais do Google Sheets e Gmail no n8n.
3. Atualize a URL do webhook em `script.js`.
4. Hospede os arquivos HTML em qualquer servidor estático.

## Página de Apresentação

Acesse: [Registro.roe](https://github.com/taysouzaa/Registro.roe)

## Licença

MIT — veja [LICENSE](./LICENSE)
# R.O.E. – Registro de Ocorrência Escolar

Sistema automatizado para registro, categorização e encaminhamento de ocorrências escolares (disciplinar e pedagógica), integrado com **n8n**, **Google Sheets** e **Gmail API**, permitindo também a emissão de pareceres institucionais.

[![Status](https://img.shields.io/badge/status-ativo-brightgreen)]()
[![n8n](https://img.shields.io/badge/built%20with-n8n-blue)](https://n8n.io)
[![Google Sheets](https://img.shields.io/badge/Google-Sheets-green)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)

**Demonstração online:** [Acesse aqui](https://documento-eight.vercel.app/)

---

## Visão Geral

O **R.O.E. (Registro de Ocorrência Escolar)** é uma solução digital que moderniza o processo de registro de ocorrências em instituições de ensino.  
Ele automatiza o fluxo de comunicação entre professores, coordenação e direção, garantindo agilidade, padronização e segurança no tratamento das informações.

---

## Funcionalidades

- Registro de ocorrências via formulário digital:
  - **Disciplinar** → notificação automática à Direção.  
  - **Pedagógico** → notificação automática à Coordenação.
- Armazenamento estruturado em **Google Sheets**.
- Envio de **e-mails automáticos** via **Gmail API**.
- Registro de pareceres institucionais em planilha separada.
- Autenticação segura via **OAuth2**.
- Fluxo automatizado com **n8n**.

---

## Tecnologias Utilizadas

- **[n8n](https://n8n.io/)** → plataforma de automação de workflows.
- **Google Sheets** → armazenamento dos registros e pareceres.
- **Gmail API** → envio de notificações automáticas.
- **OAuth2** → autenticação segura para APIs do Google.
- **Vercel** → hospedagem da documentação do projeto.

---

## Fluxo do Sistema

1. **Registro da ocorrência**  
   O usuário escolhe o tipo (disciplinar ou pedagógico), informa dados do professor, aluno, categoria e descrição.  

2. **Classificação automática**  
   O fluxo no n8n identifica o tipo da ocorrência e define o setor responsável.  

3. **Armazenamento**  
   Os dados são gravados em uma planilha no Google Sheets, separados por abas/tabelas.  

4. **Notificação**  
   Um e-mail automático é enviado ao setor responsável:  
   - Direção → ocorrências disciplinares.  
   - Coordenação → ocorrências pedagógicas.  

5. **Parecer Institucional**  
   É possível registrar pareceres via formulário, gravados em planilha própria (`Parecer.ROE`).  

---

## Licença

Este projeto é de **uso exclusivo** da autora.  
Todos os direitos reservados © 2025 **Taynara Correia de Souza**.

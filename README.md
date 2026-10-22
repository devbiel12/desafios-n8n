# ⚡ Desafios e Fluxos de Automação n8n

> Repositório destinado ao versionamento, documentação e controle dos desafios e fluxos de automação desenvolvidos no n8n.

## 📌 Sobre o Repositório

Este repositório atua como portfólio e histórico de aprendizado/desenvolvimento em automação de processos utilizando o n8n.

Atualmente, o repositório conta com a documentação completa do projeto de integração do SAP com e-mail e WhatsApp (Uzapi) para notificações de chamados da TI Infra.

## 📁 Conteúdo do Repositório
```
desafios-n8n/
├── README.md
└── Documentacao_Automacao_N8N.md  # Documentação do fluxo de notificações SAP -> E-mail / WhatsApp
```
---

## 🛠️ Desafios Registrados

### 1. [Automação de Notificações de Chamados (SAP / n8n)](./Documentacao_Automacao_N8N.md)
* **Descrição:** Automação via Webhook que recebe dados de ocorrências do SAP para a TI Infra, valida se o status está "ABERTO" e com e-mail válido, e envia alertas simultâneos por E-mail e WhatsApp (Uzapi).
* **Tecnologias/Nós:** n8n (Webhook, Edit Fields, IF, Send Email, HTTP Request), SAP Interno, Uzapi (WhatsApp).
* **Documentação:** Consulte o arquivo automacao_n8n_notificacoes.md para detalhes da arquitetura e regras de negócio.

---

## 🔧 Tecnologias Utilizadas

* [n8n.io](https://n8n.io/) — Ferramenta de automação de workflows
* Webhooks & REST APIs
* Git & GitHub — Versionamento e documentação

---

## ✍️ Autor

Desenvolvido por mim como parte dos meus estudos e práticas de automação de processos!

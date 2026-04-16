[README_WhaBot.md](https://github.com/user-attachments/files/26771915/README_WhaBot.md)
# 💬 WhaBot AI

> Bot de atendimento automático para WhatsApp que responde clientes em segundos — com palavras-chave, preços, horários e redirecionamento humano.

---

## 📌 Sobre o projeto

O **WhaBot AI** é um bot de atendimento construído com **Z-API**, **n8n** e **Make** que automatiza o primeiro contato com clientes no WhatsApp.

O sistema identifica palavras-chave nas mensagens recebidas e responde automaticamente com as informações certas — preços, horários, localização — e quando necessário, redireciona o cliente para um atendente humano. O tempo de resposta cai de minutos para segundos.

Ideal para pequenos negócios, lojas e prestadores de serviço que recebem alto volume de mensagens repetitivas no WhatsApp.

---

## ⚙️ Como funciona

```
Cliente envia mensagem no WhatsApp
             ↓
Z-API captura e encaminha para o n8n
             ↓
n8n/Make identifica palavras-chave
             ↓
     ┌────────────────────┐
     │  Preço? → Responde │
     │  Horário? → Responde│
     │  Humano? → Redireciona│
     └────────────────────┘
             ↓
Z-API envia resposta automática ao cliente
```

---

## 🛠️ Tecnologias utilizadas

| Ferramenta | Função |
|---|---|
| [Z-API](https://z-api.io) | Integração com WhatsApp Business |
| [n8n](https://n8n.io) | Orquestração do fluxo de automação |
| [Make (Integromat)](https://make.com) | Automação complementar do fluxo |

---

## ✨ Funcionalidades

- ✅ Resposta automática baseada em palavras-chave
- ✅ Informações sobre preços, horários e localização
- ✅ Redirecionamento para atendimento humano quando necessário
- ✅ Tempo de resposta reduzido para segundos
- ✅ Fluxo 100% no-code via n8n e Make

---

## 🚀 Como usar

### Pré-requisitos

- Conta na [Z-API](https://z-api.io) com número de WhatsApp conectado
- Conta no [n8n](https://n8n.io) (self-hosted ou cloud)
- Conta no [Make](https://make.com) (opcional)

### Configuração

1. Clone este repositório
2. Importe o arquivo de fluxo no n8n ou Make
3. Configure as credenciais:
   - Z-API Token e Instance ID
4. Personalize as palavras-chave e respostas no fluxo
5. Ative o webhook e o workflow

---

## 📁 Estrutura do projeto

```
WhaBot-AI/
├── index (2)       # Fluxo exportado do n8n/Make
└── README.md
```

---

## 👤 Autor

**João Pedro Silva dos Santos**  
[GitHub](https://github.com/JoaoPedroske) · [Email](mailto:joaopedrosilvadossantos94@gmail.com)

---

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

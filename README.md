[![n8n](https://img.shields.io/badge/Feito%20com-n8n-blueviolet?logo=n8n)](https://n8n.io/)
[![Tipo](https://img.shields.io/badge/Tipo-Automação-orange)](https://n8n.io/)
[![Linguagem](https://img.shields.io/badge/Linguagem-JSON-lightgrey)](https://www.json.org/)

Este projeto apresenta um workflow de automação construído na plataforma n8n que monitora uma caixa de e-mails, utiliza a IA do Google Gemini para resumir o conteúdo das novas mensagens recebidas e, por fim, envia esse resumo como uma notificação por SMS.

É uma demonstração prática de como integrar serviços de e-mail, modelos de linguagem avançados (LLMs) e serviços de comunicação para criar um agente autônomo simples e funcional.

## ✅ Pré-requisitos
Antes de configurar este workflow, você precisará de:

Uma instância do n8n (seja na nuvem ou auto-hospedada).

Uma conta do Google com o Gmail.

Credenciais da API do Google Gemini (API Key). Você pode obtê-las no Google AI Studio.

Uma conta na sms77 e uma API Key.

## ⚙️ Configuração
Siga estes passos para importar e configurar o workflow em sua instância do n8n.

1. Importar o Workflow

    Baixe o arquivo resumir-email-sms.json deste repositório.

    Na sua interface do n8n, vá em New Workflow e selecione Import from file.

    Faça o upload do arquivo JSON.

2. Configurar as Credenciais

    As credenciais são os pontos de conexão com os serviços externos. O workflow importado não inclui as chaves de API por segurança. Você precisará configurá-las manualmente.

3. Ajustar os Nós

    Nó Send an SMS:

    Altere os campos From e To para o número de telefone de origem (se aplicável no seu plano sms77) e o número de destino para o qual você deseja enviar a notificação.

## ▶️ Ativação e Uso
Após configurar todas as credenciais e os nós, salve o workflow clicando no botão Save.

Ative o workflow movendo o interruptor de Inactive para Active no canto superior direito da tela.

Pronto! A cada minuto, o sistema verificará seus e-mails. Ao receber um novo, ele será resumido pela IA e você receberá uma notificação via SMS em poucos instantes.

## 🤝 Contribuição
Sinta-se à vontade para abrir issues ou enviar pull requests com melhorias, correções de bugs ou novas funcionalidades.

## 📜 Licença
Este projeto é distribuído sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.

## 📜 Licença
Este projeto é distribuído sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.
>>>>>>> 93dc280 (alteração no readme.)

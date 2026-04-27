# 🎙️ MarketingIA: Agente Multimodal de Conteúdo via WhatsApp

Este projeto consiste em um Agente de IA avançado capaz de transformar comandos de voz e texto em ativos de marketing completos. Utilizando orquestração de Agentes e múltiplas APIs, o sistema automatiza a criação de posts, blogs e imagens diretamente pelo WhatsApp.

---

## 🚀 Funcionalidades

- 🗣️ **Interação Multimodal:** Processa mensagens de texto e áudio (transcrição via OpenAI Whisper).
- 🧠 **Cérebro Cognitivo:** Utiliza um nó de "Think" para decidir qual ferramenta utilizar com base no pedido do usuário.
- 🎨 **Criação de Imagens:** Ferramentas dedicadas para criar e editar imagens via IA.
- 📄 **Conteúdo Estruturado:** Geração automática de posts para LinkedIn e Blog com foco em engajamento.
- 💾 **Memória de Sessão:** Mantém o contexto da conversa utilizando Window Buffer Memory para interações naturais.

---

## 🧰 Tecnologias Utilizadas

- [n8n.io](https://n8n.io) – Orquestrador de workflows e agentes.
- [OpenRouter](https://openrouter.ai/) – Acesso ao GPT-4.1 e outros modelos de ponta.
- [OpenAI Whisper](https://openai.com/research/whisper) – Transcrição de áudio em tempo real.
- [Evolution API](https://evolution-api.com/) – Integração profissional com WhatsApp.
- [LangChain](https://www.langchain.com/) – Framework para gerenciamento de agentes e memória.

---

## 📂 Estrutura do Fluxo

1. **Trigger:** Recebe mensagens via WhatsApp (Evolution API).
2. **Filtro de Entrada:** Identifica se o input é texto ou áudio (transcrevendo se necessário).
3. **Marketing Team Agent:** O agente processa a solicitação e chama a ferramenta adequada:
    - `linkedinPost`: Gera publicações para redes profissionais.
    - `blogPost`: Cria artigos estruturados.
    - `createImage/editImage`: Gerencia a parte visual do marketing.
4. **Output:** Retorna o link da imagem gerada ou o conteúdo textual formatado ao usuário.

---

## 📌 Diferenciais Técnicos

- **Arquitetura de Agentes:** Implementação de ferramentas (`Tools`) que o Agente de IA decide quando e como usar.
- **Processamento de Mídia:** Conversão de base64 e tratamento de arquivos binários para garantir que áudios e imagens fluam sem erros.
- **Prompt Engineering:** Instruções de sistema rigorosas para garantir que o tom de voz da IA seja sempre profissional e clicável.

---

## 👨‍💻 Autor

**Pedro Lucas Tomazeti Fernandes** 📧 pltf8001@gmail.com  
📍 São Luís, Maranhão – Brasil  
🔗 [GitHub](https://github.com/PedroTomazeti) | [LinkedIn](www.linkedin.com/in/pedro-lucas-tomazeti-fernandes-5a35b6320)

---

## 📜 Licença

MIT

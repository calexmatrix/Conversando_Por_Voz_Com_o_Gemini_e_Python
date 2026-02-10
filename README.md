# 🎙️ Gemini Voice Assistant - Colab Edition

Este projeto demonstra como criar um assistente de voz funcional e inteligente utilizando o modelo **Gemini 1.5 Flash**. Diferente de abordagens tradicionais que usam modelos separados para transcrição (ASR), este sistema aproveita a natureza multimodal do Gemini para entender o áudio diretamente, respondendo via texto e voz.



## 🚀 Tecnologias Utilizadas

* **Google Gemini 1.5 Flash:** Responsável pelo processamento do áudio e geração da inteligência conversacional.
* **gTTS (Google Text-to-Speech):** Utilizado para converter as respostas de texto do Gemini em áudio natural.
* **Google Colab:** Ambiente de desenvolvimento em nuvem.
* **Python:** Linguagem base para integração das APIs.

## ✨ Diferenciais deste Projeto

* **Processamento de Áudio Inline:** O áudio é enviado diretamente para o modelo sem necessidade de conversão prévia em texto por ferramentas externas (como o Whisper), reduzindo a latência.
* **Integração com Google Drive:** Persistência de logs e arquivos de áudio gerados durante a conversa.
* **Tratamento de Cota:** Sistema automático de retentativa (retry) caso o limite da API seja atingido.

## 🛠️ Como Usar

1.  **Chave de API:** Obtenha sua chave no [Google AI Studio](https://aistudio.google.com/).
2.  **Configuração no Colab:**
    * No menu lateral do Colab, clique no ícone de chave (🔑).
    * Adicione um novo segredo com o nome `GOOGLE_API_KEY` e cole sua chave.
    * Habilite o acesso do notebook a esse segredo.
3.  **Execução:**
    * Execute as células de instalação e configuração.
    * Ao rodar a função `assistant.run()`, autorize o uso do microfone no seu navegador.
    * Fale sua pergunta e aguarde o Gemini responder com áudio!

## 📁 Estrutura de Arquivos

O projeto organiza automaticamente os arquivos no seu Google Drive:
* `input_audio.webm`: Última gravação capturada pelo microfone.
* `response_audio.mp3`: Última resposta sintetizada pelo assistente.

---
Desenvolvido para fins educacionais e demonstração das capacidades multimodais da IA Generativa do Google.

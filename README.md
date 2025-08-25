### Awesome AI APIs 🤖

> A curated collection of 21 AI APIs with ready-to-use Requestly collections for instant testing.

### Why This Exists

Skip the API documentation hunt. This repo provides:

  - **21 AI APIs** - Curated and ready to test. More coming soon! 
  - **Provider-level Collections** - All APIs from a single provider (e.g., OpenAI) are grouped together in one file.
  - **Simple JSON Imports** - Just download the `.json` file for the provider you want, import it, and start testing.
  - **Pre-configured Variables** - Just add your API keys, and the requests are ready to go.
  - **Working Examples** - Real requests that you can send immediately.

### 🚀 Quick Start

1.  **Download the JSON file(s)**

      - Choose a provider from the table below and download its corresponding JSON file.

2.  **Import to Requestly**

      - Open the [Requestly Desktop App](https://requestly.io/desktop/).
      - Import the downloaded JSON file.
      - All APIs for that provider will be imported instantly.

3.  **Add API Keys**

      - Go to the Variables section within the imported collection.
      - Add your API key (e.g., `OPENAI_API_KEY`).
      - Keys are stored locally and are never shared.

4.  **Start Testing**

      - Click any API → Send request.
      - Modify parameters as needed.
      - Test different AI services instantly.

### 📋 All AI APIs

This collection is organized by provider. Each JSON file contains a full suite of APIs for that provider, including chat, image generation, and more.

| Provider | Description | Use Cases | Official Docs | Requestly JSON |
| :--- | :--- | :--- | :--- | :--- |
| OpenAI | The largest collection with APIs for chat, image generation, speech-to-text, and more. | Chat, Image Generation, Voice/Speech, Code | [Docs](https://platform.openai.com/docs/api-reference) | [OpenAI.json](https://www.google.com/search?q=https://github.com/Ronakkadhi/awesome-ai-apis/blob/main/OpenAI.json) |
| Groq | Known for high-speed LLM inference. | Low-latency Chat, Q\&A, reasoning | [Docs](https://console.groq.com/docs/quickstart) | [Groq.json](https://www.google.com/search?q=https://github.com/Ronakkadhi/awesome-ai-apis/blob/main/Groq.json) |
| Anthropic | Focuses on safe and helpful AI, with APIs for chat and messages. | Chat, Q\&A, reasoning | [Docs](https://docs.anthropic.com/en/api/messages) | [Claude.json](https://www.google.com/search?q=https://github.com/Ronakkadhi/awesome-ai-apis/blob/main/Claude.json) |
| Google Gemini | Provides a multimodal LLM for text, image, and audio tasks. | Multimodal Chat, Image Analysis, Content Generation | [Docs](https://ai.google.dev/api/rest) | [Gemini.json](https://www.google.com/search?q=https://github.com/Ronakkadhi/awesome-ai-apis/blob/main/Gemini.json) |
| OpenRouter | An aggregator for multiple LLM models, often with free tiers. | Aggregator, Model Comparison, Chat | [Docs](https://openrouter.ai/docs) | [OpenRouter.json](https://www.google.com/search?q=https://github.com/Ronakkadhi/awesome-ai-apis/blob/main/OpenRouter.json) |
| Mistral | Focused on powerful, open-source-based chat models. | Chat, Q\&A, reasoning | [Docs](https://docs.mistral.ai/api/) | *Coming Soon* |
| Perplexity | Known for its conversational AI and fast responses. | Chat, Web Search, Summarization | [Docs](https://docs.perplexity.ai/reference/post_chat_completions) | *Coming Soon* |
| Together AI | Provides access to a wide range of open-source models with high performance. | Chat, Q\&A, reasoning | [Docs](https://docs.together.ai/reference/chat-completions) | *Coming Soon* |
| Stability AI | Specializes in open-source-based image generation models. | Image Generation, Image-to-Image | [Docs](https://platform.stability.ai/docs/api-reference) | *Coming Soon* |
| ElevenLabs | The industry standard for high-quality text-to-speech and voice cloning. | Text-to-Speech, Voice Cloning | [Docs](https://elevenlabs.io/docs/api-reference) | *Coming Soon* |
| AssemblyAI | Provides a robust API for speech-to-text with advanced features. | Speech-to-Text, Audio Summarization | [Docs](https://www.assemblyai.com/docs/api-reference) | *Coming Soon* |

### ⚠️ Important Notes

  - **Most APIs work immediately with just API keys**, but some may require additional setup.
  - **File upload APIs** might require specific content-type adjustments.
  - **Beta/newer APIs** may have changed since collection creation.
  - Always refer to official documentation for the most up-to-date requirements.

### 🤝 Contributing
  
  - Found a great AI API we missed? Want to add more examples?
  - Fork this repo.
  - Add the new API to an existing or new provider JSON file.
  - Add any new variables needed.
  - Update the README table.
  - Submit a PR.

    Each new API should include:
  - Proper authentication headers
  - Working example request body
  - Correct endpoint URL
  - Variables

-----

**Made with ❤️ for the developer community**

*Powered by [Requestly](https://requestly.io) for seamless API testing* 🚀

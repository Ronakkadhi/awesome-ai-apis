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

<details>
<summary>📋 View All 21 APIs</summary>

| Name | Provider | Type | Use Cases | Docs / Website | Requestly JSON |
| :--- | :--- | :--- | :--- | :--- | :--- |
| OpenAI (Chat Completions) | OpenAI | Text/Chat LLM | General-purpose conversation, Q&A, reasoning | [Docs](https://platform.openai.com/docs/api-reference/chat) | [OpenAI.json](https://github.com/Ronakkadhi/awesome-ai-apis/blob/main/OpenAI.json) |
| OpenAI Images (DALL·E) | OpenAI | Image Generation | Image Generation | [Docs](https://platform.openai.com/docs/api-reference/images) | [OpenAI.json](https://github.com/Ronakkadhi/awesome-ai-apis/blob/main/OpenAI.json) |
| OpenAI Audio (Speech-to-Text) | OpenAI | Speech-to-Text | Speech (STT / TTS / Voice) | [Docs](https://platform.openai.com/docs/api-reference/audio) | [OpenAI.json](https://github.com/Ronakkadhi/awesome-ai-apis/blob/main/OpenAI.json) |
| OpenAI Audio (Text-to-Speech) | OpenAI | Text-to-Speech | Speech (STT / TTS / Voice) | [Docs](https://platform.openai.com/docs/api-reference/audio) | [OpenAI.json](https://github.com/Ronakkadhi/awesome-ai-apis/blob/main/OpenAI.json) |
| OpenAI (GPT-3.5 family) | OpenAI | Multimodal Chat | Multimodal (Text + Image + More) | [Docs](https://platform.openai.com/docs/models/gpt-4o) | [OpenAI.json](https://github.com/Ronakkadhi/awesome-ai-apis/blob/main/OpenAI.json) |
| OpenAI Image Edits | OpenAI | Image Edit | Image Generation | [Docs](https://platform.openai.com/docs/api-reference/images/createEdit) | [OpenAI.json](https://github.com/Ronakkadhi/awesome-ai-apis/blob/main/OpenAI.json) |
| OpenAI Image Variations | OpenAI | Image Variation | Image Generation | [Docs](https://platform.openai.com/docs/api-reference/images/createVariation) | [OpenAI.json](https://github.com/Ronakkadhi/awesome-ai-apis/blob/main/OpenAI.json) |
| Anthropic (Claude Messages) | Anthropic | Text/Chat LLM | General-purpose conversation, Q&A, reasoning | [Docs](https://docs.anthropic.com/en/api/messages) | [Claude.json](https://github.com/Ronakkadhi/awesome-ai-apis/blob/main/Claude.json) |
| Google Gemini - Text generation | Gemini | Multimodal LLM | General-purpose conversation, Q&A, reasoning | [Docs](https://ai.google.dev/api/rest) | [Gemini.json](https://github.com/Ronakkadhi/awesome-ai-apis/blob/main/Gemini.json) |
| Google Gemini (Vision) | Gemini | Multimodal Chat | Multimodal (Text + Image + More) | [Docs](https://ai.google.dev/gemini-api/docs/vision) | [Gemini.json](https://github.com/Ronakkadhi/awesome-ai-apis/blob/main/Gemini.json) |
| Google Gemini - Speech generation | Gemini | Multimodal LLM | General-purpose conversation, Q&A, reasoning | [Docs](https://ai.google.dev/api/rest) | [Gemini.json](https://github.com/Ronakkadhi/awesome-ai-apis/blob/main/Gemini.json) |
| OpenRouter (Router over many LLMs) | OpenRouter | Text/Chat LLM Router | Aggregator | [Docs](https://openrouter.ai/docs) | [OpenRouter.json](https://github.com/Ronakkadhi/awesome-ai-apis/blob/main/OpenRouter.json) |
| OpenAI GPT oss 120b | OpenRouter | Text Generation | Aggregator | [Docs](https://openrouter.ai/docs) | [OpenRouter.json](https://github.com/Ronakkadhi/awesome-ai-apis/blob/main/OpenRouter.json) |
| OpenAI GPT oss 20b | OpenRouter | Text Generation | Aggregator | [Docs](https://openrouter.ai/docs) | [OpenRouter.json](https://github.com/Ronakkadhi/awesome-ai-apis/blob/main/OpenRouter.json) |
| Groq (OpenAI-compatible) | Groq | Text/Chat LLM | General-purpose conversation, Q&A, reasoning | [Docs](https://console.groq.com/docs/quickstart) | [Groq.json](https://github.com/Ronakkadhi/awesome-ai-apis/blob/main/Groq.json) |
| Meta-llama/Llama-3.1-8B-Instruct | Groq | Text/Chat LLM | General-purpose conversation, Q&A, reasoning | [Docs](https://groq.com/docs/api-reference/models) | [Groq.json](https://github.com/Ronakkadhi/awesome-ai-apis/blob/main/Groq.json) |
| Mistral (Chat Completions) | Mistral | Text/Chat LLM | General-purpose conversation, Q&A, reasoning | [Docs](https://docs.mistral.ai/api/) | *Coming Soon* |
| ElevenLabs V3 | ElevenLabs | Text-to-Speech | Speech (STT / TTS / Voice) | [Docs](https://elevenlabs.io/docs/api-reference) | *Coming Soon* |
| AssemblyAI Summarize | AssemblyAI | Summary from audio | Speech (STT / TTS / Voice) | [Docs](https://www.assemblyai.com/docs/api-reference) | *Coming Soon* |
| AssemblyAI (STT) | AssemblyAI | Speech-to-Text | Speech (STT / TTS / Voice) | [Docs](https://www.assemblyai.com/docs/api-reference) | *Coming Soon* |

</details>


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

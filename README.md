### Awesome AI APIs 🤖

> A curated collection of 21 AI APIs with ready-to-use Requestly collections for instant testing.

### Why This Exists

Skip the API documentation hunt. This repo provides:

  - **21 AI APIs** - Curated and ready to test. More coming soon!
  - **Provider-level Collections** - All APIs from a single provider (e.g., OpenAI) are grouped together in one file.
  - **Git-Controlled** - Seamlessly manage collections with standard Git commands.
  - **Pre-configured Variables** - Just add your API keys, and the requests are ready to go.
  - **Working Examples** - Real requests that you can send immediately.

***

### 🚀 Quick Start

1.  **Clone the Repository**
    - Open your terminal and run the following command to clone the repo:
    `git clone https://github.com/Ronakkadhi/awesome-ai-apis.git`

2.  **Set Up Requestly Workspace**
    - Open the [Requestly Desktop App](https://requestly.io/desktop/).
    - Go to "Workspaces" and create a new **Local Workspace**.
    - Select the `awesome-ai-apis` folder you just cloned. Requestly will automatically read and load all the collections.

3.  **Add Your API Keys**
    - Go to the "Variables" section within any imported collection.
    - Add your API key (e.g., `OPENAI_API_KEY`).
    - Keys are stored locally and are never shared.

4.  **Start Testing**
    - Select any API request and click **Send**.
    - Modify parameters as needed to test different AI services instantly.

***

### Access All 21 APIs here

| **Name** | **Provider** | **Type** | **Docs / Website** |
| :--- | :--- | :--- | :--- | 
| OpenAI (Chat Completions) | OpenAI | Text/Chat LLM | [Docs](https://platform.openai.com/docs/api-reference/chat) |
| OpenAI Images (DALL·E) | OpenAI | Image Generation | [Docs](https://platform.openai.com/docs/api-reference/images) |
| OpenAI Audio (Speech-to-Text) | OpenAI | Speech-to-Text | [Docs](https://platform.openai.com/docs/api-reference/audio) |
| OpenAI Audio (Text-to-Speech) | OpenAI | Text-to-Speech | [Docs](https://platform.openai.com/docs/api-reference/audio) |
| OpenAI (GPT-3.5 family) | OpenAI | Multimodal Chat | [Docs](https://platform.openai.com/docs/models/gpt-4o) |
| OpenAI Image Edits | OpenAI | Image Edit | [Docs](https://platform.openai.com/docs/api-reference/images/createEdit) |
| OpenAI Image Variations | OpenAI | Image Variation | [Docs](https://platform.openai.com/docs/api-reference/images/createVariation) |
| Anthropic (Claude Messages) | Anthropic | Text/Chat LLM | [Docs](https://docs.anthropic.com/en/api/messages) |
| Google Gemini - Text generation | Gemini | Multimodal LLM | [Docs](https://ai.google.dev/api/rest) |
| Google Gemini (Vision) | Gemini | Multimodal Chat | [Docs](https://ai.google.dev/gemini-api/docs/vision) |
| Google Gemini - Speech generation | Gemini | Multimodal LLM | [Docs](https://ai.google.dev/api/rest) |
| OpenRouter (Router over many LLMs) | OpenRouter | Aggregator | [Docs](https://openrouter.ai/docs) |
| OpenAI GPT oss 120b | OpenRouter | Text Generation | [Docs](https://openrouter.ai/docs) |
| OpenAI GPT oss 20b | OpenRouter | Text Generation | [Docs](https://openrouter.ai/docs) |
| Groq (OpenAI-compatible) | Groq | Text/Chat LLM | [Docs](https://console.groq.com/docs/quickstart) |
| Meta-llama/Llama-3.1-8B-Instruct | Groq | Text/Chat LLM | [Docs](https://groq.com/docs/api-reference/models) |
| Mistral (Coming soon) | Mistral | Text/Chat LLM | [Docs](https://docs.mistral.ai/api/) |
| ElevenLabs V3 (Coming soon) | ElevenLabs | Text-to-Speech | [Docs](https://elevenlabs.io/docs/api-reference) |
| AssemblyAI Summarize (Coming soon) | AssemblyAI | Summary from audio | [Docs](https://www.assemblyai.com/docs/api-reference) |
| AssemblyAI (STT)(Coming soon) | AssemblyAI | Speech-to-Text | [Docs](https://www.assemblyai.com/docs/api-reference) |

***

### ⚠️ Important Notes

- **Most APIs work immediately with just API keys**, but some may require additional setup.
- **File upload APIs** might require specific content-type adjustments.
- **Beta/newer APIs** may have changed since collection creation.
- Always refer to official documentation for the most up-to-date requirements.

***

### 🤝 Contributing
- Found a great AI API we missed? Want to add more examples?
- Fork this repo.
- Add the new API to an existing or new provider JSON file.
- Add any new variables needed.
- Update the README table.
- Submit a PR.
- Each new API should include: Proper authentication headers, variables, and body

***

**Made with ❤️ for the developer community**

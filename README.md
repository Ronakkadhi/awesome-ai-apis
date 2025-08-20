# Awesome AI APIs 🤖

> A curated collection of 50+ AI APIs with working examples and testing tools.

## Why This Exists

Finding and testing AI APIs shouldn't be a hassle. This repo gives you:
- **Curated APIs** - 50+ vetted AI services across all major categories
- **Working Examples** - Copy-paste cURL and Fetch examples that actually work
- **Easy Testing** - Individual API collections for immediate testing

## 🚀 Quick Start

1. **Browse APIs** by category in `/apis/`
2. **Copy examples** from each API page
3. **Test immediately** using the provided cURL commands
4. **Import to Requestly** for advanced testing

```bash
# Example: Test OpenAI Chat API
curl -X POST https://api.openai.com/v1/chat/completions \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{"model":"gpt-4","messages":[{"role":"user","content":"Hello!"}]}'
```

## 📂 API Categories

| Category | Count | Description |
|----------|-------|-------------|
| **Chat & Text LLMs** | 17 | Conversational AI and text generation |
| **Image Generation** | 8 | Text-to-image and image editing |
| **Speech & Audio** | 18 | Speech-to-text, text-to-speech, voice cloning |
| **Multimodal** | 4 | Text + vision + audio combined |
| **Aggregators** | 4 | Platforms hosting multiple AI models |

## 🛝 API Playground

Test APIs instantly with our examples:

```javascript
// Example: Generate image with DALL·E
const response = await fetch('https://api.openai.com/v1/images/generations', {
  method: 'POST',
  headers: {
    'Authorization': 'Bearer YOUR_API_KEY',
    'Content-Type': 'application/json'
  },
  body: JSON.stringify({
    prompt: "A sunset over mountains",
    n: 1,
    size: "1024x1024"
  })
});
```

### Advanced API Testing

Want to debug, modify headers, or test complex workflows? 

**Import individual API collections** into Requestly for:
- Header manipulation
- Response mocking  
- Request debugging
- Environment switching
- Traffic monitoring

Each API has its own Requestly collection - pick what you need!

## 📋 All AI APIs

<details>
<summary>📊 View All 51 APIs</summary>

| Name | Type | Use Cases | API Docs | Requestly |
|------|------|-----------|----------|-----------|
| [OpenAI Chat Completions](/apis/chat-llm/openai.md) | Chat LLM | General conversation, Q&A, reasoning | [Docs](https://platform.openai.com/docs/api-reference/chat) | [Import](/playground/requestly-collections/openai.json) |
| [Anthropic Claude](/apis/chat-llm/claude.md) | Chat LLM | General conversation, Q&A, reasoning | [Docs](https://docs.anthropic.com/claude/reference/messages_post) | [Import](/playground/requestly-collections/claude.json) |
| [Google Gemini](/apis/chat-llm/gemini.md) | Multimodal LLM | General conversation, Q&A, reasoning | [Docs](https://ai.google.dev/api/rest) | [Import](/playground/requestly-collections/gemini.json) |
| [Mistral](/apis/chat-llm/mistral.md) | Chat LLM | General conversation, Q&A, reasoning | [Docs](https://docs.mistral.ai/api/) | [Import](/playground/requestly-collections/mistral.json) |
| [Cohere](/apis/chat-llm/cohere.md) | Chat LLM | General conversation, Q&A, reasoning | [Docs](https://docs.cohere.com/reference/chat) | [Import](/playground/requestly-collections/cohere.json) |
| [AI21 Labs](/apis/chat-llm/ai21.md) | Chat LLM | General conversation, Q&A, reasoning | [Docs](https://docs.ai21.com/reference/jamba-complete-api-ref) | [Import](/playground/requestly-collections/ai21.json) |
| [Perplexity](/apis/chat-llm/perplexity.md) | Chat LLM | General conversation, Q&A, reasoning | [Docs](https://docs.perplexity.ai/reference/post_chat_completions) | [Import](/playground/requestly-collections/perplexity.json) |
| [OpenRouter](/apis/aggregators/openrouter.md) | LLM Router | Aggregator | [Docs](https://openrouter.ai/docs) | [Import](/playground/requestly-collections/openrouter.json) |
| [Together AI](/apis/chat-llm/together.md) | Chat LLM | General conversation, Q&A, reasoning | [Docs](https://docs.together.ai/reference/chat-completions) | [Import](/playground/requestly-collections/together.json) |
| [Groq](/apis/chat-llm/groq.md) | Chat LLM | General conversation, Q&A, reasoning | [Docs](https://console.groq.com/docs/quickstart) | [Import](/playground/requestly-collections/groq.json) |
| [DeepSeek](/apis/chat-llm/deepseek.md) | Chat LLM | General conversation, Q&A, reasoning | [Docs](https://platform.deepseek.com/api-docs/) | [Import](/playground/requestly-collections/deepseek.json) |
| [xAI Grok](/apis/chat-llm/grok.md) | Chat LLM | General conversation, Q&A, reasoning | [Docs](https://docs.x.ai/api) | [Import](/playground/requestly-collections/grok.json) |
| [NVIDIA NIM](/apis/chat-llm/nvidia-nim.md) | Chat LLM | General conversation, Q&A, reasoning | [Docs](https://docs.nvidia.com/nim/) | [Import](/playground/requestly-collections/nvidia-nim.json) |
| [Amazon Bedrock](/apis/aggregators/bedrock.md) | Model Hub | General conversation, Q&A, reasoning | [Docs](https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html) | [Import](/playground/requestly-collections/bedrock.json) |
| [Azure OpenAI](/apis/chat-llm/azure-openai.md) | Chat LLM | General conversation, Q&A, reasoning | [Docs](https://learn.microsoft.com/en-us/azure/ai-services/openai/) | [Import](/playground/requestly-collections/azure-openai.json) |
| [IBM watsonx.ai](/apis/chat-llm/watsonx.md) | Chat LLM | General conversation, Q&A, reasoning | [Docs](https://cloud.ibm.com/apidocs/watsonx-ai) | [Import](/playground/requestly-collections/watsonx.json) |
| [Databricks Mosaic AI](/apis/aggregators/databricks.md) | Gateway | General conversation, Q&A, reasoning | [Docs](https://docs.databricks.com/en/machine-learning/model-serving/ai-gateway.html) | [Import](/playground/requestly-collections/databricks.json) |
| [OpenAI DALL·E](/apis/image-generation/dalle.md) | Image Generation | Image Generation | [Docs](https://platform.openai.com/docs/api-reference/images) | [Import](/playground/requestly-collections/dalle.json) |
| [Stability AI](/apis/image-generation/stability-ai.md) | Image Generation | Image Generation | [Docs](https://platform.stability.ai/docs/api-reference) | [Import](/playground/requestly-collections/stability-ai.json) |
| [Replicate](/apis/aggregators/replicate.md) | Model Inference | AI Aggregator | [Docs](https://replicate.com/docs/reference/http) | [Import](/playground/requestly-collections/replicate.json) |
| [Hugging Face](/apis/aggregators/huggingface.md) | Model Inference | AI Aggregator | [Docs](https://huggingface.co/docs/api-inference) | [Import](/playground/requestly-collections/huggingface.json) |
| [OpenAI Speech-to-Text](/apis/speech/openai-stt.md) | Speech-to-Text | Speech Transcription | [Docs](https://platform.openai.com/docs/api-reference/audio) | [Import](/playground/requestly-collections/openai-stt.json) |
| [OpenAI Text-to-Speech](/apis/speech/openai-tts.md) | Text-to-Speech | Speech Synthesis | [Docs](https://platform.openai.com/docs/api-reference/audio) | [Import](/playground/requestly-collections/openai-tts.json) |
| [Deepgram](/apis/speech/deepgram.md) | Speech-to-Text | Speech Transcription | [Docs](https://developers.deepgram.com/reference/listen-live) | [Import](/playground/requestly-collections/deepgram.json) |
| [AssemblyAI](/apis/speech/assemblyai.md) | Speech-to-Text | Speech Transcription | [Docs](https://www.assemblyai.com/docs/api-reference) | [Import](/playground/requestly-collections/assemblyai.json) |
| [Speechmatics](/apis/speech/speechmatics.md) | Speech-to-Text | Speech Transcription | [Docs](https://docs.speechmatics.com/introduction) | [Import](/playground/requestly-collections/speechmatics.json) |
| [ElevenLabs](/apis/speech/elevenlabs.md) | Text-to-Speech | Speech Synthesis | [Docs](https://elevenlabs.io/docs/api-reference) | [Import](/playground/requestly-collections/elevenlabs.json) |
| [PlayHT](/apis/speech/playht.md) | Text-to-Speech | Speech Synthesis | [Docs](https://docs.play.ht/reference/api-getting-started) | [Import](/playground/requestly-collections/playht.json) |
| [GPT-4o](/apis/multimodal/gpt-4o.md) | Multimodal | Text + Image + Audio | [Docs](https://platform.openai.com/docs/models/gpt-4o) | [Import](/playground/requestly-collections/gpt-4o.json) |
| [Gemini Vision](/apis/multimodal/gemini-vision.md) | Multimodal | Text + Image | [Docs](https://ai.google.dev/gemini-api/docs/vision) | [Import](/playground/requestly-collections/gemini-vision.json) |
| [Perplexity Vision](/apis/multimodal/perplexity-vision.md) | Multimodal | Text + Image | [Docs](https://docs.perplexity.ai/reference/post_chat_completions) | [Import](/playground/requestly-collections/perplexity-vision.json) |
| [NVIDIA NIM Multimodal](/apis/multimodal/nvidia-nim-multimodal.md) | Multimodal | Text + Image | [Docs](https://docs.nvidia.com/nim/) | [Import](/playground/requestly-collections/nvidia-nim-multimodal.json) |
| [Poe](/apis/aggregators/poe.md) | Chat LLM | AI Aggregator | [Docs](https://developer.poe.com/server-bots/quick-start) | [Import](/playground/requestly-collections/poe.json) |
| [Meta LLaMA 2](/apis/chat-llm/llama2.md) | Chat LLM | General conversation, Q&A, reasoning | [Docs](https://llama.meta.com/docs/) | [Import](/playground/requestly-collections/llama2.json) |
| [Stability AI Retro](/apis/image-generation/stability-retro.md) | Image-to-Image | Image Generation | [Docs](https://platform.stability.ai/docs/api-reference) | [Import](/playground/requestly-collections/stability-retro.json) |
| [OpenAI Image Edits](/apis/image-generation/openai-image-edits.md) | Image Edit | Image Generation | [Docs](https://platform.openai.com/docs/api-reference/images/createEdit) | [Import](/playground/requestly-collections/openai-image-edits.json) |
| [OpenAI Image Variations](/apis/image-generation/openai-image-variations.md) | Image Variation | Image Generation | [Docs](https://platform.openai.com/docs/api-reference/images/createVariation) | [Import](/playground/requestly-collections/openai-image-variations.json) |
| [Replicate Text-to-Image](/apis/image-generation/replicate-text-to-image.md) | Image Generation | Image Generation | [Docs](https://replicate.com/docs/reference/http) | [Import](/playground/requestly-collections/replicate-text-to-image.json) |
| [Runway Gen-2](/apis/image-generation/runway.md) | Video Generation | Video Generation | [Docs](https://docs.runwayml.com/reference/inferences) | [Import](/playground/requestly-collections/runway.json) |
| [Amazon Transcribe](/apis/speech/amazon-transcribe.md) | Speech-to-Text | Speech Transcription | [Docs](https://docs.aws.amazon.com/transcribe/) | [Import](/playground/requestly-collections/amazon-transcribe.json) |
| [Amazon Polly](/apis/speech/amazon-polly.md) | Text-to-Speech | Speech Synthesis | [Docs](https://docs.aws.amazon.com/polly/) | [Import](/playground/requestly-collections/amazon-polly.json) |
| [ElevenLabs Voice Cloning](/apis/speech/elevenlabs-voice-cloning.md) | Voice Synthesis | Voice Cloning | [Docs](https://elevenlabs.io/docs/api-reference) | [Import](/playground/requestly-collections/elevenlabs-voice-cloning.json) |
| [Play.ht Voice API](/apis/speech/playht-voice.md) | Voice Synthesis | Voice Synthesis | [Docs](https://docs.play.ht/reference/api-getting-started) | [Import](/playground/requestly-collections/playht-voice.json) |
| [Rev.ai](/apis/speech/revai.md) | Speech-to-Text | Speech Transcription | [Docs](https://docs.rev.ai/api/asynchronous/) | [Import](/playground/requestly-collections/revai.json) |
| [Whisper API](/apis/speech/whisper.md) | Speech Transcription | Speech Transcription | [Docs](https://platform.openai.com/docs/api-reference/audio) | [Import](/playground/requestly-collections/whisper.json) |
| [AssemblyAI Summarize](/apis/speech/assemblyai-summarize.md) | Audio Summary | Speech Analysis | [Docs](https://www.assemblyai.com/docs/api-reference) | [Import](/playground/requestly-collections/assemblyai-summarize.json) |
| [Descript Overdub](/apis/speech/descript.md) | Voice Cloning | Voice Synthesis | [Docs](https://www.descript.com/api) | [Import](/playground/requestly-collections/descript.json) |
| [OpenAI Audio Translations](/apis/speech/openai-translations.md) | Speech Translation | Speech Translation | [Docs](https://platform.openai.com/docs/api-reference/audio) | [Import](/playground/requestly-collections/openai-translations.json) |
| [Azure Speech-to-Text](/apis/speech/azure-stt.md) | Speech-to-Text | Speech Transcription | [Docs](https://docs.microsoft.com/en-us/azure/cognitive-services/speech-service/) | [Import](/playground/requestly-collections/azure-stt.json) |
| [Azure Text-to-Speech](/apis/speech/azure-tts.md) | Text-to-Speech | Speech Synthesis | [Docs](https://docs.microsoft.com/en-us/azure/cognitive-services/speech-service/) | [Import](/playground/requestly-collections/azure-tts.json) |
| [Murf AI Voice](/apis/speech/murf.md) | Voiceover Generation | Speech Synthesis | [Docs](https://murf.ai/resources/api-documentation/) | [Import](/playground/requestly-collections/murf.json) |

</details>

## 🤝 Contributing

Found a great API we missed? Have better examples?

1. Fork this repo
2. Add your API following the format in existing files
3. Include working cURL and Fetch examples
4. Create a Requestly collection JSON
5. Submit a PR

Each API page should include:
- Basic info and use cases
- Authentication details  
- Working code examples
- Link to official docs

---

**Made with ❤️ for the developer community**

*All examples work great with [Requestly](https://requestly.io) for advanced API testing* 😉

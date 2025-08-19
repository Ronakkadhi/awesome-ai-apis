# Awesome AI 🤖

> A curated collection of 50+ AI APIs with working examples and testing tools.

## Why This Exists

Finding and testing AI APIs shouldn't be a hassle. This repo gives you:
- **Curated APIs** - 50+ vetted AI services across all major categories
- **Working Examples** - Copy-paste cURL and Fetch examples that work
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

Each API has its own Requestly collection. This helps us scale our contributions & only pick what you need!

## 📋 Browse APIs

### Chat & Text LLMs
- [OpenAI Chat Completions](/apis/chat-llm/openai.md) - Industry standard | [Import to Requestly](/playground/requestly-collections/openai.json)
- [Anthropic Claude](/apis/chat-llm/claude.md) - Constitutional AI | [Import to Requestly](/playground/requestly-collections/claude.json)
- [Google Gemini](/apis/chat-llm/gemini.md) - Multimodal reasoning | [Import to Requestly](/playground/requestly-collections/gemini.json)
- [Mistral](/apis/chat-llm/mistral.md) - European AI leader | [Import to Requestly](/playground/requestly-collections/mistral.json)
- [View all 17 →](/apis/chat-llm/)

### Image Generation  
- [OpenAI DALL·E](/apis/image-generation/dalle.md) - Text to image | [Import to Requestly](/playground/requestly-collections/dalle.json)
- [Stability AI](/apis/image-generation/stability-ai.md) - Open source models | [Import to Requestly](/playground/requestly-collections/stability-ai.json)
- [Runway](/apis/image-generation/runway.md) - Video generation | [Import to Requestly](/playground/requestly-collections/runway.json)
- [View all 8 →](/apis/image-generation/)

### Speech & Audio
- [ElevenLabs](/apis/speech/elevenlabs.md) - Voice cloning & TTS | [Import to Requestly](/playground/requestly-collections/elevenlabs.json)
- [OpenAI Audio](/apis/speech/openai-audio.md) - Whisper & TTS | [Import to Requestly](/playground/requestly-collections/openai-audio.json)
- [AssemblyAI](/apis/speech/assemblyai.md) - Speech-to-text | [Import to Requestly](/playground/requestly-collections/assemblyai.json)
- [View all 18 →](/apis/speech/)

### Multimodal
- [GPT-4o](/apis/multimodal/gpt-4o.md) - Text + vision + audio | [Import to Requestly](/playground/requestly-collections/gpt-4o.json)
- [Gemini Vision](/apis/multimodal/gemini-vision.md) - Google's multimodal | [Import to Requestly](/playground/requestly-collections/gemini-vision.json)
- [View all 4 →](/apis/multimodal/)

### Aggregators
- [Replicate](/apis/aggregators/replicate.md) - Run AI models via API | [Import to Requestly](/playground/requestly-collections/replicate.json)
- [HuggingFace](/apis/aggregators/huggingface.md) - Hosted model inference | [Import to Requestly](/playground/requestly-collections/huggingface.json)

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

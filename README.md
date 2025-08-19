# awesome-ai
AI APIs Ready-to-Run Templates
Copy a curl, paste your key, run. Or import APIs in Requestly and start testing immediately.

Quick links:

➡️ Categories: Text/Chat · Image · Multimodal · Speech · Video · Aggregators/Hubs

How to use this repo
Pick an API from the category tables below.

Open its folder under apis/<provider>/<area>/.

Run a quick test: copy the curl or JS fetch example, set your API key, and run.

(Optional) Import into Requestly for testing:

Import [collections/all-apis.json] to get everything, or the category JSON (e.g., collections/text-llms.json).

Update placeholders (e.g., YOUR_OPENAI_API_KEY) in the saved requests.

Inspect/modify/replay with Requestly to debug inputs/outputs and headers.

Conventions (auth, placeholders, structure)
Auth placeholders:

YOUR_OPENAI_API_KEY, YOUR_ANTHROPIC_API_KEY, etc.

Use env vars in examples where possible: $OPENAI_API_KEY / process.env.OPENAI_API_KEY.

Headers: every template includes Authorization and Content-Type as required.

Files per API endpoint:

perl
Copy
Edit
apis/<provider>/<endpoint-slug>/
  ├─ requestly.json        # Importable request template
  ├─ example.curl.md       # Minimal curl
  ├─ example.js.md         # Minimal JS fetch
  └─ sample-io.md          # Example input/output
Playgrounds/Demos: If the provider has a free demo, it’s linked in the table for fast trying without a key.

Ready-to-run examples (pattern we’ll follow for every API)
Example: OpenAI (Chat Completions)
Docs: <link to docs>
Playground (if any): <link>
Requestly template: apis/openai/chat/requestly.json

curl

bash
Copy
Edit
curl -X POST https://api.openai.com/v1/chat/completions \
  -H "Authorization: Bearer $OPENAI_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "gpt-4o-mini",
    "messages": [{"role":"user","content":"Say hi in one sentence."}],
    "temperature": 0.7
  }'

JS fetch

js
Copy
Edit
const resp = await fetch("https://api.openai.com/v1/chat/completions", {
  method: "POST",
  headers: {
    "Authorization": `Bearer ${process.env.OPENAI_API_KEY}`,
    "Content-Type": "application/json"
  },
  body: JSON.stringify({
    model: "gpt-4o-mini",
    messages: [{ role: "user", content: "Say hi in one sentence." }],
    temperature: 0.7
  })
});
console.log(await resp.json());
Sample I/O (apis/openai/chat/sample-io.md)

vbnet
Copy
Edit
Input: "Write a haiku about summer rain."
Output:
Soft rain kisses earth,
Distant thunder hums along—
Warm streets breathe again.
Repeat this same 4-file pattern for every API you add.

Text / Chat LLMs
Name	Type	Use cases	Docs	Requestly JSON	curl	JS	Playground
OpenAI (Chat Completions)	Text/Chat LLM	General-purpose conversation, Q&A, reasoning	[Docs]	apis/openai/chat/requestly.json	apis/openai/chat/example.curl.md	apis/openai/chat/example.js.md	link
Anthropic (Claude Messages)	Text/Chat LLM	General-purpose conversation, Q&A, reasoning	[Docs]	apis/anthropic/messages/requestly.json	apis/anthropic/messages/example.curl.md	apis/anthropic/messages/example.js.md	link
Mistral (Chat Completions)	Text/Chat LLM	General-purpose conversation, Q&A, reasoning	[Docs]	apis/mistral/chat/requestly.json	apis/mistral/chat/example.curl.md	apis/mistral/chat/example.js.md	link
Cohere (Chat)	Text/Chat LLM	General-purpose conversation, Q&A, reasoning	[Docs]	apis/cohere/chat/requestly.json	…	…	link
AI21 Labs (Jamba/Studio)	Text/Chat LLM	General-purpose conversation, Q&A, reasoning	[Docs]	apis/ai21/chat/requestly.json	…	…	link
Perplexity (Chat Completions)	Text/Chat LLM	General-purpose conversation, Q&A, reasoning	[Docs]	apis/perplexity/chat/requestly.json	…	…	—
Groq (OpenAI-compatible)	Text/Chat LLM	General-purpose conversation, Q&A, reasoning	[Docs]	apis/groq/chat/requestly.json	…	…	—
DeepSeek	Text/Chat LLM	General-purpose conversation, Q&A, reasoning	[Docs]	apis/deepseek/chat/requestly.json	…	…	—
xAI (Grok)	Text/Chat LLM	General-purpose conversation, Q&A, reasoning	[Docs]	apis/xai/grok/requestly.json	…	…	—
NVIDIA NIM (LLMs)	Text/Chat LLM (NIM)	General-purpose conversation, Q&A, reasoning	[Docs]	apis/nvidia/nim-llm/requestly.json	…	…	—
Azure OpenAI (Chat)	Text/Chat LLM (Azure)	General-purpose conversation, Q&A, reasoning	[Docs]	apis/azure/openai-chat/requestly.json	…	…	—
IBM watsonx.ai (Text Gen)	Text/Chat LLM	General-purpose conversation, Q&A, reasoning	[Docs]	apis/ibm/watsonx-textgen/requestly.json	…	…	—
Meta LLaMA 2 (API access)	Text/Chat LLM	General-purpose conversation, Q&A, reasoning	[Docs]	apis/meta/llama2-chat/requestly.json	…	…	—

Tip: keep Google Gemini (REST) and OpenAI (GPT-4o family) under Multimodal, not Text-only.

Aggregators / Model Hubs
Name	Type	Use cases	Docs	Requestly JSON	curl	JS	Playground
OpenRouter (Router over many LLMs)	Text/Chat LLM Router	Aggregator	[Docs]	apis/openrouter/chat/requestly.json	…	…	link
Replicate	Model Inference (Images/Text/etc.)	AI Aggregator	[Docs]	apis/replicate/predictions/requestly.json	…	…	link
Hugging Face Inference API	Hosted Model Inference	AI Aggregator	[Docs]	apis/hf/inference/requestly.json	…	…	link
Databricks Mosaic AI Gateway	Gateway / Model Router	Governance + routing	[Docs]	apis/databricks/gateway/requestly.json	…	…	—
Amazon Bedrock Runtime	Model Hub (LLM/Image/etc.)	Multi-provider access	[Docs]	apis/aws/bedrock-runtime/requestly.json	…	…	—
Poe (Quora)	Text/Chat LLM	AI Aggregator	[Docs]	apis/poe/chat/requestly.json	…	…	link

Image Generation & Editing
Name	Type	Use cases	Docs	Requestly JSON	curl	JS	Playground
OpenAI Images (DALL·E)	Image Generation	Image Generation	[Docs]	apis/openai/images/requestly.json	…	…	link
Stability AI (Stable Image)	Image Generation & Editing	Image Generation	[Docs]	apis/stability/image/requestly.json	…	…	link
OpenAI Image Edits	Image Edit	Image Generation	[Docs]	apis/openai/image-edits/requestly.json	…	…	—
OpenAI Image Variations	Image Variation	Image Generation	[Docs]	apis/openai/image-variations/requestly.json	…	…	—
Replicate Text-to-Image (e.g., SDXL)	Image Generation	Image Generation	[Docs]	apis/replicate/sdxl/requestly.json	…	…	link
Stability AI (Retro)	Image-to-image	Image Generation	[Docs]	apis/stability/retro/requestly.json	…	…	—

Multimodal (Text + Image + More)
Name	Type	Use cases	Docs	Requestly JSON	curl	JS	Playground
OpenAI (GPT-4o family)	Multimodal Chat	Multimodal (Text + Image + More)	[Docs]	apis/openai/gpt-4o/requestly.json	…	…	link
Google Gemini (REST)	Multimodal LLM	General-purpose conversation, Q&A, reasoning	[Docs]	apis/google/gemini-rest/requestly.json	…	…	link
Google Gemini (Vision)	Multimodal Chat	Multimodal (Text + Image + More)	[Docs]	apis/google/gemini-vision/requestly.json	…	…	link
Perplexity (Vision)	Multimodal Chat	Multimodal (Text + Image + More)	[Docs]	apis/perplexity/vision/requestly.json	…	…	—
NVIDIA NIM (Multimodal)	Multimodal	Multimodal (Text + Image + More)	[Docs]	apis/nvidia/nim-multimodal/requestly.json	…	…	—

Speech (STT / TTS / Voice)
Name	Type	Use cases	Docs	Requestly JSON	curl	JS	Playground
OpenAI Audio (Speech-to-Text)	Speech-to-Text	Speech (STT / TTS / Voice)	[Docs]	apis/openai/audio-stt/requestly.json	…	…	—
OpenAI Audio (Text-to-Speech)	Text-to-Speech	Speech (STT / TTS / Voice)	[Docs]	apis/openai/audio-tts/requestly.json	…	…	—
Deepgram (STT)	Speech-to-Text	Speech (STT / TTS / Voice)	[Docs]	apis/deepgram/stt/requestly.json	…	…	link
AssemblyAI (STT)	Speech-to-Text	Speech (STT / TTS / Voice)	[Docs]	apis/assemblyai/stt/requestly.json	…	…	link
Speechmatics (Realtime WS)	Speech-to-Text	Speech (STT / TTS / Voice)	[Docs]	apis/speechmatics/realtime-ws/requestly.json	…	…	—
ElevenLabs (TTS)	Text-to-Speech	Speech (STT / TTS / Voice)	[Docs]	apis/elevenlabs/tts/requestly.json	…	…	link
PlayHT (TTS)	Text-to-Speech	Speech (STT / TTS / Voice)	[Docs]	apis/playht/tts/requestly.json	…	…	link
Amazon Transcribe	Speech-to-Text	Speech (STT / TTS / Voice)	[Docs]	apis/aws/transcribe/requestly.json	…	…	—
Amazon Polly	Text-to-Speech	Speech (STT / TTS / Voice)	[Docs]	apis/aws/polly/requestly.json	…	…	—
ElevenLabs Voice Cloning	Voice Synthesis	Speech (STT / TTS / Voice)	[Docs]	apis/elevenlabs/voice-clone/requestly.json	…	…	—
Play.ht Voice API	Voice Synthesis	Speech (STT / TTS / Voice)	[Docs]	apis/playht/voice-clone/requestly.json	…	…	—
Rev.ai	Speech-to-Text	Speech (STT / TTS / Voice)	[Docs]	apis/revai/stt/requestly.json	…	…	—
Whisper API (OpenAI hosted)	Speech Transcription	Speech (STT / TTS / Voice)	[Docs]	apis/openai/whisper/requestly.json	…	…	—
AssemblyAI Summarize	Summary from audio	Speech (STT / TTS / Voice)	[Docs]	apis/assemblyai/summarize/requestly.json	…	…	—
Descript Overdub	Voice cloning	Speech (STT / TTS / Voice)	[Docs]	apis/descript/overdub/requestly.json	…	…	—
OpenAI Audio Translations	Speech Translation	Speech (STT / TTS / Voice)	[Docs]	apis/openai/audio-translate/requestly.json	…	…	—
Speech-to-Text Azure	STT	Speech (STT / TTS / Voice)	[Docs]	apis/azure/speech-stt/requestly.json	…	…	—
Azure TTS	Text-to-Speech	Speech (STT / TTS / Voice)	[Docs]	apis/azure/tts/requestly.json	…	…	—
Murf AI Voice	Voiceover Generation	Speech (STT / TTS / Voice)	[Docs]	apis/murf/voiceover/requestly.json	…	…	—

Video (Generation & Editing)
Name	Type	Use cases	Docs	Requestly JSON	curl	JS	Playground
Runway Gen-2	Video Generation	Video Generation	[Docs]	apis/runway/gen2/requestly.json	…	…	link
Descript Studio API	Audio/Video Edit	Video Editing	[Docs]	apis/descript/studio/requestly.json	…	…	—
Lumen5 AI Video	Video Generation	Video Generation	[Docs]	apis/lumen5/generate/requestly.json	…	…	—
Pictory AI	Video Editing	Video Editing	[Docs]	apis/pictory/edit/requestly.json	…	…	—

Auth setup (each API)
Every API folder includes a short Auth section. The pattern:

yaml
Copy
Edit
### Auth
1) Create an account: <signup link>
2) Create an API key: <dashboard link>
3) Add to Requestly:
   - Header: Authorization: Bearer YOUR_API_KEY
   - Content-Type: application/json
4) Limits: <free tier / rate limits link, if applicable>
We never commit real keys. Use env vars in examples and placeholders in JSON.

One-click import (Requestly Collections)
All APIs: add collections/all-apis.json (exported from Requestly).

By category: add collections/text-llms.json, collections/images.json, collections/multimodal.json, collections/speech.json, collections/video.json.

Keep collection item names short and consistent: OpenAI • Chat, Stability • Text-to-Image, etc.

Contributing
Pick an API and follow the 4-file template.

Verify curl works with your own key (do not commit keys).

Add a row in the category table with links to your files.

Update the relevant category collection JSON in /collections/.

Open a PR with a short demo screenshot or response JSON.

License & disclaimers
MIT for this repo’s content.

Each API is subject to its provider’s terms, pricing, and quotas.

This repo includes example requests only; you must use your own API keys.


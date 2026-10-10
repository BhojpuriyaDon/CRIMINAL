# Direct AI providers

CRIMINAL 0.22.0 includes 34 endpoint presets across hosted APIs, regional/deployment APIs and local servers. Protocol variants and regional URLs are separate presets; this is not a count of 34 distinct companies. OpenRouter is optional.

## Setup

1. Open **Settings → Connection → AI provider**.
2. Choose a saved connection or a preset under **Add · Hosted APIs**, **Add · Regional and deployment APIs**, or **Add · Local servers**.
3. Enter that provider's own API key. For a local server, start it and load a model; configure a key if the server requires one.
4. Select **Test connection & load models**, then choose a model. For manual catalogs, enter the model ID from provider documentation and use **Test selected model**. Azure also needs its resource URL and deployment name.
5. Optionally use **Test tool calling**, then select **Save settings**.

Save additional profiles for different accounts, endpoints or model defaults. The model picker can switch between saved connections. **+ Add custom AI provider** supports a custom base URL, Chat Completions, Responses, Anthropic Messages or Gemini protocols, extra headers and optional pricing.

Preset selection fills the endpoint, protocol, authentication requirement and catalog mode. It clears unsaved key/model drafts from the prior selection. Keys stay in the separate credential store; changing a saved destination or protocol clears its old key. Existing profiles and custom URLs are preserved on upgrade. A preset does not create accounts, purchase credits, install models or guarantee access.

## Model discovery and verification

- Model discovery queries the selected endpoint's `/models` API and supported pagination. Some catalogs include non-chat models; select one compatible with the chosen protocol.
- Fireworks, Cohere, Z.AI, MiniMax, Qwen and Azure presets start with manual model selection. Their model catalogs or deployment discovery can differ from the inference API. **Advanced connection options → Model discovery** lets you enable `/models` when the endpoint supports it.
- Setup guidance does not contact an endpoint or claim a successful connection. **Test selected model** sends a small real generation request. Model and tool tests may incur provider charges.
- Tool calls, vision, reasoning, context capacity and output limits depend on the model and account. A successful short test does not guarantee every agent task will complete.

## Other services

Use a custom profile for other servers implementing one of the four supported protocols. AWS Bedrock request signing, Google Vertex AI OAuth/token refresh and other vendor-specific authentication flows are not direct adapters in this release; use a compatible gateway. A matching hostname alone does not make an incompatible API work.

Preset setup links point to provider documentation. Regional keys must match their endpoints. Update a saved URL if a provider changes its service.

## Catalog

The maintained catalog is [provider-presets.json](../server/provider-presets.json), which supplies both desktop settings and the backend. Each preset includes its official setup URL and relevant instructions.

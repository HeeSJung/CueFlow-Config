# CueFlow Remote Selector Config

Remote CSS selector configuration for the [CueFlow](https://github.com/HeeSJung/CueFlow) Chrome extension.

The extension fetches `selectors.json` to stay up-to-date when AI chat platforms change their DOM structure — no extension update required.

## Supported Platforms

- ChatGPT (`chatgpt.com`)
- Claude (`claude.ai`)
- Gemini (`gemini.google.com`)
- Perplexity (`perplexity.ai`)

## How It Works

1. Extension checks its local cache (6-hour TTL)
2. If expired, fetches `selectors.json` from this repo
3. Falls back to bundled selectors if fetch fails

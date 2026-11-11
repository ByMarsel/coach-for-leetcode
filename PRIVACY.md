# Privacy policy

Effective: 11 November 2026

AI Coach for LeetCode is a browser extension that helps you practise LeetCode problems with an AI model you choose. This policy explains what data the extension handles, where it goes, and how to delete it. In short: everything stays in your browser, except what you send to the AI provider you picked, and we run no servers that could receive your data.

## What the extension handles

| Data | Where it is kept | Where it is sent |
|---|---|---|
| Your API keys for Anthropic, OpenAI or OpenRouter | Your browser's extension storage, on your device | Only to the provider the key belongs to, with each request to that provider |
| Problem statement, your code and language, the timer, your latest Run or Submit result, your messages to the coach | Your browser's extension storage | To the AI provider you chose, only when you ask the coach something or use hot-cold. A local model gets them on your computer only, and the problem statement in advance, so the model is ready when you ask |
| Settings, timers, chats, solved-problem history, what your AI requests cost | Your browser's extension storage | Nowhere |

The extension reads the problem statement and your Run and Submit results from leetcode.com while you use the site, through your own LeetCode session. It does not send them anywhere except to your chosen AI provider as described above.

To show which models you can pick, the settings may load the public model catalogue from OpenRouter and, if you saved an OpenAI key, the list of models available to your OpenAI account. These requests contain no problem or code.

If you choose a local model, the requests go only to the model server on your own computer (localhost or 127.0.0.1) at the address you set, so the problem, your code and the chat never leave it.

Requests to OpenRouter also name the extension (its title and GitHub address), so OpenRouter can count its usage in its public app rankings. These headers carry nothing about you.

## What we do not do

- We do not run servers that receive your data. There is no account, no analytics, no tracking, no advertising.
- We do not sell or share your data, and we do not use it for any purpose other than the coaching you ask for.
- We do not use your data to determine creditworthiness or for lending.

## How your keys are protected

The extension's storage is restricted to the extension's own pages. Neither leetcode.com nor the script the extension runs on LeetCode pages can read your keys. A saved key is never displayed again; the settings show only its last four characters.

The data is stored unencrypted in your browser profile, like the data of other extensions, so anyone with access to your computer account could read it.

## Third parties

When you send a request, the AI provider you chose receives it and handles it under its own terms and privacy policy:

- Anthropic: https://www.anthropic.com/legal/privacy
- OpenAI: https://openai.com/policies/privacy-policy
- OpenRouter: https://openrouter.ai/privacy

## Deleting your data

- Remove a key with **Remove** next to it in Settings.
- Clear a problem's conversation with **New chat**, or the conversation and the timer with the reset button.
- Removing the extension from Chrome deletes everything it stored.

## Children

AI Coach for LeetCode is not directed at children under 13 and does not knowingly handle their data.

## Changes

If this policy changes, the new version will be published at this address with a new effective date.

## Contact

help@marsel.engineer

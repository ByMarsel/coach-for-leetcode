# Coach for LeetCode

A learning mode for LeetCode. Coach for LeetCode adds a panel to every problem page with a timer, a ladder of hints, code review and a live "hot-cold" progress bar, so you solve the problem yourself and understand why the solution works.

It uses an AI model of your choice: Claude from Anthropic, OpenAI models, or any model on OpenRouter, with your own API key.

Coach for LeetCode is an independent project. It is not affiliated with, endorsed by or sponsored by LeetCode.

## Features

### A coach next to the problem

The panel opens on the right of any problem page (`leetcode.com/problems/…`), styled like LeetCode and following its light or dark theme. Collapse it with **›**, bring it back with the **Coach** tab on the right edge or the extension icon, and drag its left edge to resize it. The panel remembers its width and whether it is open.

With every request the coach sees the problem statement, your current code and language, the timer, and your latest Run or Submit result (passed tests, the failing input, expected and actual output, the error message), so its answers are about the code you have right now.

### Buttons

| Button | What you get |
|---|---|
| Explain problem | What the problem asks, in plain words, with the first example walked through. If the statement is in another language, a translation first. No hints about the solution. |
| Guiding question | One question that nudges you towards the key observation. The gentlest hint. |
| Hint | The key idea or pattern and why it fits here. No code, no steps. |
| Plan | A step-by-step plan in words or pseudocode, with the target complexity. No code. |
| Code review | Bugs, missed edge cases and the complexity of your current code. It points to the problem and does not rewrite your code. |
| Find a failing test | One valid test your current code fails, ready to paste into LeetCode's Testcase panel, with the expected output and what it targets. |
| Explain failure | Appears after a failed Run or Submit: why that test fails, without the fix. |
| Solution debrief | Appears after Accepted: complexity, whether the solution is optimal, edge cases to remember, similar problems to practise. |
| Show solution | The full solution with code. It needs a second click, so you do not open it by accident. |

Hover over any button to see what it does. Repeating a hint gives the same idea from another angle; it never jumps to the next level on its own.

### Chat

Type an idea or a question below the buttons. The coach tells you whether the idea works and, if not, the shortest input it breaks on, without giving away what would work instead. Ask explicitly when you want a hint or the solution. Code blocks in answers have a **Copy** button. **New chat** clears the conversation for the problem; the timer keeps going.

### Hot-cold

Click the thermometer under the timer to see, while you code, how close you are to a working solution. A bar fills from red to green; hover over it for a short note that never spoils the answer. It updates a few seconds after you stop typing, and every half minute while you keep typing. The first time you switch it on for a problem it needs a moment to get ready.

### Timer

The timer starts when you start writing code, not when you open the problem, and runs only while the problem tab is on screen. Default limits are 15, 30 and 45 minutes for Easy, Medium and Hard, and you can change them. The timer turns yellow when a fifth of the time is left and red with the overtime once the limit passes. Pause and resume it, or reset the timer together with the chat (two clicks). It keeps running while the panel is collapsed.

### History

Every problem you get Accepted on Submit lands in **History**: time against the limit, hints taken, submissions, and whether you looked at the solution or used hot-cold. The summary shows how many problems you solved within the limit and how many hints you take on average.

### Languages

The interface comes in English, Spanish, Italian, French, German and Russian, and the coach can answer in any of them, independently of the interface. Both default to your browser's language.

### Your coach, your way

- Choose the provider and the model in **Settings**: Claude (Opus, Sonnet or the low-cost Haiku), any OpenAI model, or any of the hundreds of models on OpenRouter, listed from the cheapest. Prices per million tokens are shown next to the models.
- Set the reasoning depth: low is faster and cheaper, high is more thorough.
- Rewrite the coach's prompt in any language, or go back to the default with one click.

### Fair play

The coach is switched off on contest pages (`leetcode.com/contest/…`): LeetCode's contest rules forbid AI help. Use Coach for LeetCode for learning and practice only; see the [terms of use](TERMS.md).

## Privacy and security

- Your API keys stay in your browser's extension storage. That storage is closed to everything except the extension's own pages: the LeetCode page and the scripts the extension runs on it cannot read the keys.
- A saved key is never shown again; the settings show only its last four characters. You can remove a key at any time.
- The problem, your code and your messages go only to the AI provider you chose, and only when you ask the coach something or use hot-cold. There is no server of ours in between, and no analytics or tracking.
- Your chats, timers and history stay in your browser.

Details: [privacy policy](PRIVACY.md).

## What it costs

Coach for LeetCode is free. You pay your AI provider directly for what you use, with your own key. As a rough guide, half an hour on a problem with a few hints and hot-cold on costs around $0.20 on Claude Sonnet and around $0.40 on Claude Opus; Claude Haiku and the cheaper OpenRouter models cost a fraction of that. A hot-cold check costs a fraction of a cent.

## Install

Coach for LeetCode is coming to the Chrome Web Store.

Once installed, open any problem on leetcode.com, then paste your API key from Anthropic, OpenAI or OpenRouter in **Settings** in the panel.

## Support

Write to [help@marsel.engineer](mailto:help@marsel.engineer) or open an issue on [GitHub](https://github.com/ByMarsel/coach-for-leetcode/issues).

## Legal

- [Terms of use](TERMS.md)
- [Privacy policy](PRIVACY.md)

LeetCode is a trademark of its owner. Claude is a trademark of Anthropic. OpenAI and OpenRouter are trademarks of their owners.

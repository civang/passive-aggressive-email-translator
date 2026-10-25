# The Passive-Aggressive Email Translator ✉️😤

**Type what you actually mean. Get what you're allowed to send.**

A single-page web toy that turns blunt thoughts into office-speak, and decodes
the office-speak other people send you back into what they really meant.

## Features

- **✍️ Write it:** type what you want to say ("you never replied", "I told you so",
  "this is overdue") and get a send-ready email in one of three tones:
  - 🙂 **Corporate Polite**: "I wanted to follow up as I haven't yet heard back"
  - 😤 **Peak Petty**: "Circling back on the email you've clearly been ignoring"
  - 📋 **HR-Approved**: "I appreciate that this may have slipped through"
- **🕵️ Decode theirs:** paste an email you received and find out what
  "per my last email" or "gentle reminder" actually means, with a threat level.
- **Passive-aggression meter** for every translation.
- **One-click copy** of the finished email.

## Run it

No build, no dependencies, no server, no API key. Open `index.html` in a browser.

```bash
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

## How it works

Plain HTML, CSS and JavaScript in one file. Translation is rule-based: a list
of regex patterns maps blunt phrases to a phrasing for each tone, wrapped with a
tone-appropriate greeting and sign-off. The decoder runs the same idea in
reverse, matching common office phrases to their real meaning and a 0–100
threat score.

To teach it a new phrase, add an entry to `rules` (writing) or `decodeRules`
(decoding) in `index.html`.

## License

[MIT](LICENSE)

# Contributing

Thank you for your interest in improving this project! Contributions that add API archetypes, fix code examples, clarify analogies, or improve the UI are all welcome.

## Getting Started

```bash
git clone https://github.com/your-username/apis.git
cd apis
npm install
npm run dev
```

The app runs at `http://localhost:5173` by default (Vite dev server).

## What Can I Contribute?

| Type | Description |
|------|-------------|
| New archetype | Add an entry to `APIS` in `src/api-archetypes-guide.jsx` following the existing schema |
| Better examples | Improve the server/client code snippets for clarity or correctness |
| UI improvements | Dark-theme consistent style fixes and accessibility improvements |
| Bug fixes | Typos, broken logic, incorrect technical information |
| Translations | Spanish translation of the guide content |

## Adding a New API Archetype

Each entry in `APIS` follows this schema (all fields required):

```js
soap: {
  name: "SOAP",
  subtitle: "Simple Object Access Protocol",
  icon: "📋",          // emoji shown in tabs and cards
  color: "#e2b86e",    // must contrast against #07080f background
  glyph: "⊕",         // large decorative background character
  analogy: {
    title: "Short memorable name",
    body:  "2–3 sentence fantasy analogy explaining the pattern",
  },
  howItWorks: [ /* 5–6 bullet strings */ ],
  pros:        [ /* 4–5 bullet strings */ ],
  cons:        [ /* 4–5 bullet strings */ ],
  bestFor:     [ /* 3–4 short tags */ ],
  notFor:      [ /* 3–4 short tags */ ],
  serverCode:  `# Python server example`,
  clientPy:    `# Python client example`,
  clientJs:    `// JavaScript client example`,
}
```

Also add the key to `API_ORDER` and a `soap` column to every row in `COMPARISON`.

## Coding Conventions

- All component styles use inline JavaScript style objects (no external CSS)
- Code examples use the **fantasy/quest theme** (quests, heroes, guilds) for consistency
- Keep code examples minimal but runnable — show imports and a main usage pattern
- No TypeScript in this project — plain JSX

## Pull Request Process

1. Fork the repo and create a branch: `git checkout -b feature/add-mqtt`
2. Verify the app runs: `npm run dev`
3. Run the linter: `npm run lint`
4. Open a PR with a clear title and a short description of the change

## Code of Conduct

Be respectful and constructive. This is a learning resource for software engineering students — feedback should educate, not discourage.

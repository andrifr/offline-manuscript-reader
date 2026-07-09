# Offline Manuscript Reader

A simple, private **read-aloud tool for writers**. Paste your draft and have it read
back to you using your computer's built-in text-to-speech voices — no account, no
upload, no analytics, no AI.

The entire app is a single `index.html` file. No backend, no build step, no
dependencies, nothing minified. Open it in a browser and it works.

## Why this exists

Reading your draft aloud is one of the best ways to catch awkward sentences, typos,
missing words, and pacing problems. Many writers understandably don't want to paste
unpublished manuscripts into online tools or AI services. This page is designed to run
locally in your browser using text-to-speech voices already installed on your computer.

## Use it

**Online:** [Open the tool](https://YOUR_USERNAME.github.io/offline-manuscript-reader/)
*(replace this link once GitHub Pages is enabled)*

**Offline (maximum privacy):**

1. Download [`index.html`](index.html) (or click **“Download this page for offline use”** inside the app).
2. Disconnect from the internet.
3. Open the file in your browser (double-click it).
4. Paste your draft.
5. Listen locally.

Because the whole tool is one static HTML file, you can confirm for yourself that it
keeps working with the network off.

## Features

- Paste text and have it read aloud
- Voice picker that **labels local vs. online voices** and defaults to *“Local voices only”*
- Play · Pause · Resume · Stop
- Skip to the previous / next sentence (or click any sentence to read from there)
- Current sentence highlighting while reading
- Read a **selection only** — select part of your draft before pressing Play
- Speed, pitch, and volume controls
- Word and character count
- Dark / light theme and adjustable text size
- Remembers your **settings** (voice, speed, theme, …) — but **never your manuscript**

## How privacy works

This tool runs in your browser using your computer's built-in text-to-speech voices.

Your text is **not uploaded, stored, or sent to me.**

- It does not upload your text to any server of mine.
- It does not save your manuscript (only harmless settings are stored locally, via `localStorage`).
- It does not use AI to process your writing.
- It does not include analytics, tracking, external fonts, or third-party scripts.
- It makes no intentional network requests. You can verify this in your browser's
  DevTools → Network tab.

## Important limitation — voices

Voice privacy depends on your **browser, operating system, and the voice you pick.**
Some browsers offer cloud/online voices that **do** send your text to a provider
(e.g. Microsoft or Google) to be synthesised. This tool tries to identify local voices
where the browser exposes that information (`voice.localService`) and defaults to
*“Local voices only,”* but browser support varies — where it can't tell, treat the
voice as unknown.

For maximum privacy, use a known local system voice (on Windows these are often named
Microsoft David, Zira, Mark, etc.) and run the page offline.

## Inspect the code

You are encouraged to read the source before trusting it with a manuscript. The whole
tool is one file: [`index.html`](index.html). Nothing is minified or obfuscated. In your
browser you can also use **View Source** (Ctrl+U) to see exactly what runs.

## A careful note

This tool is designed for privacy-conscious writers. It runs locally in your browser
and does not intentionally send your text anywhere. It does **not** claim to make
uploading impossible or to guarantee privacy in every environment — no web page can
promise that. Instead, it's kept small and readable so you can inspect it, download it,
and run it offline. You should only use software from sources you trust.

## Support

This is free. If it helped you catch mistakes in your manuscript, you can support the
project: **[Buy me a coffee](https://www.buymeacoffee.com/YOUR_NAME_HERE)**
*(replace with your own link)*.

## License

[MIT](LICENSE) — free to use, modify, and share.

# AgentLog Share

A free, private viewer for AI coding agent session exports (Claude Code and similar tools).

Drop in a `.zip` of `.jsonl` session files — or a single `.jsonl` — and read the conversation as a clean, searchable timeline: chat bubbles, collapsible tool calls/results, timestamps, and a search box.

## Why

Session transcripts are usually raw JSON lines — hard to read, hard to share. AgentLog Share renders them properly, without ever uploading your file anywhere.

## Privacy

**Everything runs in your browser.** No server, no backend, no upload. Your session data — which may include code and credentials — never leaves your machine. The app also automatically masks anything that looks like an API key, token, or password before displaying it.

## Profile & history

There's a lightweight "profile" (just a name you pick) and a history list of sessions you've opened before. This is **not an account system** — there's no server, no password, no real authentication. It's just a label used to organize what's saved in your browser's local storage (IndexedDB) on this specific device. Clearing your browser data clears it. Nothing syncs across devices or gets sent anywhere.

## Usage

1. Open the live site (or `index.html` locally in any browser).
2. Drop in your `.zip` or `.jsonl` file.
3. Browse, search, and export a clean HTML copy if you want to share it with someone.

## Local development

No build step — it's a single self-contained HTML file. Just open `index.html` in a browser, or serve it with any static file server:

```bash
python3 -m http.server 8000
```

## Deploy

This repo is ready to deploy as-is on Vercel, Netlify, or Cloudflare Pages — just connect the repo, no build command needed, output directory is `/`.

## License

MIT

## Legal

See [Privacy Policy](privacy.html) and [Terms of Service](terms.html) — both linked in the app's footer too.

# Student guide (Guia do Aluno) — local preview

Static HTML. Always serve over HTTP; opening `index.html` via `file://` breaks assets and some behaviors.

## Quick start

From this directory:

```bash
chmod +x serve-local.sh   # once, if needed
./serve-local.sh
```

**Default URL:** [http://127.0.0.1:8844/](http://127.0.0.1:8844/)

- macOS: `./serve-local.sh --open` starts the server and opens the default browser.
- Other port: `PORT=9000 ./serve-local.sh`

## Requirements

- Python 3 (uses `python3 -m http.server` bound to `127.0.0.1` only).

## GitHub Pages

This repo is set up for **static hosting** from the repository root (`index.html` at `/`).

1. Push to [github.com/Product-Arena/cursor-guia-do-aluno](https://github.com/Product-Arena/cursor-guia-do-aluno).
2. On GitHub: **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
4. Choose branch **`main`**, folder **`/ (root)`**, then **Save**.

After the first deploy (usually within a minute), the site is available at:

`https://product-arena.github.io/cursor-guia-do-aluno/`

(Exact URL is shown on the Pages settings screen.)

## Troubleshooting

- **Nothing loads:** run the script first and keep the terminal open.
- **Port in use:** set another port, e.g. `PORT=8845 ./serve-local.sh`.
- **Cursor Simple Browser issues with localhost:** use Safari, Chrome, or Firefox at the URL above.

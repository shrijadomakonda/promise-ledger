# Promise Ledger

A small, framework-free website for turning meeting notes into a commitment ledger. It identifies possible action items, shows the exact source note, flags missing owners and vague dates, lets you mark work complete, saves sessions on the device, and drafts a follow-up email.

## Run it

Open `index.html` directly in a modern browser, or serve the folder locally:

```powershell
cd path\to\outputs
python -m http.server 8000
```

Then visit http://localhost:8000. Click **Use sample notes**, then **Find the promises**.

## What it uses

- HTML, CSS, and plain JavaScript; no framework or package installation.
- Browser-local text parsing and `localStorage` for saved sessions.
- No Nebius Token Factory, external AI provider, API key, or server-side processing. Notes remain in the browser.

The current prototype uses transparent phrase matching to identify likely commitments. Treat its results as suggestions and review the evidence before sending the draft. A later version could add an AI provider behind an explicit opt-in, but this build is intentionally local-only.

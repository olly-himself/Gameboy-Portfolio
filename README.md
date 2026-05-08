# Gameboy Portfolio

A Game Boy-themed portfolio page that loads Construct 3 web export projects as cartridge-style entries.

## Structure

- `gameboy-portfolio.html` — main portfolio page with Game Boy UI and cartridge loader
- `GallopingGoldExport/` — example Construct 3 export folder

## Local development

Serve the folder from a local web server to avoid `file://` restrictions:

```bash
cd "c:\Users\ollye\Desktop\Work\GameboyPortfolio"
python -m http.server 8000
```

Then visit:

```
http://localhost:8000/gameboy-portfolio.html
```

## GitHub and Cloudflare Pages

1. Log in with GitHub CLI:

```bash
gh auth login
```

2. Create a remote repo and push:

```bash
gh repo create <username>/gameboy-portfolio --public --source=. --remote=origin --push
```

3. Connect the repository to Cloudflare Pages and deploy the `main` branch.

4. Use `gameboy-portfolio.html` as the site entrypoint if needed.

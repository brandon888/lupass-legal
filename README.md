# lupass-legal

Privacy policy and terms of service for the [LuPass](https://apps.apple.com) iOS app, hosted on GitHub Pages.

## URLs (after deploy)

- `https://brandon888.github.io/lupass-legal/` — landing
- `https://brandon888.github.io/lupass-legal/privacy/`
- `https://brandon888.github.io/lupass-legal/terms/`

## First-time deploy

```bash
cd legal-site
git init
git add -A
git commit -m "Initial: privacy + terms"
git branch -M main
git remote add origin git@github.com:brandon888/lupass-legal.git
git push -u origin main
```

Then on GitHub:

1. Go to **Settings → Pages**.
2. **Source**: `Deploy from a branch`.
3. **Branch**: `main`, folder `/ (root)`. Save.
4. Wait ~30 seconds, refresh the Pages settings tab to see the live URL.

## Updating

Edit `privacy.md` or `terms.md`, bump the `Last updated` line, then:

```bash
git add -A && git commit -m "Update privacy: <change>" && git push
```

GitHub Pages rebuilds within a minute.

## Local preview (optional)

```bash
bundle install
bundle exec jekyll serve
# open http://127.0.0.1:4000
```

## Source of truth

The canonical drafts also live in the main repo at `chinese-drive/docs/{privacy,terms}.md`. When updating, edit both or copy from one to the other.

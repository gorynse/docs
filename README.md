# Rynse Docs

The source for [docs.gorynse.com](https://docs.gorynse.com) (and the Mintlify "rynse" deployment).

## Local preview

```bash
# From the repo root
mint dev
```

This boots the Mintlify dev server on `localhost:3000` and hot-reloads as you edit MDX or `docs.json`.

The CLI is installed globally:

```bash
npm i -g mint
```

## Structure

- `docs.json` — site config (theme, colors, navigation, footer)
- `index.mdx` — landing page
- `logo/` — light + dark logo SVGs
- `favicon.svg` — site favicon

Content pages live as `.mdx` files in the repo root or in topic folders, and are referenced from `docs.json` `navigation.groups[*].pages`.

## Deployment

The `gorynse/rynse` Mintlify project auto-deploys from `main` on this repo.

# NSWRA Kings 2027 website

Static site served by GitHub Pages.

- `index.html` — the whole site.
- `sponsors.json` — sponsor categories and sponsors. Edit it on GitHub (pencil icon) and commit; the site updates in about a minute.
- `logos/` — sponsor logo files. Upload a logo here, then set `"logoUrl": "logos/<file>"` on the sponsor.
- `nswra-crest.png` — NSWRA crest.

In `sponsors.json`, each sponsor's `cats` lists the category ids it belongs to, e.g. `["gold", "tr"]` makes it a Match Partner presenting Target Rifle.

## Admin: saving to the website
The **Admin** tab saves straight to GitHub once a browser is connected with a token:
- Sponsors, categories and logos are saved to this repository (`sponsors.json`, `logos/`). GitHub Pages republishes in about a minute.
- Sponsorship values are saved to the **private** repository `MagnumSports/nswra-kings-2027-private` (`values.json`), so they are never public.

**Token:** a fine-grained personal access token (GitHub > Settings > Developer settings > Fine-grained tokens) with *Repository access* limited to `nswra-kings-2027` and `nswra-kings-2027-private`, and *Contents: Read and write*. Paste it into the Admin page once per browser. It is stored only in that browser; use **Disconnect this browser** to remove it.

Without a token, Admin runs as a demo: changes stay in that browser, and **Export sponsors.json** downloads the public file.

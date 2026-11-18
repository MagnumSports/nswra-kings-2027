# NSWRA Kings 2027 website

Static site served by GitHub Pages.

- `index.html` — the whole site.
- `sponsors.json` — sponsor categories and sponsors. Edit it on GitHub (pencil icon) and commit; the site updates in about a minute.
- `logos/` — sponsor logo files. Upload a logo here, then set `"logoUrl": "logos/<file>"` on the sponsor.
- `nswra-crest.png` — NSWRA crest.

In `sponsors.json`, each sponsor's `cats` lists the category ids it belongs to, e.g. `["gold", "tr"]` makes it a Match Partner presenting Target Rifle.

## Admin demo
The **Admin** tab works as a demo on this site: categories, sponsors and logo uploads are saved only in the visitor's own browser. To publish changes, click **Export sponsors.json** on the Admin page and upload that file over `sponsors.json` in this repository. **Reset demo** clears the browser copy.

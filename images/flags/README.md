# Shared flag library

Every team's dashboard shows the US flag before the team name. Each member may add up to two more flags of their choice: state, county or city. This folder holds those flags so every team can reuse them.

[FLAG-LOG.csv](FLAG-LOG.csv) lists every flag. A team packet names flags by their **ID** (for example `KS;ICT`).

## Your flag is not here? Add it once, and it is saved for everyone

1. **Check the log.** Search [FLAG-LOG.csv](FLAG-LOG.csv) for your state, county or city.
2. **Find the official image.** Use the government's own website, or a public-domain copy (for example on Wikimedia Commons). Save it as `.svg` or `.png`, at least 300 pixels wide, wide-format (3:2).
3. **Pick an ID.** Short and unique, capital letters: a state's postal code (`KS`), a city's airport code or short name (`ICT`), or a county's name (`SEDGWICK-KS`).
4. **Open one pull request** that adds the image file to this folder and one line to `FLAG-LOG.csv`:
   `id,name,level,file,source,license,added_by,added_on,status`
   Put your **call sign** in `added_by`, the image's web address in `source`, and `pending` in `status`.
5. **A reviewer checks the source** and the license, sets `status` to `approved`, and merges. From then on every member and every team can use that ID.

## Rules

- Official flags only: no logos, mascots, sports teams or party symbols.
- One file per flag. If a better image turns up, replace the file and note it in the log; the ID never changes.
- The `source` column is required. A flag with no source stays `pending` and is not shown on public dashboards.


# Displaying visual charts of github stats

Generate static SVGs with **GitHub Actions** 
and embed those local files in our profile README.  

There are two parts.

---

## 1) Create `.github/workflows/grs.yml`

```yml
name: Update README cards

on:
  schedule:
    - cron: "0 3 * * *"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest

    permissions:
      contents: write

    steps:
      - uses: actions/checkout@v6

      - name: Generate stats card
        uses: readme-tools/github-readme-stats-action@v1
        with:
          card: stats
          options: username=SaydRomey&show_icons=true&theme=tokyonight
          path: profile/stats.svg
          token: ${{ secrets.GITHUB_TOKEN }}

      - name: Generate top languages card
        uses: readme-tools/github-readme-stats-action@v1
        with:
          card: top-langs
          options: username=SaydRomey&layout=compact&theme=tokyonight&card_width=400
          path: profile/top-langs.svg
          token: ${{ secrets.GITHUB_TOKEN }}

      - name: Commit cards
        run: |
          git config user.name "github-actions[bot]"
          git config user.email "41898282+github-actions[bot]@users.noreply.github.com"
          git add profile/*.svg
          git commit -m "Update README cards" || exit 0
          git push
```

## 2) Write this in the stats section of the profile `README`
```html
<p align="center">
  <img src="./profile/top-langs.svg" alt="Top Languages" height="170"/>
  <img src="./profile/stats.svg" alt="GitHub Stats" height="170"/>
</p>
```

---

### What to do after adding the workflow

1. Commit the workflow file to our profile repo.
2. Go to the repo’s **Actions** tab.
3. Run **Update README cards** once with Run workflow.
4. Confirm these files appear in the repo:
  - `profile/stats.svg`
  - `profile/top-langs.svg`
5. Our README should then render from local files.

### One limitation  
With `GITHUB_TOKEN`, this setup uses public stats only by default;  
private stats require a `PAT` instead. 


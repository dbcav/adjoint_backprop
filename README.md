# Adjoints and Backprop

Source for the website version of the *Adjoints and Backprop* notebooks. Every push to `main` rebuilds the site and publishes it to GitHub Pages at `https://<your-username>.github.io/<repo-name>/`.

## What's in here

| Path | What it is |
|---|---|
| `notebooks/` | The notebooks themselves. The site shows whatever outputs are saved in them. |
| `index.md` | The landing page. |
| `myst.yml` | Site configuration: title, author, and page order. |
| `.github/workflows/deploy.yml` | Builds the site and deploys it. |
| `requirements.txt` | The Python packages the notebooks use, for running them locally. |

## Putting it online (one time)

1. Create a new **public** repository on GitHub (for example `adjoints-and-backprop`), with no README so it starts empty.
2. From this folder, push the contents to it:
   ```bash
   git init -b main
   git add .
   git commit -m "Initial site"
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
3. On GitHub, go to the repo's **Settings → Pages** and set **Source** to **GitHub Actions**.
4. Go to the **Actions** tab. If the first run failed because Pages wasn't enabled yet, open it and click **Re-run all jobs**. It takes a couple of minutes, and the site URL appears on the finished run.

You don't need to edit any links. The workflow fills in your username and repo name when it builds.

## Updating the site

Edit a notebook, run it top to bottom so its outputs are current, save it, then commit and push. The site displays the outputs saved in the notebook rather than re-running it, so a notebook saved without outputs will show up without plots.

To add another part later, put the notebook in `notebooks/`, add a line for it under `toc:` in `myst.yml`, and add a row for it in `index.md`.

## Previewing locally

```bash
npm install -g mystmd
myst start
```

This serves the site at `http://localhost:3000` and reloads as you edit. The "Run in your browser" and Colab links point to placeholders locally; they become real links when GitHub builds the site.

## Notes

- If you name the repo `<your-username>.github.io`, the site lives at the root of that domain. In that case, edit `deploy.yml` so that `BASE_URL` is `''` and `SITE_URL` ends at `.github.io`.
- The in-browser notebooks run in each visitor's browser, so there's no server, and nothing to pay for no matter how much traffic the site gets.

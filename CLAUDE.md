# Websites repo

This repo publishes websites to GitHub Pages for knrose007.

- GitHub repo: https://github.com/knrose007/websites
- Pages serves the `docs/` folder on the `main` branch.
- Live site root: https://knrose007.github.io/websites/

## Where sites live

- Every website lives in `docs/`.
- Each site gets its own subfolder with an `index.html`, e.g. `docs/my-site/index.html`.
- A site at `docs/<folder>/` is live at `https://knrose007.github.io/websites/<folder>/`.

## "publish"

When the user says "publish":

1. Run `git status` and find the changed or new files in `docs/`.
2. Stage only those files, each by its path (`git add docs/my-site/index.html ...`).
3. Commit with a short message describing the change.
4. Push to `origin main`.
5. Report the live URL of each site that changed. GitHub Pages takes about a minute to update, so check the URL with curl before reporting it as live.

## Rules

- Always stage files by name. Never use `git add .`, `git add -A`, `git commit -a`, or any other blanket stage of everything.
- Never force-push.
- Never commit files outside `docs/` without asking the user first.

# Pocket Git Viewer

A Sourcetree-style Git viewer for iPad and iPhone. It is one static HTML page that reads your repos through the GitHub API.

- Branch list and commit graph across branches
- Commit details with line-by-line diffs
- Compare a branch against `staging` or `main`: commits to merge, how far behind it is, the combined diff, and a link to open a PR
- Several repos with one token: switch between them from the header; the last highlighted branch is remembered per repo

It is read-only: nothing is merged or pushed from the page.

## Use it

1. Open the GitHub Pages URL in Safari and tap Share → **Add to Home Screen**.
2. Tap **Connect GitHub**, paste a fine-grained personal access token with **read-only** access to Contents, Metadata and Pull requests, then add repos by name or tap **Find my repos**.
3. Tick **Remember the token on this device** only on devices you trust. The token is stored in that browser and sent only to `api.github.com`. Without it, you paste the token once per visit; your repo list is always remembered.
4. On iPhone and iPad, open the page from its Home Screen icon. Safari may clear saved data for sites unused for 7 days, but Home Screen apps keep theirs. Safari and the Home Screen icon don't share saved data.

Without a token, the page shows a built-in sample repo.

## Hosting

Settings → Pages → Deploy from a branch → `main` / root.

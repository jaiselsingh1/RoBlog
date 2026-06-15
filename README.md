# Research Notes

Hugo + PaperMod blog scaffolded for GitHub Pages. It follows the same broad setup as Lilian Weng's blog: Markdown posts, Hugo static generation, PaperMod styling, and GitHub Pages deployment.

## Write a post

Create a new post:

```bash
hugo new content posts/2026-06-14-my-topic/index.md
```

Edit the Markdown file, set `draft: false`, and commit it. GitHub Actions will publish the site when changes land on `main`.

## Local preview

Install Hugo Extended and Go, then run:

```bash
hugo mod get
hugo server --buildDrafts
```

The PaperMod theme is pulled as a Hugo module from `github.com/adityatelange/hugo-PaperMod`.

## GitHub Pages setup

1. Create a GitHub repository, usually `USERNAME.github.io` for a user site.
2. Push this repo to GitHub on the `main` branch.
3. In repository settings, open **Pages** and set **Source** to **GitHub Actions**.
4. Update `baseURL`, `params.socialIcons`, and `params.editPost.URL` in `hugo.yaml`.

## Co-author

[Ben Evans](https://github.com/bennevans) is included as an invited co-author in the site metadata and Authors page.

After the remote repository exists, invite Ben as a collaborator with:

```bash
gh api \
  --method PUT \
  repos/OWNER/REPO/collaborators/bennevans \
  -f permission=push
```

Replace `OWNER/REPO` with the GitHub repository path.

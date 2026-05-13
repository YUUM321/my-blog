# FOCUS Hexo Blog

This repository contains the Hexo source for the `FOCUS` blog.

- Source repository: `YUUM321/my-blog`
- Published site repository: `YUUM321/YUUM321.github.io`
- Site URL: `https://YUUM321.github.io`

## Local Development

Install dependencies:

```powershell
npm.cmd ci
```

Build the static site:

```powershell
npm.cmd run build
```

Preview locally:

```powershell
npm.cmd run server
```

Create a new post:

```powershell
npx.cmd hexo new post "Post Title"
```

Posts are stored in `source/_posts/`.

## Publish

The site is configured to publish with `hexo-deployer-git` to the `main` branch of `YUUM321/YUUM321.github.io`:

```powershell
npm.cmd run deploy
```

If PowerShell blocks `npm.ps1`, use the `npm.cmd` and `npx.cmd` commands shown above.

## GitHub Workflow

Recommended update flow:

1. Edit or add posts under `source/_posts/`.
2. Run `npm.cmd run build` to verify Hexo generation.
3. Commit and push source changes to `YUUM321/my-blog`.
4. Run `npm.cmd run deploy` when the site should be published.

GitHub Actions is configured to run `npm ci` and `npm run build` on pushes to `main`, pull requests targeting `main`, and manual dispatches.

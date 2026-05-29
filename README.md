# Beibei Liu homepage for GitHub Pages

This folder is ready to publish as the repository `bbliu-astro.github.io`.

Public URL after GitHub Pages is enabled:

https://bbliu-astro.github.io/en/

## Preview locally

```bash
cd "/Users/bbliu/Myfloder/浙江大学/个人主页/github-pages"
python3 -m http.server 8002
```

Then open:

http://localhost:8002/en/

## Publish

If this folder is connected to `https://github.com/bbliu-astro/bbliu-astro.github.io`,
push the `main` branch. In GitHub, set Pages to publish from `main` / root.

## Sync English and Chinese Pages

From the parent folder:

```bash
python3 tools/sync_github_pages.py
```

That rebuilds `github-pages/en/` first, then regenerates `github-pages/cn/`
from the English pages with the Chinese translation and layout adjustments.
Use this command after changing the English source so the Chinese version stays
in sync.

The sync command runs:

```bash
python3 tools/build_github_pages.py
python3 tools/build_chinese_pages.py
```

# Editing the GitHub Pages homepage

The published homepage lives at:

`github-pages/en/index.html`

That file is Google Sites generated HTML, so it is large. Search for
`EDITABLE:` to find the safe manual-edit regions:

- Page title and metadata
- Welcome heading
- Main biography headline
- Current position headline
- Address, office, and email line
- Image carousel URLs

Keep Google Sites class names, scripts, `jsname`, `jscontroller`, and other
generated attributes unless you are intentionally redesigning the page.

After edits, preview locally:

```bash
cd "/Users/bbliu/Myfloder/浙江大学/个人主页/github-pages"
python3 -m http.server 8002
```

Open:

http://localhost:8002/en/

If you rebuild with `python3 tools/build_github_pages.py`, manual edits inside
`github-pages/en/` will be replaced by the current `site/` mirror.

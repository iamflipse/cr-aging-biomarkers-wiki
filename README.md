# CR Aging Biomarkers Wiki

A curated wiki distilling:

> Guida CA, Hsu FC, Neiberg R, Semelka C, Chen H, Kramer P, Houston DK, Nicklas B, Kritchevsky SB, Miller ME (2026). "Impact of caloric restriction on biological aging: insights from a composite biomarker index in older adults." *GeroScience*. doi: [10.1007/s11357-026-02529-9](https://doi.org/10.1007/s11357-026-02529-9)

**Public copy:** https://iamflipse.github.io/cr-aging-biomarkers-wiki/ (read-only; static build served from the `gh-pages` branch)

## Layout

- `src/` — wiki pages as markdown (`index.md`, `about.md`, `concepts/`, `sources/`)
- `book/` — mdbook-generated static site (committed for GitHub Pages)
- `tools/mdbook` — mdbook v0.4.21 binary (aarch64 Linux, built from source)

## Rebuild + republish

```sh
./tools/mdbook build -d book
git add -A && git commit -m "update" && git push origin main
# republish gh-pages: check out orphan branch, copy book/* to root, add .nojekyll, force push
```

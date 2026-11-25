# TFA2HCF3-site

Interactive publication site for the **TFA₂HCF₃** computational chemistry project (trifluoroacetic acid decarboxylation, **CF₃COOH → CF₃H + CO₂**). It hosts drag-to-rotate **3Dmol.js** molecular viewers, a 3D PES explorer, and related HTML pages synced from the sister code repository.

**Live site:** [https://glsalierno.github.io/TFA2HCF3-site/](https://glsalierno.github.io/TFA2HCF3-site/)

**Sister repo (code & data toolkit):** [https://github.com/glsalierno/TFA2HCF3](https://github.com/glsalierno/TFA2HCF3)

## Deploy (GitHub Pages)

On every push to `main` (and on manual `workflow_dispatch`), [`.github/workflows/pages.yml`](.github/workflows/pages.yml) checks out this repository, uploads the repo root as a Pages artifact, and deploys with the official GitHub Pages actions (`configure-pages`, `upload-pages-artifact`, `deploy-pages`). The site is static HTML/CSS/assets; there is no build step. A `.nojekyll` file is present so GitHub Pages does not process the tree with Jekyll.

Content is mirrored here from `TFA2HCF3` (HTML/PNG only). Updates are typically pushed from that repo via its publish script / Pages sync workflow.

## Local preview

From a clone of this repository:

```bash
python -m http.server 8000 --directory .
```

Then open [http://localhost:8000/](http://localhost:8000/) (or `/gallery_molecules.html`, etc.).

## License

MIT — see [LICENSE](LICENSE). Please confirm the copyright holder line before treating this as authoritative.

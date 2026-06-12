# SUSTAIN-HPC 2026 Workshop Website

Website for SUSTAIN-HPC 2026: Sustainable Computing for High-Performance and Distributed Systems, a half-day workshop held in conjunction with [ICPP 2026](https://icpp2026.github.io/) in Singapore.

Built with [MkDocs](https://www.mkdocs.org/) and the [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) theme, following the same setup as the ICPP 2026 main conference website.

## Local Development

```bash
pip install -r requirements.txt
mkdocs serve
```

Then open http://127.0.0.1:8000/.

## Deployment

Pushing to the `source` branch triggers the GitHub Actions workflow (`.github/workflows/publish.yml`), which builds the site and deploys it to the `main` branch via `mkdocs gh-deploy` for GitHub Pages hosting at https://icpp2026.github.io/sustain-hpc-2026/.

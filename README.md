# Resume / Curriculum Vitae

My professional résumé/CV in Markdown, version-controlled and ready to export to PDF/HTML. Multiple languages and layouts are provided.

## Direct links

- English
  - Full: [resume_en_full.md](./resume_en_full.md)
  - One‑page: [resume_en_one_page.md](./resume_en_one_page.md)
  - One‑page (Backend/Platform): [resume_en_one_page_backend.md](./resume_en_one_page_backend.md)
  - One‑page (Fintech/Payments): [resume_en_one_page_fintech.md](./resume_en_one_page_fintech.md)
  - One‑page (Cloud/Infra): [resume_en_one_page_cloud.md](./resume_en_one_page_cloud.md)

- Português (Brasil)
  - Completo: [resume_pt-BR_full.md](./resume_pt-BR_full.md)
  - Uma página: [resume_pt-BR_one_page.md](./resume_pt-BR_one_page.md)

- Español
  - Completo: [resume_es_full.md](./resume_es_full.md)
  - Una página: [resume_es_one_page.md](./resume_es_one_page.md)

## File naming

The naming scheme is: `resume_<language>_<variant>.md`

- `<language>`: `en`, `pt-BR`, `es`
- `<variant>`: `full`, `one_page`

## PDF Downloads

PDFs are automatically generated via GitHub Actions on every commit. Download them from the `pdfs/` directory:

### English
- [Full Resume (PDF)](./pdfs/resume_en_full.pdf)
- [One-page Resume (PDF)](./pdfs/resume_en_one_page.pdf)
- [Backend/Platform (PDF)](./pdfs/resume_en_one_page_backend.pdf)
- [Fintech/Payments (PDF)](./pdfs/resume_en_one_page_fintech.pdf)
- [Cloud/Infrastructure (PDF)](./pdfs/resume_en_one_page_cloud.pdf)

### Português (Brasil)
- [Currículo Completo (PDF)](./pdfs/resume_pt-BR_full.pdf)
- [Currículo Uma Página (PDF)](./pdfs/resume_pt-BR_one_page.pdf)

### Español
- [Currículum Completo (PDF)](./pdfs/resume_es_full.pdf)
- [Currículum Una Página (PDF)](./pdfs/resume_es_one_page.pdf)

## Manual PDF Generation (optional)

If you want to generate PDFs locally, install [Pandoc](https://pandoc.org/installing.html) and run:
```bash
# Generate all PDFs
mkdir -p pdfs
for md in resume_*.md; do pandoc "$md" -o "pdfs/${md%.md}.pdf"; done

# Or individual files
pandoc resume_en_full.md -o pdfs/resume_en_full.pdf
pandoc resume_en_one_page_backend.md -o pdfs/resume_en_one_page_backend.pdf
```

## License

This work is licensed under the Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License (CC BY-NC-ND 4.0). See the `LICENSE` file for details.

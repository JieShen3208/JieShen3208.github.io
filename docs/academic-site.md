# Academic site maintenance

- Navigation: `config/_default/menus.yaml`.
- Name and site description: `config/_default/params.yaml`.
- Biography, appointments and education: `data/authors/me.yaml`.
- Research: `content/research.md` and the short summary in `content/_index.md`.
- Add a personal photo at `assets/media/authors/me.png` when available. The template portrait and template CV have been removed. Add Teaching and CV navigation only when those materials are ready.

## Publications

Continue importing `publications.bib` with the existing workflow. No individual publication files need layout edits.

The homepage block and full publication archive share `layouts/_partials/academic/`. CSS lives in `assets/css/academic.css`. Author highlighting is controlled by `layouts/_partials/page_metadata_authors.html`.

The list groups papers by year in descending order, emphasizes titles and Jie Shen, italicizes the venue and uses the imported publication type for the label. It does not display the publisher. Links use HugoBlox's existing attachment and citation handlers: DOI and PDF appear only when supplied, and Cite uses each paper's `cite.bib`. Both structured links and the importer's legacy DOI/PDF fields remain supported.

Template demonstration sections and the three example publications are excluded via build cascades in `config/_default/hugo.yaml`. Remove the relevant exclusion when replacing a demonstration section with real content. The demonstration source files and the imported publication files remain intact.

# ipcc-verifier-guide

**IPCC Tier 1 Greenhouse Gas Inventories for Forests and Other Land**

*A Coding Guide to the 2019 Refinement, Volume 4, Chapters 1 to 9*

Seamus Murphy ([0000-0002-1792-0351](https://orcid.org/0000-0002-1792-0351)).

This is a book written as an executable Quarto project. It works through the IPCC Tier 1 methods for land, one chapter of the 2019 Refinement at a time, and every equation and default table is written as code that runs when the book is rendered. Forest land comes first. Cropland, grassland, wetlands, settlements and other land follow.

The master is the set of `.qmd` files under [`01.manuscript/`](01.manuscript/), one file per chapter, listed in [`01.manuscript/_quarto.yml`](01.manuscript/_quarto.yml).

    cd 01.manuscript && quarto render

The render writes the Word document and the website to `01.manuscript/_book/`, and the figures to `03.outputs/figures/`.

## Layout

| Folder | Contents |
|---|---|
| `01.manuscript/` | The book, one `.qmd` per chapter, with all analysis code inside the chapters |
| `02.inputs/` | Raw data, ignored by git, with `MANIFEST.md` and the committed derived files |
| `03.outputs/` | Figures and tables, written at render time |
| `04.references/` | Bibliography, citation style and the Word reference document |

Third-party guidance, standards and reports are not committed. [`04.references/README.md`](04.references/README.md) records what they are and where they came from.

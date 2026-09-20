# Reference manifest

This file records the provenance of everything in this folder. Third-party PDFs and their markdown conversions are not committed to git, and this manifest records what they are and where they came from.

## Committed files

| File | What it is |
|---|---|
| `references.bib` | The bibliography, one entry per IPCC chapter with the authors printed on its title page, and four whole-document entries. Rebuilt on 2026-09-17. |
| `elsevier-harvard.csl` | Elsevier author-date citation style, copied on 2026-09-17 from `ipcc-carbon-gains/04.references/`. |
| `style-formal.docx` | Word reference document for the docx render, copied on 2026-09-17 from `ipcc-carbon-gains/04.references/`. |

## IPCC guidance

The 26 PDFs under `standards/IPCC-pdf/` were downloaded on 2026-09-17 by the `sources` chunk of `01.manuscript/A1-sources.qmd`, which holds the address of each and downloads any that are missing. They are the 2006 Guidelines, Volume 4, Chapters 1 to 9 with Annexes 1 and 2 and Appendices 1 to 3, and the 2019 Refinement, Volume 4, Chapters 1 to 9 with Annexes 1 and 2 and the Chapter 2 Appendix 4. The pages they came from are `https://www.ipcc-nggip.iges.or.jp/public/2006gl/vol4.html` and `https://www.ipcc-nggip.iges.or.jp/public/2019rf/vol4.html`.

Chapters 10 to 12 of Volume 4 and the uncertainty chapter of Volume 1 were not downloaded, because they fall outside the first edition's scope.

## Personal library

`/Volumes/PortableSSD/Github/library-methodologies/IPCC/` was compared with the downloads on 2026-09-17 by SHA-256 checksum. Fourteen of the 26 downloads were byte-identical to a file there. The other twelve had no copy there, namely the 2006 Chapters 1, 6, 7 and 8, the 2006 Annex 1 and Appendices 1 to 3, the 2019 Chapters 7 and 9, the 2019 Annex 2 and the 2019 Chapter 2 Appendix 4.

Four files in that library are not what their names say, found by reading the first pages of each on 2026-09-17.

| File in `library-methodologies/` | What it is |
|---|---|
| `IPCC/IPCC-2006-V4-Ch11-Combustion-Managed-Soils.pdf` | The 2019 Refinement Chapter 11, not the 2006 chapter. Its first page reads "2019 Refinement to the 2006 IPCC Guidelines". |
| `IPCC/IPCC-2006-V4-Annex-Equations.pdf` | Byte-identical to `IPCC-2006-V4-Annex-Equations-Summary.pdf`, both the 2006 Annex 2, Summary of Equations. |
| `IPCC/USFS-2012-IPCC-Tier-1-Update-Guide.pdf` | Chapter 5, "Quantifying Greenhouse Gas Sources and Sinks in Managed Forest Systems", of the USDA report "Quantifying Greenhouse Gas Fluxes in Agriculture and Forestry: Methods for Entity-Scale Inventory". The PDF was created in March 2024. It is not an IPCC document and not from 2012. |
| `GOFC/GOFC-GOLD_2020-SOC-Guidelines.pdf` | Gold Standard for the Global Goals, Soil Organic Carbon Framework Methodology, Version 1.0, January 2020. It is not a GOFC-GOLD document. |

Four other files there bear on later chapters. They are `IPCC/IPCC-2019-V1-Ch3-Uncertainties.pdf`, the 2019 Refinement Volume 1 Chapter 3, 47 pages; `IPCC/IPCC-2024-Land-Representation-Guide.pdf`, the IPCC Inventory Software land representation guidebook of 6 April 2024, 124 pages; `Satellites/UNFCCC-2023-Tier-1-2-3-Guide.pdf`, the UNFCCC review training course B5 on land use, land-use change and forestry, first edition, September 2023, 281 pages; and `FCFP/FCPF_Monte-Carlo-Guidelines-2021.pdf`, the FCPF guidance note on Monte Carlo uncertainty, Version 1.0, September 2021, 33 pages.

## Citability warnings

These were found on 2026-09-17 by reading the first 600 bytes of every file in `/Volumes/PortableSSD/Github/markdown-resources/`.

| File in `markdown-resources/` | Problem |
|---|---|
| `IPCC-2019-V4-Ch6-Grassland.md` | Not the IPCC text. It is a 7.5 KB paraphrase that opens "You can copy the content inside the code block below". |
| `IPCC-2013-Wetlands-Supplement-Ch.5.md` | A superseded draft, stamped "DO NOT CITE OR QUOTE DRAFT" in its first line. |
| `IPCC-2013-Wetlands-Supplement-Ch.1.md` | 864 KB against 47 KB for the Chapter 1 file in `ipcc-carbon-gains`, so it holds more than Chapter 1. |
| `ISO-14064-1-2018.md`, `ISO-14064-3-2019.md` | Empty, 0 bytes. |

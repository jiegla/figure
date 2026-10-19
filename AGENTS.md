# Codex Instructions: Figure Reference Library

Use this repository as a visual and methodological reference for clinical research, translational oncology, single-cell analysis, and spatial omics. It is not a source of data for the current analysis.

## Required workflow

1. Read `README.md` and identify the closest category.
2. Search and actually inspect relevant examples before designing a new figure. Do not claim an image was inspected unless it was accessible and viewed.
3. Check `sources/figure_index.csv` and source notes for citations and reuse conditions.
4. Borrow layout, visual hierarchy, color logic, legend/axis design, and annotation style—not values, sample sizes, P values, conclusions, or patient data.
5. If no relevant example exists, say so and apply established scientific visualization principles.
6. In the final response, briefly identify the reference(s) used when useful.

## Scientific integrity

- Use only the current project's data and validated analysis results. Never invent or copy results from a reference image.
- Preserve group definitions, time points, units, denominators, sample sizes, missing-data handling, and statistical methods.
- Do not add unsupported significance annotations or overstate association, prediction, or causality.
- Avoid misleading axes/scales; label transformations and units clearly.
- For survival plots, verify time/event definitions and, where appropriate, include numbers at risk, censor marks, HR and confidence intervals.
- For cell-composition plots, clearly state whether the denominator is all cells, a parent population, or per-sample fractions. Do not treat cells as independent biological replicates.
- For UMAP, DotPlot, heatmap, GSEA, trajectory, and communication plots, preserve interpretable legends and avoid overcrowding.

## Style and export defaults

Follow explicit task/project instructions first. Otherwise:
- Use the project's existing language and plotting framework; use R/ggplot2 and Seurat ecosystem for R projects, or Python/Scanpy for Python projects.
- When appropriate for publication, export PDF plus PNG (300 dpi), keeping dimensions consistent across related figures.
- Prefer vector output for text and ordinary shapes. Rasterize only dense layers when supported.
- Keep typography, line widths, panel labels, margins, and legend styles consistent.
- Default binary colors only if the project has no palette: Positive `#B2182B`, Negative `#999999`, Missing `#D9D9D9`. Do not silently override established biological or clinical meanings.
- Save plotting code and key parameters for reproducibility.

## Copyright and privacy

- A reference image is not automatically licensed for redistribution. Check source records and license terms.
- Do not upload full papers, patient identifiers, identifiable images, credentials, or confidential unpublished data without authorization.
- If license status is unknown, record `unknown`; do not imply permission.
- Do not overwrite reference assets without authorization; add new versions with clear filenames.

## Final checklist

- Scientific question, labels, units, groups, denominators, sample sizes, and statistics are correct.
- Text/legends are readable; panels align; nothing is clipped or overlapping.
- Colors are semantically appropriate and consistent.
- Output files open correctly in requested formats.
- Code and key settings are available for reproduction.
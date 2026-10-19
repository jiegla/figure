# Subcluster proportions across samples

**Expected figure file:** `All_lineages_subcluster_heatmap_percent_parent_NR_R_column_clustered.pdf`

**Status:** Metadata registered; the binary PDF still needs to be uploaded to this folder.

## Figure summary

- **Domain:** Single-cell analysis
- **Category:** Cell composition / subtype proportions
- **Plot type:** Heatmap with hierarchically clustered sample columns and clinical annotation tracks
- **Content:** 41 subtypes across 7 lineages, 10 capture samples, and 7 patients
- **Denominator:** Within-parent lineage percentage = subtype cells / all retained cells of the same lineage in the same sample × 100
- **Sample selection:** NR_R-complete samples only; R is defined in the source figure as shrinkage ≥40%
- **Scope notes:** Endothelial cells excluded; epithelial cells retained; no row clustering or imputation; NR_R is annotation only
- **Clinical annotation tracks:** Patient, time (pre/post), MPR, pCR, ORR, and pathological response

## What Codex can learn from this reference

- Combining subtype composition heatmaps with multiple clinical annotation tracks
- Grouping rows by major lineage and adding a lineage color bar
- Clustering samples while preserving the source order of subtype rows
- Using a continuous color scale with values printed in cells
- Presenting a compact legend and explanatory footnotes beside the heatmap

## Interpretation cautions

- Percentages use the parent lineage within each sample as the denominator; they are not percentages of all cells.
- Missing values can represent missing clinical data or an absent parent lineage, as noted in the source figure.
- Use the reference for visual design only. Do not reuse its values, sample identifiers, or clinical annotations in another analysis.
- The source PDF notes that exact values and parent counts are available in an associated Excel workbook; that workbook was not included with this upload.

## Source and permission

Source: PDF supplied by the user in this conversation. Publication citation, DOI, and redistribution permission were not provided; verify before public redistribution if this is a figure from a manuscript or publication.

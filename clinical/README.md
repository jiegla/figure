# 临床科研图形参考导航

按**图形结构**选择主分类，再按治疗组、终点或生物标志物检索。以下为 2026-11-06 收录的 **7 个独立示例、11 个原始文件**；同名 PDF/PNG 是同一示例的两种格式，不算两张独立图。

## 已收录示例

| 原图号 | 识别类型 | 主归档目录 | 原件 | 分析与绘图说明 |
| --- | --- | --- | --- | --- |
| Figure_1A | 四治疗组客观缓解率（ORR）柱状图 | [04_treatment_response](04_treatment_response/) | [PDF](04_treatment_response/20261106_clinical_orr-bar_four-treatment-groups_Figure_1A_v01.pdf) | [说明](04_treatment_response/20261106_clinical_orr-bar_four-treatment-groups_Figure_1A_v01.md) |
| Figure_1C | 四治疗组 PFS Kaplan–Meier 生存曲线 | [03_survival_analysis](03_survival_analysis/) | [PDF](03_survival_analysis/20261106_clinical_km-pfs_four-treatment-groups_Figure_1C_v01.pdf) / [PNG](03_survival_analysis/20261106_clinical_km-pfs_four-treatment-groups_Figure_1C_v01.png) | [说明](03_survival_analysis/20261106_clinical_km-pfs_four-treatment-groups_Figure_1C_v01.md) |
| Figure_2A | 按 PD-L1 三分组的 OS Kaplan–Meier 曲线 | [03_survival_analysis](03_survival_analysis/) | [PDF](03_survival_analysis/20261106_clinical_km-os_pdl1-three-strata_Figure_2A_v01.pdf) / [PNG](03_survival_analysis/20261106_clinical_km-os_pdl1-three-strata_Figure_2A_v01.png) | [说明](03_survival_analysis/20261106_clinical_km-os_pdl1-three-strata_Figure_2A_v01.md) |
| Figure_S6A | TP53 变异状态与 PFS 的双组 KM 曲线 | [03_survival_analysis](03_survival_analysis/) | [PNG](03_survival_analysis/20261106_clinical_km-pfs_tp53-alteration_Figure_S6A_v01.png) | [说明](03_survival_analysis/20261106_clinical_km-pfs_tp53-alteration_Figure_S6A_v01.md) |
| Figure_S4A | 多基因变异与 PFS 关联的 Cox 森林图 | [05_forest_plots_subgroup](05_forest_plots_subgroup/) | [PDF](05_forest_plots_subgroup/20261106_clinical_cox-forest_gene-alteration-pfs_Figure_S4A_v01.pdf) / [PNG](05_forest_plots_subgroup/20261106_clinical_cox-forest_gene-alteration-pfs_Figure_S4A_v01.png) | [说明](05_forest_plots_subgroup/20261106_clinical_cox-forest_gene-alteration-pfs_Figure_S4A_v01.md) |
| Figure_4A | 伴随基因变异谱与临床注释 Oncoprint | [06_biomarkers](06_biomarkers/) | [PDF](06_biomarkers/20261106_clinical_oncoprint_genomic-alterations_Figure_4A_v01.pdf) / [PNG](06_biomarkers/20261106_clinical_oncoprint_genomic-alterations_Figure_4A_v01.png) | [说明](06_biomarkers/20261106_clinical_oncoprint_genomic-alterations_Figure_4A_v01.md) |
| Figure_4B | 基因变异频率的治疗组汇总热图 | [06_biomarkers](06_biomarkers/) | [PNG](06_biomarkers/20261106_clinical_frequency-heatmap_genes-by-treatment_Figure_4B_v01.png) | [说明](06_biomarkers/20261106_clinical_frequency-heatmap_genes-by-treatment_Figure_4B_v01.md) |

## 按任务选参考

- **多治疗组 PFS / OS 比较**：先看 Figure_1C；主要参考多组 KM 曲线、删失标记、置信带、风险表和总体检验的位置。
- **生物标志物分层生存**：三层变量看 Figure_2A，双组基因状态并展示 HR 看 Figure_S6A。这两张按 KM 结构收在生存分析目录，可从生物标志物目录交叉检索。
- **ORR / DCR 等应答比例比较**：看 Figure_1A 的分组柱形、分母和区间展示；先确认当前终点与区间定义。
- **逐基因 Cox 关联结果**：看 Figure_S4A 的对数 HR 轴、人数/事件数、CI、P 与 BH q 列。该图没有展示治疗×基因交互分析。
- **样本级基因变异谱**：看 Figure_4A 的 Oncoprint、治疗分块、临床注释和变异类型图例。
- **组水平基因变异频率**：看 Figure_4B 的百分比矩阵、列分母和数字注释。

## Codex 使用流程

1. 阅读根目录 [AGENTS.md](../AGENTS.md)，从本表选择图形，再实际打开对应原图和说明。
2. 查阅 [来源索引](../sources/figure_index.csv)；同一图的配对格式及校验值见 [原件清单](../sources/20261106_clinical_upload_manifest.json)。
3. 按说明列出的数据要求，核对当前项目的分析单位、终点、事件编码、分母、检测覆盖和缺失处理。
4. 参考布局、颜色映射、线型、图例与统计注释；统计方法须与当前数据及方案匹配，不能从图面补全未知设置。
5. 使用当前数据重新计算结果，保存代码与参数，适用时输出 PDF 和 300 dpi PNG；报告参考了哪个示例。

各图可能采用不同分析集，例如本批 ORR 与 PFS 中 Ivo + CT 的图面分母不同。保留这种区别，不能为了模仿版式而统一人数。不得从图像反推患者级原始数据来替代当前分析。

## 后续任务可直接使用的指令

> 请读取 jiegla/figure 的 AGENTS.md 和 clinical/README.md，选择与本次任务一致的图形示例，实际查看原图和配套说明。参考其布局与配色，使用我本次提供的数据重新分析和绘图。先核对终点、分组、事件编码、分母和缺失值，说明统计方法，并保存可复现代码及 PDF/PNG；不要沿用参考图的数值或结论。

## 其他临床分类

`01_cohort_flow` 队列流程；`02_baseline_characteristics` 基线特征；`07_prediction_models` 预测模型；`08_longitudinal_and_real_world` 纵向/真实世界；`09_clinical_trials_meta_analysis` 临床试验/Meta；`10_graphical_abstract` 图形摘要。本批没有归入这些目录的图片。

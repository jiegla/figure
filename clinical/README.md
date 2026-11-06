# 临床科研图形类型参考库

按**图形类型及关键结构**命名和检索，每种类型或关键子类型保留一个代表性示例。KM 曲线按两组、三组和四组区分；同一示例的 PDF/PNG 是配对格式，共用类型名称和一份说明。

## 类型导航

| 图形类型与说明 | 文件名 / 类型标识 | 原图 |
| --- | --- | --- |
| [应答率柱状图](04_treatment_response/response_rate_bar.md) | `response_rate_bar` | [PDF](04_treatment_response/response_rate_bar.pdf) |
| [四组 KM 生存曲线](03_survival_analysis/km_four_group.md) | `km_four_group` | [PDF](03_survival_analysis/km_four_group.pdf) / [PNG](03_survival_analysis/km_four_group.png) |
| [三组 KM 生存曲线](03_survival_analysis/km_three_group.md) | `km_three_group` | [PDF](03_survival_analysis/km_three_group.pdf) / [PNG](03_survival_analysis/km_three_group.png) |
| [双组 KM 生存曲线（附 Cox HR）](03_survival_analysis/km_two_group_cox.md) | `km_two_group_cox` | [PNG](03_survival_analysis/km_two_group_cox.png) |
| [Cox 关联森林图](05_forest_plots_subgroup/cox_association_forest.md) | `cox_association_forest` | [PDF](05_forest_plots_subgroup/cox_association_forest.pdf) / [PNG](05_forest_plots_subgroup/cox_association_forest.png) |
| [基因变异谱 Oncoprint](06_biomarkers/oncoprint.md) | `oncoprint` | [PDF](06_biomarkers/oncoprint.pdf) / [PNG](06_biomarkers/oncoprint.png) |
| [基因变异频率热图](06_biomarkers/gene_frequency_heatmap.md) | `gene_frequency_heatmap` | [PNG](06_biomarkers/gene_frequency_heatmap.png) |

文件名不使用论文图号、面板编号或研究专属名称。当前共 7 个类型/子类型示例、11 个原始格式文件。

## 根据任务选择

- **四组生存比较**：选 `km_four_group`，参考多组颜色和线型、置信带、删失标记、风险表与总体检验布局。
- **三组生存比较**：选 `km_three_group`，适用于三层标志物或其他三组变量。
- **双组生存比较并展示 HR**：选 `km_two_group_cox`，参考 Cox HR/CI、Cox P 与 log-rank P 的分开标注。
- **应答比例比较**：选 `response_rate_bar`，参考柱形、比例、分母和区间展示。
- **Cox 关联结果汇总**：选 `cox_association_forest`，参考对数 HR 轴及样本数、事件数、CI、P、BH q 列。
- **样本级变异模式**：选 `oncoprint`，参考矩阵、临床注释与变异类型图例。
- **组水平变异频率**：选 `gene_frequency_heatmap`，参考百分比矩阵、数字注释和分母。

## Codex 使用流程

1. 阅读根目录 [AGENTS.md](../AGENTS.md)，按类型选择示例，实际查看原图和同名 Markdown 说明。
2. 查阅 [来源索引](../sources/figure_index.csv) 与 [原件校验清单](../sources/20261106_clinical_upload_manifest.json)。原上传文件名仅用于来源追溯。
3. 根据说明核对当前项目的数据结构、分析单位、终点、事件编码、分母、检测覆盖和缺失处理。
4. 借鉴布局、颜色、线型、图例与注释，用当前数据重新计算结果；原例的 PFS/OS、基因名称和治疗组是示例背景，不限定类型的适用范围。
5. 保存可复现代码与参数，适用时输出 PDF 和 300 dpi PNG，并报告所用图形类型。

不同类型的示例可以采用不同分析集，不能为了统一视觉效果而改动人数或分母。方法设置应以当前方案与数据为准，不从图面猜测未知设置。

## 添加或更新示例

- 先检查是否已有相应类型，默认每种类型/关键子类型只保留一个代表性示例。
- 只有关键结构不同才新增子类型；更换终点、基因或论文图号不自动构成新类型。
- 使用小写英文和下划线命名，PDF、PNG 与说明文件共用文件名主体。
- 更新示例时保持导航、来源索引、说明与校验清单一致；历史版本可通过 Git 追溯。

## 后续可直接使用的指令

> 请从 jiegla/figure 的 clinical/README.md 选择四组 KM 生存曲线类型，查看原图和说明，参考其布局与配色，用我本次的数据完成分析和绘图，并输出可复现代码及 PDF/PNG。

## 其他临床分类

`01_cohort_flow` 队列流程；`02_baseline_characteristics` 基线特征；`07_prediction_models` 预测模型；`08_longitudinal_and_real_world` 纵向/真实世界；`09_clinical_trials_meta_analysis` 临床试验/Meta；`10_graphical_abstract` 图形摘要。

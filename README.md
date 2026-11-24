# Awesome Clinical Pharmacokinetics & Pharmacometrics (ClinPharm & PMx)

> 面向临床药代动力学（Clinical Pharmacokinetics）与定量药理学（Pharmacometrics）的多语种开源工具目录，按解决的具体科学或工程问题归类，覆盖英、中、日、韩、德、法、西、葡、意等生态。  
> A curated, problem-oriented, multi-lingual directory of open-source GitHub repositories for Clinical Pharmacokinetics (Clin. Pharm.) and Pharmacometrics (PMx), spanning English, Chinese, Japanese, Korean, German, French, Spanish, Portuguese, and Italian ecosystems.

---

## 目录 / Contents

- [1. NONMEM / Monolix / Phoenix 工作流自动化与算力运维 / Workflow & Orchestration](#1-nonmem--monolix--phoenix-工作流自动化与算力运维--workflow--orchestration)
- [2. 开源 PopPK / PopPKPD / QSP 建模与 ODE 仿真引擎 / Open-Source Modeling & ODE Engines](#2-开源-poppk--poppkpd--qsp-建模与-ode-仿真引擎--open-source-modeling--ode-engines)
- [3. 数据准备、CDISC 转换与数据质控 / Data Preparation, CDISC & QC](#3-数据准备cdisc-转换与数据质控--data-preparation-cdisc--qc)
- [4. 非房室分析（NCA）与生物等效性（BE）/ NCA & Bioequivalence](#4-非房室分析nca与生物等效性be--nca--bioequivalence)
- [5. 模型诊断、可视化与自动化报告 / Diagnostics, Visualization & Reporting](#5-模型诊断可视化与自动化报告--diagnostics-visualization--reporting)
- [6. 暴露-效应（E-R）、肿瘤 TGI、CTS、最优设计与 FIH / E-R, Oncology TGI, CTS, Optimal Design & FIH](#6-暴露-效应e-r肿瘤-tgicts最优设计与-fih--e-r-oncology-tgi-cts-optimal-design--fih)
- [7. 模型引导精准给药（MIPD）、临床 TDM 与围术期 TCI / Clinical MIPD, TDM & TCI](#7-模型引导精准给药mipd临床-tdm-与围术期-tci--clinical-mipd-tdm--tci)
  - [7.1 通用贝叶斯 / MIPD 引擎与外部验证 / General MIPD Engines & Validation](#71-通用贝叶斯--mipd-引擎与外部验证--general-mipd-engines--validation)
  - [7.2 特定药物临床 TDM 与合理用药 / Drug-Specific TDM & Clinical Dosing](#72-特定药物临床-tdm-与合理用药--drug-specific-tdm--clinical-dosing)
  - [7.3 围术期麻醉 / ICU 靶控输注（TCI）/ Anesthesia & ICU TCI Simulators](#73-围术期麻醉--icu-靶控输注tci--anesthesia--icu-tci-simulators)
  - [7.4 多房室血药浓度追踪与动态校准 / Multi-Compartment Tracking & Dynamic Calibration](#74-多房室血药浓度追踪与动态校准--multi-compartment-tracking--dynamic-calibration)
- [8. 生理药代动力学（PBPK）、IVIVE、DDI 与特殊人群 / PBPK, IVIVE, DDI & Special Populations](#8-生理药代动力学pbpkiviveddi-与特殊人群--pbpk-ivive-ddi--special-populations)
- [9. AI / LLM / MCP 智能体、知识抽取与开源教材 / AI Agents, Data Mining & Open Textbooks](#9-ai--llm--mcp-智能体知识抽取与开源教材--ai-agents-data-mining--open-textbooks)
  - [9.1 AI Agent、MCP、RAG 与数据挖掘 / AI Agents, MCP, RAG & Data Mining](#91-ai-agentmcprag-与数据挖掘--ai-agents-mcp-rag--data-mining)
  - [9.2 多语种开源教材与代码库 / Multi-Lingual Open Textbooks & Workshops](#92-多语种开源教材与代码库--multi-lingual-open-textbooks--workshops)

---

## 1. NONMEM / Monolix / Phoenix 工作流自动化与算力运维 / Workflow & Orchestration

- [UUPharmacometrics/PsN](https://github.com/UUPharmacometrics/PsN) `(Perl)` — NONMEM 自动化工作流核心工具集（Bootstrap、SCM、VPC、SIR）。 / Core CLI toolkit automating NONMEM workflows (bootstrapping, SCM, VPC, SIR).
- [metrumresearchgroup/bbi](https://github.com/metrumresearchgroup/bbi) `(Go)` — 跨平台、支持本地与 Slurm/SGE 集群的 NONMEM 高速执行引擎。 / Cross-platform, scheduler-agnostic CLI execution engine for NONMEM runs (local, Slurm, SGE).
- [metrumresearchgroup/bbr](https://github.com/metrumresearchgroup/bbr) `(R)` — 基于 `bbi` 的 R 语言建模管理包，实现 NONMEM/Stan 模型谱系追踪与审计日志。 / R package for NONMEM/Stan run management, model ancestry tracking, and reproducible run logs.
- [metrumresearchgroup/nmrec](https://github.com/metrumresearchgroup/nmrec) `(R)` — 精准解析与修改 NONMEM 控制流记录与缩写语法的底层库。 / Low-level R parser and serializer for programmatically reading and editing NONMEM control streams.
- [nlmixr2/babelmixr2](https://github.com/nlmixr2/babelmixr2) `(R)` — 将统一 `nlmixr2`/`rxode2` 模型转译并在 NONMEM、Monolix、PKNCA、PopED 上运行。 / Cross-engine bridge translating `nlmixr2`/`rxode2` models to NONMEM, Monolix, PKNCA, and PopED.
- [certara/R-RsNLME](https://github.com/certara/R-RsNLME) `(R)` — 用可复现的 tidyverse R 脚本替代 GUI 操作调用 Phoenix NLME 引擎。 / Scriptable tidyverse-style R interface for running the Phoenix NLME estimation engine.
- [a2-ai/slurmtools](https://github.com/a2-ai/slurmtools) `(R)` — 在 R 定量药理环境中直接提交、监控和管理 Slurm HPC 集群任务。 / R utilities for submitting, monitoring, and managing Slurm HPC jobs directly from R.
- [billdenney/Pharmacometrics-Docker](https://github.com/billdenney/Pharmacometrics-Docker) `(Docker)` — 标准化多版本 NONMEM（含 gfortran）与 PsN 的 Docker 容器化部署配置。 / Community Dockerfiles for reproducible multi-version NONMEM and PsN deployments.
- [kinginsun/nonmem](https://github.com/kinginsun/nonmem) `(Docker/Shell)` — 跨平台（Win/macOS Apple Silicon/Linux）NONMEM + PsN + MPICH 容器镜像与一键封装脚本。 / Cross-platform Docker setup and wrapper scripts for NONMEM, PsN, and MPICH parallel execution.
- [FelicienLL/runnonmem](https://github.com/FelicienLL/runnonmem) `(R)` — 轻量级 R 封装工具，用于从 R 脚本直接调用运行 NONMEM。 / Lightweight R wrapper for invoking NONMEM directly from R scripts.
- [s0521/nonmem_cn](https://github.com/s0521/nonmem_cn) `(TS | 中文)` — NONMEM 控制文件 VS Code 扩展，提供语法高亮、自动补全与中英双语注释提示。 / VS Code extension for NONMEM control files with syntax highlighting, snippets, and bilingual CN/EN tooltips.
- [TingjieGuo/MINGA](https://github.com/TingjieGuo/MINGA) `(Hugo/Shell | 中文)` — 面向中文用户的 NONMEM、PsN、Pirana 与 R 定量药理环境安装教程与脚本。 / Chinese-language installation guide and shell scripts for NONMEM, PsN, Pirana, and R PMx tools.
- [Slow-Walker66/PPK-workbench-assistance-demo](https://github.com/Slow-Walker66/PPK-workbench-assistance-demo) `(TS | 中英)` — 本地优先的 NONMEM+PsN 群体药动学工作台（Pirana 开源替代），含模型树、诊断与报告生成。 / Local-first PopPK workbench (Pirana alternative) for NONMEM+PsN with model lineage, diagnostics, and reporting.

---

## 2. 开源 PopPK / PopPKPD / QSP 建模与 ODE 仿真引擎 / Open-Source Modeling & ODE Engines

- [nlmixr2/nlmixr2](https://github.com/nlmixr2/nlmixr2) `(R/C++)` — 开源 CRAN 级非线性混合效应（NLME）建模框架，支持 FOCE-I 与 SAEM。 / Open-source R framework for population PK/PD NLME modeling (FOCE-I, SAEM, nlme).
- [nlmixr2/rxode2](https://github.com/nlmixr2/rxode2) `(R/C/C++)` — 将药动学 ODE 模型编译为 C 代码并支持 NONMEM 风格事件表的高速仿真引擎。 / High-speed C-compiled ODE solver and clinical trial simulator with NONMEM-style event tables.
- [nlmixr2/nlmixr2lib](https://github.com/nlmixr2/nlmixr2lib) `(R)` — 标准化临床 PopPK/PD 文献模型库，可直接供 `nlmixr2`/`rxode2` 调用。 / Curated library of published clinical PopPK/PD models ready for `nlmixr2` and `rxode2`.
- [metrumresearchgroup/mrgsolve](https://github.com/metrumresearchgroup/mrgsolve) `(R/C++)` — 类 NONMEM 语法的 C++ 编译型分层 ODE 仿真引擎，广泛用于 PopPK/PBPK/QSP。 / Fast C++-compiled hierarchical ODE simulator in R with NONMEM-inspired syntax for PopPK/PBPK/QSP.
- [InsightRX/PKPDsim](https://github.com/InsightRX/PKPDsim) `(R/C++)` — 面向临床精准给药的 C++ 编译型 ODE 与解析房室 PK/PD 仿真引擎。 / Compiled C++ ODE and analytical PK/PD simulator tailored for clinical precision dosing.
- [john-harrold/ubiquity](https://github.com/john-harrold/ubiquity) `(R)` — 统一 PK/PD、PBPK 与 QSP 建模、参数估计、自动 Word/PPT 报告与 Shiny GUI 生成的框架。 / End-to-end R modeling framework generating simulations, estimates, Word/PPT reports, and Shiny apps.
- [pharmpy/pharmpy](https://github.com/pharmpy/pharmpy) `(Python)` — 现代 Python 药动学模型抽象层与自动化模型构建（AMD）工具，跨 NONMEM 与 `nlmixr2`。 / Python pharmacometrics library and Automated Model Development (AMD) tool across NONMEM and `nlmixr2`.
- [metrumresearchgroup/Torsten](https://github.com/metrumresearchgroup/Torsten) `(C++/Stan)` — 扩展 Stan 数学库以支持自动微分房室解析解、ODE 求解器与 NMTRAN 给药事件。 / Stan extension library providing pharmacometric compartmental/ODE solvers and NMTRAN events for Bayesian PopPK/PD.
- [iame-researchCenter/saemix](https://github.com/iame-researchCenter/saemix) `(R)` — 开源 R 语言随机逼近期望最大化（SAEM）非线性混合效应建模包。 / Open-source R implementation of the SAEM algorithm for NLME population PK/PD modeling.
- [MarcLavielle/mlxR](https://github.com/MarcLavielle/mlxR) `(R)` — 面向混合效应模型的纵向 PopPK/PD 仿真与可视化包，衔接 Monolix/Simulx 生态。 / Longitudinal PopPK/PD simulation and visualization package interfacing with Monolix/Simulx.
- [LAPKB/Pmetrics](https://github.com/LAPKB/Pmetrics) `(R/Rust)` — 支持非参数与参数群体 PK/PD 建模及贝叶斯 MAP/MMopt 最优给药估计的引擎。 / Non-parametric and parametric PopPK/PD modeling and Bayesian dosing engine powered by Rust.
- [DavAug/chi](https://github.com/DavAug/chi) `(Python)` — 纯 Python 机制性 ODE PK/PD、QSP 与贝叶斯 MIPD 分层推断框架。 / Native Python framework for mechanistic ODE PK/PD, QSP, and hierarchical Bayesian MIPD inference.
- [shramish2057/NeoPKPD](https://github.com/shramish2057/NeoPKPD) `(Julia/Python)` — 结合 Julia 高速核心与 Python API/CLI 的开源 PK/PD、NLME、NCA 与 BE 平台。 / Multi-language (Julia core + Python API/CLI) platform for PK/PD simulation, NLME, NCA, and BE.
- [TommyGiak/pharmacoNODE](https://github.com/TommyGiak/pharmacoNODE) `(Python/PyTorch)` — 将神经常微分方程（Neural ODE）应用于 Monolix/NONMEM 风格纵向临床 PK 预测。 / Neural ODE codebase for longitudinal PK concentration-time prediction with patient covariates.
- [Janssena/DeepCompartmentModels.jl](https://github.com/Janssena/DeepCompartmentModels.jl) `(Julia)` — 深度房室模型（DCM），在房室 ODE 结构约束下用神经网络学习协变量-参数关系。 / Deep Compartment Models combining compartmental ODE constraints with neural networks for covariate learning.
- [wahlquisty/learning-pharmacometric-covariate-structures](https://github.com/wahlquisty/learning-pharmacometric-covariate-structures) `(Julia)` — 基于神经网络符号回归自动发现群体药动学协变量数学结构。 / Neural symbolic regression prototype for automated pharmacometric covariate structure discovery.
- [liucann/PKparmas1.0](https://github.com/liucann/PKparmas1.0) `(Python/Streamlit | 中文)` — 轻量级中文在线房室模型药代动力学参数拟合 Web 工具。 / Lightweight Chinese Streamlit web app for interactive compartmental PK parameter fitting from Excel data.
- [SnowLeopard-io/ErgalicsStudio](https://github.com/SnowLeopard-io/ErgalicsStudio) `(TS/WebGPU | 中英)` — 浏览器端高性能科学计算工作台，内置药代动力学室分析、DDI 与 TDM 曲线拟合插件。 / Browser-based WebGPU/Wasm scientific studio with built-in PK compartmental, DDI, and TDM simulation plugins.

---

## 3. 数据准备、CDISC 转换与数据质控 / Data Preparation, CDISC & QC

- [NMautoverse/NMdata](https://github.com/NMautoverse/NMdata) `(R)` — 全链路 NONMEM 数据集准备、结构 QC、排除标记审计与运行结果自动合并工具。 / End-to-end NONMEM dataset prep, structural QC (`NMcheckData`), exclusion tracking, and output merging.
- [metrumresearchgroup/mrgda](https://github.com/metrumresearchgroup/mrgda) `(R)` — 整合多源临床试验域并派生标准定量药理分析数据集的装配工具包。 / Data assembly toolkit for consolidating clinical trial domains into modeling-ready PMx datasets.
- [metrumresearchgroup/yspec](https://github.com/metrumresearchgroup/yspec) `(R)` — 基于 YAML 的定量药理数据规范管理、自动校验与 `define.pdf` 文档生成工具。 / YAML-based PMx dataset specification manager for automated validation, labeling, and `define.pdf` generation.
- [pharmaverse/admiral](https://github.com/pharmaverse/admiral) `(R)` — Pharmaverse 模块化 CDISC ADaM 构建工具箱，内置 `ADPC`/`ADPP`/`ADPPK` 派生模板。 / Modular pharmaverse toolbox for building CDISC ADaM datasets including `ADPC`, `ADPP`, and `ADPPK`.
- [kestrel99/pmxTools](https://github.com/kestrel99/pmxTools) `(R)` — 涵盖数据处理、闭式房室 PK 计算与 PsN/NONMEM 输出解析制表的实用工具集。 / Practical R utility suite for PMx data manipulation, closed-form PK math, and PsN output parsing.

---

## 4. 非房室分析（NCA）与生物等效性（BE）/ NCA & Bioequivalence

- [humanpred/pknca](https://github.com/humanpred/pknca) `(R)` — 全功能稀疏与密集采样非房室分析（NCA）引擎，支持自动单位换算与 CDISC 输出。 / Comprehensive R engine for dense and sparse NCA with unit conversion, imputation, and CDISC support.
- [pharmaverse/aNCA](https://github.com/pharmaverse/aNCA) `(R/Shiny)` — 端到端交互式临床 NCA Web 应用，支持交互式 $\lambda_z$ 选点、CDISC 导出与可复现脚本生成。 / Interactive pharmaverse Shiny app for clinical NCA with visual $\lambda_z$ selection and reproducible R script export.
- [asancpt/NonCompart](https://github.com/asancpt/NonCompart) `(R | 韩国)` — 算法对齐 Phoenix WinNonlin 与 CDISC SDTM 的工业级 NCA 核心计算包。 / Industrial-strength R NCA package aligned with Phoenix WinNonlin formulas and CDISC SDTM conventions.
- [asancpt/ncar](https://github.com/asancpt/ncar) `(R | 韩国)` — 基于 `NonCompart` 一键生成含个体药时曲线的监管级 PDF/RTF NCA 报告。 / Regulatory-style PDF and RTF NCA report generator built on top of `NonCompart`.
- [asancpt/pkrshiny](https://github.com/asancpt/pkrshiny) `(R/Shiny | 韩英)` — 封装 `pkr`/`NonCompart` 的免代码交互式非房室分析 Shiny 网页应用。 / No-code interactive Shiny web interface for running noncompartmental PK analysis.
- [asancpt/BE-apps](https://github.com/asancpt/BE-apps) `(R/Shiny | 韩英)` — 集成非房室分析与生物等效性（BE）统计评估的交互式 Shiny 应用。 / Interactive Shiny application integrating PK noncompartmental analysis with bioequivalence statistics.
- [Detlew/PowerTOST](https://github.com/Detlew/PowerTOST) `(R | 德/奥)` — 行业标准生物等效性统计功效与样本量计算包（TOST、ABE、RSABE、ABEL）。 / Industry-standard R package for bioequivalence power and sample size calculations (TOST, RSABE, ABEL).
- [Helmut01/replicateBE](https://github.com/Helmut01/replicateBE) `(R)` — 遵循 EMA 指南（Method A/B）的高变异药物重复交叉设计 ABEL 生物等效性评价包。 / EMA-aligned ABEL bioequivalence evaluation package for replicate crossover designs of highly variable drugs.
- [juntotechnologies/bioeq](https://github.com/juntotechnologies/bioeq) `(Python)` — 纯 Python 生物等效性（BE）计算包，支持交叉与平行试验设计。 / Pure-Python package for pharmacokinetic data processing and crossover/parallel bioequivalence statistics.
- [PharmCat/MetidaNCA.jl](https://github.com/PharmCat/MetidaNCA.jl) `(Julia)` — 面向药物研发与大规模临床试验仿真后处理的高性能 Julia NCA 库。 / High-performance Julia NCA library suited for drug development and large-scale trial simulation post-processing.
- [matthiaskoenig/pkpdutils](https://github.com/matthiaskoenig/pkpdutils) `(Python | 德国)` — 支持单位感知 NCA、NONMEM/Monolix/ADNCA 读写、曲线拟合、BE 统计与 DDI 分级的 Python 库。 / Pure-Python PK/PD analysis library supporting unit-aware NCA, NONMEM/ADNCA I/O, curve fitting, BE, and DDI.
- [Shipbuilder/Bioequivalence](https://github.com/Shipbuilder/Bioequivalence) `(Scripts | 中文)` — 中文开发者上传的生物等效性（BE）试验统计分析参考脚本。 / Chinese-language statistical reference scripts for bioequivalence studies.

---

## 5. 模型诊断、可视化与自动化报告 / Diagnostics, Visualization & Reporting

- [UUPharmacometrics/xpose](https://github.com/UUPharmacometrics/xpose) `(R)` — 现代 `ggplot2` 模型诊断框架，用于导入 NONMEM 输出并绘制 GOF、残差与 VPC 图。 / Modern `ggplot2`-based diagnostics framework for NONMEM/NLME goodness-of-fit and VPC plots.
- [ggPMXdevelopment/ggPMX](https://github.com/ggPMXdevelopment/ggPMX) `(R)` — 跨 Monolix、NONMEM、`nlmixr2` 一键生成符合 ISoP 标准的申报级 GOF 诊断图与报告。 / Standardized ISoP-aligned GOF diagnostic plotting and reporting across Monolix, NONMEM, and `nlmixr2`.
- [certara/tidyvpc](https://github.com/certara/tidyvpc) `(R)` — 基于 `data.table` 的高速管道式 VPC 引擎，支持分箱、无分箱（AQR/LOESS）、pcVPC 与 BLQ。 / Fast `data.table`-backed VPC engine supporting binned/binless (AQR/LOESS) VPCs, pcVPC, and BLQ censoring.
- [UUPharmacometrics/ncappc](https://github.com/UUPharmacometrics/ncappc) `(R)` — 基于 NCA 暴露指标（$C_{max}$、$AUC$）对 PopPK/PD 模型执行后验预测检验（PPC）。 / Simulation-based posterior predictive check (PPC) evaluating PopPK/PD models via NCA exposure metrics.
- [pharmetheus/PMXForest](https://github.com/pharmetheus/PMXForest) `(R)` — 直接从 NONMEM `.cov`、PsN Bootstrap 或 SIR 输出自动生成含不确定性的协变量森林图。 / Automated covariate forest plots with uncertainty directly from NONMEM `.cov`, PsN bootstrap, or SIR outputs.
- [certara/coveffectsplot](https://github.com/certara/coveffectsplot) `(R/Shiny)` — 提供函数与交互式 Shiny 应用，绘制申报级协变量暴露影响森林图。 / R package and Shiny app for producing standardized covariate-effect forest plots in PopPK/PD reports.
- [Novartis/xgxr](https://github.com/Novartis/xgxr) `(R)` — 诺华探索性图形（xGx）框架，提供标准化 PK/PD 与暴露-效应作图助手与草稿标注。 / Novartis exploratory graphics (`ggplot2`) helpers for reproducible PK/PD and exposure-response plotting.
- [metrumresearchgroup/pmtables](https://github.com/metrumresearchgroup/pmtables) `(R)` — 专为定量药理申报报告打造的 LaTeX/TeX 人口学、数据清单与参数估计表格生成器。 / Publication- and submission-grade LaTeX summary table generator tailored for pharmacometric reports.
- [kylebaron/mrgsim.sa](https://github.com/kylebaron/mrgsim.sa) `(R)` — 面向 `mrgsolve` 模型的局部与序列参数敏感度分析及可视化扩展包。 / Local and graphical parameter sensitivity analysis extension for `mrgsolve` PK/PD and QSP models.
- [nlmixr2/nlmixr2rpt](https://github.com/nlmixr2/nlmixr2rpt) `(R)` — 基于 YAML 规范自动将 `nlmixr2` 拟合结果生成结构化 Word 与 PPT 定量药理报告。 / YAML-driven automated Microsoft Word and PowerPoint report generator for `nlmixr2` model fits.
- [john-harrold/ruminate](https://github.com/john-harrold/ruminate) `(R/Shiny)` — 整合数据整理、绘图、PKNCA、`rxode2` 仿真与 Office 报告导出的低代码 Shiny 工作台。 / Modular Shiny PMx workbench combining data wrangling, PKNCA, `rxode2` simulation, and Word/PPT/Excel reporting.
- [Genentech/gPKPDviz](https://github.com/Genentech/gPKPDviz) `(R/Shiny)` — 基因泰克开源的交互式 `mrgsolve` PopPK/PD 仿真与虚拟人群探索 Shiny 平台。 / Interactive `mrgsolve`-powered Shiny platform for real-time PopPK/PD simulation and virtual population exploration.
- [Boehringer-Ingelheim/MVPapp](https://github.com/Boehringer-Ingelheim/MVPapp) `(R/Shiny | 德国)` — 支持在线编辑 `mrgsolve` 代码、NCA、敏感度分析与 NHANES 虚拟人群的模型可视化平台。 / Model Visualization Platform (Shiny) with live `mrgsolve` editing, NCA, sensitivity analysis, and NHANES demographics.
- [pipetcpt/2025-jscpt](https://github.com/pipetcpt/2025-jscpt) `(R/NONMEM | 韩/日)` — 直接从 NONMEM 输出自动生成项目反应理论（IRT）纵向药效模型发表级信息图。 / Automated publication-grade pharmacometric infographic generator from NONMEM IRT model outputs.

---

## 6. 暴露-效应（E-R）、肿瘤 TGI、CTS、最优设计与 FIH / E-R, Oncology TGI, CTS, Optimal Design & FIH

- [Genentech/BayesERtools](https://github.com/Genentech/BayesERtools) `(R/Stan)` — 基因泰克开源贝叶斯暴露-效应（E-R）建模工具包，支持二分类/连续终点与决策森林图。 / Bayesian exposure-response modeling toolkit over Stan for binary/continuous endpoints and decision forest plots.
- [metrumresearchgroup/confounded-exposure-metrics](https://github.com/metrumresearchgroup/confounded-exposure-metrics) `(R/NONMEM)` — 揭示肿瘤 E-R 与生存分析（TTE）中不同暴露指标引入混杂偏倚的仿真方法学仓库。 / Methodological simulation pipeline demonstrating exposure-metric confounding bias in oncology E-R and TTE analyses.
- [clay-good/onkos](https://github.com/clay-good/onkos) `(Python)` — 分级标注的肿瘤生长抑制（TGI）与 E-R 模型库，支持导出至 NONMEM、SBML、`rxode2` 与 Pumas。 / Curated oncology TGI and E-R model library with transpilation to NONMEM, SBML, `rxode2`, and Pumas.
- [orlacchioresearch/tumor-growth-inhibition-modeling](https://github.com/orlacchioresearch/tumor-growth-inhibition-modeling) `(Python)` — 临床前异种移植瘤生长曲线拟合（指数/Gompertz/Logistic）与 TGI%/%T/C 计算工具。 / Python toolkit for preclinical xenograft tumor growth curve fitting and TGI% / %T/C calculation.
- [campsisverse/campsis](https://github.com/campsisverse/campsis) `(R)` — 引擎无关的临床试验仿真（CTS）平台，解耦试验设计与底层 `rxode2`/`mrgsolve` 求解器。 / Engine-agnostic clinical trial simulation (CTS) platform supporting both `rxode2` and `mrgsolve` backends.
- [andrewhooker/PopED](https://github.com/andrewhooker/PopED) `(R)` — 基于费雪信息矩阵（FIM）的 NLME 群体与个体最优临床采样与给药试验设计工具。 / Optimal experimental design for NLME models using the Fisher Information Matrix (FIM) to optimize sampling and dosing.
- [iame-researchCenter/PFIM](https://github.com/iame-researchCenter/PFIM) `(R | 法国)` — 基于群体 FIM 评估与优化 NLME 临床采样设计，支持协变量、IOV 与多种优化算法。 / Population FIM optimal design package supporting covariates, IOV, and Fedorov-Wynn/PSO optimization.
- [phuse-org/toxSummary](https://github.com/phuse-org/toxSummary) `(R/Shiny)` — 交互式汇总重复给药毒理暴露安全窗与跨种属转化，支撑首次人体（FIH）起始剂量论证。 / PHUSE Shiny app summarizing repeat-dose tox exposure margins and cross-species translation for FIH dose justification.
- [pipetcpt/DallphinAtoM](https://github.com/pipetcpt/DallphinAtoM) `(R | 韩英)` — 利用异速生长缩放与生理参数从临床前动物数据预测人体 PK 参数。 / Allometric scaling and physiological animal-to-human PK parameter prediction tool for early FIH projection.

---

## 7. 模型引导精准给药（MIPD）、临床 TDM 与围术期 TCI / Clinical MIPD, TDM & TCI

### 7.1 通用贝叶斯 / MIPD 引擎与外部验证 / General MIPD Engines & Validation

- [sotalya/tucuxi-core](https://github.com/sotalya/tucuxi-core) `(C++ | 瑞士/法)` — 医院验证的开源贝叶斯 TDM/MIPD 核心计算引擎，提供 CLI 与 REST 服务。 / Hospital-validated open-source Bayesian TDM/MIPD computing engine with CLI and REST server.
- [sotalya/tucuxi-gui](https://github.com/sotalya/tucuxi-gui) `(C++/Qt | 瑞士/法)` — 配套 `tucuxi-core` 的临床桌面端血药浓度解读与个体化调量图形界面。 / Clinical desktop GUI for interpreting drug concentrations and computing individualized dosage adaptations via Tucuxi.
- [sotalya/tucuxi-drugs](https://github.com/sotalya/tucuxi-drugs) `(XML | 瑞士/法)` — 供 Tucuxi 引擎调用的窄治疗窗药物开源 XML 群体药动学模型库。 / Open XML repository of population PK drug models for narrow-therapeutic-index drugs used by Tucuxi.
- [sotalya/tucuxi-python](https://github.com/sotalya/tucuxi-python) `(Python/C++ | 瑞士/法)` — `tucuxi-core` 的 Python 绑定，用于脚本化 PK 预测与批量回顾性 TDM 评估。 / Python bindings for `tucuxi-core` enabling scripted PK predictions and batch retrospective TDM evaluation.
- [levenc/posologyr](https://github.com/levenc/posologyr) `(R | 法国)` — 基于 `rxode2` 的开源 MIPD 包，提供贝叶斯 MAP 估计及目标 AUC/谷浓度最优剂量反推。 / `rxode2`-based MIPD package for MAP-Bayesian estimation and target AUC/trough dose optimization.
- [FelicienLL/mapbayr](https://github.com/FelicienLL/mapbayr) `(R | 法国)` — 基于 `mrgsolve` 模型实现亚秒级临床 TDM 贝叶斯 MAP 参数估计的轻量引擎。 / Lightweight, fast MAP-Bayesian estimation engine built on `mrgsolve` PopPK models for clinical TDM.
- [FelicienLL/mapbayr-shiny](https://github.com/FelicienLL/mapbayr-shiny) `(R/Shiny | 法国)` — 基于 `mapbayr` 的即用型贝叶斯 TDM 计算器 Shiny 应用模板集。 / Ready-to-deploy R Shiny application templates for building `mapbayr`-powered Bayesian TDM calculators.
- [InsightRX/PKPDmap](https://github.com/InsightRX/PKPDmap) `(R)` — 直接在 `PKPDsim` 模型对象上执行个体化 MAP 贝叶斯参数估计。 / Modular MAP-Bayesian parameter estimation engine operating directly on `PKPDsim` models.
- [InsightRX/PKPDposterior](https://github.com/InsightRX/PKPDposterior) `(R/Stan)` — 基于 Stan/Torsten 的全贝叶斯 MCMC 精准给药推断，量化个体暴露与毒性完整后验不确定性。 / Full-Bayesian MCMC inference via Stan/Torsten quantifying posterior uncertainty in individualized dosing predictions.
- [InsightRX/clinPK](https://github.com/InsightRX/clinPK) `(R)` — 封装经验证的临床药理标准公式（肾功能 eGFR/CG、体重指标 IBW/LBW/BSA 与基础房室方程）。 / Standardized clinical pharmacology equations for renal function, body weight descriptors, and basic PK math.
- [Martin-Umpierrez/exeval](https://github.com/Martin-Umpierrez/exeval) `(R)` — 自动化执行文献 PopPK/PD 模型在独立医院本地临床队列上的外部验证与贝叶斯预测评估。 / Reproducible external evaluation framework for benchmarking published PopPK/PD models on local hospital TDM cohorts.

### 7.2 特定药物临床 TDM 与合理用药 / Drug-Specific TDM & Clinical Dosing

- [liangRXdev/vanco-auc-calc](https://github.com/liangRXdev/vanco-auc-calc) `(JS/PWA | 繁中/英)` — 纯前端离线万古霉素 AUC 个体化计算器，含 Sawchuk-Zaske 双点反算、双室贝叶斯与 AKI/妊娠警示。 / Offline browser PWA for vancomycin AUC dosing with Sawchuk-Zaske, 2-compartment Bayesian MAP, and clinical alerts.
- [asancpt/shiny-vtdm](https://github.com/asancpt/shiny-vtdm) `(R/Shiny | 韩英)` — 韩国峨山医院万古霉素二室 PopPK 贝叶斯精准给药 Shiny 应用。 / Korean vancomycin TDM Shiny app implementing a 2-compartment PopPK Bayesian dosing model.
- [pipetcpt/tdm-vancomycin](https://github.com/pipetcpt/tdm-vancomycin) `(R/Shiny | 韩英)` — 韩国天主教大学 PIPET 万古霉素 PopPK 给药仿真与 TDM 自动化 Shiny 应用。 / Open-source Shiny app for vancomycin PopPK dosing simulation and TDM automation.
- [kpessa/vanco-auc](https://github.com/kpessa/vanco-auc) `(Excel/VBA)` — 美国医院实际部署的万古霉素经验给药与双点梯形法 AUC24/MIC 计算工具包。 / Hospital-deployed Excel/VBA toolkit for vancomycin empirical dosing and paired-level trapezoidal AUC24/MIC.
- [Yunwoolee17/Vancomycin_prediction_AI](https://github.com/Yunwoolee17/Vancomycin_prediction_AI) `(Python | 韩国)` — 融合多种树模型与 SHAP 可解释性预测万古霉素达标 AUC 起始剂量的机器学习流水线。 / ML pipeline with SHAP explainability predicting initial vancomycin doses to achieve target AUC (400–600 mg·h/L).
- [FelicienLL/BUSULFANAPP](https://github.com/FelicienLL/BUSULFANAPP) `(R/Shiny | 法国)` — 面向儿童造血干细胞移植（HSCT）患者的白消安（Busulfan）贝叶斯精准给药 Shiny 应用。 / `mapbayr`-powered Shiny application for model-informed precision dosing of busulfan in pediatric HSCT patients.
- [727397883/Rifampicin-PopPK-Repository](https://github.com/727397883/Rifampicin-PopPK-Repository) `(R/Shiny | 中国)` — 中南大学湘雅医院开源的抗结核药利福平 PopPK 文献模型库与 `mrgsolve` 给药模拟应用。 / Open-source rifampicin PopPK model repository and interactive `mrgsolve` Shiny dosing simulator.
- [wojjy001/infliximab-bayes](https://github.com/wojjy001/infliximab-bayes) `(R)` — 炎症性肠病（IBD）英夫利昔单抗维持治疗的贝叶斯预测与自适应给药仿真。 / Bayesian forecasting and adaptive dosing simulation for infliximab maintenance therapy in IBD.
- [karneslab/warfarin-machinelearning](https://github.com/karneslab/warfarin-machinelearning) `(R)` — 结合 CYP2C9/VKORC1 药物基因组学与临床协变量预测华法林维持剂量的机器学习代码。 / Machine learning scripts predicting stable warfarin maintenance doses using pharmacogenetic and clinical covariates.
- [cloveropen/pass](https://github.com/cloveropen/pass) `(Web | 中文)` — 临床合理用药监测系统（PASS）开源参考实现，含医嘱审方、四级风险警示与 DDI 审查。 / Open-source clinical prescription automatic screening system (PASS) with tiered alerts and DDI checks.
- [yusuketakuma/pharma-free-tools](https://github.com/yusuketakuma/pharma-free-tools) `(HTML/JS | 日文)` — 面向日本临床药师的 24 款免费网页工具，含基于肌酐清除率的抗菌药肾功能调量计算器。 / Collection of ~24 browser-based clinical pharmacy tools for Japanese pharmacists including renal dosing calculators.
- [koikelab/medication_eq_R](https://github.com/koikelab/medication_eq_R) `(R | 日英)` — 基于日本精神科标准自动计算精神科药物等效剂量的 R 工具。 / Automated calculation of psychotropic medication equivalent doses using Japanese psychiatric standards.
- [teezeit/medication-calculator](https://github.com/teezeit/medication-calculator) `(TS/React | 德国)` — 纯前端双指数药动学计算与 Plotly 多方案血药浓度对比单页应用。 / Client-side SPA for bi-exponential pharmacokinetic calculations and Plotly multi-regimen curve comparisons.

### 7.3 围术期麻醉 / ICU 靶控输注（TCI）/ Anesthesia & ICU TCI Simulators

- [vitaldb/tivatci](https://github.com/vitaldb/tivatci) `(Python | 韩国)` — 开源全凭静脉麻醉（TIVA）与靶控输注（TCI）Python 库，内置 Schnider/Marsh/Minto/Eleveld 模型。 / Open-source Python library for TIVA/TCI PK/PD modeling (Schnider, Marsh, Minto, Eleveld, Gepts) and LBM formulas.
- [seazuma/pkpd](https://github.com/seazuma/pkpd) `(JS/HTML | 日英)` — 离线可用的浏览器端麻醉药三室 PK/PD 与 TCI 模拟器（丙泊酚/芬太尼/咪达唑仑，含 BIS 预测）。 / Offline browser-based 3-compartment anesthetic PK/PD and TCI simulator with variability bands and BIS prediction.
- [ysuzuki1978/rocuronium-pkpd-simulator](https://github.com/ysuzuki1978/rocuronium-pkpd-simulator) `(JS/PWA | 日英)` — 模拟罗库溴铵 PK 与肌松药效（TOF 比值）的离线 PWA，集成 5 个含日本临床协变量的验证模型。 / Offline PWA simulating rocuronium PK and neuromuscular blockade (TOF) across 5 validated clinical models.
- [ysuzuki1978/remimazolam-tci-simulator](https://github.com/ysuzuki1978/remimazolam-tci-simulator) `(JS/HTML | 日英)` — 实现日本 Masui (2022) 模型的瑞马唑仑效应室浓度 TCI/TIVA 模拟器，支持 CSV 导出。 / Effect-site TCI simulator for remimazolam implementing the Masui (2022) PK model with CSV export.
- [ysuzuki1978/propofol-tci-simulator](https://github.com/ysuzuki1978/propofol-tci-simulator) `(JS/HTML | 日英)` — 基于 Eleveld (2018) 框架的丙泊酚效应室靶控输注交互式模拟器。 / Interactive propofol effect-site TCI simulator built on the Eleveld (2018) PK/PD framework.
- [Clinical-Pharmacy-Saarland-University/pi_pumpsim](https://github.com/Clinical-Pharmacy-Saarland-University/pi_pumpsim) `(Python/Svelte | 德英)` — 德国萨尔大学“Dr. Dosis”静脉输注药动学实时仿真触屏教学演示系统。 / Interactive FastAPI + Svelte IV infusion pharmacokinetics simulation demo ("Dr. Dosis") with pump visualization.

### 7.4 多房室血药浓度追踪与动态校准 / Multi-Compartment Tracking & Dynamic Calibration

- [xingqimiao/Kira-HRT-Tracker](https://github.com/xingqimiao/Kira-HRT-Tracker) `(TS | 中英)` — 隐私优先给药追踪与 PopPK 模拟应用，内置 MAP/EKF/OU-Kalman 4 种血检校准器并支持 MCP 协议。 / Privacy-first PK tracker featuring 4 blood-level calibration estimators (MAP, EKF, OU-Kalman) and MCP integration.
- [LaoZhong-Mihari/HRT-Recorder-PKcomponent-Test](https://github.com/LaoZhong-Mihari/HRT-Recorder-PKcomponent-Test) `(Swift | 中英)` — 原生三室模型与双相肌注库房动力学解析计算引擎，支持多途径吸收与体重校正。 / Native Swift PK engine implementing 3-compartment, biphasic depot kinetics, and multi-route absorption models.
- [TransmtfTeam/Transmtf-HRT-Tracker](https://github.com/TransmtfTeam/Transmtf-HRT-Tracker) `(TS | 中英)` — 支持翻转动力学（flip-flop）、三室透皮级联吸收及贝叶斯/EKF 实测校准的 PK 仿真框架。 / Web PK tracker supporting flip-flop kinetics, 3-compartment cascade absorption, and Bayesian/EKF calibration.
- [meowhuan/Oyama-s-HRT-Tracker](https://github.com/meowhuan/Oyama-s-HRT-Tracker) `(TS | 多语言)` — 基于三室与双相库房解析式的本地血药浓度与 AUC 实时模拟可视化 Web 工具。 / Multi-lingual local web simulator for real-time 3-compartment concentration-time curves and AUC visualization.
- [Trans-Prism/Trans-Prism](https://github.com/Trans-Prism/Trans-Prism) `(Flutter/JS | 中文)` — 跨平台隐私优先工具箱，内置多室指数衰减叠加血药浓度曲线模拟器与用药时间线。 / Cross-platform Flutter offline toolkit with multi-compartment superposition PK curve simulation and dosing timeline.

---

## 8. 生理药代动力学（PBPK）、IVIVE、DDI 与特殊人群 / PBPK, IVIVE, DDI & Special Populations

- [Open-Systems-Pharmacology/PK-Sim](https://github.com/Open-Systems-Pharmacology/PK-Sim) `(C#/.NET | 德国)` — 旗舰级开源全身 PBPK 建模与仿真平台，内置成人、儿科及特殊人群生理数据库。 / Flagship open-source whole-body PBPK modeling platform with adult, pediatric, and special-population physiology.
- [Open-Systems-Pharmacology/OSPSuite-R](https://github.com/Open-Systems-Pharmacology/OSPSuite-R) `(R/C++ | 德国)` — PK-Sim 与 MoBi 的编程式 R 接口，支持无 GUI 批量运行 PBPK 仿真与参数扫描。 / Programmatic R interface for headless PK-Sim/MoBi batch simulations, parameter sweeps, and reporting.
- [Open-Systems-Pharmacology/OSP-PBPK-Model-Library](https://github.com/Open-Systems-Pharmacology/OSP-PBPK-Model-Library) `(PK-Sim/R)` — 经同行评议的开源 PBPK 化合物验证模型与评估报告库。 / Peer-reviewed library of qualified open-source PBPK substance models and evaluation reports.
- [Open-Systems-Pharmacology/Qualification-DDI-CYP3A4](https://github.com/Open-Systems-Pharmacology/Qualification-DDI-CYP3A4) `(PK-Sim/R)` — 针对 CYP3A4 介导药物相互作用（DDI）的监管级全身 PBPK 资格验证方案与数据集。 / Regulatory-grade PBPK qualification plan and datasets evaluating CYP3A4-mediated drug-drug interactions.
- [Open-Systems-Pharmacology/Vancomycin-Model](https://github.com/Open-Systems-Pharmacology/Vancomycin-Model) `(PK-Sim/R)` — 聚焦肾小球滤过清除的万古霉素全身 PBPK 模型与验证报告。 / Whole-body PBPK model and evaluation report for vancomycin focusing on GFR-mediated renal clearance.
- [Open-Systems-Pharmacology/Pregnancy-Models](https://github.com/Open-Systems-Pharmacology/Pregnancy-Models) `(PK-Sim/MoBi)` — 纳入孕期生理变化与母胎/胎盘转运模块的妊娠期全身 PBPK 框架。 / Whole-body pregnancy PBPK framework incorporating gestational physiology and maternal-fetal placental transfer.
- [Open-Systems-Pharmacology/Lactation-PBPK-model](https://github.com/Open-Systems-Pharmacology/Lactation-PBPK-model) `(MoBi/SQLite)` — 模拟母体药物向乳汁转运及婴儿相对摄入剂量（RID）的哺乳期 PBPK 构建模块。 / Lactation PBPK building blocks for simulating drug transfer into breast milk and infant systemic exposure.
- [Clinical-Pharmacy-Saarland-University/PBPK-Models](https://github.com/Clinical-Pharmacy-Saarland-University/PBPK-Models) `(PK-Sim/R | 德国)` — 德国萨尔大学维护的经同行评议 PBPK 与药物-药物/药物-基因相互作用（DDI/DDGI）模型库。 / Peer-reviewed PBPK and DDI/DDGI model repository maintained by Saarland University.
- [Sanofi-Public/saemixPBPK](https://github.com/Sanofi-Public/saemixPBPK) `(R | 法国)` — 将开源 SAEM 非线性混合效应算法与 OSP Suite 全身 PBPK/QSP 模型结合进行群体估计。 / Integrates SAEM NLME parameter estimation with OSP Suite whole-body PBPK/QSP models.
- [esqLABS/esqlabsR](https://github.com/esqLABS/esqlabsR) `(R)` — 基于结构化 Excel 配置模板标准化管理大型多情景 OSP Suite PBPK/QSP 工作流。 / Standardized R workflow package managing multi-scenario OSP Suite PBPK/QSP projects via Excel templates.
- [USEPA/CompTox-ExpoCast-httk](https://github.com/USEPA/CompTox-ExpoCast-httk) `(R/C)` — 美国 EPA 高通量毒代动力学包，提供通用 PBPK 模型、组织分配系数预测与 IVIVE 流水线。 / High-throughput toxicokinetics (`httk`) package for generic PBPK modeling, partition coefficients, and IVIVE.
- [metrumresearchgroup/bioPBPK](https://github.com/metrumresearchgroup/bioPBPK) `(Julia/R)` — 代码优先的生物大分子/单抗（mAb）全身 PBPK 模型，显式刻画 FcRn 再循环与淋巴回流。 / Code-first biologics/mAb whole-body PBPK models with FcRn recycling and lymphatics in Julia and R.
- [metrumresearchgroup/cptpsp-tutorial-2019](https://github.com/metrumresearchgroup/cptpsp-tutorial-2019) `(R)` — *CPT:PSP* `mrgsolve` PBPK/QSP 教程配套代码，含透明的 Poulin & Theil $K_p$ 计算脚本。 / Companion code for `mrgsolve` PBPK/QSP modeling including transparent Poulin & Theil $K_p$ calculation scripts.
- [SystemsForecasting/ManchesterPBPK](https://github.com/SystemsForecasting/ManchesterPBPK) `(R)` — 基于 `rxode2` 的透明代码优先全身 PBPK 教学与原型模型（*PBPKedu*）。 / Open-source, code-first whole-body PBPK model (*PBPKedu*) written transparently in `rxode2`.
- [matthiaskoenig/pkdb](https://github.com/matthiaskoenig/pkdb) `(Python/Django | 德国)` — 遵循 FAIR 原则的开源临床/临床前药动学数据库（PK-DB）与 REST API。 / FAIR open pharmacokinetics database (PK-DB) curating clinical PK curves, genotypes, and organ impairment via API.
- [matthiaskoenig/sbmlsim](https://github.com/matthiaskoenig/sbmlsim) `(Python | 德国)` — 基于 `libRoadRunner` 的 SBML PBPK 仿真、参数扫描、敏感度分析与自动报告框架。 / Python simulation and reporting framework built on `libRoadRunner` for reproducible SBML PBPK models.
- [matthiaskoenig/glimepiride-model](https://github.com/matthiaskoenig/glimepiride-model) `(Python/SBML | 德国)` — 显式模拟肾损伤、肝硬化与 CYP2C9 基因多态性影响的格列美脲全身 PBPK 模型。 / Whole-body SBML PBPK model of glimepiride explicitly modeling renal impairment, cirrhosis, and CYP2C9 genetics.
- [matthiaskoenig/dapagliflozin-model](https://github.com/matthiaskoenig/dapagliflozin-model) `(Python/SBML | 德国)` — 评估肝肾联合损伤、食物效应及尿糖排泄药效的达格列净全身 PBPK/PD 模型。 / Coupled PBPK/PD SBML model of dapagliflozin evaluating hepatorenal impairment and urinary glucose excretion.
- [ahmedn12/oral-pbpk-model](https://github.com/ahmedn12/oral-pbpk-model) `(Python/R)` — 对齐 FDA 研讨会流程的多途径口服 PBPK 模型，刻画肝脏首过代谢与蛋白结合率敏感度。 / Dual Python/R oral PBPK model capturing hepatic first-pass metabolism and protein-binding ($f_u$) sensitivity.
- [lucis-e/PopPBPK-RL_Bnzpril](https://github.com/lucis-e/PopPBPK-RL_Bnzpril) `(Python/R)` — 将群体 PBPK 与强化学习（RL）结合，在肾损伤虚拟队列中优化贝那普利精准给药。 / Integrates population PBPK with reinforcement learning to optimize benazepril dosing in renal-impaired cohorts.
- [pipetcpt/DallphinDDI](https://github.com/pipetcpt/DallphinDDI) `(R | 韩英)` — 韩国 EDISON 资助开发的生理/PBPK 代谢酶与转运体药物相互作用（DDI）仿真工具。 / Academic R-based physiological/PBPK modeling tool for simulating metabolic and transporter DDIs.
- [cosbi-research/PBPKmRNABiTE](https://github.com/cosbi-research/PBPKmRNABiTE) `(MATLAB | 意大利)` — 模拟 mRNA 编码双特异性 T 细胞衔接器（BiTE）转运、翻译与抗体药动学的多尺度 PBPK 模型。 / Multi-scale PBPK model for mRNA-encoded BiTE cancer therapy capturing trafficking, translation, and antibody PK.
- [cosbi-research/Campanile_et_al_PBPKmRNATherapeutics](https://github.com/cosbi-research/Campanile_et_al_PBPKmRNATherapeutics) `(MATLAB | 意大利)` — 基于 SimBiology 的脂质纳米颗粒（LNP）递送与 mRNA 抗体疗法 PBPK 建模框架。 / SimBiology PBPK framework for lipid nanoparticle (LNP) delivery and mRNA-encoded antibody therapeutics.
- [RomanCohort/confluencia](https://github.com/RomanCohort/confluencia) `(Python | 中英)` — 面向小样本 circRNA 药物研发的计算平台，集成首个 circRNA 六室机制性 PK 模型（RNACTM）。 / Small-sample circRNA discovery platform featuring the first 6-compartment mechanistic circRNA PK model (RNACTM).

---

## 9. AI / LLM / MCP 智能体、知识抽取与开源教材 / AI Agents, Data Mining & Open Textbooks

### 9.1 AI Agent、MCP、RAG 与数据挖掘 / AI Agents, MCP, RAG & Data Mining

- [PeterBloomingdale/pmxagent](https://github.com/PeterBloomingdale/pmxagent) `(R/Python/Docker)` — 将真实 R 定量药理函数封装为 REST API 与 MCP 服务，供 AI 智能体安全执行调用。 / Open-source agentic platform exposing R pharmacometrics functions as REST APIs and an MCP server for LLMs.
- [Slow-Walker66/PK-Sim-Mobi-RAG-Tool](https://github.com/Slow-Walker66/PK-Sim-Mobi-RAG-Tool) `(Python | 中英)` — 面向 PK-Sim/MoBi 官方文档与构建模块的本地 RAG 问答排错助手。 / Local RAG assistant indexing PK-Sim and MoBi technical documentation and building blocks for PBPK troubleshooting.
- [lfcypo/hrt-pk-mcp](https://github.com/lfcypo/hrt-pk-mcp) `(Python/MCP | 中文)` — 将多房室 PK 算法封装为标准 MCP 服务端，向 AI Agent 暴露给药记录与血药浓度查询工具。 / Standard Python MCP server wrapping multi-compartment PK algorithms for AI-agent dose logging and queries.
- [kimmingul/clinical-pharmacology-study-protocol-development](https://github.com/kimmingul/clinical-pharmacology-study-protocol-development) `(Claude Plugin | 韩英)` — 辅助临床药理学家起草 I 期临床药理方案（FIH/SAD/MAD/DDI）与知情同意书的 LLM 插件。 / Claude Code plugin assisting clinical pharmacologists in drafting Phase 1 protocols (FIH, SAD/MAD, DDI) and ICFs.
- [dueyama/pmda-pk-curve-viewer](https://github.com/dueyama/pmda-pk-curve-viewer) `(TS/Next.js | 日英)` — 自动解析日本 PMDA 电子药品说明书 XML，提取 PK 参数并实时绘制血药浓度曲线。 / Parses official Japanese PMDA package insert XML files to extract PK parameters and plot estimated concentration curves.
- [pablosierrafernandez/FarmacoDB](https://github.com/pablosierrafernandez/FarmacoDB) `(Python | 西班牙文)` — 利用 LLM 文本挖掘自动化抽取多源药动学数据（>1,000 药物）并预测人体半衰期。 / LLM-assisted text mining pipeline standardizing multi-source PK data (>1,000 drugs) with half-life prediction models.
- [valentinnavalos/pharmawatch-api](https://github.com/valentinnavalos/pharmawatch-api) `(API | 西班牙文)` — 支持处方校验与药动学药物相互作用（血浆蛋白置换等）分析的药物警戒 REST API。 / Pharmacovigilance REST API providing prescription checking and PK drug-drug interaction analysis.
- [PharMolix/OpenBioMed](https://github.com/PharMolix/OpenBioMed) `(Python | 中英)` — 清华 AIR 开源生物医药多模态大模型与智能体框架，内置 ADMET 与 DDI 预测工具链。 / Multimodal biomedical LLM and agent framework featuring built-in ADMET prediction and DDI analysis tools.
- [datamllab/CAi_copilot](https://github.com/datamllab/CAi_copilot) `(Python | 中英)` — 自然语言驱动的开源药物设计智能体，集成 ADMET-AI 预测吸收、代谢、清除与毒性。 / Natural-language drug design agent integrating ADMET-AI for clearance, absorption, metabolism, and toxicity screening.
- [MasterDGL/admet-literature](https://github.com/MasterDGL/admet-literature) `(Markdown | 中英)` — 系统梳理 AI 药物发现中 ADMET 与药代动力学性质预测的论文、数据集与方法笔记。 / Curated bilingual literature and benchmark dataset index for AI-driven ADMET and PK property prediction.

### 9.2 多语种开源教材与代码库 / Multi-Lingual Open Textbooks & Workshops

- [asancpt/book-ncar](https://github.com/asancpt/book-ncar) `(Bookdown | 韩文)` — 韩国峨山医院开源教材《使用 R 进行非房室分析与生物等效性评价》。 / Open-source Korean textbook teaching practical NCA and bioequivalence evaluation in R.
- [asancpt/nmw-nonmem](https://github.com/asancpt/nmw-nonmem) `(R/NONMEM | 韩英)` — 演示 FO/FOCE/FOCE-I 混合效应估计算法并桥接 R 与 NONMEM 的教学代码库。 / Educational code demonstrating NLME estimation algorithms (FO/FOCE/FOCE-I) bridging R and NONMEM.
- [AMC-CPT/PKwR](https://github.com/AMC-CPT/PKwR) `(R/Shiny | 韩英)` — 《Pharmacokinetics with R》配套可复现脚本与万古霉素 TDM Shiny 示例。 / Companion repository for *Pharmacokinetics with R* with reproducible scripts and a vancomycin TDM Shiny app.
- [AMC-CPT/PMx](https://github.com/AMC-CPT/PMx) `(R/NONMEM | 韩英)` — 《Pharmacometrics with NONMEM and R》配套控制流模板与 R 诊断后处理代码。 / Companion repository for *Pharmacometrics with NONMEM and R* with verified NONMEM control streams and R code.
- [pipetcpt/basic](https://github.com/pipetcpt/basic) `(Bookdown/NONMEM | 韩文)` — 韩国 PIPET 定量药理入门讲义，覆盖 NONMEM 控制流、数据准备、协变量与 PK-PD。 / PIPET beginner pharmacometrics workshop covering NONMEM coding, dataset prep, covariates, and PK-PD linkage.
- [pipetcpt/pharmapk](https://github.com/pipetcpt/pharmapk) `(Bookdown | 韩文)` — 面向新药研发的《实战药动学 I》开源教材，详解 ADME、清除率、分布与房室解析。 / Open textbook explaining ADME, clearance, distribution, NCA, and compartmental PK for drug development.
- [pipetcpt/book-poppk](https://github.com/pipetcpt/book-poppk) `(Bookdown | 韩文)` — 韩国 MFDS 群体药代动力学监管指导原则的开源网络化拆解参考。 / Web-based compilation of Korea MFDS Population Pharmacokinetics regulatory guidelines and validation practices.
- [pipetcpt/capstone-qsp](https://github.com/pipetcpt/capstone-qsp) `(R/Shiny | 韩英)` — 将机制性定量系统药理学（QSP）ODE 模型转化为交互式 Shiny 看板的实战案例集。 / Capstone projects demonstrating how to turn mechanistic QSP ODE models into interactive R Shiny dashboards.
- [matthiaskoenig/course-pharmacokinetic-modelling](https://github.com/matthiaskoenig/course-pharmacokinetic-modelling) `(Python/Jupyter | 德英)` — 柏林洪堡大学药动学与 PBPK 建模互动 Jupyter Notebook 课程库。 / University-level interactive Jupyter Notebook course covering compartmental PK, PBPK, and dosing optimization.
- [Clinical-Pharmacy-Saarland-University/RTutorial](https://github.com/Clinical-Pharmacy-Saarland-University/RTutorial) `(R Markdown | 德英)` — 德国萨尔大学临床药学与定量药理 R 语言数据分析教学教程。 / Structured R tutorials for clinical pharmacy and pharmacometrics data analysis from Saarland University.
- [Kalo0m/pharmacocinetique](https://github.com/Kalo0m/pharmacocinetique) `(TS | 法文)` — 法国兽医/药学专业学生开发的药代动力学基础概念学习与计算 Web 应用。 / French-language educational web app for learning and calculating fundamental pharmacokinetics concepts.
- [douglasufs/matematica-aplicada-ciencias-farmaceuticas](https://github.com/douglasufs/matematica-aplicada-ciencias-farmaceuticas) `(OER | 葡萄牙文)` — 巴西联邦大学药学应用数学开放教材，包含稀释计算、生物等效性与计算药动学脚本。 / Portuguese OER textbook covering pharmaceutical math, dilution, bioequivalence, and computational pharmacokinetics.

# Awesome Clinical Pharmacokinetics & Pharmacometrics (ClinPharm & PMx)

> 面向**临床药代动力学（Clinical Pharmacokinetics）**、**定量药理学（Pharmacometrics）**以及 **AI × ClinPharm/PMx** 的多语种开源工具目录。不以 Star 数为门槛，按解决的具体科学或工程问题归类，覆盖英、中、日、韩、德、法、西、葡、意等全球生态（v2.0 收录 **343** 个经核验开源仓库，零重复）。  
> A curated, problem-oriented, multi-lingual directory of open-source GitHub repositories for **Clinical Pharmacokinetics (Clin. Pharm.)**, **Pharmacometrics (PMx)**, and **AI × ClinPharm/PMx**, spanning English, Chinese, Japanese, Korean, German, French, Spanish, Portuguese, and Italian ecosystems (v2.0: **343** verified repositories, zero duplicates).

---

## 目录 / Contents

- [1. NONMEM / Monolix / Phoenix 工作流、编辑器插件与算力运维 / Workflow, Editors & Orchestration](#1-nonmem--monolix--phoenix-工作流编辑器插件与算力运维--workflow-editors--orchestration)
- [2. 开源 PopPK / NLME 建模与多语言 ODE 仿真引擎 / Open-Source NLME & ODE Engines](#2-开源-poppk--nlme-建模与多语言-ode-仿真引擎--open-source-nlme--ode-engines)
- [3. 数据准备、CDISC 转换与数据质控 / Data Preparation, CDISC & QC](#3-数据准备cdisc-转换与数据质控--data-preparation-cdisc--qc)
- [4. 非房室分析（NCA）、生物等效性（BE）、IVIVC 与溶出 / NCA, Bioequivalence, IVIVC & Dissolution](#4-非房室分析nca生物等效性beivivc-与溶出--nca-bioequivalence-ivivc--dissolution)
- [5. 模型诊断、可视化与自动化报告 / Diagnostics, Visualization & Automated Reporting](#5-模型诊断可视化与自动化报告--diagnostics-visualization--automated-reporting)
- [6. 临床药理监管、C-QTc、I/II 期剂量探索、E-R、CTS 与 FIH / Regulatory ClinPharm, C-QTc, Dose-Finding, E-R & FIH](#6-临床药理监管c-qtciii-期剂量探索e-rcts-与-fih--regulatory-clinpharm-c-qtc-dose-finding-e-r--fih)
- [7. 模型引导精准给药（MIPD）、临床 TDM、抗感染 PTA 与 TCI / Clinical MIPD, TDM, Antimicrobial PTA & TCI](#7-模型引导精准给药mipd临床-tdm抗感染-pta-与-tci--clinical-mipd-tdm-antimicrobial-pta--tci)
  - [7.1 通用贝叶斯 / MIPD 引擎与外部验证 / General MIPD Engines & Validation](#71-通用贝叶斯--mipd-引擎与外部验证--general-mipd-engines--validation)
  - [7.2 抗感染 PK/PD、PTA/CFR 与抗菌/抗真菌 TDM / Antimicrobial PK/PD, PTA/CFR & TDM](#72-抗感染-pkpdptacfr-与抗菌抗真菌-tdm--antimicrobial-pkpd-ptacfr--tdm)
  - [7.3 免疫抑制剂、窄治疗窗药物与临床计算器（含儿科/CRRT）/ Immunosuppressant, NTI & Hospital Calculators](#73-免疫抑制剂窄治疗窗药物与临床计算器含儿科crrt--immunosuppressant-nti--hospital-calculators)
  - [7.4 围术期麻醉 TCI、阿片解救与胰岛素-血糖 PK/PD / Anesthesia TCI, Opioid Rescue & Glucose-Insulin PK/PD](#74-围术期麻醉-tci阿片解救与胰岛素-血糖-pkpd--anesthesia-tci-opioid-rescue--glucose-insulin-pkpd)
  - [7.5 多房室血药浓度追踪与动态校准 / Multi-Compartment Tracking & Dynamic Calibration](#75-多房室血药浓度追踪与动态校准--multi-compartment-tracking--dynamic-calibration)
- [8. 生理药代动力学（PBPK）、IVIVE、DDI 与特殊人群 / PBPK, IVIVE, DDI & Special Populations](#8-生理药代动力学pbpkiviveddi-与特殊人群--pbpk-ivive-ddi--special-populations)
- [9. 生物大分子、TMDD、ADC、CAR-T、免疫原性与 QSP / Biologics, TMDD, ADC, CAR-T, Immunogenicity & QSP](#9-生物大分子tmddadccar-t免疫原性与-qsp--biologics-tmdd-adc-car-t-immunogenicity--qsp)
- [10. AI / ML / DL / SciML / RL × 临床药理与定量药理 / AI, ML, SciML & RL for ClinPharm & PMx](#10-ai--ml--dl--sciml--rl--临床药理与定量药理--ai-ml-sciml--rl-for-clinpharm--pmx)
  - [10.1 LLM 智能体、MCP 协议、RAG 与知识挖掘 / LLM Agents, MCP, RAG & Knowledge Mining](#101-llm-智能体mcp-协议rag-与知识挖掘--llm-agents-mcp-rag--knowledge-mining)
  - [10.2 物理信息神经网络（PINNs）、Neural ODE 与 SciML / PINNs, Neural ODEs, UDEs & SciML](#102-物理信息神经网络pinnsneural-ode-与-sciml--pinns-neural-odes-udes--sciml)
  - [10.3 强化学习（RL）与深度学习精准给药 / RL & Deep Learning for Precision Dosing & TDM](#103-强化学习rl与深度学习精准给药--rl--deep-learning-for-precision-dosing--tdm)
  - [10.4 自动化定量药理、ML 协变量筛选与合成患者数据 / Automated PMx, ML Covariates & Synthetic Data](#104-自动化定量药理ml-协变量筛选与合成患者数据--automated-pmx-ml-covariates--synthetic-data)
  - [10.5 AI / ML / GNN 预测人体 PK 参数、药时曲线与 ADME / ML/DL Prediction of Human PK & ADME](#105-ai--ml--gnn-预测人体-pk-参数药时曲线与-adme--mldl-prediction-of-human-pk--adme)
- [11. 开源临床 PK 数据集、基准与精选索引 / Open Clinical PK Datasets, Benchmarks & Awesome Lists](#11-开源临床-pk-数据集基准与精选索引--open-clinical-pk-datasets-benchmarks--awesome-lists)
- [12. 多语种开源教材与代码库 / Multi-Lingual Open Textbooks & Workshops](#12-多语种开源教材与代码库--multi-lingual-open-textbooks--workshops)

---

## 1. NONMEM / Monolix / Phoenix 工作流、编辑器插件与算力运维 / Workflow, Editors & Orchestration

- [UUPharmacometrics/PsN](https://github.com/UUPharmacometrics/PsN) `(Perl)` — NONMEM 自动化工作流核心工具集（Bootstrap、SCM、VPC、SIR）。 / Core CLI toolkit automating NONMEM workflows (bootstrapping, SCM, VPC, SIR).
- [metrumresearchgroup/bbi](https://github.com/metrumresearchgroup/bbi) `(Go)` — 跨平台、支持本地与 Slurm/SGE 集群的 NONMEM 高速执行引擎。 / Cross-platform, scheduler-agnostic CLI execution engine for NONMEM runs (local, Slurm, SGE).
- [metrumresearchgroup/bbr](https://github.com/metrumresearchgroup/bbr) `(R)` — 基于 `bbi` 的 R 语言建模管理包，实现 NONMEM 模型谱系追踪与审计日志。 / R package for NONMEM run management, model ancestry tracking, and reproducible run logs.
- [metrumresearchgroup/bbr.bayes](https://github.com/metrumresearchgroup/bbr.bayes) `(R)` — 扩展 `bbr` 工作流，支持通过 Stan（`cmdstanr`）和 NONMEM 贝叶斯方法管理贝叶斯药动学模型。 / Extends `bbr` to manage, execute, and summarize Bayesian pharmacometric models using Stan and NONMEM.
- [metrumresearchgroup/nmrec](https://github.com/metrumresearchgroup/nmrec) `(R)` — 精准解析与修改 NONMEM 控制流记录与缩写语法的底层库。 / Low-level R parser and serializer for programmatically reading and editing NONMEM control streams.
- [metrumresearchgroup/mrgvalidate](https://github.com/metrumresearchgroup/mrgvalidate) `(R)` — 自动生成符合监管合规要求的 R 包验证计划、可追溯性矩阵与测试报告。 / Automates regulatory software validation documentation (plans, traceability matrices, test summaries) for R packages.
- [metrumresearchgroup/pkgr](https://github.com/metrumresearchgroup/pkgr) `(Go)` — 快速构建与管理可复现、隔离 R 定量药理环境的命令行依赖管理工具。 / CLI dependency manager for installing and curating reproducible, isolated R package environments.
- [NMautoverse/NMsim](https://github.com/NMautoverse/NMsim) `(R)` — 无需手动改控制流，直接基于现有 NONMEM 估计模型与新数据集从 R 执行 NONMEM 模拟。 / Seamless R interface to run NONMEM simulations directly from existing estimation control streams without manual edits.
- [nlmixr2/babelmixr2](https://github.com/nlmixr2/babelmixr2) `(R)` — 将统一 `nlmixr2`/`rxode2` 模型转译并在 NONMEM、Monolix、PKNCA、PopED 上运行。 / Cross-engine bridge translating `nlmixr2`/`rxode2` models to NONMEM, Monolix, PKNCA, and PopED.
- [nlmixr2/nonmem2rx](https://github.com/nlmixr2/nonmem2rx) `(R/C)` — 将 NONMEM 控制流及估计结果解析并转换为 `rxode2`/`nlmixr2` 模型。 / Parses and converts NONMEM control streams and outputs into `rxode2` or `nlmixr2` models.
- [nlmixr2/monolix2rx](https://github.com/nlmixr2/monolix2rx) `(R/C)` — 将 Monolix `.mlxtran` 模型与结果导入并转换为 `rxode2`/`nlmixr2` 对象。 / Imports and translates Monolix `.mlxtran` models and results into `rxode2`/`nlmixr2` objects.
- [Andy0000000000/nonmem2mrgsolve](https://github.com/Andy0000000000/nonmem2mrgsolve) `(R)` — 自动将含全模型及 QSS TMDD 在内的 NONMEM 控制流翻译为高速 `mrgsolve` 代码。 / Translates NONMEM control streams—including full and QSS TMDD models—into fast `mrgsolve` simulation code.
- [UUPharmacometrics/assemblerr](https://github.com/UUPharmacometrics/assemblerr) `(R)` — 通过模块化 R 组件编程式组装药动学模型并编译生成规范的 NONMEM 控制流。 / Programmatically constructs pharmacometric models from R building blocks and compiles them into NONMEM control streams.
- [certara/R-Certara](https://github.com/certara/R-Certara) `(R)` — Certara 开源定量药理 R 工具套件的一键安装与统一加载元包（`Certara.R`）。 / Meta-package and installer unifying Certara's open-source pharmacometric R packages and Shiny apps.
- [certara/R-RsNLME](https://github.com/certara/R-RsNLME) `(R)` — 用可复现的 tidyverse R 脚本替代 GUI 操作调用 Phoenix NLME 引擎。 / Scriptable tidyverse-style R interface for running the Phoenix NLME estimation engine.
- [certara/R-RsNLME-model-builder](https://github.com/certara/R-RsNLME-model-builder) `(R/Shiny)` — 可视化构建 NLME 模型并实时生成可复现 PML 与 `RsNLME` R 脚本的 Shiny 应用。 / Interactive Shiny GUI for building NLME models while live-generating reproducible PML and `RsNLME` code.
- [MarcLavielle/Rsmlx](https://github.com/MarcLavielle/Rsmlx) `(R)` — “R Speaks Monolix”：在 R 中调用 Monolix 实现自动化建模、协变量筛选与收敛性评估。 / Automates Monolix model building, statistical covariate search, and convergence assessment from R.
- [tsahota/NMproject](https://github.com/tsahota/NMproject) `(R)` — 将 RStudio 打造为管道式脚本化 NONMEM 建模开发环境，集成运行追踪与自动诊断。 / Turns RStudio into an integrated, script-based NONMEM model development environment with piped workflows.
- [dpastoor/nonmemutils](https://github.com/dpastoor/nonmemutils) `(Go)` — 高速 Go 命令行工具集，用于解析 NONMEM `.lst` 输出文件与管理任务提交。 / Fast Go CLI utilities for parsing NONMEM `.lst` output files and managing run submissions.
- [Robterheine/nmgui2](https://github.com/Robterheine/nmgui2) `(Python/PyQt6)` — 跨平台纯 Python 桌面客户端（类 Pirana 替代），管理对比 NONMEM 模型并联动 PsN。 / Cross-platform PyQt6 desktop GUI (Pirana alternative) for browsing, comparing, and running NONMEM + PsN workflows.
- [OpenPKPD/OpenPKPD](https://github.com/OpenPKPD/OpenPKPD) `(Python)` — 面向将 NONMEM 工作流迁移至 Python 的开源平台，提供 `.ctl` 解析与输出复现。 / Open-source Python platform for migrating NONMEM workflows with `.ctl` control-stream parsing.
- [a2-ai/slurmtools](https://github.com/a2-ai/slurmtools) `(R)` — 在 R 定量药理环境中直接提交、监控和管理 Slurm HPC 集群任务。 / R utilities for submitting, monitoring, and managing Slurm HPC jobs directly from R.
- [billdenney/Pharmacometrics-Docker](https://github.com/billdenney/Pharmacometrics-Docker) `(Docker)` — 标准化多版本 NONMEM（含 gfortran）与 PsN 的 Docker 容器化部署配置。 / Community Dockerfiles for reproducible multi-version NONMEM and PsN deployments.
- [kinginsun/nonmem](https://github.com/kinginsun/nonmem) `(Docker/Shell)` — 跨平台（Win/macOS Apple Silicon/Linux）NONMEM + PsN + MPICH 容器镜像与一键脚本。 / Cross-platform Docker setup and wrapper scripts for NONMEM, PsN, and MPICH parallel execution.
- [FelicienLL/runnonmem](https://github.com/FelicienLL/runnonmem) `(R)` — 轻量级 R 封装工具，用于从 R 脚本直接调用运行 NONMEM。 / Lightweight R wrapper for invoking NONMEM directly from R scripts.
- [s0521/nonmem_cn](https://github.com/s0521/nonmem_cn) `(TS | 中文)` — NONMEM 控制文件 VS Code 扩展，提供语法高亮、自动补全与中英双语注释提示。 / VS Code extension for NONMEM control files with syntax highlighting, snippets, and bilingual CN/EN tooltips.
- [vrognas/nmtran](https://github.com/vrognas/nmtran) `(TS)` — 为 NMTRAN/NONMEM 控制流提供语言智能感知、实时诊断与悬停文档的 VS Code 扩展。 / VS Code extension delivering language intelligence, diagnostics, and hover docs for NMTRAN/NONMEM.
- [UUPharmacometrics/vim-nonmem](https://github.com/UUPharmacometrics/vim-nonmem) `(Vim)` — 专为 Vim/Neovim 打造的 NONMEM 控制流与模型文件语法高亮插件。 / Dedicated Vim/Neovim syntax highlighting plugin for editing NONMEM control streams.
- [nmusers/nm-mode](https://github.com/nmusers/nm-mode) `(Emacs Lisp)` — 极简风格 Emacs 主模式，提供 NONMEM 控制流语法高亮与编辑支持。 / Minimalist Emacs major mode providing syntax highlighting and editing support for NONMEM.
- [TingjieGuo/MINGA](https://github.com/TingjieGuo/MINGA) `(Hugo/Shell | 中文)` — 面向中文用户的 NONMEM、PsN、Pirana 与 R 定量药理环境安装教程与脚本。 / Chinese-language installation guide and shell scripts for NONMEM, PsN, Pirana, and R PMx tools.
- [Slow-Walker66/PPK-workbench-assistance-demo](https://github.com/Slow-Walker66/PPK-workbench-assistance-demo) `(TS | 中英)` — 本地优先的 NONMEM+PsN 群体药动学工作台（Pirana 开源替代），含模型树、诊断与报告生成。 / Local-first PopPK workbench (Pirana alternative) for NONMEM+PsN with model lineage, diagnostics, and reporting.

---

## 2. 开源 PopPK / NLME 建模与多语言 ODE 仿真引擎 / Open-Source NLME & ODE Engines

- [nlmixr2/nlmixr2](https://github.com/nlmixr2/nlmixr2) `(R/C++)` — 开源 CRAN 级非线性混合效应（NLME）建模框架，支持 FOCE-I 与 SAEM。 / Open-source R framework for population PK/PD NLME modeling (FOCE-I, SAEM, nlme).
- [nlmixr2/rxode2](https://github.com/nlmixr2/rxode2) `(R/C/C++)` — 将药动学 ODE 模型编译为 C 代码并支持 NONMEM 风格事件表的高速仿真引擎。 / High-speed C-compiled ODE solver and clinical trial simulator with NONMEM-style event tables.
- [nlmixr2/nlmixr2lib](https://github.com/nlmixr2/nlmixr2lib) `(R)` — 标准化临床 PopPK/PD 及生物大分子 TMDD 文献模型库，可直接供 `nlmixr2`/`rxode2` 调用。 / Curated library of published clinical PopPK/PD and biologics/TMDD models for `nlmixr2` and `rxode2`.
- [nlmixr2/nlmixr2extra](https://github.com/nlmixr2/nlmixr2extra) `(R)` — 为 `nlmixr2` 补充 Bootstrap、逐步协变量筛选与预处理拟合等核心建模工具。 / Adds bootstrapping, stepwise covariate selection, and preconditioned fits to `nlmixr2`.
- [nlmixr2/lotri](https://github.com/nlmixr2/lotri) `(R/C)` — 提供简洁语法定义 `nlmixr2`/`rxode2` 中的下三角分块协方差矩阵（IIV/IOV）。 / Concise DSL for specifying lower-triangular block covariance matrices (IIV/IOV) in `nlmixr2` and `rxode2`.
- [metrumresearchgroup/mrgsolve](https://github.com/metrumresearchgroup/mrgsolve) `(R/C++)` — 类 NONMEM 语法的 C++ 编译型分层 ODE 仿真引擎，广泛用于 PopPK/PBPK/QSP。 / Fast C++-compiled hierarchical ODE simulator in R with NONMEM-inspired syntax for PopPK/PBPK/QSP.
- [mrgsolve/depot](https://github.com/mrgsolve/depot) `(R/C++)` — `mrgsolve` 官方配套即用型 ODE 模型库，收录全/近似 TMDD 与 PBPK 基准模板。 / Official companion repository of ready-to-run `mrgsolve` ODE templates including TMDD and PBPK models.
- [kylebaron/mrgsim.parallel](https://github.com/kylebaron/mrgsim.parallel) `(R)` — 通过拆分数据集并利用 `parallel`/`future` 并行执行大幅加速大规模 `mrgsolve` 模拟。 / Accelerates large-scale `mrgsolve` simulations via chunked parallel execution with `parallel` or `future`.
- [metrumresearchgroup/mrgsim.ds](https://github.com/metrumresearchgroup/mrgsim.ds) `(R)` — 将 `mrgsolve` 模拟输出存为 Apache Arrow 数据集，大幅降低超大规模仿真内存占用。 / Stores `mrgsolve` simulation outputs in Apache Arrow datasets to reduce memory overhead at scale.
- [InsightRX/PKPDsim](https://github.com/InsightRX/PKPDsim) `(R/C++)` — 面向临床精准给药的 C++ 编译型 ODE 与解析房室 PK/PD 仿真引擎。 / Compiled C++ ODE and analytical PK/PD simulator tailored for clinical precision dosing.
- [john-harrold/ubiquity](https://github.com/john-harrold/ubiquity) `(R)` — 统一 PK/PD、PBPK 与 QSP 建模、参数估计、自动 Word/PPT 报告与 Shiny GUI 生成的框架。 / End-to-end R modeling framework generating simulations, estimates, Word/PPT reports, and Shiny apps.
- [pharmpy/pharmpy](https://github.com/pharmpy/pharmpy) `(Python)` — 现代 Python 药动学模型抽象层与自动化模型构建（AMD）工具，跨 NONMEM 与 `nlmixr2`。 / Python pharmacometrics library and Automated Model Development (AMD) tool across NONMEM and `nlmixr2`.
- [pharmpy/pharmr](https://github.com/pharmpy/pharmr) `(R)` — Pharmpy 官方 R 语言封装，使 R 用户直接调用自动化建模与多引擎工作流。 / Official R wrapper around Pharmpy for automated model development and control-stream manipulation.
- [metrumresearchgroup/Torsten](https://github.com/metrumresearchgroup/Torsten) `(C++/Stan)` — 扩展 Stan 数学库以支持自动微分房室解析解、ODE 求解器与 NMTRAN 给药事件。 / Stan extension library providing pharmacometric compartmental/ODE solvers and NMTRAN events for Bayesian PopPK/PD.
- [iame-researchCenter/saemix](https://github.com/iame-researchCenter/saemix) `(R)` — 开源 R 语言随机逼近期望最大化（SAEM）非线性混合效应建模包。 / Open-source R implementation of the SAEM algorithm for NLME population PK/PD modeling.
- [MarcLavielle/mlxR](https://github.com/MarcLavielle/mlxR) `(R)` — 面向混合效应模型的纵向 PopPK/PD 仿真与可视化包，衔接 Monolix/Simulx 生态。 / Longitudinal PopPK/PD simulation and visualization package interfacing with Monolix/Simulx.
- [LAPKB/Pmetrics](https://github.com/LAPKB/Pmetrics) `(R/Rust)` — 支持非参数与参数群体 PK/PD 建模及贝叶斯 MAP/MMopt 最优给药估计的引擎。 / Non-parametric and parametric PopPK/PD modeling and Bayesian dosing engine powered by Rust.
- [LAPKB/pharmsol](https://github.com/LAPKB/pharmsol) `(Rust)` — 高性能 Rust 药代/药效动力学求解库，支持解析解、ODE/SDE 仿真、NCA 与内置 DSL。 / High-performance Rust library for PK/PD analytical/ODE/SDE simulation, NCA, and model DSLs.
- [LAPKB/PMcore](https://github.com/LAPKB/PMcore) `(Rust)` — 纯 Rust 编写的非参数群体药动学核心引擎与 ODE 求解器（NPAG、NPOD、NPSA）。 / Core Rust computational engine implementing non-parametric PopPK estimation algorithms (NPAG, NPOD, NPSA).
- [FeRx-NLME/ferx-core](https://github.com/FeRx-NLME/ferx-core) `(Rust)` — 纯 Rust 开源非线性混合效应（NLME）引擎，支持 FOCE/FOCEI、SAEM 与 `.ferx` 语法。 / Open-source Rust NLME engine supporting FOCE/FOCEI, SAEM, importance sampling, and a `.ferx` DSL.
- [DavAug/chi](https://github.com/DavAug/chi) `(Python)` — 纯 Python 机制性 ODE PK/PD、QSP 与贝叶斯 MIPD 分层推断框架。 / Native Python framework for mechanistic ODE PK/PD, QSP, and hierarchical Bayesian MIPD inference.
- [MSDLLCpapers/cpk](https://github.com/MSDLLCpapers/cpk) `(Python)` — 默沙东开源的 1/2 室静脉与血管外 PK 非线性回归拟合工具，支持 AICc 自动选模与异常值检测。 / Nonlinear regression for 1- and 2-compartment IV/extravascular PK with AICc model selection and outlier detection.
- [gumgo91/PKPy](https://github.com/gumgo91/PKPy) `(Python)` — 自动化 Python 群体药动学（PopPK）分析框架，集成参数初始化、NCA、协变量筛选与 GOF。 / Automated Python PopPK framework with parameter initialization, 1-/2-compartment models, NCA, and GOF.
- [orlacchioresearch/pharmacokinetics-pkpd-toolkit](https://github.com/orlacchioresearch/pharmacokinetics-pkpd-toolkit) `(Python)` — 仅依赖 NumPy 的轻量 PK/PD 工具包，支持 NCA、一室拟合与 Emax 剂量-效应评估。 / Lightweight NumPy-only PK/PD toolkit for NCA, 1-compartment IV/oral fitting, and Emax modeling.
- [Down-To-Programme/PK_Model](https://github.com/Down-To-Programme/PK_Model) `(Python)` — 可 pip 安装的房室 PK 库（`dtp-pkmodel`），支持 SciPy ODE 求解与多方案对比绘图。 / Pip-installable compartmental PK library (`dtp-pkmodel`) with SciPy ODE solving and comparative plotting.
- [blakeaw/pysb-pkpd](https://github.com/blakeaw/pysb-pkpd) `(Python)` — 为 PySB 规则化建模框架扩展 1/2/3 室经验性与机制性 PK/PD 专用宏。 / Extends PySB rule-based modeling with domain macros for 1-, 2-, and 3-compartment PK/PD models.
- [shramish2057/NeoPKPD](https://github.com/shramish2057/NeoPKPD) `(Julia/Python)` — 结合 Julia 高速核心与 Python API/CLI 的开源 PK/PD、NLME、NCA 与 BE 平台。 / Multi-language (Julia core + Python API/CLI) platform for PK/PD simulation, NLME, NCA, and BE.
- [manuhuth/NoLimits.jl](https://github.com/manuhuth/NoLimits.jl) `(Julia)` — 开源 Julia NLME 框架，融合机制性 ODE、马尔可夫、Neural ODE、标准化流随机效应与 VPC。 / Open-source Julia NLME framework combining mechanistic ODEs, Markov models, Neural ODEs, and VPCs.
- [wahlquisty/FastPKSim.jl](https://github.com/wahlquisty/FastPKSim.jl) `(Julia)` — 专注恒速输注与静脉推注多房室药动学快速仿真的轻量高速 Julia 模拟器。 / Lightweight, high-speed Julia simulator for multi-compartment PK under infusions and bolus dosing.
- [simkaryote/gPKPDSim](https://github.com/simkaryote/gPKPDSim) `(MATLAB)` — 基于 MATLAB SimBiology 的开源图形界面应用，支持 PK/PD 仿真、参数扫描、拟合与 NCA。 / Open-source MATLAB SimBiology GUI app for PK/PD simulation, parameter scanning, fitting, and NCA.
- [benjaminrich/linpk](https://github.com/benjaminrich/linpk) `(R)` — 通过解析解快速模拟线性房室 PK 曲线并精确计算 $C_{\max}$、$T_{\max}$、AUC 与半衰期。 / Analytically simulates linear compartmental PK profiles and computes exact $C_{\max}$, $T_{\max}$, AUC, and $t_{1/2}$.
- [liucann/PKparmas1.0](https://github.com/liucann/PKparmas1.0) `(Python/Streamlit | 中文)` — 轻量级中文在线房室模型药代动力学参数拟合 Web 工具。 / Lightweight Chinese Streamlit web app for interactive compartmental PK parameter fitting from Excel data.
- [peytoncchen/PK-Visualization](https://github.com/peytoncchen/PK-Visualization) `(JS/Wasm)` — 斯坦福大学 Appel 实验室开发的纯前端 WebAssembly（Pyodide）房室 PK 模拟与可视化应用。 / Browser-based compartmental PK modeling and visualization app powered by WebAssembly (Pyodide).
- [SnowLeopard-io/ErgalicsStudio](https://github.com/SnowLeopard-io/ErgalicsStudio) `(TS/WebGPU | 中英)` — 浏览器端高性能科学计算工作台，内置药代动力学室分析、DDI 与 TDM 曲线拟合插件。 / Browser-based WebGPU/Wasm scientific studio with built-in PK compartmental, DDI, and TDM simulation plugins.

---

## 3. 数据准备、CDISC 转换与数据质控 / Data Preparation, CDISC & QC

- [NMautoverse/NMdata](https://github.com/NMautoverse/NMdata) `(R)` — 全链路 NONMEM 数据集准备、结构 QC、排除标记审计与运行结果自动合并工具。 / End-to-end NONMEM dataset prep, structural QC (`NMcheckData`), exclusion tracking, and output merging.
- [NMautoverse/NMcalc](https://github.com/NMautoverse/NMcalc) `(R)` — 轻量级药动学核心计算函数（梯形法 AUC、CV% 等），便于快速探索与模拟汇总。 / Lightweight essential pharmacometric calculations (trapezoidal AUC, CV%) for exploratory and simulation summaries.
- [metrumresearchgroup/mrgda](https://github.com/metrumresearchgroup/mrgda) `(R)` — 整合多源临床试验域并派生标准定量药理分析数据集的装配工具包。 / Data assembly toolkit for consolidating clinical trial domains into modeling-ready PMx datasets.
- [metrumresearchgroup/yspec](https://github.com/metrumresearchgroup/yspec) `(R)` — 基于 YAML 的定量药理数据规范管理、自动校验与 `define.pdf` 文档生成工具。 / YAML-based PMx dataset specification manager for automated validation, labeling, and `define.pdf` generation.
- [metrumresearchgroup/lastdose](https://github.com/metrumresearchgroup/lastdose) `(R/C++)` — 在复杂药动学给药记录中高速计算末次给药后时间（TAD）与最近一次给药剂量。 / Rapidly computes time after last dose (TAD) and most-recent dose amount across complex dosing records.
- [pharmaverse/admiral](https://github.com/pharmaverse/admiral) `(R)` — Pharmaverse 模块化 CDISC ADaM 构建工具箱，内置 `ADPC`/`ADPP`/`ADPPK` 派生模板。 / Modular pharmaverse toolbox for building CDISC ADaM datasets including `ADPC`, `ADPP`, and `ADPPK`.
- [kestrel99/pmxTools](https://github.com/kestrel99/pmxTools) `(R)` — 涵盖数据处理、闭式房室 PK 计算与 PsN/NONMEM 输出解析制表的实用工具集。 / Practical R utility suite for PMx data manipulation, closed-form PK math, and PsN output parsing.

---

## 4. 非房室分析（NCA）、生物等效性（BE）、IVIVC 与溶出 / NCA, Bioequivalence, IVIVC & Dissolution

- [humanpred/pknca](https://github.com/humanpred/pknca) `(R)` — 全功能稀疏与密集采样非房室分析（NCA）引擎，支持自动单位换算与 CDISC 输出。 / Comprehensive R engine for dense and sparse NCA with unit conversion, imputation, and CDISC support.
- [pharmaverse/aNCA](https://github.com/pharmaverse/aNCA) `(R/Shiny)` — 端到端交互式临床 NCA Web 应用，支持交互式 $\lambda_z$ 选点、CDISC 导出与可复现脚本生成。 / Interactive pharmaverse Shiny app for clinical NCA with visual $\lambda_z$ selection and reproducible R script export.
- [asancpt/NonCompart](https://github.com/asancpt/NonCompart) `(R | 韩国)` — 算法对齐 Phoenix WinNonlin 与 CDISC SDTM 的工业级 NCA 核心计算包。 / Industrial-strength R NCA package aligned with Phoenix WinNonlin formulas and CDISC SDTM conventions.
- [asancpt/ncar](https://github.com/asancpt/ncar) `(R | 韩国)` — 基于 `NonCompart` 一键生成含个体药时曲线的监管级 PDF/RTF NCA 报告。 / Regulatory-style PDF and RTF NCA report generator built on top of `NonCompart`.
- [asancpt/pkrshiny](https://github.com/asancpt/pkrshiny) `(R/Shiny | 韩英)` — 封装 `pkr`/`NonCompart` 的免代码交互式非房室分析 Shiny 网页应用。 / No-code interactive Shiny web interface for running noncompartmental PK analysis.
- [asancpt/BE](https://github.com/asancpt/BE) `(R | 韩国)` — 面向 2×2、2×4、4×4、Williams 与 Balaam 交叉设计的生物等效性统计与样本量包，对标 SAS PROC GLM/MIXED。 / Bioequivalence statistical analysis and sample size estimation across crossover designs replicating SAS PROC GLM/MIXED.
- [asancpt/BE-apps](https://github.com/asancpt/BE-apps) `(R/Shiny | 韩英)` — 集成非房室分析与生物等效性（BE）统计评估的交互式 Shiny 应用。 / Interactive Shiny application integrating PK noncompartmental analysis with bioequivalence statistics.
- [cran/bear](https://github.com/cran/bear) `(R)` — 面向 2×2×2 交叉与平行设计的平均生物等效性（ABE）与相对生物利用度统计分析 R 包。 / Average bioequivalence (ABE) and comparative bioavailability statistical analysis for crossover and parallel designs.
- [Detlew/PowerTOST](https://github.com/Detlew/PowerTOST) `(R | 德/奥)` — 行业标准生物等效性统计功效与样本量计算包（TOST、ABE、RSABE、ABEL）。 / Industry-standard R package for bioequivalence power and sample size calculations (TOST, RSABE, ABEL).
- [Helmut01/replicateBE](https://github.com/Helmut01/replicateBE) `(R)` — 遵循 EMA 指南（Method A/B）的高变异药物重复交叉设计 ABEL 生物等效性评价包。 / EMA-aligned ABEL bioequivalence evaluation package for replicate crossover designs of highly variable drugs.
- [juntotechnologies/bioeq](https://github.com/juntotechnologies/bioeq) `(Python)` — 纯 Python 生物等效性（BE）计算包，支持交叉与平行试验设计。 / Pure-Python package for pharmacokinetic data processing and crossover/parallel bioequivalence statistics.
- [PharmCat/MetidaNCA.jl](https://github.com/PharmCat/MetidaNCA.jl) `(Julia)` — 面向药物研发与大规模临床试验仿真后处理的高性能 Julia NCA 库。 / High-performance Julia NCA library suited for drug development and large-scale trial simulation post-processing.
- [PharmCat/MetidaBioeq.jl](https://github.com/PharmCat/MetidaBioeq.jl) `(Julia)` — 基于混合效应与广义线性模型计算几何均值比及 90% 置信区间的 Julia BE 评估包。 / Julia package for regulatory bioequivalence assessment using mixed-effects and generalized linear models.
- [matthiaskoenig/pkpdutils](https://github.com/matthiaskoenig/pkpdutils) `(Python | 德国)` — 支持单位感知 NCA、NONMEM/Monolix/ADNCA 读写、曲线拟合、BE 统计与 DDI 分级的 Python 库。 / Pure-Python PK/PD analysis library supporting unit-aware NCA, NONMEM/ADNCA I/O, curve fitting, BE, and DDI.
- [Open-Systems-Pharmacology/IVIVC-with-particle-dissolution-module-in-OSP](https://github.com/Open-Systems-Pharmacology/IVIVC-with-particle-dissolution-module-in-OSP) `(R/PK-Sim)` — 基于 OSP 套件的机制性 PBPK-IVIVC 工作流，将粒径分布与体外溶出关联至体内口服 PK。 / Mechanistic PBPK-based IVIVC workflow linking particle size distribution and dissolution kinetics to *in vivo* oral PK.
- [cran/Rivivc](https://github.com/cran/Rivivc) `(R)` — 通过数值反卷积与卷积实现线性 A 级体内外相关性（IVIVC）建模，支持非等距采样点。 / Performs Linear Level A IVIVC via numerical deconvolution and convolution handling unequal time grids.
- [vkaralis/ivivs-be](https://github.com/vkaralis/ivivs-be) `(Python)` — 结合胃肠道分段溶出、房室 PK ODE 与蒙特卡洛虚拟试验预测生物等效性的体内外模拟（IVIVS）工具。 / Python IVIVS framework combining GI dissolution, compartmental PK ODEs, and Monte Carlo trials to predict BE.
- [zhengguoxu/bootf2](https://github.com/zhengguoxu/bootf2) `(R)` — 依据 FDA/EMA 指南采用相似因子（$f_2$）与自助法 $f_2$ 90% 置信区间比较高变异体外溶出曲线。 / FDA/EMA-aligned dissolution profile comparison using similarity factor ($f_2$) and bootstrap $f_2$ 90% CIs.
- [piusdahinden/disprofas](https://github.com/piusdahinden/disprofas) `(R)` — 非参数体外溶出曲线相似性检验工具，支持 $f_1$/$f_2$、Shah 自助法 $f_2$、MCR 与 $T^2$ 检验。 / Non-parametric dissolution profile similarity testing including $f_1$, $f_2$, bootstrap $f_2$, MCR, and $T^2$ tests.
- [Shipbuilder/Bioequivalence](https://github.com/Shipbuilder/Bioequivalence) `(Scripts | 中文)` — 中文开发者上传的生物等效性（BE）试验统计分析参考脚本。 / Chinese-language statistical reference scripts for bioequivalence studies.

---

## 5. 模型诊断、可视化与自动化报告 / Diagnostics, Visualization & Automated Reporting

- [UUPharmacometrics/xpose](https://github.com/UUPharmacometrics/xpose) `(R)` — 现代 `ggplot2` 模型诊断框架，用于导入 NONMEM 输出并绘制 GOF、残差与 VPC 图。 / Modern `ggplot2`-based diagnostics framework for NONMEM/NLME goodness-of-fit and VPC plots.
- [UUPharmacometrics/xpose4](https://github.com/UUPharmacometrics/xpose4) `(R)` — 经典 NONMEM 建模辅助诊断包，基于 lattice 提供 GOF、VPC 与协变量筛选图。 / Classic NONMEM model-building aid providing lattice-based GOF diagnostics, VPCs, and covariate screening plots.
- [nlmixr2/xpose.nlmixr2](https://github.com/nlmixr2/xpose.nlmixr2) `(R)` — 将 `nlmixr2` 拟合对象桥接为标准 `xpose` 数据库对象以复用全套 `xpose` 诊断图。 / Bridges `nlmixr2` fit objects into standard `xpose` databases (`xpdb`) for GOF diagnostics.
- [nlmixr2/nlmixr2plot](https://github.com/nlmixr2/nlmixr2plot) `(R)` — 面向 `nlmixr2` 模型拟合结果的原生 `ggplot2` 诊断图与 VPC 绘图包。 / Native `ggplot2`-based diagnostic and visual predictive check plotting routines for `nlmixr2`.
- [certara/R-Xpose-NLME](https://github.com/certara/R-Xpose-NLME) `(R)` — 从 `Certara.RsNLME`/Phoenix NLME 输出构建 `xpose` 数据库对象（`Certara.Xpose.NLME`）。 / Creates `xpose` database (`xpdb`) objects directly from `Certara.RsNLME` and Phoenix NLME outputs.
- [ggPMXdevelopment/ggPMX](https://github.com/ggPMXdevelopment/ggPMX) `(R)` — 跨 Monolix、NONMEM、`nlmixr2` 一键生成符合 ISoP 标准的申报级 GOF 诊断图与报告。 / Standardized ISoP-aligned GOF diagnostic plotting and reporting across Monolix, NONMEM, and `nlmixr2`.
- [metrumresearchgroup/pmplots](https://github.com/metrumresearchgroup/pmplots) `(R)` — 提供面向定量药理分析的标准化、申报级探索性与拟合优度诊断图表。 / Standardized, publication-ready exploratory and goodness-of-fit diagnostic plots for pharmacometrics.
- [certara/tidyvpc](https://github.com/certara/tidyvpc) `(R)` — 基于 `data.table` 的高速管道式 VPC 引擎，支持分箱、无分箱（AQR/LOESS）、pcVPC 与 BLQ。 / Fast `data.table`-backed VPC engine supporting binned/binless (AQR/LOESS) VPCs, pcVPC, and BLQ censoring.
- [certara/R-VPCResults](https://github.com/certara/R-VPCResults) `(R/Shiny)` — 基于 `tidyvpc` 的交互式 VPC 配置与可复现绘图代码导出 Shiny 应用（`Certara.VPCResults`）。 / Interactive Shiny app built on `tidyvpc` to customize and export reproducible VPC code for NONMEM and NLME.
- [certara/R-ModelResults](https://github.com/certara/R-ModelResults) `(R/Shiny)` — 面向 NLME/NONMEM 结果的交互式 GOF 图表与表格定制 Shiny 应用（`Certara.ModelResults`）。 / Interactive Shiny GUI for generating customizable GOF plots and tables with exportable `xpose`/`flextable` code.
- [ronkeizer/vpc](https://github.com/ronkeizer/vpc) `(R)` — 灵活的跨平台 R 语言 VPC 工具包，支持连续型、分类型与事件时间（TTE）视觉预测检验。 / Flexible R package for continuous, categorical, and time-to-event Visual Predictive Checks across platforms.
- [UUPharmacometrics/ncappc](https://github.com/UUPharmacometrics/ncappc) `(R)` — 基于 NCA 暴露指标（$C_{max}$、$AUC$）对 PopPK/PD 模型执行后验预测检验（PPC）。 / Simulation-based posterior predictive check (PPC) evaluating PopPK/PD models via NCA exposure metrics.
- [pharmetheus/PMXForest](https://github.com/pharmetheus/PMXForest) `(R)` — 直接从 NONMEM `.cov`、PsN Bootstrap 或 SIR 输出自动生成含不确定性的协变量森林图。 / Automated covariate forest plots with uncertainty directly from NONMEM `.cov`, PsN bootstrap, or SIR outputs.
- [metrumresearchgroup/pmforest](https://github.com/metrumresearchgroup/pmforest) `(R)` — 直接基于模型参数与 `mrgsolve` 模拟输出生成高度可定制的协变量效应森林图。 / Generates customizable covariate effect forest plots directly from model parameters and `mrgsolve` simulations.
- [certara/coveffectsplot](https://github.com/certara/coveffectsplot) `(R/Shiny)` — 提供函数与交互式 Shiny 应用，绘制申报级协变量暴露影响森林图（亦见 [smouksassi/coveffectsplot](https://github.com/smouksassi/coveffectsplot)）。 / R package and Shiny app for producing standardized covariate-effect forest plots in PopPK/PD reports.
- [Novartis/xgxr](https://github.com/Novartis/xgxr) `(R)` — 诺华探索性图形（xGx）框架，提供标准化 PK/PD 与暴露-效应作图助手与草稿标注。 / Novartis exploratory graphics (`ggplot2`) helpers for reproducible PK/PD and exposure-response plotting.
- [metrumresearchgroup/pmtables](https://github.com/metrumresearchgroup/pmtables) `(R)` — 专为定量药理申报报告打造的 LaTeX/TeX 人口学、数据清单与参数估计表格生成器。 / Publication- and submission-grade LaTeX summary table generator tailored for pharmacometric reports.
- [certara/pmxpartabc](https://github.com/certara/pmxpartabc) `(R)` — 自动解析 NONMEM 运行目录与 YAML 配置，生成可直接申报的参数估计表（含 Bootstrap）。 / Parses NONMEM run directories and YAML specs to generate clean, report-ready parameter estimate tables.
- [philipdelff/tracee](https://github.com/philipdelff/tracee) `(R)` — 自动为保存的图表嵌入源脚本路径、时间戳与元数据印记，保障监管级代码可追溯性。 / Automates saving plots and tables with embedded source-script paths and timestamps for regulatory traceability.
- [kylebaron/mrgsim.sa](https://github.com/kylebaron/mrgsim.sa) `(R)` — 面向 `mrgsolve` 模型的局部与序列参数敏感度分析及可视化扩展包。 / Local and graphical parameter sensitivity analysis extension for `mrgsolve` PK/PD and QSP models.
- [nlmixr2/nlmixr2rpt](https://github.com/nlmixr2/nlmixr2rpt) `(R)` — 基于 YAML 规范自动将 `nlmixr2` 拟合结果生成结构化 Word 与 PPT 定量药理报告。 / YAML-driven automated Microsoft Word and PowerPoint report generator for `nlmixr2` model fits.
- [john-harrold/ruminate](https://github.com/john-harrold/ruminate) `(R/Shiny)` — 整合数据整理、绘图、PKNCA、`rxode2` 仿真与 Office 报告导出的低代码 Shiny 工作台。 / Modular Shiny PMx workbench combining data wrangling, PKNCA, `rxode2` simulation, and Word/PPT/Excel reporting.
- [Genentech/gPKPDviz](https://github.com/Genentech/gPKPDviz) `(R/Shiny)` — 基因泰克开源的交互式 `mrgsolve` PopPK/PD 仿真与虚拟人群探索 Shiny 平台。 / Interactive `mrgsolve`-powered Shiny platform for real-time PopPK/PD simulation and virtual population exploration.
- [Boehringer-Ingelheim/MVPapp](https://github.com/Boehringer-Ingelheim/MVPapp) `(R/Shiny | 德国)` — 支持在线编辑 `mrgsolve` 代码、NCA、敏感度分析与 NHANES 虚拟人群的模型可视化平台。 / Model Visualization Platform (Shiny) with live `mrgsolve` editing, NCA, sensitivity analysis, and NHANES demographics.
- [pipetcpt/2025-jscpt](https://github.com/pipetcpt/2025-jscpt) `(R/NONMEM | 韩/日)` — 直接从 NONMEM 输出自动生成项目反应理论（IRT）纵向药效模型发表级信息图。 / Automated publication-grade pharmacometric infographic generator from NONMEM IRT model outputs.

---

## 6. 临床药理监管、C-QTc、I/II 期剂量探索、E-R、CTS 与 FIH / Regulatory ClinPharm, C-QTc, Dose-Finding, E-R & FIH

- [FDA/PKView](https://github.com/FDA/PKView) `(R/Shiny)` — 美国 FDA 交互式临床药理审评工具，读取 CDISC SDTM/ADaM 数据自动生成 PK、剂量-效应与安全性报告。 / U.S. FDA interactive clinical pharmacology review app ingesting CDISC SDTM/ADaM data for automated PK/safety reviews.
- [A2-ai/cqtkit](https://github.com/A2-ai/cqtkit) `(R)` — 对齐 Garnett 白皮书标准的浓度-QTc（C-QTc）建模工作流包，涵盖预处理、EDA、LME 拟合与诊断。 / Streamlines Garnett white-paper Concentration-QTc (C-QTc) modeling: preprocessing, EDA, LME fitting, and diagnostics.
- [joannaparkinson/C-QTc-hands-on-tutorial](https://github.com/joannaparkinson/C-QTc-hands-on-tutorial) `(R)` — 《浓度-QTc 建模实践指南》配套可复现 R 脚本库，基于公开 PhysioNet 数据演示 ΔΔQTc 预测全流程。 / Reproducible hands-on C-QTc analysis tutorial implementing Garnett white-paper LME modeling and ΔΔQTc predictions.
- [FDA/CiPA](https://github.com/FDA/CiPA) `(R)` — 美国 FDA 官方 CiPA 心脏安全性计算机模拟代码库，支持 hERG 动力学拟合与人心室动作电位仿真。 / Official U.S. FDA CiPA *in silico* cardiac safety suite for hERG kinetics, Bayesian Hill MCMC, and action potential simulations.
- [Novartis/OncoBayes2](https://github.com/Novartis/OncoBayes2) `(R/Stan)` — 诺华开源贝叶斯逻辑回归模型（BLRM），支持 EXNEX 分层借用与 EWOC 准则，用于单药/联合肿瘤 I 期剂量递增。 / Bayesian Logistic Regression Models (BLRM) with EXNEX borrowing and EWOC for single/combination Phase I escalation.
- [openpharma/crmPack](https://github.com/openpharma/crmPack) `(R)` — 面向对象的模型驱动剂量递增框架，支持 CRM、BLRM 及毒性-生物标志物双终点试验设计。 / Object-oriented framework for model-based Phase I dose-escalation including CRM, BLRM, and dual-endpoint designs.
- [brockk/escalation](https://github.com/brockk/escalation) `(R)` — 统一模块化语法的 I/II 期剂量探索框架，支持 BOIN、BOIN12、mTPI-2、CRM 与 TITE-CRM 模拟。 / Modular grammar to specify, chain stopping rules, and simulate BOIN, mTPI-2, CRM, and TITE-CRM dose-finding designs.
- [openpharma/DoseFinding](https://github.com/openpharma/DoseFinding) `(R/C)` — 实现监管认可的 MCP-Mod 方法，用于 II 期剂量探索试验的规划、最优设计与剂量-效应分析。 / Regulatory-endorsed MCP-Mod methodology for planning, optimal design, and dose-response analysis in Phase II trials.
- [cran/BOIN](https://github.com/cran/BOIN) `(R)` — 实现单药与联合用药 I 期贝叶斯最优区间（BOIN）设计，广泛用于 FDA Project Optimus 剂量优化。 / Bayesian Optimal Interval (BOIN) design for single-agent and combination Phase I trials under Project Optimus.
- [yamagubed/boinet](https://github.com/yamagubed/boinet) `(R)` — 实现综合评估疗效与毒性的 BOIN-ET 系列 I/II 期设计，以确定最佳生物学剂量（OBD）。 / Model-assisted Phase I/II BOIN-ET designs jointly optimizing efficacy and toxicity to identify Optimal Biological Dose.
- [brockk/trialr](https://github.com/brockk/trialr) `(R/Stan)` — 基于 RStan 的贝叶斯临床试验设计工具集，涵盖 CRM、TITE-CRM 与 EffTox 无缝 I/II 期模型。 / Collection of Bayesian clinical trial designs in RStan including CRM, TITE-CRM, and EffTox seamless Phase I/II.
- [mikesweeting/bcrm](https://github.com/mikesweeting/bcrm) `(R)` — 实现单/双参数贝叶斯连续重新评估法（CRM）及 I 期试验运行特征模拟。 / One- and two-parameter Bayesian Continual Reassessment Method (CRM) designs and operating-characteristic simulations.
- [cran/dfcrm](https://github.com/cran/dfcrm) `(R)` — 经典 I 期剂量探索 R 包，提供标准 CRM 及针对迟发性毒性的 TITE-CRM 算法。 / Foundational R package for Phase I dose-finding via CRM and Time-to-Event CRM (TITE-CRM).
- [cran/clinDR](https://github.com/cran/clinDR) `(R)` — 面向临床药理 II 期剂量范围研究的贝叶斯与最大似然 Emax 剂量-效应建模包。 / Bayesian and maximum-likelihood Emax dose-response modeling tools tailored for Phase II dose-ranging analyses.
- [Genentech/BayesERtools](https://github.com/Genentech/BayesERtools) `(R/Stan)` — 基因泰克开源贝叶斯暴露-效应（E-R）建模工具包，支持二分类/连续终点与决策森林图。 / Bayesian exposure-response modeling toolkit over Stan for binary/continuous endpoints and decision forest plots.
- [metrumresearchgroup/confounded-exposure-metrics](https://github.com/metrumresearchgroup/confounded-exposure-metrics) `(R/NONMEM)` — 揭示肿瘤 E-R 与生存分析（TTE）中不同暴露指标引入混杂偏倚的仿真方法学仓库。 / Methodological simulation pipeline demonstrating exposure-metric confounding bias in oncology E-R and TTE analyses.
- [clay-good/onkos](https://github.com/clay-good/onkos) `(Python)` — 分级标注的肿瘤生长抑制（TGI）与 E-R 模型库，支持导出至 NONMEM、SBML、`rxode2` 与 Pumas。 / Curated oncology TGI and E-R model library with transpilation to NONMEM, SBML, `rxode2`, and Pumas.
- [orlacchioresearch/tumor-growth-inhibition-modeling](https://github.com/orlacchioresearch/tumor-growth-inhibition-modeling) `(Python)` — 临床前异种移植瘤生长曲线拟合（指数/Gompertz/Logistic）与 TGI%/%T/C 计算工具。 / Python toolkit for preclinical xenograft tumor growth curve fitting and TGI% / %T/C calculation.
- [campsisverse/campsis](https://github.com/campsisverse/campsis) `(R)` — 引擎无关的临床试验仿真（CTS）平台，解耦试验设计与底层 `rxode2`/`mrgsolve` 求解器。 / Engine-agnostic clinical trial simulation (CTS) platform supporting both `rxode2` and `mrgsolve` backends.
- [andrewhooker/PopED](https://github.com/andrewhooker/PopED) `(R)` — 基于费雪信息矩阵（FIM）的 NLME 群体与个体最优临床采样与给药试验设计工具。 / Optimal experimental design for NLME models using the Fisher Information Matrix (FIM) to optimize sampling and dosing.
- [iame-researchCenter/PFIM](https://github.com/iame-researchCenter/PFIM) `(R | 法国)` — 基于群体 FIM 评估与优化 NLME 临床采样设计，支持协变量、IOV 与多种优化算法。 / Population FIM optimal design package supporting covariates, IOV, and Fedorov-Wynn/PSO optimization.
- [phuse-org/toxSummary](https://github.com/phuse-org/toxSummary) `(R/Shiny)` — 交互式汇总重复给药毒理暴露安全窗与跨种属转化，支撑首次人体（FIH）起始剂量论证。 / PHUSE Shiny app summarizing repeat-dose tox exposure margins and cross-species translation for FIH dose justification.
- [pipetcpt/DallphinAtoM](https://github.com/pipetcpt/DallphinAtoM) `(R | 韩英)` — 利用异速生长缩放与生理参数从临床前动物数据预测人体 PK 参数。 / Allometric scaling and physiological animal-to-human PK parameter prediction tool for early FIH projection.
- [m-amanda/Analytical-Methods-Validation-with-R](https://github.com/m-amanda/Analytical-Methods-Validation-with-R) `(R/Shiny)` — 生物分析方法学验证 Shiny 应用，支持基质效应、标准曲线线性、方差齐性与 LOD/LOQ 评估。 / Interactive Shiny app for bioanalytical method validation covering selectivity, linearity, homoscedasticity, and LOD/LOQ.
- [giovannisolarino/Methods-Validation-App-Web](https://github.com/giovannisolarino/Methods-Validation-App-Web) `(Python)` — 面向受监管生物分析实验室评估多日多水平 LC-MS 标曲及准确度/精密度的 Web 应用。 / Python web app for regulated bioanalytical labs to evaluate multi-day LC-MS calibration curves and validation metrics.

---

## 7. 模型引导精准给药（MIPD）、临床 TDM、抗感染 PTA 与 TCI / Clinical MIPD, TDM, Antimicrobial PTA & TCI

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
- [InsightRX/mipdeval](https://github.com/InsightRX/mipdeval) `(R)` — 在历史临床 TDM 数据集上评估群体 PK/PD 模型迭代贝叶斯预测准确度与偏倚的工具包。 / Evaluates predictive accuracy and bias of population PK/PD models on historical TDM datasets under Bayesian forecasting.
- [InsightRX/mipdtrial](https://github.com/InsightRX/mipdtrial) `(R)` — 在模型引导精准给药（MIPD）自适应临床试验方案下模拟 PK/PD 终点与目标达标率。 / Simulates clinical PK/PD endpoints and target attainment metrics under adaptive MIPD trial protocols.
- [Martin-Umpierrez/exeval](https://github.com/Martin-Umpierrez/exeval) `(R)` — 自动化执行文献 PopPK/PD 模型在独立医院本地临床队列上的外部验证与贝叶斯预测评估。 / Reproducible external evaluation framework for benchmarking published PopPK/PD models on local hospital TDM cohorts.

### 7.2 抗感染 PK/PD、PTA/CFR 与抗菌/抗真菌 TDM / Antimicrobial PK/PD, PTA/CFR & TDM

- [liangRXdev/vanco-auc-calc](https://github.com/liangRXdev/vanco-auc-calc) `(JS/PWA | 繁中/英)` — 纯前端离线万古霉素 AUC 个体化计算器，含 Sawchuk-Zaske 双点反算、双室贝叶斯与 AKI/妊娠警示。 / Offline browser PWA for vancomycin AUC dosing with Sawchuk-Zaske, 2-compartment Bayesian MAP, and clinical alerts.
- [asancpt/shiny-vtdm](https://github.com/asancpt/shiny-vtdm) `(R/Shiny | 韩英)` — 韩国峨山医院万古霉素二室 PopPK 贝叶斯精准给药 Shiny 应用。 / Korean vancomycin TDM Shiny app implementing a 2-compartment PopPK Bayesian dosing model.
- [pipetcpt/tdm-vancomycin](https://github.com/pipetcpt/tdm-vancomycin) `(R/Shiny | 韩英)` — 韩国天主教大学 PIPET 万古霉素 PopPK 给药仿真与 TDM 自动化 Shiny 应用。 / Open-source Shiny app for vancomycin PopPK dosing simulation and TDM automation.
- [kpessa/vanco-auc](https://github.com/kpessa/vanco-auc) `(Excel/VBA)` — 美国医院实际部署的万古霉素经验给药与双点梯形法 AUC24/MIC 计算工具包。 / Hospital-deployed Excel/VBA toolkit for vancomycin empirical dosing and paired-level trapezoidal AUC24/MIC.
- [njrhodes/bds-app](https://github.com/njrhodes/bds-app) `(R/Shiny/Stan)` — 贝叶斯给药模拟应用集合，内置美罗培南与哌拉西林-他唑巴坦 MIPD 精准给药模块。 / Shiny-based Bayesian Dosing Simulator monorepo featuring meropenem and piperacillin-tazobactam MIPD modules.
- [cptbern/ShinyFlucloxacillin](https://github.com/cptbern/ShinyFlucloxacillin) `(R/Shiny | 瑞士)` — 伯尔尼大学开发的住院患者氟氯西林个体化贝叶斯 TDM 交互式 Shiny 应用。 / Interactive clinical TDM/MIPD Shiny web app (University of Bern) for personalized flucloxacillin dosing.
- [piranfar/caz-avi-evidence-composite-pkpd](https://github.com/piranfar/caz-avi-evidence-composite-pkpd) `(R/Python)` — 评估持续输注头孢他啶-阿维巴坦联合达标概率（PTA）与累积反应分数（CFR）的蒙特卡洛 PK/PD 模拟库。 / Reproducible Monte Carlo PK/PD simulation workflow evaluating joint PTA and CFR for ceftazidime-avibactam.
- [shemtsai/Aminoglycoside-Calculator](https://github.com/shemtsai/Aminoglycoside-Calculator) `(HTML/JS)` — 感染科药师开发的轻量级浏览器端氨基糖苷类非梯形法药动学给药计算器。 / Lightweight browser-based non-trapezoidal aminoglycoside pharmacokinetic dosing calculator by an ID pharmacist.
- [joshcase/code-blue-gentamicin](https://github.com/joshcase/code-blue-gentamicin) `(Python/Web)` — 面向临床医生和药师的教学型庆大霉素药动学给药与安全校验计算器。 / Educational gentamicin dosing calculator demonstrating clinical pharmacokinetic dosing rules and safety checks.
- [727397883/Rifampicin-PopPK-Repository](https://github.com/727397883/Rifampicin-PopPK-Repository) `(R/Shiny | 中国)` — 中南大学湘雅医院开源的抗结核药利福平 PopPK 文献模型库与 `mrgsolve` 给药模拟应用。 / Open-source rifampicin PopPK model repository and interactive `mrgsolve` Shiny dosing simulator.
- [HassDhia/antibiosim](https://github.com/HassDhia/antibiosim) `(Python)` — 兼容 Gymnasium 的抗菌药物 PK/PD 达标、剂量优化与细菌动力学仿真环境。 / Gymnasium-compatible simulation environments modeling antibiotic PK/PD target attainment and bacterial dynamics.

### 7.3 免疫抑制剂、窄治疗窗药物与临床计算器（含儿科/CRRT）/ Immunosuppressant, NTI & Hospital Calculators

- [FelicienLL/BUSULFANAPP](https://github.com/FelicienLL/BUSULFANAPP) `(R/Shiny | 法国)` — 面向儿童造血干细胞移植（HSCT）患者的白消安（Busulfan）贝叶斯精准给药 Shiny 应用。 / `mapbayr`-powered Shiny application for model-informed precision dosing of busulfan in pediatric HSCT patients.
- [wojjy001/infliximab-bayes](https://github.com/wojjy001/infliximab-bayes) `(R)` — 炎症性肠病（IBD）英夫利昔单抗维持治疗的贝叶斯预测与自适应给药仿真（配套 [wojjy001/adaptive-infliximab](https://github.com/wojjy001/adaptive-infliximab)）。 / Bayesian forecasting and adaptive dosing simulation for infliximab maintenance therapy in IBD.
- [abusuraihsakhri/digoxin-therapeutic-level-estimator](https://github.com/abusuraihsakhri/digoxin-therapeutic-level-estimator) `(HTML/JS)` — 根据患者生理参数与给药史估算地高辛血药浓度与治疗窗状态的轻量工具。 / Estimates digoxin plasma concentrations and therapeutic-range status from physiological variables and dosing history.
- [pharmot/multipurpose-calculator](https://github.com/pharmot/multipurpose-calculator) `(HTML/JS)` — 综合医院药学计算套件（VMFH），含万古霉素 AUC、氨基糖苷类、校正苯妥英钠、肝素、CrCl 与 NICU TPN。 / Comprehensive hospital pharmacy calculator suite covering vancomycin AUC, aminoglycosides, phenytoin, heparin, and NICU TPN.
- [jeremy-steinberg/Paediatric-Dosing](https://github.com/jeremy-steinberg/Paediatric-Dosing) `(JS/HTML5)` — 零依赖纯前端儿科按体重给药（mg/mL）临床计算器（基于新西兰处方集）。 / Zero-dependency client-side pediatric weight-based dosing calculator (mg and mL) based on NZF guidelines.
- [stalex444/CRRT_simulator](https://github.com/stalex444/CRRT_simulator) `(HTML/JS)` — 交互式 ICU 连续性肾脏替代治疗（CRRT）模拟器，含实时滤过分数监测与内置药物给药计算器。 / Interactive ICU CRRT training simulator with real-time filtration fraction monitoring and integrated drug dosing calculator.
- [Londopy/Clinical_IQ](https://github.com/Londopy/Clinical_IQ) `(TS/Python)` — 全栈临床决策支持 Web 应用，集成肾功能调量体重计算器与静脉输注滴速计算器。 / Full-stack clinical decision support web app bundling renal-adjusted weight dosing and IV infusion rate calculators.
- [cloveropen/pass](https://github.com/cloveropen/pass) `(Web | 中文)` — 临床合理用药监测系统（PASS）开源参考实现，含医嘱审方、四级风险警示与 DDI 审查。 / Open-source clinical prescription automatic screening system (PASS) with tiered alerts and DDI checks.
- [yusuketakuma/pharma-free-tools](https://github.com/yusuketakuma/pharma-free-tools) `(HTML/JS | 日文)` — 面向日本临床药师的 24 款免费网页工具，含基于肌酐清除率的抗菌药肾功能调量计算器。 / Collection of ~24 browser-based clinical pharmacy tools for Japanese pharmacists including renal dosing calculators.
- [koikelab/medication_eq_R](https://github.com/koikelab/medication_eq_R) `(R | 日英)` — 基于日本精神科标准自动计算精神科药物等效剂量的 R 工具。 / Automated calculation of psychotropic medication equivalent doses using Japanese psychiatric standards.
- [teezeit/medication-calculator](https://github.com/teezeit/medication-calculator) `(TS/React | 德国)` — 纯前端双指数药动学计算与 Plotly 多方案血药浓度对比单页应用。 / Client-side SPA for bi-exponential pharmacokinetic calculations and Plotly multi-regimen curve comparisons.

### 7.4 围术期麻醉 TCI、阿片解救与胰岛素-血糖 PK/PD / Anesthesia TCI, Opioid Rescue & Glucose-Insulin PK/PD

- [vitaldb/tivatci](https://github.com/vitaldb/tivatci) `(Python | 韩国)` — 开源全凭静脉麻醉（TIVA）与靶控输注（TCI）Python 库，内置 Schnider/Marsh/Minto/Eleveld 模型。 / Open-source Python library for TIVA/TCI PK/PD modeling (Schnider, Marsh, Minto, Eleveld, Gepts) and LBM formulas.
- [luktinghin/simtiva](https://github.com/luktinghin/simtiva) `(JS/PWA)` — 离线 PWA 靶控输注模拟器，支持丙泊酚与瑞芬太尼多模型及双药 PD 协同交互模拟。 / Offline PWA simulating TCI/TIVA for propofol and remifentanil with dual-drug PD interaction modeling.
- [BobAubouin/Python_Anesthesia_Simulator](https://github.com/BobAubouin/Python_Anesthesia_Simulator) `(Python)` — 模拟丙泊酚、瑞芬太尼、去甲肾上腺素对 BIS/MAP/心输出量 PK/PD 效应的闭环麻醉基准仿真器。 / Multi-drug anesthesia PK/PD simulator (BIS, MAP, cardiac output) serving as a benchmark for closed-loop/RL control.
- [ManuMerlo/AReS-Anesthesia-Response-Simulator](https://github.com/ManuMerlo/AReS-Anesthesia-Response-Simulator) `(Python/MATLAB)` — 综合 TIVA 患者响应模拟器（AReS），涵盖 4 药 TCI 输注、手术应激与体液丢失动力学。 / Comprehensive TIVA patient response simulator modeling 4 drugs, TCI pumps, surgical stress, and fluid dynamics.
- [jarretrt/tci](https://github.com/jarretrt/tci) `(R)` — 实现丙泊酚与瑞芬太尼房室 PK/PD 靶控输注速率算法及闭环贝叶斯参数更新。 / Implements TCI infusion-rate algorithms and closed-loop Bayesian updating for propofol and remifentanil PK/PD.
- [fra-mar/tci_simulator](https://github.com/fra-mar/tci_simulator) `(Python)` — Python 多房室药动学 TCI 泵输注速率与血浆/效应室浓度曲线模拟器。 / Python multi-compartment PK simulator computing TCI pump infusion rates and plasma vs. effect-site curves.
- [seazuma/pkpd](https://github.com/seazuma/pkpd) `(JS/HTML | 日英)` — 离线可用的浏览器端麻醉药三室 PK/PD 与 TCI 模拟器（丙泊酚/芬太尼/咪达唑仑，含 BIS 预测）。 / Offline browser-based 3-compartment anesthetic PK/PD and TCI simulator with variability bands and BIS prediction.
- [ysuzuki1978/rocuronium-pkpd-simulator](https://github.com/ysuzuki1978/rocuronium-pkpd-simulator) `(JS/PWA | 日英)` — 模拟罗库溴铵 PK 与肌松药效（TOF 比值）的离线 PWA，集成 5 个含日本临床协变量的验证模型。 / Offline PWA simulating rocuronium PK and neuromuscular blockade (TOF) across 5 validated clinical models.
- [ysuzuki1978/remimazolam-tci-simulator](https://github.com/ysuzuki1978/remimazolam-tci-simulator) `(JS/HTML | 日英)` — 实现日本 Masui (2022) 模型的瑞马唑仑效应室浓度 TCI/TIVA 模拟器，支持 CSV 导出。 / Effect-site TCI simulator for remimazolam implementing the Masui (2022) PK model with CSV export.
- [ysuzuki1978/propofol-tci-simulator](https://github.com/ysuzuki1978/propofol-tci-simulator) `(JS/HTML | 日英)` — 基于 Eleveld (2018) 框架的丙泊酚效应室靶控输注交互式模拟器。 / Interactive propofol effect-site TCI simulator built on the Eleveld (2018) PK/PD framework.
- [Clinical-Pharmacy-Saarland-University/pi_pumpsim](https://github.com/Clinical-Pharmacy-Saarland-University/pi_pumpsim) `(Python/Svelte | 德英)` — 德国萨尔大学“Dr. Dosis”静脉输注药动学实时仿真触屏教学演示系统。 / Interactive FastAPI + Svelte IV infusion pharmacokinetics simulation demo ("Dr. Dosis") with pump visualization.
- [FDA/Mechanistic-PK-PD-Model-to-Rescue-Opioid-Overdose](https://github.com/FDA/Mechanistic-PK-PD-Model-to-Rescue-Opioid-Overdose) `(R)` — 美国 FDA 机制性 PK/PD 模型，模拟芬太尼/卡芬太尼所致呼吸抑制并评估纳洛酮解救给药方案。 / U.S. FDA mechanistic PK/PD model simulating opioid-induced respiratory depression and naloxone rescue regimens.
- [practicefusion/mmecalculator](https://github.com/practicefusion/mmecalculator) `(C#)` — 解析自由文本处方用法并计算每日最大吗啡毫克当量（MME）以监测阿片过量风险的库与 API。 / C# library and API parsing free-text prescription sigs to calculate maximum daily Morphine Milligram Equivalents (MME).
- [jxx123/simglucose](https://github.com/jxx123/simglucose) `(Python)` — 经 FDA 批准的 UVA/Padova 1 型糖尿病葡萄糖-胰岛素 PK/PD 模拟器（兼容 Gymnasium）。 / Python implementation of the FDA-approved UVA/Padova Type 1 Diabetes glucose-insulin PK/PD simulator.
- [Perceptus/GlucoSym](https://github.com/Perceptus/GlucoSym) `(JS/Python)` — 模拟人体葡萄糖-胰岛素代谢与胰岛素 PK 以测试闭环人工胰腺控制算法。 / Simulates human glucose-insulin metabolic dynamics and insulin PK for closed-loop artificial pancreas testing.
- [1paulpo1/uva-padova-glucose-control-system](https://github.com/1paulpo1/uva-padova-glucose-control-system) `(C++/Python)` — 基于 CGM、饮食与胰岛素泵记录实现个体化 UVA/Padova PK/PD 参数辨识与血糖预测。 / Personalized UVA/Padova glucose-insulin PK/PD parameter identification and forecasting from CGM and pump logs.

### 7.5 多房室血药浓度追踪与动态校准 / Multi-Compartment Tracking & Dynamic Calibration

- [xingqimiao/Kira-HRT-Tracker](https://github.com/xingqimiao/Kira-HRT-Tracker) `(TS | 中英)` — 隐私优先给药追踪与 PopPK 模拟应用，内置 MAP/EKF/OU-Kalman 4 种血检校准器并支持 MCP 协议。 / Privacy-first PK tracker featuring 4 blood-level calibration estimators (MAP, EKF, OU-Kalman) and MCP integration.
- [LaoZhong-Mihari/HRT-Recorder-PKcomponent-Test](https://github.com/LaoZhong-Mihari/HRT-Recorder-PKcomponent-Test) `(Swift | 中英)` — 原生三室模型与双相肌注库房动力学解析计算引擎，支持多途径吸收与体重校正。 / Native Swift PK engine implementing 3-compartment, biphasic depot kinetics, and multi-route absorption models.
- [TransmtfTeam/Transmtf-HRT-Tracker](https://github.com/TransmtfTeam/Transmtf-HRT-Tracker) `(TS | 中英)` — 支持翻转动力学（flip-flop）、三室透皮级联吸收及贝叶斯/EKF 实测校准的 PK 仿真框架。 / Web PK tracker supporting flip-flop kinetics, 3-compartment cascade absorption, and Bayesian/EKF calibration.
- [meowhuan/Oyama-s-HRT-Tracker](https://github.com/meowhuan/Oyama-s-HRT-Tracker) `(TS | 多语言)` — 基于三室与双相库房解析式的本地血药浓度与 AUC 实时模拟可视化 Web 工具。 / Multi-lingual local web simulator for real-time 3-compartment concentration-time curves and AUC visualization.
- [Trans-Prism/Trans-Prism](https://github.com/Trans-Prism/Trans-Prism) `(Flutter/JS | 中文)` — 跨平台隐私优先工具箱，内置多室指数衰减叠加血药浓度曲线模拟器与用药时间线。 / Cross-platform Flutter offline toolkit with multi-compartment superposition PK curve simulation and dosing timeline.
- [WHSAH/estrannaise.js](https://github.com/WHSAH/estrannaise.js) `(JS)` — 纯前端浏览器三房室雌二醇药动学与贝叶斯参数推断模拟器，支持任意给药方案。 / Client-side browser simulator for 3-compartment estradiol PK and Bayesian inference under arbitrary dosing regimens.

---

## 8. 生理药代动力学（PBPK）、IVIVE、DDI 与特殊人群 / PBPK, IVIVE, DDI & Special Populations

- [Open-Systems-Pharmacology/PK-Sim](https://github.com/Open-Systems-Pharmacology/PK-Sim) `(C#/.NET | 德国)` — 旗舰级开源全身 PBPK 建模与仿真平台，内置成人、儿科及特殊人群生理数据库。 / Flagship open-source whole-body PBPK modeling platform with adult, pediatric, and special-population physiology.
- [Open-Systems-Pharmacology/MoBi](https://github.com/Open-Systems-Pharmacology/MoBi) `(C#/.NET | 德国)` — 与 PK-Sim 互补的多尺度生物仿真与机理 QSP/PBPK 建模软件，支持自定义生化反应网络。 / Multiscale biosimulation and mechanistic QSP/PBPK tool complementing PK-Sim for custom reaction networks.
- [Open-Systems-Pharmacology/OSPSuite.Core](https://github.com/Open-Systems-Pharmacology/OSPSuite.Core) `(C#/.NET)` — PK-Sim、MoBi 及各语言绑定共用的底层核心 PBPK 计算引擎与仿真内核。 / Foundational core computational engine, data structures, and simulation kernel shared across the OSP Suite.
- [Open-Systems-Pharmacology/OSPSuite-R](https://github.com/Open-Systems-Pharmacology/OSPSuite-R) `(R/C++)` — PK-Sim 与 MoBi 的编程式 R 接口，支持无 GUI 批量运行 PBPK 仿真与参数扫描。 / Programmatic R interface for headless PK-Sim/MoBi batch simulations, parameter sweeps, and reporting.
- [Open-Systems-Pharmacology/Matlab-Toolbox](https://github.com/Open-Systems-Pharmacology/Matlab-Toolbox) `(MATLAB)` — 从 MATLAB 程序化操控、批量仿真与参数识别 PK-Sim/MoBi 模型的官方工具箱。 / Programmatic MATLAB interface for batch simulation and parameter identification of PK-Sim and MoBi models.
- [Open-Systems-Pharmacology/OSPSuite.ReportingEngine](https://github.com/Open-Systems-Pharmacology/OSPSuite.ReportingEngine) `(R)` — 自动生成 OSP PBPK/QSP 模型标准化资质验证流程、诊断图与申报级报告的 R 工具包。 / Automates standardized qualification workflows, diagnostics, and regulatory reports for OSP PBPK/QSP models.
- [Open-Systems-Pharmacology/OSPSuite.ParameterIdentification](https://github.com/Open-Systems-Pharmacology/OSPSuite.ParameterIdentification) `(R)` — 为 PK-Sim/MoBi 模型提供程序化参数识别、优化拟合与不确定性分析。 / Programmatic parameter estimation, optimization, and uncertainty analysis for PK-Sim and MoBi models.
- [Open-Systems-Pharmacology/TLF-Library](https://github.com/Open-Systems-Pharmacology/TLF-Library) `(R)` — 面向 OSP 生态生成标准化药动学表格、清单与验证图表的面向对象 R 可视化框架。 / Object-oriented R visualization framework (`tlf`) for standardized tables, listings, and qualification figures.
- [Open-Systems-Pharmacology/OSPSuite.RUtils](https://github.com/Open-Systems-Pharmacology/OSPSuite.RUtils) `(R)` — 为全部 OSP Suite R 包提供数据校验、类型检查与日志记录的共享底层工具包。 / Shared utility package supplying validation, type-checking, and helper routines across OSP R packages.
- [Open-Systems-Pharmacology/OSP-PBPK-Model-Library](https://github.com/Open-Systems-Pharmacology/OSP-PBPK-Model-Library) `(PK-Sim/R)` — 经同行评议的开源 PBPK 化合物验证模型与评估报告库。 / Peer-reviewed library of qualified open-source PBPK substance models and evaluation reports.
- [Open-Systems-Pharmacology/OSP-Qualification-Reports](https://github.com/Open-Systems-Pharmacology/OSP-Qualification-Reports) `(Markdown/R)` — 集中汇总并在每次版本发布时自动编译平台级 PBPK 资质验证报告的官方仓库。 / Centralized repository auto-compiling platform-wide PBPK qualification reports (DDIs, pediatrics, transporters).
- [Open-Systems-Pharmacology/Qualification-DDI-CYP3A4](https://github.com/Open-Systems-Pharmacology/Qualification-DDI-CYP3A4) `(PK-Sim/R)` — 针对 CYP3A4 介导药物相互作用（DDI）的监管级全身 PBPK 资格验证方案与数据集。 / Regulatory-grade PBPK qualification plan and datasets evaluating CYP3A4-mediated drug-drug interactions.
- [Open-Systems-Pharmacology/Pediatric_Qualification_Package_CYP3A4_Ontogeny](https://github.com/Open-Systems-Pharmacology/Pediatric_Qualification_Package_CYP3A4_Ontogeny) `(PK-Sim)` — 验证从婴幼儿到青少年 CYP3A4 酶发育（Ontogeny）与儿科外推性能的官方资质包。 / Formal OSP qualification package validating pediatric scaling and CYP3A4 enzyme ontogeny from infants to adolescents.
- [Open-Systems-Pharmacology/Vancomycin-Model](https://github.com/Open-Systems-Pharmacology/Vancomycin-Model) `(PK-Sim/R)` — 聚焦肾小球滤过清除的万古霉素全身 PBPK 模型与验证报告。 / Whole-body PBPK model and evaluation report for vancomycin focusing on GFR-mediated renal clearance.
- [Open-Systems-Pharmacology/Voriconazole-Model](https://github.com/Open-Systems-Pharmacology/Voriconazole-Model) `(PK-Sim)` — 刻画伏立康唑非线性代谢、CYP2C19 多态性与 CYP3A4 时间依赖性抑制的全身 PBPK 模型。 / Validated whole-body PBPK model of voriconazole capturing nonlinear metabolism and CYP2C19/CYP3A4 effects.
- [Open-Systems-Pharmacology/Voriconazole-Tacrolimus-DDGI](https://github.com/Open-Systems-Pharmacology/Voriconazole-Tacrolimus-DDGI) `(PK-Sim)` — 量化伏立康唑与他克莫司之间高风险药物-药物-基因相互作用（DDGI）的全身 PBPK 模型。 / Whole-body PBPK modeling of clinically critical drug-drug-gene interactions between voriconazole and tacrolimus.
- [Open-Systems-Pharmacology/Pregnancy-Models](https://github.com/Open-Systems-Pharmacology/Pregnancy-Models) `(PK-Sim/MoBi)` — 纳入孕期生理变化与母胎/胎盘转运模块的妊娠期全身 PBPK 框架。 / Whole-body pregnancy PBPK framework incorporating gestational physiology and maternal-fetal placental transfer.
- [Open-Systems-Pharmacology/Lactation-PBPK-model](https://github.com/Open-Systems-Pharmacology/Lactation-PBPK-model) `(MoBi/SQLite)` — 模拟母体药物向乳汁转运及婴儿相对摄入剂量（RID）的哺乳期 PBPK 构建模块。 / Lactation PBPK building blocks for simulating drug transfer into breast milk and infant systemic exposure.
- [Clinical-Pharmacy-Saarland-University/PBPK-Models](https://github.com/Clinical-Pharmacy-Saarland-University/PBPK-Models) `(PK-Sim/R | 德国)` — 德国萨尔大学维护的经同行评议 PBPK 与药物-药物/药物-基因相互作用（DDI/DDGI）模型库。 / Peer-reviewed PBPK and DDI/DDGI model repository maintained by Saarland University.
- [Sanofi-Public/saemixPBPK](https://github.com/Sanofi-Public/saemixPBPK) `(R | 法国)` — 将开源 SAEM 非线性混合效应算法与 OSP Suite 全身 PBPK/QSP 模型结合进行群体估计。 / Integrates SAEM NLME parameter estimation with OSP Suite whole-body PBPK/QSP models.
- [esqLABS/esqlabsR](https://github.com/esqLABS/esqlabsR) `(R)` — 基于结构化 Excel 配置模板标准化管理大型多情景 OSP Suite PBPK/QSP 工作流。 / Standardized R workflow package managing multi-scenario OSP Suite PBPK/QSP projects via Excel templates.
- [certara/Simcyp-R-Scripts](https://github.com/certara/Simcyp-R-Scripts) `(R)` — Certara 官方 Simcyp R 集成示例脚本库，支持程序化操控 Simcyp 模拟器与解析输出。 / Official Certara R scripts for programmatically controlling the Simcyp Simulator and parsing PBPK outputs.
- [mba16hk/Simcyp-R-Workflow](https://github.com/mba16hk/Simcyp-R-Workflow) `(R)` — 自动查询 ChEMBL/PubChem 理化参数并对接 Simcyp 执行批量 PBPK 仿真的工作流（SimRFlow）。 / High-throughput R workflow (`SimRFlow`) querying ChEMBL/PubChem properties for batch Simcyp PBPK runs.
- [USEPA/CompTox-ExpoCast-httk](https://github.com/USEPA/CompTox-ExpoCast-httk) `(R/C)` — 美国 EPA 高通量毒代动力学包，提供通用 PBPK 模型、组织分配系数预测与 IVIVE 流水线。 / High-throughput toxicokinetics (`httk`) package for generic PBPK modeling, partition coefficients, and IVIVE.
- [ScitoVation/plethem](https://github.com/ScitoVation/plethem) `(R/Shiny)` — 集成 `httk` 与 `deSolve` 的高通量 PBPK、IVIVE 与反向剂量估算交互式 Shiny 平台。 / Interactive Shiny platform (`PLETHEM`) integrating `httk` and `deSolve` for high-throughput PBPK, IVIVE, and reverse dosimetry.
- [metrumresearchgroup/PBPK_PC](https://github.com/metrumresearchgroup/PBPK_PC) `(R/mrgsolve)` — 在 `mrgsolve` PBPK 中实现并系统对比 Rodgers & Rowland、Berezhkovskiy 等组织分配系数（$K_p$）方法。 / Implements and benchmarks tissue partition coefficient ($K_p$) methods (Rodgers & Rowland, Berezhkovskiy, etc.) in `mrgsolve`.
- [metrumresearchgroup/pbpk-qsp-mrgsolve](https://github.com/metrumresearchgroup/pbpk-qsp-mrgsolve) `(R/mrgsolve)` — Metrum 与佛罗里达大学联合开发的 `mrgsolve` 全身 PBPK/QSP 实战模板与案例库。 / Workshop repository providing hands-on `mrgsolve` code templates and case studies for whole-body PBPK and QSP.
- [metrumresearchgroup/cptpsp-tutorial-2019](https://github.com/metrumresearchgroup/cptpsp-tutorial-2019) `(R)` — *CPT:PSP* `mrgsolve` PBPK/QSP 教程配套代码，含透明的 Poulin & Theil $K_p$ 计算脚本。 / Companion code for `mrgsolve` PBPK/QSP modeling including transparent Poulin & Theil $K_p$ calculation scripts.
- [metrumresearchgroup/BayesPBPK-tutorial](https://github.com/metrumresearchgroup/BayesPBPK-tutorial) `(Julia/Stan/R)` — 演示基于 Julia（SciML/Turing.jl）、Stan/Torsten 与 R 的开源贝叶斯分层 PBPK 建模工作流。 / Open-source Bayesian hierarchical PBPK modeling workflows using Julia (Turing.jl), Stan/Torsten, and R.
- [SystemsForecasting/ManchesterPBPK](https://github.com/SystemsForecasting/ManchesterPBPK) `(R)` — 基于 `rxode2` 的透明代码优先全身 PBPK 教学与原型模型（*PBPKedu*）。 / Open-source, code-first whole-body PBPK model (*PBPKedu*) written transparently in `rxode2`.
- [matthiaskoenig/sbmlsim](https://github.com/matthiaskoenig/sbmlsim) `(Python | 德国)` — 基于 `libRoadRunner` 的 SBML PBPK 仿真、参数扫描、敏感度分析与自动报告框架。 / Python simulation and reporting framework built on `libRoadRunner` for reproducible SBML PBPK models.
- [matthiaskoenig/glimepiride-model](https://github.com/matthiaskoenig/glimepiride-model) `(Python/SBML | 德国)` — 显式模拟肾损伤、肝硬化与 CYP2C9 基因多态性影响的格列美脲全身 PBPK 模型。 / Whole-body SBML PBPK model of glimepiride explicitly modeling renal impairment, cirrhosis, and CYP2C9 genetics.
- [matthiaskoenig/dapagliflozin-model](https://github.com/matthiaskoenig/dapagliflozin-model) `(Python/SBML | 德国)` — 评估肝肾联合损伤、食物效应及尿糖排泄药效的达格列净全身 PBPK/PD 模型。 / Coupled PBPK/PD SBML model of dapagliflozin evaluating hepatorenal impairment and urinary glucose excretion.
- [ahmedn12/oral-pbpk-model](https://github.com/ahmedn12/oral-pbpk-model) `(Python/R)` — 对齐 FDA 研讨会流程的多途径口服 PBPK 模型，刻画肝脏首过代谢与蛋白结合率敏感度。 / Dual Python/R oral PBPK model capturing hepatic first-pass metabolism and protein-binding ($f_u$) sensitivity.
- [mathworks/Chemistry-Cheminformatics-Pharmacokinetics](https://github.com/mathworks/Chemistry-Cheminformatics-Pharmacokinetics) `(MATLAB/Python)` — MathWorks 官方打通 Python/RDKit 分子描述符与 MATLAB SimBiology 预测口服吸收的工作流。 / Official MathWorks workflow bridging Python/RDKit descriptors with MATLAB SimBiology for oral absorption simulation.
- [qurit/PSMA-PBPK-Model-Matlab](https://github.com/qurit/PSMA-PBPK-Model-Matlab) `(MATLAB)` — 针对 PSMA 靶向放射性核素药物的 SimBiology/SBML 全身 PBPK 模型。 / MATLAB SimBiology/SBML whole-body PBPK model for PSMA-targeted radiopharmaceuticals.
- [pipetcpt/DallphinDDI](https://github.com/pipetcpt/DallphinDDI) `(R | 韩英)` — 韩国 EDISON 资助开发的生理/PBPK 代谢酶与转运体药物相互作用（DDI）仿真工具。 / Academic R-based physiological/PBPK modeling tool for simulating metabolic and transporter DDIs.

---

## 9. 生物大分子、TMDD、ADC、CAR-T、免疫原性与 QSP / Biologics, TMDD, ADC, CAR-T, Immunogenicity & QSP

- [metrumresearchgroup/bioPBPK](https://github.com/metrumresearchgroup/bioPBPK) `(Julia/R)` — 代码优先的生物大分子/单抗（mAb）全身 PBPK 模型，显式刻画 FcRn 再循环与淋巴回流。 / Code-first biologics/mAb whole-body PBPK models with FcRn recycling and lymphatics in Julia and R.
- [Open-Systems-Pharmacology/BAY794620-Model](https://github.com/Open-Systems-Pharmacology/BAY794620-Model) `(PK-Sim)` — 针对抗体偶联药物（ADC）BAY-794620 的全身 PBPK 模型，刻画大分子分布与分解代谢。 / Whole-body PBPK model for the antibody-drug conjugate (ADC) BAY-794620 capturing macromolecular disposition.
- [azelys/tce](https://github.com/azelys/tce) `(Julia/MATLAB)` — 针对双特异性 T 细胞衔接器（BiTE/TCE）三元复合物结合、PK、结构可辨识性与最优控制的机理建模。 / Mechanistic modeling of binding criteria, PK, identifiability, and optimal control for bispecific T-cell engagers (TCEs).
- [cosbi-research/PBPKmRNABiTE](https://github.com/cosbi-research/PBPKmRNABiTE) `(MATLAB | 意大利)` — 模拟 mRNA 编码双特异性 T 细胞衔接器（BiTE）转运、翻译与抗体药动学的多尺度 PBPK 模型。 / Multi-scale PBPK model for mRNA-encoded BiTE cancer therapy capturing trafficking, translation, and antibody PK.
- [cosbi-research/Campanile_et_al_PBPKmRNATherapeutics](https://github.com/cosbi-research/Campanile_et_al_PBPKmRNATherapeutics) `(MATLAB | 意大利)` — 基于 SimBiology 的脂质纳米颗粒（LNP）递送与 mRNA 抗体疗法 PBPK 建模框架。 / SimBiology PBPK framework for lipid nanoparticle (LNP) delivery and mRNA-encoded antibody therapeutics.
- [RomanCohort/confluencia](https://github.com/RomanCohort/confluencia) `(Python | 中英)` — 面向小样本 circRNA 药物研发的计算平台，集成首个 circRNA 六室机制性 PK 模型（RNACTM）。 / Small-sample circRNA discovery platform featuring the first 6-compartment mechanistic circRNA PK model (RNACTM).
- [maximvpolyakov/CAR-T-model](https://github.com/maximvpolyakov/CAR-T-model) `(C++/OpenMP)` — 基于三维耦合非线性 PDE 模拟实体瘤 CAR-T 耗竭、抗原逃逸与缺氧微环境的时空仿真器。 / Spatiotemporal 3D coupled PDE simulator modeling CAR-T exhaustion, antigen escape, and hypoxia in solid tumors.
- [BioTender-max/CARTCellEngine](https://github.com/BioTender-max/CARTCellEngine) `(Python)` — 纯 Python 实现基于 ODE 的 CAR-T 效靶杀伤动力学、T 细胞耗竭评分与疗效预测流程。 / Pure-Python ODE pipeline for CAR-T effector-target killing kinetics, T-cell exhaustion, and response prediction.
- [compiler-research/CARTopiaX](https://github.com/compiler-research/CARTopiaX) `(C++)` — 基于 BioDynaMo 的高性能多智能体（ABM）实体瘤微环境 CAR-T 细胞迁移与杀伤仿真平台。 / High-performance agent-based platform modeling CAR-T trafficking, infiltration, and tumor-organoid killing.
- [FDA/TCPro](https://github.com/FDA/TCPro) `(MATLAB)` — 美国 FDA（CBER）机理计算工具，预测治疗性蛋白的 T 细胞增殖动力学及免疫原性/ADA 风险。 / U.S. FDA mechanistic tool predicting ex vivo T-cell proliferation and MHC-II immunogenicity/ADA risk for biologics.
- [singhharsh1708/QSPAtlas.jl](https://github.com/singhharsh1708/QSPAtlas.jl) `(Julia)` — 基于 Julia 重现并验证已发表 PK/PD、QSP 及 CAR-T 细胞动力学模型的开源模型集合。 / Open-source Julia collection reconstructing and validating published PK/PD, QSP, and CAR-T cellular kinetics models.
- [BMSQSP/QSPToolbox](https://github.com/BMSQSP/QSPToolbox) `(MATLAB)` — 百时美施贵宝开源 QSP 工具箱，标准化 SimBiology 仿真、全局敏感性分析与虚拟人群（VPop）校准。 / BMS MATLAB toolbox standardizing SimBiology QSP workflows, global sensitivity analysis, and VPop calibration.
- [feigelman/gQSPsim-release](https://github.com/feigelman/gQSPsim-release) `(MATLAB)` — 基因泰克基于 SimBiology 开发的图形化 QSP 平台，支持模型校准与虚拟人群交互式诊断。 / Genentech SimBiology GUI app enabling reproducible QSP model calibration, virtual population generation, and diagnostics.
- [pfizer-opensource/integrated-qsp-vpop-onco-efficacy-CPT-PSP](https://github.com/pfizer-opensource/integrated-qsp-vpop-onco-efficacy-CPT-PSP) `(MATLAB)` — 辉瑞开源肿瘤 QSP 虚拟人群框架，实现 Metropolis-Hastings 合理患者采样与纵向疗效校准。 / Pfizer QSP virtual population framework with Metropolis-Hastings sampling and longitudinal oncology efficacy calibration.
- [popellab/QSPIO-TNBC](https://github.com/popellab/QSPIO-TNBC) `(MATLAB)` — 约翰霍普金斯 Popel 实验室开源多尺度肿瘤免疫 QSP 平台，模拟三阴性乳腺癌/非小细胞肺癌免疫联合疗法。 / Mechanistic multi-scale immuno-oncology QSP platform modeling tumor-immune interactions and checkpoint therapies.
- [NVIDIA-BioNeMo/nvQSP](https://github.com/NVIDIA-BioNeMo/nvQSP) `(C++/CUDA/Python)` — 英伟达 BioNeMo 推出的 GPU 加速刚性 ODE 求解库，专为超大规模 QSP 虚拟人群并行仿真优化。 / GPU-accelerated stiff ODE solver library from NVIDIA BioNeMo for ultra-fast, large-scale QSP VPop simulations.
- [SciML/Catalyst.jl](https://github.com/SciML/Catalyst.jl) `(Julia)` — Julia SciML 符号化学反应网络 DSL，将 QSP 与系统生物学模型编译为高性能 ODE/SDE 求解器。 / Symbolic reaction network DSL compiling mechanistic QSP models into high-performance ODE/SDE/jump solvers.
- [pysb/pysb](https://github.com/pysb/pysb) `(Python)` — 基于规则的 Python 系统生物学与 QSP 建模框架，自动生成生化信号反应网络与 ODE。 / Rule-based Python framework for modular biochemical signaling and QSP models generating reaction networks and ODEs.
- [sys-bio/tellurium](https://github.com/sys-bio/tellurium) `(Python)` — 集成 Antimony 建模语言与 libRoadRunner 高速 SBML 引擎的 Python 系统生物学与 QSP 环境。 / Python systems biology and QSP environment combining Antimony model definitions with libRoadRunner SBML simulation.
- [copasi/COPASI](https://github.com/copasi/COPASI) `(C++)` — 开源复杂通路仿真器，支持基于 SBML 的 QSP 网络确定性/随机仿真、稳态分析与参数估计。 / Open-source Complex Pathway Simulator supporting deterministic/stochastic simulation and parameter estimation for SBML QSP.

---

## 10. AI / ML / DL / SciML / RL × 临床药理与定量药理 / AI, ML, SciML & RL for ClinPharm & PMx

### 10.1 LLM 智能体、MCP 协议、RAG 与知识挖掘 / LLM Agents, MCP, RAG & Knowledge Mining

- [PeterBloomingdale/pmxagent](https://github.com/PeterBloomingdale/pmxagent) `(R/Python/Docker)` — 将真实 R 定量药理函数封装为 REST API 与 MCP 服务，供 AI 智能体安全执行调用。 / Open-source agentic platform exposing R pharmacometrics functions as REST APIs and an MCP server for LLMs.
- [MomentumMetrix/PK_Claude](https://github.com/MomentumMetrix/PK_Claude) `(R/Claude Code)` — 将 Claude Code 集成到定量药理工作流中，辅助开展 AI 驱动的群体 PK 分析与建模执行。 / Integrates Claude Code into pharmacometrics workflows for AI-driven population PK analysis and scripting.
- [MomentumMetrix/RstudioMCP](https://github.com/MomentumMetrix/RstudioMCP) `(TS/R)` — 面向 RStudio IDE 的 MCP 服务器，使大模型智能体可直接执行 R 定量药理脚本并捕获诊断图。 / MCP server for RStudio IDE allowing LLM agents to run R pharmacometrics scripts and capture diagnostic plots.
- [pharmacometricsai/nonmem-library](https://github.com/pharmacometricsai/nonmem-library) `(NONMEM/MD)` — 与多位大语言模型（Claude/Gemini/Kimi）协同开发调试的 NONMEM 群体 PK/PD 控制流基准库。 / Curated library of NONMEM PopPK/PD control streams co-developed and debugged with LLMs as a coding benchmark.
- [VirtualPatientEngine/AIAgents4Pharma](https://github.com/VirtualPatientEngine/AIAgents4Pharma) `(Python)` — 开源制药 AI 智能体套件（含 *Talk2BioModels*），支持自然语言交互与仿真系统药理数学模型。 / Open-source LLM agent suite (including *Talk2BioModels*) for querying and simulating systems pharmacology models.
- [openpharma-org/fda-mcp](https://github.com/openpharma-org/fda-mcp) `(TS)` — 对接 openFDA 药品说明书、FAERS 不良事件、橙皮书与紫皮书的 MCP 服务器。 / MCP server connecting LLM agents directly to openFDA drug labels, FAERS, Orange Book, and Purple Book.
- [Slow-Walker66/PK-Sim-Mobi-RAG-Tool](https://github.com/Slow-Walker66/PK-Sim-Mobi-RAG-Tool) `(Python | 中英)` — 面向 PK-Sim/MoBi 官方文档与构建模块的本地 RAG 问答排错助手。 / Local RAG assistant indexing PK-Sim and MoBi technical documentation and building blocks for PBPK troubleshooting.
- [lfcypo/hrt-pk-mcp](https://github.com/lfcypo/hrt-pk-mcp) `(Python/MCP | 中文)` — 将多房室 PK 算法封装为标准 MCP 服务端，向 AI Agent 暴露给药记录与血药浓度查询工具。 / Standard Python MCP server wrapping multi-compartment PK algorithms for AI-agent dose logging and queries.
- [kimmingul/clinical-pharmacology-study-protocol-development](https://github.com/kimmingul/clinical-pharmacology-study-protocol-development) `(Claude Plugin | 韩英)` — 辅助临床药理学家起草 I 期临床药理方案（FIH/SAD/MAD/DDI）与知情同意书的 LLM 插件。 / Claude Code plugin assisting clinical pharmacologists in drafting Phase 1 protocols (FIH, SAD/MAD, DDI) and ICFs.
- [QSong-github/DrugClaw](https://github.com/QSong-github/DrugClaw) `(Python)` — 基于 LangGraph 的循证药物智能体 RAG 框架，覆盖 DDI、药物基因组学（PGx）、不良反应与 FDA 说明书。 / LangGraph agentic RAG runtime for evidence-grounded DDI, pharmacogenomics (PGx), ADR, and FDA label intelligence.
- [gadevito/LLMDDI](https://github.com/gadevito/LLMDDI) `(Python)` — 从 DrugBank 抽取知识、微调大语言模型并与深度学习基线对比评测的 DDI 预测代码库。 / Pipelines for knowledge extraction, LLM fine-tuning, and benchmarking for drug-drug interaction (DDI) prediction.
- [reddy-nithin/TruPharma-Clinical-Intelligence](https://github.com/reddy-nithin/TruPharma-Clinical-Intelligence) `(Python)` — 混合 RAG（FAISS+BM25+LLM）应用，解析官方 FDA 说明书并与 FAERS 信号交叉比对实现用药安全问答。 / Hybrid RAG app parsing official FDA drug labels and cross-referencing FAERS signals for clinical safety Q&A.
- [nikhilreddy00/pharma-agent](https://github.com/nikhilreddy00/pharma-agent) `(Python)` — 基于 LangGraph 与 ChromaDB 交叉检索 FDA 说明书、PubMed 与临床指南的药物警戒/DDI 智能体。 / Autonomous LangGraph + ChromaDB agentic RAG cross-referencing FDA labels, PubMed, and guidelines for DDI queries.
- [Genentech/CLADD](https://github.com/Genentech/CLADD) `(Python)` — 基因泰克 RAG 增强多智能体 LLM 框架，动态检索生物医学知识库辅助药物发现与分子性质推理。 / Genentech's RAG-enhanced multi-agent LLM system querying biomedical knowledge bases for molecular property reasoning.
- [PKPDAI/PKDocClassifier](https://github.com/PKPDAI/PKDocClassifier) `(Python)` — 基于 NLP/ML 自动筛选报道体内药代动力学参数生物医学文献的二分类器。 / NLP/ML binary text classifier automatically screening biomedical literature for *in vivo* PK parameter studies.
- [dueyama/pmda-pk-curve-viewer](https://github.com/dueyama/pmda-pk-curve-viewer) `(TS/Next.js | 日英)` — 自动解析日本 PMDA 电子药品说明书 XML，提取 PK 参数并实时绘制血药浓度曲线。 / Parses official Japanese PMDA package insert XML files to extract PK parameters and plot estimated concentration curves.
- [pablosierrafernandez/FarmacoDB](https://github.com/pablosierrafernandez/FarmacoDB) `(Python | 西班牙文)` — 利用 LLM 文本挖掘自动化抽取多源药动学数据（>1,000 药物）并预测人体半衰期。 / LLM-assisted text mining pipeline standardizing multi-source PK data (>1,000 drugs) with half-life prediction models.
- [valentinnavalos/pharmawatch-api](https://github.com/valentinnavalos/pharmawatch-api) `(API | 西班牙文)` — 支持处方校验与药动学药物相互作用（血浆蛋白置换等）分析的药物警戒 REST API。 / Pharmacovigilance REST API providing prescription checking and PK drug-drug interaction analysis.
- [PharMolix/OpenBioMed](https://github.com/PharMolix/OpenBioMed) `(Python | 中英)` — 清华 AIR 开源生物医药多模态大模型与智能体框架，内置 ADMET 与 DDI 预测工具链。 / Multimodal biomedical LLM and agent framework featuring built-in ADMET prediction and DDI analysis tools.
- [datamllab/CAi_copilot](https://github.com/datamllab/CAi_copilot) `(Python | 中英)` — 自然语言驱动的开源药物设计智能体，集成 ADMET-AI 预测吸收、代谢、清除与毒性。 / Natural-language drug design agent integrating ADMET-AI for clearance, absorption, metabolism, and toxicity screening.

### 10.2 物理信息神经网络（PINNs）、Neural ODE 与 SciML / PINNs, Neural ODEs, UDEs & SciML

- [jameslu01/Neural_PK](https://github.com/jameslu01/Neural_PK) `(Python/PyTorch)` — 将神经常微分方程应用于跨给药方案的临床 PK 血药浓度外推，并与 NLME/LSTM/LightGBM 对比。 / Applies Neural ODEs to clinical PK forecasting across unseen dosing regimens, benchmarked against NLME and LSTM.
- [TommyGiak/pharmacoNODE](https://github.com/TommyGiak/pharmacoNODE) `(Python/PyTorch)` — 将 Neural ODE 应用于 Monolix/NONMEM 风格纵向临床 PK 预测，解决房室结构误设。 / Neural ODE codebase for longitudinal PK concentration-time prediction with patient covariates.
- [emotionor/UniPKModel](https://github.com/emotionor/UniPKModel) `(Python/PyTorch)` — *JCIM* 配套可解释 Neural ODE 框架与预训练权重，用于高泛化数据驱动 PK 曲线预测。 / Interpretable Neural ODE framework with pre-trained weights for generalizable data-driven PK curve forecasting.
- [FraunhoferChalmersCentre/neuralODEpopulation](https://github.com/FraunhoferChalmersCentre/neuralODEpopulation) `(Python)` — 融合 Transformer、Neural ODE 与 VAE/EBVAE 随机效应的端到端群体 PK/PD 深度学习框架（含 VPC）。 / End-to-end population PMx pipeline combining Transformers, Neural ODEs, and VAE random effects with VPCs.
- [Janssena/DeepCompartmentModels.jl](https://github.com/Janssena/DeepCompartmentModels.jl) `(Julia)` — 深度房室模型（DCM），在房室 ODE 结构约束下用神经网络学习协变量-参数关系。 / Deep Compartment Models combining compartmental ODE constraints with neural networks for covariate learning.
- [PumasAI-Labs/DeepPumas_workshop_2026_PAGE](https://github.com/PumasAI-Labs/DeepPumas_workshop_2026_PAGE) `(Julia)` — PumasAI 官方 PAGE 研讨会代码，演示将 Neural ODE 与通用微分方程（UDE）嵌入 DeepNLME 群体模型。 / Official PAGE workshop demonstrating DeepPumas (DeepNLME) embedding Neural ODEs and UDEs in PopPK/PD models.
- [SCAI-BIO/MMPK-SciML](https://github.com/SCAI-BIO/MMPK-SciML) `(Python/Julia)` — 弗劳恩霍夫 SCAI 官方基准库，系统对比 SciML、传统 PopPK 与经典 ML 在抗肿瘤药浓度预测中的表现。 / Fraunhofer SCAI repository benchmarking SciML against mechanistic PopPK and classical ML for oncology PK prediction.
- [NazAhmadi/CMINNs](https://github.com/NazAhmadi/CMINNs) `(Python/JAX)` — 房室模型物理信息神经网络（CMINNs/分数阶 PINNs），刻画复杂 PK/PD 中的反常扩散与时变参数。 / Compartment Model-Informed Neural Networks (PINNs/fPINNs) capturing anomalous diffusion and time-varying PK/PD.
- [yapici/open-pk-pinn](https://github.com/yapici/open-pk-pinn) `(Python/PyTorch)` — 开源可复现的房室物理信息神经网络（CMT-PINN）药动学浓度-时间预测基准。 / Open, reproducible compartmental Physics-Informed Neural Network (CMT-PINN) benchmark on public *in vivo* PK data.
- [novainsilico/vpop-calibration](https://github.com/novainsilico/vpop-calibration) `(Python)` — 将 NLME 推断与机器学习代理模型结合，大幅加速 QSP 虚拟人群校准。 / Accelerates QSP virtual population calibration by coupling NLME inference with ML surrogate models.

### 10.3 强化学习（RL）与深度学习精准给药 / RL & Deep Learning for Precision Dosing & TDM

- [hamilton-health-sciences/warfarin](https://github.com/hamilton-health-sciences/warfarin) `(Python/PyTorch)` — 基于 COMBINE-AF 临床试验数据的离线深度强化学习（`smdbcq`），优化房颤华法林序贯给药。 / Offline deep RL (`smdbcq`) trained on COMBINE-AF trial data to optimize sequential warfarin dosing.
- [rudra2112/Warfarin-Dosage-Prediction](https://github.com/rudra2112/Warfarin-Dosage-Prediction) `(Python)` — 结合患者特征与 *CYP2C9*/*VKORC1* 基因型的上下文多臂老虎机（Linear-UCB）华法林强化学习给药。 / Contextual multi-armed bandit (Linear-UCB) RL for individualized warfarin dosing with clinical and genotype features.
- [karneslab/warfarin-machinelearning](https://github.com/karneslab/warfarin-machinelearning) `(R)` — 结合 CYP2C9/VKORC1 药物基因组学与临床协变量预测华法林维持剂量的机器学习代码。 / Machine learning scripts predicting stable warfarin maintenance doses using pharmacogenetic and clinical covariates.
- [lucis-e/PopPBPK-RL_Bnzpril](https://github.com/lucis-e/PopPBPK-RL_Bnzpril) `(Python/R)` — 将群体 PBPK 与强化学习（RL）结合，在肾损伤虚拟队列中优化贝那普利精准给药。 / Integrates population PBPK with reinforcement learning to optimize benazepril dosing in renal-impaired cohorts.
- [FatemehRabie/chemotherapy](https://github.com/FatemehRabie/chemotherapy) `(Python)` — 将 3D 肿瘤 PDE 仿真器与 Gymnasium/SB3 结合，利用物理引导深度强化学习优化个体化化疗方案。 / Couples a 3D tumor PDE simulator with Gymnasium/SB3 for physics-guided deep RL of personalized chemotherapy dosing.
- [sumanabasu/On-the-Challenges-of-using-Reinforcement-Learning-in-Precision-Drug-Dosing-Delay-and-Prolongedness](https://github.com/sumanabasu/On-the-Challenges-of-using-Reinforcement-Learning-in-Precision-Drug-Dosing-Delay-and-Prolongedness) `(Python)` — 研究并基准评测药物 PK/PD 延迟与长效作用给强化学习精准给药带来的非马尔可夫挑战。 / Benchmarks delayed and prolonged PK/PD drug-action challenges when applying RL to precision drug dosing.
- [ZhiGroup/PK-RNN](https://github.com/ZhiGroup/PK-RNN) `(Python)` — 利用电子病历纵向给药与检验数据动态预测万古霉素血药浓度的循环神经网络（PK-RNN-V）。 / Recurrent neural network (PK-RNN-V) leveraging longitudinal EHR dosing/lab records for vancomycin TDM forecasting.
- [BingyuMao/vanco_2cm](https://github.com/BingyuMao/vanco_2cm) `(Python)` — 将自回归 RNN 与机理二室 PK 预测头融合的混合模型（PKRNN-2CM），实现可解释万古霉素动态预测。 / Hybrid autoregressive RNN + mechanistic 2-compartment PK head (PKRNN-2CM) for interpretable vancomycin forecasting.
- [Yunwoolee17/Vancomycin_prediction_AI](https://github.com/Yunwoolee17/Vancomycin_prediction_AI) `(Python | 韩国)` — 融合多种树模型与 SHAP 可解释性预测万古霉素达标 AUC 起始剂量的机器学习流水线。 / ML pipeline with SHAP explainability predicting initial vancomycin doses to achieve target AUC (400–600 mg·h/L).
- [y-babdalla/tacrolimus_predictions](https://github.com/y-babdalla/tacrolimus_predictions) `(Python/PyTorch)` — 结合注意力/时间感知 LSTM 与合成数据增强（*DoseTAIlor*/*TacroNET*）预测个体化他克莫司谷浓度。 / End-to-end attention/time-aware LSTM pipeline with synthetic data augmentation for tacrolimus trough forecasting.
- [huiyum/tac_dose_adjustments](https://github.com/huiyum/tac_dose_adjustments) `(Python/Streamlit)` — 结合 GRU 药动学深度学习与 Streamlit 界面，预测移植/ICU 患者他克莫司谷浓度并辅助调量。 / Modular GRU deep learning pipeline and Streamlit app for tacrolimus trough prediction and dose adjustments.
- [sebboie/aptt-prediction](https://github.com/sebboie/aptt-prediction) `(Python)` — 基于回顾性临床数据构建 RNN 模型动态预测静脉输注肝素后的 aPTT 凝血轨迹。 / Recurrent neural network forecasting activated partial thromboplastin time (aPTT) trajectories during IV heparin therapy.

### 10.4 自动化定量药理、ML 协变量筛选与合成患者数据 / Automated PMx, ML Covariates & Synthetic Data

- [certara/pyDarwin](https://github.com/certara/pyDarwin) `(Python)` — 运用遗传算法、随机森林、GBRT、高斯过程与粒子群算法自动搜索最优 NONMEM/NLME 模型结构与协变量。 / Automates NONMEM/NLME PopPK/PD structural and covariate selection using GA, RF, GBRT, Gaussian Processes, and PSO.
- [gengbo-genentech/Pharm-AutoML](https://github.com/gengbo-genentech/Pharm-AutoML) `(Python)` — 基因泰克发表于 *CPT:PSP* 的开源制药 AutoML 框架，覆盖临床药理预处理、调参与可解释分析。 / Genentech's *CPT:PSP* AutoML framework streamlining end-to-end modeling and interpretability for clinical pharmacology.
- [Janssena/pkSHAP](https://github.com/Janssena/pkSHAP) `(Python/Julia)` — 利用 SHAP 可解释性解析 ML 模型，推断药动学模型中患者协变量的最优数学函数形式。 / Applies SHAP values to ML models to infer optimal mathematical functional forms of patient covariates in PK modeling.
- [AstraZeneca/Stochastic-gates-for-covariate-selection-in-population-pharmacokinetics-modelling-](https://github.com/AstraZeneca/Stochastic-gates-for-covariate-selection-in-population-pharmacokinetics-modelling-) `(Python)` — 阿斯利康开源可微随机门（STG）神经网络特征选择方法，加速群体药动学协变量筛选。 / Uses differentiable Stochastic Gates neural feature selection to automate and accelerate PopPK covariate screening.
- [wahlquisty/learning-pharmacometric-covariate-structures](https://github.com/wahlquisty/learning-pharmacometric-covariate-structures) `(Julia)` — 基于神经网络符号回归自动发现群体药动学协变量数学结构。 / Neural symbolic regression prototype for automated pharmacometric covariate structure discovery.
- [iasiimwe/unite4tb_ml](https://github.com/iasiimwe/unite4tb_ml) `(R/Python)` — UNITE4TB 联盟在高维药物基因组 PopPK 数据中对比 ML 与传统 GWAS/定量药理协变量筛选的基准。 / Benchmarks ML against traditional PMx/GWAS for high-dimensional SNP covariate imputation and selection in PopPK.
- [jbwoillard/synthetic_data_pharmacogenetics](https://github.com/jbwoillard/synthetic_data_pharmacogenetics) `(R/Python)` — 面向临床药理与药物基因组队列评估 Avatar、生存 VAE 与 CTGAN 等隐私保护合成患者数据生成。 / Evaluates privacy-preserving synthetic patient data generators (Avatar, VAE, CTGAN) for clinical pharmacology cohorts.

### 10.5 AI / ML / GNN 预测人体 PK 参数、药时曲线与 ADME / ML/DL Prediction of Human PK & ADME

- [Novartis/DeepCt](https://github.com/Novartis/DeepCt) `(Python)` — 诺华开源深度学习框架，直接从 SMILES 化学结构预测完整血浆浓度-时间曲线及房室 PK 参数。 / Novartis deep learning framework predicting full plasma concentration-time profiles and compartmental PK from SMILES.
- [srijitseal/PKSmart](https://github.com/srijitseal/PKSmart) `(Python)` — 两阶段跨物种 ML 流水线，结合化学描述符与动物 PK 预测人体体内清除率、分布容积与半衰期。 / Two-stage ML pipeline combining chemical descriptors and predicted animal PK to forecast human CL, Vdss, t1/2, and fu.
- [swansonk14/admet_ai](https://github.com/swansonk14/admet_ai) `(Python)` — 基于 Chemprop 图神经网络与 TDC 基准的高速、大规模 40+ 项 ADMET 与 PK 性质预测平台。 / Fast Chemprop-based GNN platform trained on TDC benchmarks predicting 40+ ADMET and PK properties at scale.
- [xli7654321/MMPK](https://github.com/xli7654321/MMPK) `(Python)` — 融合多尺度分子表征与子结构交叉注意力的端到端多模态深度模型，预测人体口服 PK 参数。 / Multimodal deep learning framework with substructure cross-attention predicting human oral PK (CL/F, Vz/F, t1/2, AUC, F).
- [xtalpi-xic/pk-model](https://github.com/xtalpi-xic/pk-model) `(Python)` — 将图神经网络（Chemprop/D-MPNN）与树模型、PBPK 结合预测小分子人体药代动力学。 / Combines GNNs (Chemprop/D-MPNN) and ensemble ML with PBPK workflows to predict human small-molecule PK.
- [dreadlesss/pharmacokinetic_prediction](https://github.com/dreadlesss/pharmacokinetic_prediction) `(Python)` — 基于 1,352 个化合物与梯度提升树/分子指纹预测人体静脉给药 PK 参数（CL、Vd、t1/2、MRT、fu）。 / Gradient-boosted decision trees predicting human IV PK parameters (CL, Vd, t1/2, MRT, fu) from 1,352 compounds.
- [eugenebang/ADME-DL](https://github.com/eugenebang/ADME-DL) `(Python)` — 通过药动学引导的序贯 ADME 多任务学习增强分子基础模型，提升 PK 性质预测。 / Enriches molecular foundation models via sequential ADME PK-guided multi-task learning.
- [Sanofi-Public/DMPK-US-ML-mTPA](https://github.com/Sanofi-Public/DMPK-US-ML-mTPA) `(Python)` — 赛诺菲将极简 PBPK/TMDD 与树模型结合，用于单克隆抗体早期靶点药理与 PK/PD 可行性评估。 / Integrates minimal PBPK/TMDD with tree-based ML classifiers to evaluate early mAb target pharmacology and PK/PD feasibility.
- [UFPBPK/Nano-AI-PBPK-G1](https://github.com/UFPBPK/Nano-AI-PBPK-G1) `(Python/R)` — 佛罗里达大学 AI 辅助 PBPK 建模框架，预测纳米颗粒在小鼠体内的肿瘤递送与组织 PK。 / AI-assisted PBPK modeling framework predicting nanoparticle tumor delivery and tissue pharmacokinetics.
- [molecularinformatics/Computational-ADME](https://github.com/molecularinformatics/Computational-ADME) `(Python)` — 渤健（Biogen）工业界体外 ADME 数据集与代码，前瞻性验证 XGBoost/LightGBM/DeepChem 预测效能。 / Biogen's industrial benchmark code and datasets for prospective validation of ML/DL on *in vitro* ADME endpoints.
- [OpenADMET/openadmet-models](https://github.com/OpenADMET/openadmet-models) `(Python)` — 开放科学可扩展 ML 模型架构与训练流水线，用于可复现 ADMET 与 DMPK（如 CYP 抑制）预测。 / Scalable open-science ML architectures and pipelines for reproducible ADMET and DMPK endpoint prediction.
- [abinittio/CYP450-Metabolism-Predictor](https://github.com/abinittio/CYP450-Metabolism-Predictor) `(Python)` — 基于 ChEMBL 构建多任务图神经网络，同步预测 5 种主要 CYP450 酶抑制与 DDI 风险。 / Multi-task GNN trained on ChEMBL predicting inhibition across 5 major CYP450 isoforms for DDI liability screening.
- [CDDLeiden/PK-in-generative-drug-design](https://github.com/CDDLeiden/PK-in-generative-drug-design) `(Python)` — 将 Lombardo 人体静脉 PK 数据集与 QSP/PK 建模结合用于生成式药物设计。 / Integrates the Lombardo human IV PK dataset with QSP/PK modeling pipelines for generative drug design.

---

## 11. 开源临床 PK 数据集、基准与精选索引 / Open Clinical PK Datasets, Benchmarks & Awesome Lists

- [matthiaskoenig/pkdb](https://github.com/matthiaskoenig/pkdb) `(Python/Django | 德国)` — 遵循 FAIR 原则的开源临床/临床前药动学数据库（PK-DB）与 REST API。 / FAIR open pharmacokinetics database (PK-DB) curating clinical PK curves, genotypes, and organ impairment via API.
- [Open-Systems-Pharmacology/Database-for-observed-data](https://github.com/Open-Systems-Pharmacology/Database-for-observed-data) `(Excel/CSV)` — OSP 维护的文献数字化临床血药浓度-时间曲线与 DDI 实测数据库，广泛用于 PBPK 验证。 / Curated digitized clinical PK concentration-time profiles and DDI datasets from literature for PBPK qualification.
- [nlmixr2/nlmixr2data](https://github.com/nlmixr2/nlmixr2data) `(R)` — 为 `nlmixr2`/`rxode2` 生态打包的标准群体 PK/PD 基准与教学数据集。 / Standard benchmark and tutorial PopPK/PD datasets (1- and 2-compartment bolus/infusion) for `nlmixr2`/`rxode2`.
- [dpastoor/PKPDdatasets](https://github.com/dpastoor/PKPDdatasets) `(R)` — 面向定量药理、转化医学与建模仿真测试的即用型标准化 PK/PD 数据集集合。 / Curated ready-to-use pharmacokinetic and pharmacodynamic datasets for M&S benchmarking and education.
- [billdenney/PKdata](https://github.com/billdenney/PKdata) `(R)` — 专为测试和验证 NCA 与 PK 软件准确性构建的真实与模拟单次/多次给药 PK 数据集。 / Real and simulated single-/multiple-dose PK datasets structured for validating NCA and PK software implementations.
- [mims-harvard/TDC](https://github.com/mims-harvard/TDC) `(Python)` — 哈佛 Therapeutics Data Commons（PyTDC），提供 ML 就绪的清除率、半衰期、PPB、CYP 等基准数据集。 / Standardized AI-ready ADME/PK benchmark datasets (CL, t1/2, Caco-2, PPB, CYP) with scaffold splits and leaderboards.
- [mindrank-ai/PharmaBench](https://github.com/mindrank-ai/PharmaBench) `(Python/Data)` — 基于大模型挖掘清洗构建的综合性 ADMET 与药动学基准数据集（吸收、PPB、BBB、CYP、清除率）。 / Cleaned, LLM-mined ADMET and PK property benchmark suite covering absorption, PPB, BBB, CYP, and clearance.
- [isop-phmx/awesome-pharmacometrics](https://github.com/isop-phmx/awesome-pharmacometrics) `(Markdown)` — 国际定量药理学会（ISoP）维护的高校项目、期刊、会议、教程与经典教材精选索引。 / ISoP-maintained directory of pharmacometrics university programs, journals, conferences, tutorials, and textbooks.
- [AIML-SIG/awesome-ai-ml-pharmacometrics](https://github.com/AIML-SIG/awesome-ai-ml-pharmacometrics) `(Markdown)` — 聚焦 AI/ML 在定量药理、PBPK 与 QSP 中应用的社区精选文献与开源资源列表。 / Curated community list of AI/ML papers, tools, and resources for pharmacometrics, PBPK, and QSP.
- [MasterDGL/admet-literature](https://github.com/MasterDGL/admet-literature) `(Markdown | 中英)` — 系统梳理 AI 药物发现中 ADMET 与药代动力学性质预测的论文、数据集与方法笔记。 / Curated bilingual literature and benchmark dataset index for AI-driven ADMET and PK property prediction.

---

## 12. 多语种开源教材与代码库 / Multi-Lingual Open Textbooks & Workshops

- [PumasAI-Labs/PumasIntroTutorial-ContinuousData](https://github.com/PumasAI-Labs/PumasIntroTutorial-ContinuousData) `(Julia/Quarto)` — PumasAI 官方开源教程，涵盖 Julia 临床 PK 数据整理、FDA/EMA 规范 NCA 与连续型建模。 / Official PumasAI open tutorial covering clinical PK prep, FDA/EMA-aligned NCA, and continuous-data workflows in Julia.
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

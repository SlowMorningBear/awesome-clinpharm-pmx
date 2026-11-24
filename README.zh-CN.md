# Awesome Clinical Pharmacokinetics & Pharmacometrics (ClinPharm & PMx)

[English](README.md) | **简体中文**

> 面向**临床药代动力学（Clinical Pharmacokinetics）**、**定量药理学（Pharmacometrics）**以及 **AI × ClinPharm/PMx** 的多语种开源工具目录。不以 Star 数为门槛，按解决的具体科学或工程问题归类，覆盖英、中、日、韩、德、法、西、葡、意等全球生态（v2.0 收录 **335** 个经核验开源仓库，零重复）。

---

## 目录

- [1. NONMEM / Monolix / Phoenix 工作流、编辑器插件与算力运维](#1-nonmem--monolix--phoenix-工作流编辑器插件与算力运维)
- [2. 开源 PopPK / NLME 建模与多语言 ODE 仿真引擎](#2-开源-poppk--nlme-建模与多语言-ode-仿真引擎)
- [3. 数据准备、CDISC 转换与数据质控](#3-数据准备cdisc-转换与数据质控)
- [4. 非房室分析（NCA）、生物等效性（BE）、IVIVC 与溶出](#4-非房室分析nca生物等效性beivivc-与溶出)
- [5. 模型诊断、可视化与自动化报告](#5-模型诊断可视化与自动化报告)
- [6. 临床药理监管、C-QTc、I/II 期剂量探索、E-R、CTS 与 FIH](#6-临床药理监管c-qtciii-期剂量探索e-rcts-与-fih)
- [7. 模型引导精准给药（MIPD）、临床 TDM、抗感染 PTA 与 TCI](#7-模型引导精准给药mipd临床-tdm抗感染-pta-与-tci)
  - [7.1 通用贝叶斯 / MIPD 引擎与外部验证](#71-通用贝叶斯--mipd-引擎与外部验证)
  - [7.2 抗感染 PK/PD、PTA/CFR 与抗菌/抗真菌 TDM](#72-抗感染-pkpdptacfr-与抗菌抗真菌-tdm)
  - [7.3 免疫抑制剂、窄治疗窗药物与临床计算器（含儿科/CRRT）](#73-免疫抑制剂窄治疗窗药物与临床计算器含儿科crrt)
  - [7.4 围术期麻醉 TCI、阿片解救与胰岛素-血糖 PK/PD](#74-围术期麻醉-tci阿片解救与胰岛素-血糖-pkpd)
  - [7.5 多房室血药浓度追踪与动态校准](#75-多房室血药浓度追踪与动态校准)
- [8. 生理药代动力学（PBPK）、IVIVE、DDI 与特殊人群](#8-生理药代动力学pbpkiviveddi-与特殊人群)
- [9. 生物大分子、TMDD、ADC、CAR-T、免疫原性与 QSP](#9-生物大分子tmddadccar-t免疫原性与-qsp)
- [10. AI / ML / DL / SciML / RL × 临床药理与定量药理](#10-ai--ml--dl--sciml--rl--临床药理与定量药理)
  - [10.1 LLM 智能体、MCP 协议、RAG 与知识挖掘](#101-llm-智能体mcp-协议rag-与知识挖掘)
  - [10.2 物理信息神经网络（PINNs）、Neural ODE 与 SciML](#102-物理信息神经网络pinnsneural-ode-与-sciml)
  - [10.3 强化学习（RL）与深度学习精准给药](#103-强化学习rl与深度学习精准给药)
  - [10.4 自动化定量药理、ML 协变量筛选与合成患者数据](#104-自动化定量药理ml-协变量筛选与合成患者数据)
  - [10.5 AI / ML / GNN 预测人体 PK 参数、药时曲线与 ADME](#105-ai--ml--gnn-预测人体-pk-参数药时曲线与-adme)
- [11. 开源临床 PK 数据集、基准与精选索引](#11-开源临床-pk-数据集基准与精选索引)
- [12. 多语种开源教材与代码库](#12-多语种开源教材与代码库)

---

## 1. NONMEM / Monolix / Phoenix 工作流、编辑器插件与算力运维

- [UUPharmacometrics/PsN](https://github.com/UUPharmacometrics/PsN) `(Perl)` — NONMEM 自动化工作流核心工具集（Bootstrap、SCM、VPC、SIR）。
- [metrumresearchgroup/bbi](https://github.com/metrumresearchgroup/bbi) `(Go)` — 跨平台、支持本地与 Slurm/SGE 集群的 NONMEM 高速执行引擎。
- [metrumresearchgroup/bbr](https://github.com/metrumresearchgroup/bbr) `(R)` — 基于 `bbi` 的 R 语言建模管理包，实现 NONMEM 模型谱系追踪与审计日志。
- [metrumresearchgroup/bbr.bayes](https://github.com/metrumresearchgroup/bbr.bayes) `(R)` — 扩展 `bbr` 工作流，支持通过 Stan（`cmdstanr`）和 NONMEM 贝叶斯方法管理贝叶斯药动学模型。
- [metrumresearchgroup/nmrec](https://github.com/metrumresearchgroup/nmrec) `(R)` — 精准解析与修改 NONMEM 控制流记录与缩写语法的底层库。
- [metrumresearchgroup/mrgvalidate](https://github.com/metrumresearchgroup/mrgvalidate) `(R)` — 自动生成符合监管合规要求的 R 包验证计划、可追溯性矩阵与测试报告。
- [metrumresearchgroup/pkgr](https://github.com/metrumresearchgroup/pkgr) `(Go)` — 快速构建与管理可复现、隔离 R 定量药理环境的命令行依赖管理工具。
- [NMautoverse/NMsim](https://github.com/NMautoverse/NMsim) `(R)` — 无需手动改控制流，直接基于现有 NONMEM 估计模型与新数据集从 R 执行 NONMEM 模拟。
- [nlmixr2/babelmixr2](https://github.com/nlmixr2/babelmixr2) `(R)` — 将统一 `nlmixr2`/`rxode2` 模型转译并在 NONMEM、Monolix、PKNCA、PopED 上运行。
- [nlmixr2/nonmem2rx](https://github.com/nlmixr2/nonmem2rx) `(R/C)` — 将 NONMEM 控制流及估计结果解析并转换为 `rxode2`/`nlmixr2` 模型。
- [nlmixr2/monolix2rx](https://github.com/nlmixr2/monolix2rx) `(R/C)` — 将 Monolix `.mlxtran` 模型与结果导入并转换为 `rxode2`/`nlmixr2` 对象。
- [UUPharmacometrics/assemblerr](https://github.com/UUPharmacometrics/assemblerr) `(R)` — 通过模块化 R 组件编程式组装药动学模型并编译生成规范的 NONMEM 控制流。
- [certara/R-Certara](https://github.com/certara/R-Certara) `(R)` — Certara 开源定量药理 R 工具套件的一键安装与统一加载元包（`Certara.R`）。
- [certara/R-RsNLME-Examples](https://github.com/certara/R-RsNLME-Examples) `(R)` — 用可复现的 tidyverse R 脚本替代 GUI 操作调用 Phoenix NLME 引擎。
- [MarcLavielle/Rsmlx](https://github.com/MarcLavielle/Rsmlx) `(R)` — “R Speaks Monolix”：在 R 中调用 Monolix 实现自动化建模、协变量筛选与收敛性评估。
- [tsahota/NMproject](https://github.com/tsahota/NMproject) `(R)` — 将 RStudio 打造为管道式脚本化 NONMEM 建模开发环境，集成运行追踪与自动诊断。
- [dpastoor/nonmemutils](https://github.com/dpastoor/nonmemutils) `(Go)` — 高速 Go 命令行工具集，用于解析 NONMEM `.lst` 输出文件与管理任务提交。
- [Robterheine/nmgui2](https://github.com/Robterheine/nmgui2) `(Python/PyQt6)` — 跨平台纯 Python 桌面客户端（类 Pirana 替代），管理对比 NONMEM 模型并联动 PsN。
- [a2-ai/slurmtools](https://github.com/a2-ai/slurmtools) `(R)` — 在 R 定量药理环境中直接提交、监控和管理 Slurm HPC 集群任务。
- [billdenney/Pharmacometrics-Docker](https://github.com/billdenney/Pharmacometrics-Docker) `(Docker)` — 标准化多版本 NONMEM（含 gfortran）与 PsN 的 Docker 容器化部署配置。
- [kinginsun/nonmem](https://github.com/kinginsun/nonmem) `(Docker/Shell)` — 跨平台（Win/macOS Apple Silicon/Linux）NONMEM + PsN + MPICH 容器镜像与一键脚本。
- [FelicienLL/runnonmem](https://github.com/FelicienLL/runnonmem) `(R)` — 轻量级 R 封装工具，用于从 R 脚本直接调用运行 NONMEM。
- [s0521/nonmem_cn](https://github.com/s0521/nonmem_cn) `(TS | 中文)` — NONMEM 控制文件 VS Code 扩展，提供语法高亮、自动补全与中英双语注释提示。
- [vrognas/vrognas-nmtran](https://github.com/vrognas/vrognas-nmtran) `(TS)` — 为 NMTRAN/NONMEM 控制流提供语言智能感知、实时诊断与悬停文档的 VS Code 扩展。
- [UUPharmacometrics/vim-nonmem](https://github.com/UUPharmacometrics/vim-nonmem) `(Vim)` — 专为 Vim/Neovim 打造的 NONMEM 控制流与模型文件语法高亮插件。
- [nmusers/nm-mode](https://github.com/nmusers/nm-mode) `(Emacs Lisp)` — 极简风格 Emacs 主模式，提供 NONMEM 控制流语法高亮与编辑支持。
- [TingjieGuo/MINGA](https://github.com/TingjieGuo/MINGA) `(Hugo/Shell | 中文)` — 面向中文用户的 NONMEM、PsN、Pirana 与 R 定量药理环境安装教程与脚本。
- [Slow-Walker66/PPK-workbench-assistance-demo](https://github.com/Slow-Walker66/PPK-workbench-assistance-demo) `(TS | 中英)` — 本地优先的 NONMEM+PsN 群体药动学工作台（Pirana 开源替代），含模型树、诊断与报告生成。

---

## 2. 开源 PopPK / NLME 建模与多语言 ODE 仿真引擎

- [nlmixr2/nlmixr2](https://github.com/nlmixr2/nlmixr2) `(R/C++)` — 开源 CRAN 级非线性混合效应（NLME）建模框架，支持 FOCE-I 与 SAEM。
- [nlmixr2/rxode2](https://github.com/nlmixr2/rxode2) `(R/C/C++)` — 将药动学 ODE 模型编译为 C 代码并支持 NONMEM 风格事件表的高速仿真引擎。
- [nlmixr2/nlmixr2lib](https://github.com/nlmixr2/nlmixr2lib) `(R)` — 标准化临床 PopPK/PD 及生物大分子 TMDD 文献模型库，可直接供 `nlmixr2`/`rxode2` 调用。
- [nlmixr2/nlmixr2extra](https://github.com/nlmixr2/nlmixr2extra) `(R)` — 为 `nlmixr2` 补充 Bootstrap、逐步协变量筛选与预处理拟合等核心建模工具。
- [nlmixr2/lotri](https://github.com/nlmixr2/lotri) `(R/C)` — 提供简洁语法定义 `nlmixr2`/`rxode2` 中的下三角分块协方差矩阵（IIV/IOV）。
- [metrumresearchgroup/mrgsolve](https://github.com/metrumresearchgroup/mrgsolve) `(R/C++)` — 类 NONMEM 语法的 C++ 编译型分层 ODE 仿真引擎，广泛用于 PopPK/PBPK/QSP。
- [mrgsolve/depot](https://github.com/mrgsolve/depot) `(R/C++)` — `mrgsolve` 官方配套即用型 ODE 模型库，收录全/近似 TMDD 与 PBPK 基准模板。
- [kylebaron/mrgsim.parallel](https://github.com/kylebaron/mrgsim.parallel) `(R)` — 通过拆分数据集并利用 `parallel`/`future` 并行执行大幅加速大规模 `mrgsolve` 模拟。
- [metrumresearchgroup/mrgsim.ds](https://github.com/metrumresearchgroup/mrgsim.ds) `(R)` — 将 `mrgsolve` 模拟输出存为 Apache Arrow 数据集，大幅降低超大规模仿真内存占用。
- [InsightRX/PKPDsim](https://github.com/InsightRX/PKPDsim) `(R/C++)` — 面向临床精准给药的 C++ 编译型 ODE 与解析房室 PK/PD 仿真引擎。
- [john-harrold/ubiquity](https://github.com/john-harrold/ubiquity) `(R)` — 统一 PK/PD、PBPK 与 QSP 建模、参数估计、自动 Word/PPT 报告与 Shiny GUI 生成的框架。
- [pharmpy/pharmpy](https://github.com/pharmpy/pharmpy) `(Python)` — 现代 Python 药动学模型抽象层与自动化模型构建（AMD）工具，跨 NONMEM 与 `nlmixr2`。
- [pharmpy/pharmr](https://github.com/pharmpy/pharmr) `(R)` — Pharmpy 官方 R 语言封装，使 R 用户直接调用自动化建模与多引擎工作流。
- [metrumresearchgroup/Torsten](https://github.com/metrumresearchgroup/Torsten) `(C++/Stan)` — 扩展 Stan 数学库以支持自动微分房室解析解、ODE 求解器与 NMTRAN 给药事件。
- [iame-researchCenter/saemix](https://github.com/iame-researchCenter/saemix) `(R)` — 开源 R 语言随机逼近期望最大化（SAEM）非线性混合效应建模包。
- [MarcLavielle/mlxR](https://github.com/MarcLavielle/mlxR) `(R)` — 面向混合效应模型的纵向 PopPK/PD 仿真与可视化包，衔接 Monolix/Simulx 生态。
- [LAPKB/Pmetrics](https://github.com/LAPKB/Pmetrics) `(R/Rust)` — 支持非参数与参数群体 PK/PD 建模及贝叶斯 MAP/MMopt 最优给药估计的引擎。
- [LAPKB/pharmsol](https://github.com/LAPKB/pharmsol) `(Rust)` — 高性能 Rust 药代/药效动力学求解库，支持解析解、ODE/SDE 仿真、NCA 与内置 DSL。
- [LAPKB/PMcore](https://github.com/LAPKB/PMcore) `(Rust)` — 纯 Rust 编写的非参数群体药动学核心引擎与 ODE 求解器（NPAG、NPOD、NPSA）。
- [FeRx-NLME/ferx-core](https://github.com/FeRx-NLME/ferx-core) `(Rust)` — 纯 Rust 开源非线性混合效应（NLME）引擎，支持 FOCE/FOCEI、SAEM 与 `.ferx` 语法。
- [DavAug/chi](https://github.com/DavAug/chi) `(Python)` — 纯 Python 机制性 ODE PK/PD、QSP 与贝叶斯 MIPD 分层推断框架。
- [MSDLLCpapers/cpk](https://github.com/MSDLLCpapers/cpk) `(Python)` — 默沙东开源的 1/2 室静脉与血管外 PK 非线性回归拟合工具，支持 AICc 自动选模与异常值检测。
- [gumgo91/PKPy](https://github.com/gumgo91/PKPy) `(Python)` — 自动化 Python 群体药动学（PopPK）分析框架，集成参数初始化、NCA、协变量筛选与 GOF。
- [orlacchioresearch/pharmacokinetics-pkpd-toolkit](https://github.com/orlacchioresearch/pharmacokinetics-pkpd-toolkit) `(Python)` — 仅依赖 NumPy 的轻量 PK/PD 工具包，支持 NCA、一室拟合与 Emax 剂量-效应评估。
- [Down-To-Programme/PK_Model](https://github.com/Down-To-Programme/PK_Model) `(Python)` — 可 pip 安装的房室 PK 库（`dtp-pkmodel`），支持 SciPy ODE 求解与多方案对比绘图。
- [blakeaw/pysb-pkpd](https://github.com/blakeaw/pysb-pkpd) `(Python)` — 为 PySB 规则化建模框架扩展 1/2/3 室经验性与机制性 PK/PD 专用宏。
- [shramish2057/NeoPKPD](https://github.com/shramish2057/NeoPKPD) `(Julia/Python)` — 结合 Julia 高速核心与 Python API/CLI 的开源 PK/PD、NLME、NCA 与 BE 平台。
- [manuhuth/NoLimits.jl](https://github.com/manuhuth/NoLimits.jl) `(Julia)` — 开源 Julia NLME 框架，融合机制性 ODE、马尔可夫、Neural ODE、标准化流随机效应与 VPC。
- [wahlquisty/FastPKSim.jl](https://github.com/wahlquisty/FastPKSim.jl) `(Julia)` — 专注恒速输注与静脉推注多房室药动学快速仿真的轻量高速 Julia 模拟器。
- [simkaryote/gPKPDSim](https://github.com/simkaryote/gPKPDSim) `(MATLAB)` — 基于 MATLAB SimBiology 的开源图形界面应用，支持 PK/PD 仿真、参数扫描、拟合与 NCA。
- [benjaminrich/linpk](https://github.com/benjaminrich/linpk) `(R)` — 通过解析解快速模拟线性房室 PK 曲线并精确计算 $C_{\max}$、$T_{\max}$、AUC 与半衰期。
- [liucann/PKparmas1.0](https://github.com/liucann/PKparmas1.0) `(Python/Streamlit | 中文)` — 轻量级中文在线房室模型药代动力学参数拟合 Web 工具。
- [peytoncchen/PK-Visualization](https://github.com/peytoncchen/PK-Visualization) `(JS/Wasm)` — 斯坦福大学 Appel 实验室开发的纯前端 WebAssembly（Pyodide）房室 PK 模拟与可视化应用。
- [SnowLeopard-io/ErgalicsStudio](https://github.com/SnowLeopard-io/ErgalicsStudio) `(TS/WebGPU | 中英)` — 浏览器端高性能科学计算工作台，内置药代动力学室分析、DDI 与 TDM 曲线拟合插件。

---

## 3. 数据准备、CDISC 转换与数据质控

- [NMautoverse/NMdata](https://github.com/NMautoverse/NMdata) `(R)` — 全链路 NONMEM 数据集准备、结构 QC、排除标记审计与运行结果自动合并工具。
- [NMautoverse/NMcalc](https://github.com/NMautoverse/NMcalc) `(R)` — 轻量级药动学核心计算函数（梯形法 AUC、CV% 等），便于快速探索与模拟汇总。
- [metrumresearchgroup/mrgda](https://github.com/metrumresearchgroup/mrgda) `(R)` — 整合多源临床试验域并派生标准定量药理分析数据集的装配工具包。
- [metrumresearchgroup/yspec](https://github.com/metrumresearchgroup/yspec) `(R)` — 基于 YAML 的定量药理数据规范管理、自动校验与 `define.pdf` 文档生成工具。
- [metrumresearchgroup/lastdose](https://github.com/metrumresearchgroup/lastdose) `(R/C++)` — 在复杂药动学给药记录中高速计算末次给药后时间（TAD）与最近一次给药剂量。
- [pharmaverse/admiral](https://github.com/pharmaverse/admiral) `(R)` — Pharmaverse 模块化 CDISC ADaM 构建工具箱，内置 `ADPC`/`ADPP`/`ADPPK` 派生模板。
- [kestrel99/pmxTools](https://github.com/kestrel99/pmxTools) `(R)` — 涵盖数据处理、闭式房室 PK 计算与 PsN/NONMEM 输出解析制表的实用工具集。

---

## 4. 非房室分析（NCA）、生物等效性（BE）、IVIVC 与溶出

- [humanpred/pknca](https://github.com/humanpred/pknca) `(R)` — 全功能稀疏与密集采样非房室分析（NCA）引擎，支持自动单位换算与 CDISC 输出。
- [pharmaverse/aNCA](https://github.com/pharmaverse/aNCA) `(R/Shiny)` — 端到端交互式临床 NCA Web 应用，支持交互式 $\lambda_z$ 选点、CDISC 导出与可复现脚本生成。
- [asancpt/NonCompart](https://github.com/asancpt/NonCompart) `(R | 韩国)` — 算法对齐 Phoenix WinNonlin 与 CDISC SDTM 的工业级 NCA 核心计算包。
- [asancpt/ncar](https://github.com/asancpt/ncar) `(R | 韩国)` — 基于 `NonCompart` 一键生成含个体药时曲线的监管级 PDF/RTF NCA 报告。
- [asancpt/pkrshiny](https://github.com/asancpt/pkrshiny) `(R/Shiny | 韩英)` — 封装 `pkr`/`NonCompart` 的免代码交互式非房室分析 Shiny 网页应用。
- [asancpt/BE](https://github.com/asancpt/BE) `(R | 韩国)` — 面向 2×2、2×4、4×4、Williams 与 Balaam 交叉设计的生物等效性统计与样本量包，对标 SAS PROC GLM/MIXED。
- [asancpt/BE-apps](https://github.com/asancpt/BE-apps) `(R/Shiny | 韩英)` — 集成非房室分析与生物等效性（BE）统计评估的交互式 Shiny 应用。
- [cran/bear](https://github.com/cran/bear) `(R)` — 面向 2×2×2 交叉与平行设计的平均生物等效性（ABE）与相对生物利用度统计分析 R 包。
- [Detlew/PowerTOST](https://github.com/Detlew/PowerTOST) `(R | 德/奥)` — 行业标准生物等效性统计功效与样本量计算包（TOST、ABE、RSABE、ABEL）。
- [Helmut01/replicateBE](https://github.com/Helmut01/replicateBE) `(R)` — 遵循 EMA 指南（Method A/B）的高变异药物重复交叉设计 ABEL 生物等效性评价包。
- [juntotechnologies/bioeq](https://github.com/juntotechnologies/bioeq) `(Python)` — 纯 Python 生物等效性（BE）计算包，支持交叉与平行试验设计。
- [PharmCat/MetidaNCA.jl](https://github.com/PharmCat/MetidaNCA.jl) `(Julia)` — 面向药物研发与大规模临床试验仿真后处理的高性能 Julia NCA 库。
- [PharmCat/MetidaBioeq.jl](https://github.com/PharmCat/MetidaBioeq.jl) `(Julia)` — 基于混合效应与广义线性模型计算几何均值比及 90% 置信区间的 Julia BE 评估包。
- [matthiaskoenig/pkpdutils](https://github.com/matthiaskoenig/pkpdutils) `(Python | 德国)` — 支持单位感知 NCA、NONMEM/Monolix/ADNCA 读写、曲线拟合、BE 统计与 DDI 分级的 Python 库。
- [Open-Systems-Pharmacology/IVIVC-with-particle-dissolution-module-in-OSP](https://github.com/Open-Systems-Pharmacology/IVIVC-with-particle-dissolution-module-in-OSP) `(R/PK-Sim)` — 基于 OSP 套件的机制性 PBPK-IVIVC 工作流，将粒径分布与体外溶出关联至体内口服 PK。
- [cran/Rivivc](https://github.com/cran/Rivivc) `(R)` — 通过数值反卷积与卷积实现线性 A 级体内外相关性（IVIVC）建模，支持非等距采样点。
- [vkaralis/ivivs-be](https://github.com/vkaralis/ivivs-be) `(Python)` — 结合胃肠道分段溶出、房室 PK ODE 与蒙特卡洛虚拟试验预测生物等效性的体内外模拟（IVIVS）工具。
- [zhengguoxu/bootf2](https://github.com/zhengguoxu/bootf2) `(R)` — 依据 FDA/EMA 指南采用相似因子（$f_2$）与自助法 $f_2$ 90% 置信区间比较高变异体外溶出曲线。
- [piusdahinden/disprofas](https://github.com/piusdahinden/disprofas) `(R)` — 非参数体外溶出曲线相似性检验工具，支持 $f_1$/$f_2$、Shah 自助法 $f_2$、MCR 与 $T^2$ 检验。
- [Shipbuilder/Bioequivalence](https://github.com/Shipbuilder/Bioequivalence) `(Scripts | 中文)` — 中文开发者上传的生物等效性（BE）试验统计分析参考脚本。

---

## 5. 模型诊断、可视化与自动化报告

- [UUPharmacometrics/xpose](https://github.com/UUPharmacometrics/xpose) `(R)` — 现代 `ggplot2` 模型诊断框架，用于导入 NONMEM 输出并绘制 GOF、残差与 VPC 图。
- [UUPharmacometrics/xpose4](https://github.com/UUPharmacometrics/xpose4) `(R)` — 经典 NONMEM 建模辅助诊断包，基于 lattice 提供 GOF、VPC 与协变量筛选图。
- [nlmixr2/xpose.nlmixr2](https://github.com/nlmixr2/xpose.nlmixr2) `(R)` — 将 `nlmixr2` 拟合对象桥接为标准 `xpose` 数据库对象以复用全套 `xpose` 诊断图。
- [nlmixr2/nlmixr2plot](https://github.com/nlmixr2/nlmixr2plot) `(R)` — 面向 `nlmixr2` 模型拟合结果的原生 `ggplot2` 诊断图与 VPC 绘图包。
- [ggPMXdevelopment/ggPMX](https://github.com/ggPMXdevelopment/ggPMX) `(R)` — 跨 Monolix、NONMEM、`nlmixr2` 一键生成符合 ISoP 标准的申报级 GOF 诊断图与报告。
- [metrumresearchgroup/pmplots](https://github.com/metrumresearchgroup/pmplots) `(R)` — 提供面向定量药理分析的标准化、申报级探索性与拟合优度诊断图表。
- [certara/tidyvpc](https://github.com/certara/tidyvpc) `(R)` — 基于 `data.table` 的高速管道式 VPC 引擎，支持分箱、无分箱（AQR/LOESS）、pcVPC 与 BLQ。
- [ronkeizer/vpc](https://github.com/ronkeizer/vpc) `(R)` — 灵活的跨平台 R 语言 VPC 工具包，支持连续型、分类型与事件时间（TTE）视觉预测检验。
- [UUPharmacometrics/ncappc](https://github.com/UUPharmacometrics/ncappc) `(R)` — 基于 NCA 暴露指标（$C_{max}$、$AUC$）对 PopPK/PD 模型执行后验预测检验（PPC）。
- [pharmetheus/PMXForest](https://github.com/pharmetheus/PMXForest) `(R)` — 直接从 NONMEM `.cov`、PsN Bootstrap 或 SIR 输出自动生成含不确定性的协变量森林图。
- [metrumresearchgroup/pmforest](https://github.com/metrumresearchgroup/pmforest) `(R)` — 直接基于模型参数与 `mrgsolve` 模拟输出生成高度可定制的协变量效应森林图。
- [certara/coveffectsplot](https://github.com/certara/coveffectsplot) `(R/Shiny)` — 提供函数与交互式 Shiny 应用，绘制申报级协变量暴露影响森林图（亦见 [smouksassi/coveffectsplot](https://github.com/smouksassi/coveffectsplot)）。
- [Novartis/xgxr](https://github.com/Novartis/xgxr) `(R)` — 诺华探索性图形（xGx）框架，提供标准化 PK/PD 与暴露-效应作图助手与草稿标注。
- [metrumresearchgroup/pmtables](https://github.com/metrumresearchgroup/pmtables) `(R)` — 专为定量药理申报报告打造的 LaTeX/TeX 人口学、数据清单与参数估计表格生成器。
- [certara/pmxpartabc](https://github.com/certara/pmxpartabc) `(R)` — 自动解析 NONMEM 运行目录与 YAML 配置，生成可直接申报的参数估计表（含 Bootstrap）。
- [NMautoverse/tracee](https://github.com/NMautoverse/tracee) `(R)` — 自动为保存的图表嵌入源脚本路径、时间戳与元数据印记，保障监管级代码可追溯性。
- [kylebaron/mrgsim.sa](https://github.com/kylebaron/mrgsim.sa) `(R)` — 面向 `mrgsolve` 模型的局部与序列参数敏感度分析及可视化扩展包。
- [nlmixr2/nlmixr2rpt](https://github.com/nlmixr2/nlmixr2rpt) `(R)` — 基于 YAML 规范自动将 `nlmixr2` 拟合结果生成结构化 Word 与 PPT 定量药理报告。
- [john-harrold/ruminate](https://github.com/john-harrold/ruminate) `(R/Shiny)` — 整合数据整理、绘图、PKNCA、`rxode2` 仿真与 Office 报告导出的低代码 Shiny 工作台。
- [Genentech/gPKPDviz](https://github.com/Genentech/gPKPDviz) `(R/Shiny)` — 基因泰克开源的交互式 `mrgsolve` PopPK/PD 仿真与虚拟人群探索 Shiny 平台。
- [Boehringer-Ingelheim/MVPapp](https://github.com/Boehringer-Ingelheim/MVPapp) `(R/Shiny | 德国)` — 支持在线编辑 `mrgsolve` 代码、NCA、敏感度分析与 NHANES 虚拟人群的模型可视化平台。
- [pipetcpt/2025-jscpt](https://github.com/pipetcpt/2025-jscpt) `(R/NONMEM | 韩/日)` — 直接从 NONMEM 输出自动生成项目反应理论（IRT）纵向药效模型发表级信息图。

---

## 6. 临床药理监管、C-QTc、I/II 期剂量探索、E-R、CTS 与 FIH

- [FDA/PKView](https://github.com/FDA/PKView) `(R/Shiny)` — 美国 FDA 交互式临床药理审评工具，读取 CDISC SDTM/ADaM 数据自动生成 PK、剂量-效应与安全性报告。
- [A2-ai/cqtkit](https://github.com/A2-ai/cqtkit) `(R)` — 对齐 Garnett 白皮书标准的浓度-QTc（C-QTc）建模工作流包，涵盖预处理、EDA、LME 拟合与诊断。
- [joannaparkinson/C-QTc-hands-on-tutorial](https://github.com/joannaparkinson/C-QTc-hands-on-tutorial) `(R)` — 《浓度-QTc 建模实践指南》配套可复现 R 脚本库，基于公开 PhysioNet 数据演示 ΔΔQTc 预测全流程。
- [FDA/CiPA](https://github.com/FDA/CiPA) `(R)` — 美国 FDA 官方 CiPA 心脏安全性计算机模拟代码库，支持 hERG 动力学拟合与人心室动作电位仿真。
- [Novartis/OncoBayes2](https://github.com/Novartis/OncoBayes2) `(R/Stan)` — 诺华开源贝叶斯逻辑回归模型（BLRM），支持 EXNEX 分层借用与 EWOC 准则，用于单药/联合肿瘤 I 期剂量递增。
- [openpharma/crmPack](https://github.com/openpharma/crmPack) `(R)` — 面向对象的模型驱动剂量递增框架，支持 CRM、BLRM 及毒性-生物标志物双终点试验设计。
- [brockk/escalation](https://github.com/brockk/escalation) `(R)` — 统一模块化语法的 I/II 期剂量探索框架，支持 BOIN、BOIN12、mTPI-2、CRM 与 TITE-CRM 模拟。
- [openpharma/DoseFinding](https://github.com/openpharma/DoseFinding) `(R/C)` — 实现监管认可的 MCP-Mod 方法，用于 II 期剂量探索试验的规划、最优设计与剂量-效应分析。
- [cran/BOIN](https://github.com/cran/BOIN) `(R)` — 实现单药与联合用药 I 期贝叶斯最优区间（BOIN）设计，广泛用于 FDA Project Optimus 剂量优化。
- [yamagubed/boinet](https://github.com/yamagubed/boinet) `(R)` — 实现综合评估疗效与毒性的 BOIN-ET 系列 I/II 期设计，以确定最佳生物学剂量（OBD）。
- [brockk/trialr](https://github.com/brockk/trialr) `(R/Stan)` — 基于 RStan 的贝叶斯临床试验设计工具集，涵盖 CRM、TITE-CRM 与 EffTox 无缝 I/II 期模型。
- [mikesweeting/bcrm](https://github.com/mikesweeting/bcrm) `(R)` — 实现单/双参数贝叶斯连续重新评估法（CRM）及 I 期试验运行特征模拟。
- [cran/dfcrm](https://github.com/cran/dfcrm) `(R)` — 经典 I 期剂量探索 R 包，提供标准 CRM 及针对迟发性毒性的 TITE-CRM 算法。
- [cran/clinDR](https://github.com/cran/clinDR) `(R)` — 面向临床药理 II 期剂量范围研究的贝叶斯与最大似然 Emax 剂量-效应建模包。
- [Genentech/BayesERtools](https://github.com/Genentech/BayesERtools) `(R/Stan)` — 基因泰克开源贝叶斯暴露-效应（E-R）建模工具包，支持二分类/连续终点与决策森林图。
- [metrumresearchgroup/confounded-exposure-metrics](https://github.com/metrumresearchgroup/confounded-exposure-metrics) `(R/NONMEM)` — 揭示肿瘤 E-R 与生存分析（TTE）中不同暴露指标引入混杂偏倚的仿真方法学仓库。
- [clay-good/onkos](https://github.com/clay-good/onkos) `(Python)` — 分级标注的肿瘤生长抑制（TGI）与 E-R 模型库，支持导出至 NONMEM、SBML、`rxode2` 与 Pumas。
- [orlacchioresearch/tumor-growth-inhibition-modeling](https://github.com/orlacchioresearch/tumor-growth-inhibition-modeling) `(Python)` — 临床前异种移植瘤生长曲线拟合（指数/Gompertz/Logistic）与 TGI%/%T/C 计算工具。
- [campsisverse/campsis](https://github.com/campsisverse/campsis) `(R)` — 引擎无关的临床试验仿真（CTS）平台，解耦试验设计与底层 `rxode2`/`mrgsolve` 求解器。
- [andrewhooker/PopED](https://github.com/andrewhooker/PopED) `(R)` — 基于费雪信息矩阵（FIM）的 NLME 群体与个体最优临床采样与给药试验设计工具。
- [iame-researchCenter/PFIM](https://github.com/iame-researchCenter/PFIM) `(R | 法国)` — 基于群体 FIM 评估与优化 NLME 临床采样设计，支持协变量、IOV 与多种优化算法。
- [phuse-org/toxSummary](https://github.com/phuse-org/toxSummary) `(R/Shiny)` — 交互式汇总重复给药毒理暴露安全窗与跨种属转化，支撑首次人体（FIH）起始剂量论证。
- [pipetcpt/DallphinAtoM](https://github.com/pipetcpt/DallphinAtoM) `(R | 韩英)` — 利用异速生长缩放与生理参数从临床前动物数据预测人体 PK 参数。
- [m-amanda/Analytical-Methods-Validation-with-R](https://github.com/m-amanda/Analytical-Methods-Validation-with-R) `(R/Shiny)` — 生物分析方法学验证 Shiny 应用，支持基质效应、标准曲线线性、方差齐性与 LOD/LOQ 评估。
- [giovannisolarino/Methods-Validation-App-Web](https://github.com/giovannisolarino/Methods-Validation-App-Web) `(Python)` — 面向受监管生物分析实验室评估多日多水平 LC-MS 标曲及准确度/精密度的 Web 应用。

---

## 7. 模型引导精准给药（MIPD）、临床 TDM、抗感染 PTA 与 TCI

### 7.1 通用贝叶斯 / MIPD 引擎与外部验证

- [sotalya/tucuxi-core](https://github.com/sotalya/tucuxi-core) `(C++ | 瑞士/法)` — 医院验证的开源贝叶斯 TDM/MIPD 核心计算引擎，提供 CLI 与 REST 服务。
- [sotalya/tucuxi-gui](https://github.com/sotalya/tucuxi-gui) `(C++/Qt | 瑞士/法)` — 配套 `tucuxi-core` 的临床桌面端血药浓度解读与个体化调量图形界面。
- [sotalya/tucuxi-drugs](https://github.com/sotalya/tucuxi-drugs) `(XML | 瑞士/法)` — 供 Tucuxi 引擎调用的窄治疗窗药物开源 XML 群体药动学模型库。
- [sotalya/tucuxi-python](https://github.com/sotalya/tucuxi-python) `(Python/C++ | 瑞士/法)` — `tucuxi-core` 的 Python 绑定，用于脚本化 PK 预测与批量回顾性 TDM 评估。
- [levenc/posologyr](https://github.com/levenc/posologyr) `(R | 法国)` — 基于 `rxode2` 的开源 MIPD 包，提供贝叶斯 MAP 估计及目标 AUC/谷浓度最优剂量反推。
- [FelicienLL/mapbayr](https://github.com/FelicienLL/mapbayr) `(R | 法国)` — 基于 `mrgsolve` 模型实现亚秒级临床 TDM 贝叶斯 MAP 参数估计的轻量引擎。
- [FelicienLL/mapbayr-shiny](https://github.com/FelicienLL/mapbayr-shiny) `(R/Shiny | 法国)` — 基于 `mapbayr` 的即用型贝叶斯 TDM 计算器 Shiny 应用模板集。
- [InsightRX/PKPDmap](https://github.com/InsightRX/PKPDmap) `(R)` — 直接在 `PKPDsim` 模型对象上执行个体化 MAP 贝叶斯参数估计。
- [InsightRX/PKPDposterior](https://github.com/InsightRX/PKPDposterior) `(R/Stan)` — 基于 Stan/Torsten 的全贝叶斯 MCMC 精准给药推断，量化个体暴露与毒性完整后验不确定性。
- [InsightRX/clinPK](https://github.com/InsightRX/clinPK) `(R)` — 封装经验证的临床药理标准公式（肾功能 eGFR/CG、体重指标 IBW/LBW/BSA 与基础房室方程）。
- [InsightRX/mipdeval](https://github.com/InsightRX/mipdeval) `(R)` — 在历史临床 TDM 数据集上评估群体 PK/PD 模型迭代贝叶斯预测准确度与偏倚的工具包。
- [InsightRX/mipdtrial](https://github.com/InsightRX/mipdtrial) `(R)` — 在模型引导精准给药（MIPD）自适应临床试验方案下模拟 PK/PD 终点与目标达标率。
- [Martin-Umpierrez/exeval](https://github.com/Martin-Umpierrez/exeval) `(R)` — 自动化执行文献 PopPK/PD 模型在独立医院本地临床队列上的外部验证与贝叶斯预测评估。

### 7.2 抗感染 PK/PD、PTA/CFR 与抗菌/抗真菌 TDM

- [liangRXdev/vanco-auc-calc](https://github.com/liangRXdev/vanco-auc-calc) `(JS/PWA | 繁中/英)` — 纯前端离线万古霉素 AUC 个体化计算器，含 Sawchuk-Zaske 双点反算、双室贝叶斯与 AKI/妊娠警示。
- [asancpt/shiny-vtdm](https://github.com/asancpt/shiny-vtdm) `(R/Shiny | 韩英)` — 韩国峨山医院万古霉素二室 PopPK 贝叶斯精准给药 Shiny 应用。
- [pipetcpt/tdm-vancomycin](https://github.com/pipetcpt/tdm-vancomycin) `(R/Shiny | 韩英)` — 韩国天主教大学 PIPET 万古霉素 PopPK 给药仿真与 TDM 自动化 Shiny 应用。
- [kpessa/vanco-auc](https://github.com/kpessa/vanco-auc) `(Excel/VBA)` — 美国医院实际部署的万古霉素经验给药与双点梯形法 AUC24/MIC 计算工具包。
- [njrhodes/bds-app](https://github.com/njrhodes/bds-app) `(R/Shiny/Stan)` — 贝叶斯给药模拟应用集合，内置美罗培南与哌拉西林-他唑巴坦 MIPD 精准给药模块。
- [cptbern/ShinyFlucloxacillin](https://github.com/cptbern/ShinyFlucloxacillin) `(R/Shiny | 瑞士)` — 伯尔尼大学开发的住院患者氟氯西林个体化贝叶斯 TDM 交互式 Shiny 应用。
- [piranfar/caz-avi-evidence-composite-pkpd](https://github.com/piranfar/caz-avi-evidence-composite-pkpd) `(R/Python)` — 评估持续输注头孢他啶-阿维巴坦联合达标概率（PTA）与累积反应分数（CFR）的蒙特卡洛 PK/PD 模拟库。
- [shemtsai/Aminoglycoside-Calculator](https://github.com/shemtsai/Aminoglycoside-Calculator) `(HTML/JS)` — 感染科药师开发的轻量级浏览器端氨基糖苷类非梯形法药动学给药计算器。
- [joshcase/code-blue-gentamicin](https://github.com/joshcase/code-blue-gentamicin) `(Python/Web)` — 面向临床医生和药师的教学型庆大霉素药动学给药与安全校验计算器。
- [727397883/Rifampicin-PopPK-Repository](https://github.com/727397883/Rifampicin-PopPK-Repository) `(R/Shiny | 中国)` — 中南大学湘雅医院开源的抗结核药利福平 PopPK 文献模型库与 `mrgsolve` 给药模拟应用。
- [HassDhia/antibiosim](https://github.com/HassDhia/antibiosim) `(Python)` — 兼容 Gymnasium 的抗菌药物 PK/PD 达标、剂量优化与细菌动力学仿真环境。

### 7.3 免疫抑制剂、窄治疗窗药物与临床计算器（含儿科/CRRT）

- [FelicienLL/BUSULFANAPP](https://github.com/FelicienLL/BUSULFANAPP) `(R/Shiny | 法国)` — 面向儿童造血干细胞移植（HSCT）患者的白消安（Busulfan）贝叶斯精准给药 Shiny 应用。
- [wojjy001/infliximab-bayes](https://github.com/wojjy001/infliximab-bayes) `(R)` — 炎症性肠病（IBD）英夫利昔单抗维持治疗的贝叶斯预测与自适应给药仿真（配套 [wojjy001/adaptive-infliximab](https://github.com/wojjy001/adaptive-infliximab)）。
- [abusuraihsakhri/digoxin-therapeutic-level-estimator](https://github.com/abusuraihsakhri/digoxin-therapeutic-level-estimator) `(HTML/JS)` — 根据患者生理参数与给药史估算地高辛血药浓度与治疗窗状态的轻量工具。
- [pharmot/multipurpose-calculator](https://github.com/pharmot/multipurpose-calculator) `(HTML/JS)` — 综合医院药学计算套件（VMFH），含万古霉素 AUC、氨基糖苷类、校正苯妥英钠、肝素、CrCl 与 NICU TPN。
- [jeremy-steinberg/Paediatric-Dosing](https://github.com/jeremy-steinberg/Paediatric-Dosing) `(JS/HTML5)` — 零依赖纯前端儿科按体重给药（mg/mL）临床计算器（基于新西兰处方集）。
- [stalex444/CRRT_simulator](https://github.com/stalex444/CRRT_simulator) `(HTML/JS)` — 交互式 ICU 连续性肾脏替代治疗（CRRT）模拟器，含实时滤过分数监测与内置药物给药计算器。
- [Londopy/Clinical_IQ](https://github.com/Londopy/Clinical_IQ) `(TS/Python)` — 全栈临床决策支持 Web 应用，集成肾功能调量体重计算器与静脉输注滴速计算器。
- [cloveropen/pass](https://github.com/cloveropen/pass) `(Web | 中文)` — 临床合理用药监测系统（PASS）开源参考实现，含医嘱审方、四级风险警示与 DDI 审查。
- [yusuketakuma/pharma-free-tools](https://github.com/yusuketakuma/pharma-free-tools) `(HTML/JS | 日文)` — 面向日本临床药师的 24 款免费网页工具，含基于肌酐清除率的抗菌药肾功能调量计算器。
- [koikelab/medication_eq_R](https://github.com/koikelab/medication_eq_R) `(R | 日英)` — 基于日本精神科标准自动计算精神科药物等效剂量的 R 工具。
- [teezeit/medication-calculator](https://github.com/teezeit/medication-calculator) `(TS/React | 德国)` — 纯前端双指数药动学计算与 Plotly 多方案血药浓度对比单页应用。

### 7.4 围术期麻醉 TCI、阿片解救与胰岛素-血糖 PK/PD

- [vitaldb/tivatci](https://github.com/vitaldb/tivatci) `(Python | 韩国)` — 开源全凭静脉麻醉（TIVA）与靶控输注（TCI）Python 库，内置 Schnider/Marsh/Minto/Eleveld 模型。
- [luktinghin/simtiva](https://github.com/luktinghin/simtiva) `(JS/PWA)` — 离线 PWA 靶控输注模拟器，支持丙泊酚与瑞芬太尼多模型及双药 PD 协同交互模拟。
- [BobAubouin/Python_Anesthesia_Simulator](https://github.com/BobAubouin/Python_Anesthesia_Simulator) `(Python)` — 模拟丙泊酚、瑞芬太尼、去甲肾上腺素对 BIS/MAP/心输出量 PK/PD 效应的闭环麻醉基准仿真器。
- [ManuMerlo/AReS-Anesthesia-Response-Simulator](https://github.com/ManuMerlo/AReS-Anesthesia-Response-Simulator) `(Python/MATLAB)` — 综合 TIVA 患者响应模拟器（AReS），涵盖 4 药 TCI 输注、手术应激与体液丢失动力学。
- [jarretrt/tci](https://github.com/jarretrt/tci) `(R)` — 实现丙泊酚与瑞芬太尼房室 PK/PD 靶控输注速率算法及闭环贝叶斯参数更新。
- [fra-mar/tci_simulator](https://github.com/fra-mar/tci_simulator) `(Python)` — Python 多房室药动学 TCI 泵输注速率与血浆/效应室浓度曲线模拟器。
- [seazuma/pkpd](https://github.com/seazuma/pkpd) `(JS/HTML | 日英)` — 离线可用的浏览器端麻醉药三室 PK/PD 与 TCI 模拟器（丙泊酚/芬太尼/咪达唑仑，含 BIS 预测）。
- [ysuzuki1978/rocuronium-pkpd-simulator](https://github.com/ysuzuki1978/rocuronium-pkpd-simulator) `(JS/PWA | 日英)` — 模拟罗库溴铵 PK 与肌松药效（TOF 比值）的离线 PWA，集成 5 个含日本临床协变量的验证模型。
- [ysuzuki1978/remimazolam-tci-simulator](https://github.com/ysuzuki1978/remimazolam-tci-simulator) `(JS/HTML | 日英)` — 实现日本 Masui (2022) 模型的瑞马唑仑效应室浓度 TCI/TIVA 模拟器，支持 CSV 导出。
- [ysuzuki1978/propofol-tci-simulator](https://github.com/ysuzuki1978/propofol-tci-simulator) `(JS/HTML | 日英)` — 基于 Eleveld (2018) 框架的丙泊酚效应室靶控输注交互式模拟器。
- [Clinical-Pharmacy-Saarland-University/pi_pumpsim](https://github.com/Clinical-Pharmacy-Saarland-University/pi_pumpsim) `(Python/Svelte | 德英)` — 德国萨尔大学“Dr. Dosis”静脉输注药动学实时仿真触屏教学演示系统。
- [FDA/Mechanistic-PK-PD-Model-to-Rescue-Opioid-Overdose](https://github.com/FDA/Mechanistic-PK-PD-Model-to-Rescue-Opioid-Overdose) `(R)` — 美国 FDA 机制性 PK/PD 模型，模拟芬太尼/卡芬太尼所致呼吸抑制并评估纳洛酮解救给药方案。
- [practicefusion/mmecalculator](https://github.com/practicefusion/mmecalculator) `(C#)` — 解析自由文本处方用法并计算每日最大吗啡毫克当量（MME）以监测阿片过量风险的库与 API。
- [jxx123/simglucose](https://github.com/jxx123/simglucose) `(Python)` — 经 FDA 批准的 UVA/Padova 1 型糖尿病葡萄糖-胰岛素 PK/PD 模拟器（兼容 Gymnasium）。
- [Perceptus/GlucoSym](https://github.com/Perceptus/GlucoSym) `(JS/Python)` — 模拟人体葡萄糖-胰岛素代谢与胰岛素 PK 以测试闭环人工胰腺控制算法。
- [1paulpo1/uva-padova-glucose-control-system](https://github.com/1paulpo1/uva-padova-glucose-control-system) `(C++/Python)` — 基于 CGM、饮食与胰岛素泵记录实现个体化 UVA/Padova PK/PD 参数辨识与血糖预测。

### 7.5 多房室血药浓度追踪与动态校准

- [xingqimiao/Kira-HRT-Tracker](https://github.com/xingqimiao/Kira-HRT-Tracker) `(TS | 中英)` — 隐私优先给药追踪与 PopPK 模拟应用，内置 MAP/EKF/OU-Kalman 4 种血检校准器并支持 MCP 协议。
- [LaoZhong-Mihari/HRT-Recorder-PKcomponent-Test](https://github.com/LaoZhong-Mihari/HRT-Recorder-PKcomponent-Test) `(Swift | 中英)` — 原生三室模型与双相肌注库房动力学解析计算引擎，支持多途径吸收与体重校正。
- [TransmtfTeam/Transmtf-HRT-Tracker](https://github.com/TransmtfTeam/Transmtf-HRT-Tracker) `(TS | 中英)` — 支持翻转动力学（flip-flop）、三室透皮级联吸收及贝叶斯/EKF 实测校准的 PK 仿真框架。
- [meowhuan/Oyama-s-HRT-Tracker](https://github.com/meowhuan/Oyama-s-HRT-Tracker) `(TS | 多语言)` — 基于三室与双相库房解析式的本地血药浓度与 AUC 实时模拟可视化 Web 工具。
- [Trans-Prism/Trans-Prism](https://github.com/Trans-Prism/Trans-Prism) `(Flutter/JS | 中文)` — 跨平台隐私优先工具箱，内置多室指数衰减叠加血药浓度曲线模拟器与用药时间线。
- [WHSAH/estrannaise.js](https://github.com/WHSAH/estrannaise.js) `(JS)` — 纯前端浏览器三房室雌二醇药动学与贝叶斯参数推断模拟器，支持任意给药方案。

---

## 8. 生理药代动力学（PBPK）、IVIVE、DDI 与特殊人群

- [Open-Systems-Pharmacology/PK-Sim](https://github.com/Open-Systems-Pharmacology/PK-Sim) `(C#/.NET | 德国)` — 旗舰级开源全身 PBPK 建模与仿真平台，内置成人、儿科及特殊人群生理数据库。
- [Open-Systems-Pharmacology/MoBi](https://github.com/Open-Systems-Pharmacology/MoBi) `(C#/.NET | 德国)` — 与 PK-Sim 互补的多尺度生物仿真与机理 QSP/PBPK 建模软件，支持自定义生化反应网络。
- [Open-Systems-Pharmacology/OSPSuite.Core](https://github.com/Open-Systems-Pharmacology/OSPSuite.Core) `(C#/.NET)` — PK-Sim、MoBi 及各语言绑定共用的底层核心 PBPK 计算引擎与仿真内核。
- [Open-Systems-Pharmacology/OSPSuite-R](https://github.com/Open-Systems-Pharmacology/OSPSuite-R) `(R/C++)` — PK-Sim 与 MoBi 的编程式 R 接口，支持无 GUI 批量运行 PBPK 仿真与参数扫描。
- [Open-Systems-Pharmacology/Matlab-Toolbox](https://github.com/Open-Systems-Pharmacology/Matlab-Toolbox) `(MATLAB)` — 从 MATLAB 程序化操控、批量仿真与参数识别 PK-Sim/MoBi 模型的官方工具箱。
- [Open-Systems-Pharmacology/OSPSuite.ReportingEngine](https://github.com/Open-Systems-Pharmacology/OSPSuite.ReportingEngine) `(R)` — 自动生成 OSP PBPK/QSP 模型标准化资质验证流程、诊断图与申报级报告的 R 工具包。
- [Open-Systems-Pharmacology/OSPSuite.ParameterIdentification](https://github.com/Open-Systems-Pharmacology/OSPSuite.ParameterIdentification) `(R)` — 为 PK-Sim/MoBi 模型提供程序化参数识别、优化拟合与不确定性分析。
- [Open-Systems-Pharmacology/TLF-Library](https://github.com/Open-Systems-Pharmacology/TLF-Library) `(R)` — 面向 OSP 生态生成标准化药动学表格、清单与验证图表的面向对象 R 可视化框架。
- [Open-Systems-Pharmacology/OSPSuite.RUtils](https://github.com/Open-Systems-Pharmacology/OSPSuite.RUtils) `(R)` — 为全部 OSP Suite R 包提供数据校验、类型检查与日志记录的共享底层工具包。
- [Open-Systems-Pharmacology/OSP-PBPK-Model-Library](https://github.com/Open-Systems-Pharmacology/OSP-PBPK-Model-Library) `(PK-Sim/R)` — 经同行评议的开源 PBPK 化合物验证模型与评估报告库。
- [Open-Systems-Pharmacology/OSP-Qualification-Reports](https://github.com/Open-Systems-Pharmacology/OSP-Qualification-Reports) `(Markdown/R)` — 集中汇总并在每次版本发布时自动编译平台级 PBPK 资质验证报告的官方仓库。
- [Open-Systems-Pharmacology/Qualification-DDI-CYP3A4](https://github.com/Open-Systems-Pharmacology/Qualification-DDI-CYP3A4) `(PK-Sim/R)` — 针对 CYP3A4 介导药物相互作用（DDI）的监管级全身 PBPK 资格验证方案与数据集。
- [Open-Systems-Pharmacology/Pediatric_Qualification_Package_CYP3A4_Ontogeny](https://github.com/Open-Systems-Pharmacology/Pediatric_Qualification_Package_CYP3A4_Ontogeny) `(PK-Sim)` — 验证从婴幼儿到青少年 CYP3A4 酶发育（Ontogeny）与儿科外推性能的官方资质包。
- [Open-Systems-Pharmacology/Vancomycin-Model](https://github.com/Open-Systems-Pharmacology/Vancomycin-Model) `(PK-Sim/R)` — 聚焦肾小球滤过清除的万古霉素全身 PBPK 模型与验证报告。
- [Open-Systems-Pharmacology/Voriconazole-Model](https://github.com/Open-Systems-Pharmacology/Voriconazole-Model) `(PK-Sim)` — 刻画伏立康唑非线性代谢、CYP2C19 多态性与 CYP3A4 时间依赖性抑制的全身 PBPK 模型。
- [Open-Systems-Pharmacology/Voriconazole-Tacrolimus-DDGI](https://github.com/Open-Systems-Pharmacology/Voriconazole-Tacrolimus-DDGI) `(PK-Sim)` — 量化伏立康唑与他克莫司之间高风险药物-药物-基因相互作用（DDGI）的全身 PBPK 模型。
- [Open-Systems-Pharmacology/Pregnancy-Models](https://github.com/Open-Systems-Pharmacology/Pregnancy-Models) `(PK-Sim/MoBi)` — 纳入孕期生理变化与母胎/胎盘转运模块的妊娠期全身 PBPK 框架。
- [Open-Systems-Pharmacology/Lactation-PBPK-model](https://github.com/Open-Systems-Pharmacology/Lactation-PBPK-model) `(MoBi/SQLite)` — 模拟母体药物向乳汁转运及婴儿相对摄入剂量（RID）的哺乳期 PBPK 构建模块。
- [Clinical-Pharmacy-Saarland-University/PBPK-Models](https://github.com/Clinical-Pharmacy-Saarland-University/PBPK-Models) `(PK-Sim/R | 德国)` — 德国萨尔大学维护的经同行评议 PBPK 与药物-药物/药物-基因相互作用（DDI/DDGI）模型库。
- [Sanofi-Public/saemixPBPK](https://github.com/Sanofi-Public/saemixPBPK) `(R | 法国)` — 将开源 SAEM 非线性混合效应算法与 OSP Suite 全身 PBPK/QSP 模型结合进行群体估计。
- [esqLABS/esqlabsR](https://github.com/esqLABS/esqlabsR) `(R)` — 基于结构化 Excel 配置模板标准化管理大型多情景 OSP Suite PBPK/QSP 工作流。
- [certara/Simcyp-R-Scripts](https://github.com/certara/Simcyp-R-Scripts) `(R)` — Certara 官方 Simcyp R 集成示例脚本库，支持程序化操控 Simcyp 模拟器与解析输出。
- [mba16hk/Simcyp-R-Workflow](https://github.com/mba16hk/Simcyp-R-Workflow) `(R)` — 自动查询 ChEMBL/PubChem 理化参数并对接 Simcyp 执行批量 PBPK 仿真的工作流（SimRFlow）。
- [USEPA/CompTox-ExpoCast-httk](https://github.com/USEPA/CompTox-ExpoCast-httk) `(R/C)` — 美国 EPA 高通量毒代动力学包，提供通用 PBPK 模型、组织分配系数预测与 IVIVE 流水线。
- [ScitoVation/plethem](https://github.com/ScitoVation/plethem) `(R/Shiny)` — 集成 `httk` 与 `deSolve` 的高通量 PBPK、IVIVE 与反向剂量估算交互式 Shiny 平台。
- [metrumresearchgroup/PBPK_PC](https://github.com/metrumresearchgroup/PBPK_PC) `(R/mrgsolve)` — 在 `mrgsolve` PBPK 中实现并系统对比 Rodgers & Rowland、Berezhkovskiy 等组织分配系数（$K_p$）方法。
- [metrumresearchgroup/pbpk-qsp-mrgsolve](https://github.com/metrumresearchgroup/pbpk-qsp-mrgsolve) `(R/mrgsolve)` — Metrum 与佛罗里达大学联合开发的 `mrgsolve` 全身 PBPK/QSP 实战模板与案例库。
- [metrumresearchgroup/cptpsp-tutorial-2019](https://github.com/metrumresearchgroup/cptpsp-tutorial-2019) `(R)` — *CPT:PSP* `mrgsolve` PBPK/QSP 教程配套代码，含透明的 Poulin & Theil $K_p$ 计算脚本。
- [metrumresearchgroup/BayesPBPK-tutorial](https://github.com/metrumresearchgroup/BayesPBPK-tutorial) `(Julia/Stan/R)` — 演示基于 Julia（SciML/Turing.jl）、Stan/Torsten 与 R 的开源贝叶斯分层 PBPK 建模工作流。
- [SystemsForecasting/ManchesterPBPK](https://github.com/SystemsForecasting/ManchesterPBPK) `(R)` — 基于 `rxode2` 的透明代码优先全身 PBPK 教学与原型模型（*PBPKedu*）。
- [matthiaskoenig/sbmlsim](https://github.com/matthiaskoenig/sbmlsim) `(Python | 德国)` — 基于 `libRoadRunner` 的 SBML PBPK 仿真、参数扫描、敏感度分析与自动报告框架。
- [matthiaskoenig/glimepiride-model](https://github.com/matthiaskoenig/glimepiride-model) `(Python/SBML | 德国)` — 显式模拟肾损伤、肝硬化与 CYP2C9 基因多态性影响的格列美脲全身 PBPK 模型。
- [matthiaskoenig/dapagliflozin-model](https://github.com/matthiaskoenig/dapagliflozin-model) `(Python/SBML | 德国)` — 评估肝肾联合损伤、食物效应及尿糖排泄药效的达格列净全身 PBPK/PD 模型。
- [ahmedn12/oral-pbpk-model](https://github.com/ahmedn12/oral-pbpk-model) `(Python/R)` — 对齐 FDA 研讨会流程的多途径口服 PBPK 模型，刻画肝脏首过代谢与蛋白结合率敏感度。
- [mathworks/Chemistry-Cheminformatics-Pharmacokinetics](https://github.com/mathworks/Chemistry-Cheminformatics-Pharmacokinetics) `(MATLAB/Python)` — MathWorks 官方打通 Python/RDKit 分子描述符与 MATLAB SimBiology 预测口服吸收的工作流。
- [qurit/PSMA-PBPK-Model-Matlab](https://github.com/qurit/PSMA-PBPK-Model-Matlab) `(MATLAB)` — 针对 PSMA 靶向放射性核素药物的 SimBiology/SBML 全身 PBPK 模型。
- [pipetcpt/DallphinDDI](https://github.com/pipetcpt/DallphinDDI) `(R | 韩英)` — 韩国 EDISON 资助开发的生理/PBPK 代谢酶与转运体药物相互作用（DDI）仿真工具。

---

## 9. 生物大分子、TMDD、ADC、CAR-T、免疫原性与 QSP

- [metrumresearchgroup/bioPBPK](https://github.com/metrumresearchgroup/bioPBPK) `(Julia/R)` — 代码优先的生物大分子/单抗（mAb）全身 PBPK 模型，显式刻画 FcRn 再循环与淋巴回流。
- [Open-Systems-Pharmacology/BAY794620-Model](https://github.com/Open-Systems-Pharmacology/BAY794620-Model) `(PK-Sim)` — 针对抗体偶联药物（ADC）BAY-794620 的全身 PBPK 模型，刻画大分子分布与分解代谢。
- [azelys/tce](https://github.com/azelys/tce) `(Julia/MATLAB)` — 针对双特异性 T 细胞衔接器（BiTE/TCE）三元复合物结合、PK、结构可辨识性与最优控制的机理建模。
- [cosbi-research/PBPKmRNABiTE](https://github.com/cosbi-research/PBPKmRNABiTE) `(MATLAB | 意大利)` — 模拟 mRNA 编码双特异性 T 细胞衔接器（BiTE）转运、翻译与抗体药动学的多尺度 PBPK 模型。
- [cosbi-research/Campanile_et_al_PBPKmRNATherapeutics](https://github.com/cosbi-research/Campanile_et_al_PBPKmRNATherapeutics) `(MATLAB | 意大利)` — 基于 SimBiology 的脂质纳米颗粒（LNP）递送与 mRNA 抗体疗法 PBPK 建模框架。
- [RomanCohort/confluencia](https://github.com/RomanCohort/confluencia) `(Python | 中英)` — 面向小样本 circRNA 药物研发的计算平台，集成首个 circRNA 六室机制性 PK 模型（RNACTM）。
- [maximvpolyakov/CAR-T-model](https://github.com/maximvpolyakov/CAR-T-model) `(C++/OpenMP)` — 基于三维耦合非线性 PDE 模拟实体瘤 CAR-T 耗竭、抗原逃逸与缺氧微环境的时空仿真器。
- [BioTender-max/CARTCellEngine](https://github.com/BioTender-max/CARTCellEngine) `(Python)` — 纯 Python 实现基于 ODE 的 CAR-T 效靶杀伤动力学、T 细胞耗竭评分与疗效预测流程。
- [compiler-research/CARTopiaX](https://github.com/compiler-research/CARTopiaX) `(C++)` — 基于 BioDynaMo 的高性能多智能体（ABM）实体瘤微环境 CAR-T 细胞迁移与杀伤仿真平台。
- [FDA/TCPro](https://github.com/FDA/TCPro) `(MATLAB)` — 美国 FDA（CBER）机理计算工具，预测治疗性蛋白的 T 细胞增殖动力学及免疫原性/ADA 风险。
- [singhharsh1708/QSPAtlas.jl](https://github.com/singhharsh1708/QSPAtlas.jl) `(Julia)` — 基于 Julia 重现并验证已发表 PK/PD、QSP 及 CAR-T 细胞动力学模型的开源模型集合。
- [BMSQSP/QSPToolbox](https://github.com/BMSQSP/QSPToolbox) `(MATLAB)` — 百时美施贵宝开源 QSP 工具箱，标准化 SimBiology 仿真、全局敏感性分析与虚拟人群（VPop）校准。
- [feigelman/gQSPsim-release](https://github.com/feigelman/gQSPsim-release) `(MATLAB)` — 基因泰克基于 SimBiology 开发的图形化 QSP 平台，支持模型校准与虚拟人群交互式诊断。
- [pfizer-opensource/integrated-qsp-vpop-onco-efficacy-CPT-PSP](https://github.com/pfizer-opensource/integrated-qsp-vpop-onco-efficacy-CPT-PSP) `(MATLAB)` — 辉瑞开源肿瘤 QSP 虚拟人群框架，实现 Metropolis-Hastings 合理患者采样与纵向疗效校准。
- [popellab/QSPIO-TNBC](https://github.com/popellab/QSPIO-TNBC) `(MATLAB)` — 约翰霍普金斯 Popel 实验室开源多尺度肿瘤免疫 QSP 平台，模拟三阴性乳腺癌/非小细胞肺癌免疫联合疗法。
- [NVIDIA-BioNeMo/nvQSP](https://github.com/NVIDIA-BioNeMo/nvQSP) `(C++/CUDA/Python)` — 英伟达 BioNeMo 推出的 GPU 加速刚性 ODE 求解库，专为超大规模 QSP 虚拟人群并行仿真优化。
- [SciML/Catalyst.jl](https://github.com/SciML/Catalyst.jl) `(Julia)` — Julia SciML 符号化学反应网络 DSL，将 QSP 与系统生物学模型编译为高性能 ODE/SDE 求解器。
- [pysb/pysb](https://github.com/pysb/pysb) `(Python)` — 基于规则的 Python 系统生物学与 QSP 建模框架，自动生成生化信号反应网络与 ODE。
- [sys-bio/tellurium](https://github.com/sys-bio/tellurium) `(Python)` — 集成 Antimony 建模语言与 libRoadRunner 高速 SBML 引擎的 Python 系统生物学与 QSP 环境。
- [copasi/COPASI](https://github.com/copasi/COPASI) `(C++)` — 开源复杂通路仿真器，支持基于 SBML 的 QSP 网络确定性/随机仿真、稳态分析与参数估计。

---

## 10. AI / ML / DL / SciML / RL × 临床药理与定量药理

### 10.1 LLM 智能体、MCP 协议、RAG 与知识挖掘

- [PeterBloomingdale/pmxagent](https://github.com/PeterBloomingdale/pmxagent) `(R/Python/Docker)` — 将真实 R 定量药理函数封装为 REST API 与 MCP 服务，供 AI 智能体安全执行调用。
- [MomentumMetrix/PK_Claude](https://github.com/MomentumMetrix/PK_Claude) `(R/Claude Code)` — 将 Claude Code 集成到定量药理工作流中，辅助开展 AI 驱动的群体 PK 分析与建模执行。
- [MomentumMetrix/RstudioMCP](https://github.com/MomentumMetrix/RstudioMCP) `(TS/R)` — 面向 RStudio IDE 的 MCP 服务器，使大模型智能体可直接执行 R 定量药理脚本并捕获诊断图。
- [pharmacometricsai/nonmem-library](https://github.com/pharmacometricsai/nonmem-library) `(NONMEM/MD)` — 与多位大语言模型（Claude/Gemini/Kimi）协同开发调试的 NONMEM 群体 PK/PD 控制流基准库。
- [VirtualPatientEngine/AIAgents4Pharma](https://github.com/VirtualPatientEngine/AIAgents4Pharma) `(Python)` — 开源制药 AI 智能体套件（含 *Talk2BioModels*），支持自然语言交互与仿真系统药理数学模型。
- [openpharma-org/fda-mcp](https://github.com/openpharma-org/fda-mcp) `(TS)` — 对接 openFDA 药品说明书、FAERS 不良事件、橙皮书与紫皮书的 MCP 服务器。
- [Slow-Walker66/PK-Sim-Mobi-RAG-Tool](https://github.com/Slow-Walker66/PK-Sim-Mobi-RAG-Tool) `(Python | 中英)` — 面向 PK-Sim/MoBi 官方文档与构建模块的本地 RAG 问答排错助手。
- [lfcypo/hrt-pk-mcp](https://github.com/lfcypo/hrt-pk-mcp) `(Python/MCP | 中文)` — 将多房室 PK 算法封装为标准 MCP 服务端，向 AI Agent 暴露给药记录与血药浓度查询工具。
- [kimmingul/clinical-pharmacology-study-protocol-development](https://github.com/kimmingul/clinical-pharmacology-study-protocol-development) `(Claude Plugin | 韩英)` — 辅助临床药理学家起草 I 期临床药理方案（FIH/SAD/MAD/DDI）与知情同意书的 LLM 插件。
- [QSong-github/DrugClaw](https://github.com/QSong-github/DrugClaw) `(Python)` — 基于 LangGraph 的循证药物智能体 RAG 框架，覆盖 DDI、药物基因组学（PGx）、不良反应与 FDA 说明书。
- [gadevito/LLMDDI](https://github.com/gadevito/LLMDDI) `(Python)` — 从 DrugBank 抽取知识、微调大语言模型并与深度学习基线对比评测的 DDI 预测代码库。
- [reddy-nithin/TruPharma-Clinical-Intelligence](https://github.com/reddy-nithin/TruPharma-Clinical-Intelligence) `(Python)` — 混合 RAG（FAISS+BM25+LLM）应用，解析官方 FDA 说明书并与 FAERS 信号交叉比对实现用药安全问答。
- [nikhilreddy00/pharma-agent](https://github.com/nikhilreddy00/pharma-agent) `(Python)` — 基于 LangGraph 与 ChromaDB 交叉检索 FDA 说明书、PubMed 与临床指南的药物警戒/DDI 智能体。
- [Genentech/CLADD](https://github.com/Genentech/CLADD) `(Python)` — 基因泰克 RAG 增强多智能体 LLM 框架，动态检索生物医学知识库辅助药物发现与分子性质推理。
- [PKPDAI/PKDocClassifier](https://github.com/PKPDAI/PKDocClassifier) `(Python)` — 基于 NLP/ML 自动筛选报道体内药代动力学参数生物医学文献的二分类器。
- [dueyama/pmda-pk-curve-viewer](https://github.com/dueyama/pmda-pk-curve-viewer) `(TS/Next.js | 日英)` — 自动解析日本 PMDA 电子药品说明书 XML，提取 PK 参数并实时绘制血药浓度曲线。
- [pablosierrafernandez/FarmacoDB](https://github.com/pablosierrafernandez/FarmacoDB) `(Python | 西班牙文)` — 利用 LLM 文本挖掘自动化抽取多源药动学数据（>1,000 药物）并预测人体半衰期。
- [valentinnavalos/pharmawatch-api](https://github.com/valentinnavalos/pharmawatch-api) `(API | 西班牙文)` — 支持处方校验与药动学药物相互作用（血浆蛋白置换等）分析的药物警戒 REST API。
- [PharMolix/OpenBioMed](https://github.com/PharMolix/OpenBioMed) `(Python | 中英)` — 清华 AIR 开源生物医药多模态大模型与智能体框架，内置 ADMET 与 DDI 预测工具链。
- [datamllab/CAi_copilot](https://github.com/datamllab/CAi_copilot) `(Python | 中英)` — 自然语言驱动的开源药物设计智能体，集成 ADMET-AI 预测吸收、代谢、清除与毒性。

### 10.2 物理信息神经网络（PINNs）、Neural ODE 与 SciML

- [jameslu01/Neural_PK](https://github.com/jameslu01/Neural_PK) `(Python/PyTorch)` — 将神经常微分方程应用于跨给药方案的临床 PK 血药浓度外推，并与 NLME/LSTM/LightGBM 对比。
- [TommyGiak/pharmacoNODE](https://github.com/TommyGiak/pharmacoNODE) `(Python/PyTorch)` — 将 Neural ODE 应用于 Monolix/NONMEM 风格纵向临床 PK 预测，解决房室结构误设。
- [emotionor/UniPKModel](https://github.com/emotionor/UniPKModel) `(Python/PyTorch)` — *JCIM* 配套可解释 Neural ODE 框架与预训练权重，用于高泛化数据驱动 PK 曲线预测。
- [FraunhoferChalmersCentre/neuralODEpopulation](https://github.com/FraunhoferChalmersCentre/neuralODEpopulation) `(Python)` — 融合 Transformer、Neural ODE 与 VAE/EBVAE 随机效应的端到端群体 PK/PD 深度学习框架（含 VPC）。
- [Janssena/DeepCompartmentModels.jl](https://github.com/Janssena/DeepCompartmentModels.jl) `(Julia)` — 深度房室模型（DCM），在房室 ODE 结构约束下用神经网络学习协变量-参数关系。
- [PumasAI-Labs/DeepPumas_workshop_2026_PAGE](https://github.com/PumasAI-Labs/DeepPumas_workshop_2026_PAGE) `(Julia)` — PumasAI 官方 PAGE 研讨会代码，演示将 Neural ODE 与通用微分方程（UDE）嵌入 DeepNLME 群体模型。
- [SCAI-BIO/MMPK-SciML](https://github.com/SCAI-BIO/MMPK-SciML) `(Python/Julia)` — 弗劳恩霍夫 SCAI 官方基准库，系统对比 SciML、传统 PopPK 与经典 ML 在抗肿瘤药浓度预测中的表现。
- [NazAhmadi/CMINNs](https://github.com/NazAhmadi/CMINNs) `(Python/JAX)` — 房室模型物理信息神经网络（CMINNs/分数阶 PINNs），刻画复杂 PK/PD 中的反常扩散与时变参数。
- [yapici/open-pk-pinn](https://github.com/yapici/open-pk-pinn) `(Python/PyTorch)` — 开源可复现的房室物理信息神经网络（CMT-PINN）药动学浓度-时间预测基准。
- [novainsilico/vpop-calibration](https://github.com/novainsilico/vpop-calibration) `(Python)` — 将 NLME 推断与机器学习代理模型结合，大幅加速 QSP 虚拟人群校准。

### 10.3 强化学习（RL）与深度学习精准给药

- [hamilton-health-sciences/warfarin](https://github.com/hamilton-health-sciences/warfarin) `(Python/PyTorch)` — 基于 COMBINE-AF 临床试验数据的离线深度强化学习（`smdbcq`），优化房颤华法林序贯给药。
- [rudra2112/Warfarin-Dosage-Prediction](https://github.com/rudra2112/Warfarin-Dosage-Prediction) `(Python)` — 结合患者特征与 *CYP2C9*/*VKORC1* 基因型的上下文多臂老虎机（Linear-UCB）华法林强化学习给药。
- [karneslab/warfarin-machinelearning](https://github.com/karneslab/warfarin-machinelearning) `(R)` — 结合 CYP2C9/VKORC1 药物基因组学与临床协变量预测华法林维持剂量的机器学习代码。
- [lucis-e/PopPBPK-RL_Bnzpril](https://github.com/lucis-e/PopPBPK-RL_Bnzpril) `(Python/R)` — 将群体 PBPK 与强化学习（RL）结合，在肾损伤虚拟队列中优化贝那普利精准给药。
- [FatemehRabie/chemotherapy](https://github.com/FatemehRabie/chemotherapy) `(Python)` — 将 3D 肿瘤 PDE 仿真器与 Gymnasium/SB3 结合，利用物理引导深度强化学习优化个体化化疗方案。
- [ZhiGroup/PK-RNN](https://github.com/ZhiGroup/PK-RNN) `(Python)` — 利用电子病历纵向给药与检验数据动态预测万古霉素血药浓度的循环神经网络（PK-RNN-V）。
- [BingyuMao/vanco_2cm](https://github.com/BingyuMao/vanco_2cm) `(Python)` — 将自回归 RNN 与机理二室 PK 预测头融合的混合模型（PKRNN-2CM），实现可解释万古霉素动态预测。
- [Yunwoolee17/Vancomycin_prediction_AI](https://github.com/Yunwoolee17/Vancomycin_prediction_AI) `(Python | 韩国)` — 融合多种树模型与 SHAP 可解释性预测万古霉素达标 AUC 起始剂量的机器学习流水线。
- [y-babdalla/tacrolimus_predictions](https://github.com/y-babdalla/tacrolimus_predictions) `(Python/PyTorch)` — 结合注意力/时间感知 LSTM 与合成数据增强（*DoseTAIlor*/*TacroNET*）预测个体化他克莫司谷浓度。
- [huiyum/tac_dose_adjustments](https://github.com/huiyum/tac_dose_adjustments) `(Python/Streamlit)` — 结合 GRU 药动学深度学习与 Streamlit 界面，预测移植/ICU 患者他克莫司谷浓度并辅助调量。
- [sebboie/aptt-prediction](https://github.com/sebboie/aptt-prediction) `(Python)` — 基于回顾性临床数据构建 RNN 模型动态预测静脉输注肝素后的 aPTT 凝血轨迹。

### 10.4 自动化定量药理、ML 协变量筛选与合成患者数据

- [certara/pyDarwin](https://github.com/certara/pyDarwin) `(Python)` — 运用遗传算法、随机森林、GBRT、高斯过程与粒子群算法自动搜索最优 NONMEM/NLME 模型结构与协变量。
- [gengbo-genentech/Pharm-AutoML](https://github.com/gengbo-genentech/Pharm-AutoML) `(Python)` — 基因泰克发表于 *CPT:PSP* 的开源制药 AutoML 框架，覆盖临床药理预处理、调参与可解释分析。
- [Janssena/pkSHAP](https://github.com/Janssena/pkSHAP) `(Python/Julia)` — 利用 SHAP 可解释性解析 ML 模型，推断药动学模型中患者协变量的最优数学函数形式。
- [AstraZeneca/Stochastic-gates-for-covariate-selection-in-population-pharmacokinetics-modelling-](https://github.com/AstraZeneca/Stochastic-gates-for-covariate-selection-in-population-pharmacokinetics-modelling-) `(Python)` — 阿斯利康开源可微随机门（STG）神经网络特征选择方法，加速群体药动学协变量筛选。
- [wahlquisty/learning-pharmacometric-covariate-structures](https://github.com/wahlquisty/learning-pharmacometric-covariate-structures) `(Julia)` — 基于神经网络符号回归自动发现群体药动学协变量数学结构。
- [iasiimwe/unite4tb_ml](https://github.com/iasiimwe/unite4tb_ml) `(R/Python)` — UNITE4TB 联盟在高维药物基因组 PopPK 数据中对比 ML 与传统 GWAS/定量药理协变量筛选的基准。
- [jbwoillard/synthetic_data_pharmacogenetics](https://github.com/jbwoillard/synthetic_data_pharmacogenetics) `(R/Python)` — 面向临床药理与药物基因组队列评估 Avatar、生存 VAE 与 CTGAN 等隐私保护合成患者数据生成。

### 10.5 AI / ML / GNN 预测人体 PK 参数、药时曲线与 ADME

- [Novartis/DeepCt](https://github.com/Novartis/DeepCt) `(Python)` — 诺华开源深度学习框架，直接从 SMILES 化学结构预测完整血浆浓度-时间曲线及房室 PK 参数。
- [srijitseal/PKSmart](https://github.com/srijitseal/PKSmart) `(Python)` — 两阶段跨物种 ML 流水线，结合化学描述符与动物 PK 预测人体体内清除率、分布容积与半衰期。
- [swansonk14/admet_ai](https://github.com/swansonk14/admet_ai) `(Python)` — 基于 Chemprop 图神经网络与 TDC 基准的高速、大规模 40+ 项 ADMET 与 PK 性质预测平台。
- [xli7654321/MMPK](https://github.com/xli7654321/MMPK) `(Python)` — 融合多尺度分子表征与子结构交叉注意力的端到端多模态深度模型，预测人体口服 PK 参数。
- [xtalpi-xic/pk-model](https://github.com/xtalpi-xic/pk-model) `(Python)` — 将图神经网络（Chemprop/D-MPNN）与树模型、PBPK 结合预测小分子人体药代动力学。
- [dreadlesss/pharmacokinetic_prediction](https://github.com/dreadlesss/pharmacokinetic_prediction) `(Python)` — 基于 1,352 个化合物与梯度提升树/分子指纹预测人体静脉给药 PK 参数（CL、Vd、t1/2、MRT、fu）。
- [eugenebang/ADME-DL](https://github.com/eugenebang/ADME-DL) `(Python)` — 通过药动学引导的序贯 ADME 多任务学习增强分子基础模型，提升 PK 性质预测。
- [Sanofi-Public/DMPK-US-ML-mTPA](https://github.com/Sanofi-Public/DMPK-US-ML-mTPA) `(Python)` — 赛诺菲将极简 PBPK/TMDD 与树模型结合，用于单克隆抗体早期靶点药理与 PK/PD 可行性评估。
- [UFPBPK/Nano-AI-PBPK-G1](https://github.com/UFPBPK/Nano-AI-PBPK-G1) `(Python/R)` — 佛罗里达大学 AI 辅助 PBPK 建模框架，预测纳米颗粒在小鼠体内的肿瘤递送与组织 PK。
- [molecularinformatics/Computational-ADME](https://github.com/molecularinformatics/Computational-ADME) `(Python)` — 渤健（Biogen）工业界体外 ADME 数据集与代码，前瞻性验证 XGBoost/LightGBM/DeepChem 预测效能。
- [OpenADMET/openadmet-models](https://github.com/OpenADMET/openadmet-models) `(Python)` — 开放科学可扩展 ML 模型架构与训练流水线，用于可复现 ADMET 与 DMPK（如 CYP 抑制）预测。
- [abinittio/CYP450-Metabolism-Predictor](https://github.com/abinittio/CYP450-Metabolism-Predictor) `(Python)` — 基于 ChEMBL 构建多任务图神经网络，同步预测 5 种主要 CYP450 酶抑制与 DDI 风险。
- [CDDLeiden/PK-in-generative-drug-design](https://github.com/CDDLeiden/PK-in-generative-drug-design) `(Python)` — 将 Lombardo 人体静脉 PK 数据集与 QSP/PK 建模结合用于生成式药物设计。

---

## 11. 开源临床 PK 数据集、基准与精选索引

- [matthiaskoenig/pkdb](https://github.com/matthiaskoenig/pkdb) `(Python/Django | 德国)` — 遵循 FAIR 原则的开源临床/临床前药动学数据库（PK-DB）与 REST API。
- [Open-Systems-Pharmacology/Database-for-observed-data](https://github.com/Open-Systems-Pharmacology/Database-for-observed-data) `(Excel/CSV)` — OSP 维护的文献数字化临床血药浓度-时间曲线与 DDI 实测数据库，广泛用于 PBPK 验证。
- [nlmixr2/nlmixr2data](https://github.com/nlmixr2/nlmixr2data) `(R)` — 为 `nlmixr2`/`rxode2` 生态打包的标准群体 PK/PD 基准与教学数据集。
- [dpastoor/PKPDdatasets](https://github.com/dpastoor/PKPDdatasets) `(R)` — 面向定量药理、转化医学与建模仿真测试的即用型标准化 PK/PD 数据集集合。
- [billdenney/PKdata](https://github.com/billdenney/PKdata) `(R)` — 专为测试和验证 NCA 与 PK 软件准确性构建的真实与模拟单次/多次给药 PK 数据集。
- [mims-harvard/TDC](https://github.com/mims-harvard/TDC) `(Python)` — 哈佛 Therapeutics Data Commons（PyTDC），提供 ML 就绪的清除率、半衰期、PPB、CYP 等基准数据集。
- [mindrank-ai/PharmaBench](https://github.com/mindrank-ai/PharmaBench) `(Python/Data)` — 基于大模型挖掘清洗构建的综合性 ADMET 与药动学基准数据集（吸收、PPB、BBB、CYP、清除率）。
- [isop-phmx/awesome-pharmacometrics](https://github.com/isop-phmx/awesome-pharmacometrics) `(Markdown)` — 国际定量药理学会（ISoP）维护的高校项目、期刊、会议、教程与经典教材精选索引。
- [AIML-SIG/awesome-ai-ml-pharmacometrics](https://github.com/AIML-SIG/awesome-ai-ml-pharmacometrics) `(Markdown)` — 聚焦 AI/ML 在定量药理、PBPK 与 QSP 中应用的社区精选文献与开源资源列表。

---

## 12. 多语种开源教材与代码库

- [PumasAI-Labs/PumasIntroTutorial-ContinuousData](https://github.com/PumasAI-Labs/PumasIntroTutorial-ContinuousData) `(Julia/Quarto)` — PumasAI 官方开源教程，涵盖 Julia 临床 PK 数据整理、FDA/EMA 规范 NCA 与连续型建模。
- [asancpt/book-ncar](https://github.com/asancpt/book-ncar) `(Bookdown | 韩文)` — 韩国峨山医院开源教材《使用 R 进行非房室分析与生物等效性评价》。
- [asancpt/nmw-nonmem](https://github.com/asancpt/nmw-nonmem) `(R/NONMEM | 韩英)` — 演示 FO/FOCE/FOCE-I 混合效应估计算法并桥接 R 与 NONMEM 的教学代码库。
- [AMC-CPT/PKwR](https://github.com/AMC-CPT/PKwR) `(R/Shiny | 韩英)` — 《Pharmacokinetics with R》配套可复现脚本与万古霉素 TDM Shiny 示例。
- [AMC-CPT/PMx](https://github.com/AMC-CPT/PMx) `(R/NONMEM | 韩英)` — 《Pharmacometrics with NONMEM and R》配套控制流模板与 R 诊断后处理代码。
- [pipetcpt/basic](https://github.com/pipetcpt/basic) `(Bookdown/NONMEM | 韩文)` — 韩国 PIPET 定量药理入门讲义，覆盖 NONMEM 控制流、数据准备、协变量与 PK-PD。
- [pipetcpt/pharmapk](https://github.com/pipetcpt/pharmapk) `(Bookdown | 韩文)` — 面向新药研发的《实战药动学 I》开源教材，详解 ADME、清除率、分布与房室解析。
- [pipetcpt/book-poppk](https://github.com/pipetcpt/book-poppk) `(Bookdown | 韩文)` — 韩国 MFDS 群体药代动力学监管指导原则的开源网络化拆解参考。
- [pipetcpt/capstone-qsp](https://github.com/pipetcpt/capstone-qsp) `(R/Shiny | 韩英)` — 将机制性定量系统药理学（QSP）ODE 模型转化为交互式 Shiny 看板的实战案例集。
- [matthiaskoenig/course-pharmacokinetic-modelling](https://github.com/matthiaskoenig/course-pharmacokinetic-modelling) `(Python/Jupyter | 德英)` — 柏林洪堡大学药动学与 PBPK 建模互动 Jupyter Notebook 课程库。
- [Clinical-Pharmacy-Saarland-University/RTutorial](https://github.com/Clinical-Pharmacy-Saarland-University/RTutorial) `(R Markdown | 德英)` — 德国萨尔大学临床药学与定量药理 R 语言数据分析教学教程。
- [Kalo0m/pharmacocinetique](https://github.com/Kalo0m/pharmacocinetique) `(TS | 法文)` — 法国兽医/药学专业学生开发的药代动力学基础概念学习与计算 Web 应用。
- [douglasufs/matematica-aplicada-ciencias-farmaceuticas](https://github.com/douglasufs/matematica-aplicada-ciencias-farmaceuticas) `(OER | 葡萄牙文)` — 巴西联邦大学药学应用数学开放教材，包含稀释计算、生物等效性与计算药动学脚本。
---

## 免责声明

本仓库系个人基于公开 GitHub 开源项目独立整理的资源索引，仅供信息参考与学习交流。所有整理内容与观点仅代表个人，不代表雇主或任何关联机构的立场。收录某一仓库不构成对相关软件、机构或临床给药方法的背书、验证或推荐，亦不构成任何医疗或监管建议。使用任何收录项目前，请自行核查其开源协议、验证状态及合规要求。

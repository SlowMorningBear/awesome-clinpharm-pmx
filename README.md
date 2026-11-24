# Awesome Clinical Pharmacokinetics & Pharmacometrics (ClinPharm & PMx)

**English** | [简体中文](README.zh-CN.md)

> A curated, problem-oriented, multi-lingual directory of open-source GitHub repositories for **Clinical Pharmacokinetics (Clin. Pharm.)**, **Pharmacometrics (PMx)**, and **AI × ClinPharm/PMx**, spanning English, Chinese, Japanese, Korean, German, French, Spanish, Portuguese, and Italian ecosystems (v2.0: **335** verified repositories, zero duplicates).

---

## Contents

- [1. Workflow, Editors & Orchestration](#1-workflow-editors--orchestration)
- [2. Open-Source NLME & ODE Engines](#2-open-source-nlme--ode-engines)
- [3. Data Preparation, CDISC & QC](#3-data-preparation-cdisc--qc)
- [4. NCA, Bioequivalence, IVIVC & Dissolution](#4-nca-bioequivalence-ivivc--dissolution)
- [5. Diagnostics, Visualization & Automated Reporting](#5-diagnostics-visualization--automated-reporting)
- [6. Regulatory ClinPharm, C-QTc, Dose-Finding, E-R & FIH](#6-regulatory-clinpharm-c-qtc-dose-finding-e-r--fih)
- [7. Clinical MIPD, TDM, Antimicrobial PTA & TCI](#7-clinical-mipd-tdm-antimicrobial-pta--tci)
  - [7.1 General MIPD Engines & Validation](#71-general-mipd-engines--validation)
  - [7.2 Antimicrobial PK/PD, PTA/CFR & TDM](#72-antimicrobial-pkpd-ptacfr--tdm)
  - [7.3 Immunosuppressant, NTI & Hospital Calculators](#73-immunosuppressant-nti--hospital-calculators)
  - [7.4 Anesthesia TCI, Opioid Rescue & Glucose-Insulin PK/PD](#74-anesthesia-tci-opioid-rescue--glucose-insulin-pkpd)
  - [7.5 Multi-Compartment Tracking & Dynamic Calibration](#75-multi-compartment-tracking--dynamic-calibration)
- [8. PBPK, IVIVE, DDI & Special Populations](#8-pbpk-ivive-ddi--special-populations)
- [9. Biologics, TMDD, ADC, CAR-T, Immunogenicity & QSP](#9-biologics-tmdd-adc-car-t-immunogenicity--qsp)
- [10. AI, ML, SciML & RL for ClinPharm & PMx](#10-ai-ml-sciml--rl-for-clinpharm--pmx)
  - [10.1 LLM Agents, MCP, RAG & Knowledge Mining](#101-llm-agents-mcp-rag--knowledge-mining)
  - [10.2 PINNs, Neural ODEs, UDEs & SciML](#102-pinns-neural-odes-udes--sciml)
  - [10.3 RL & Deep Learning for Precision Dosing & TDM](#103-rl--deep-learning-for-precision-dosing--tdm)
  - [10.4 Automated PMx, ML Covariates & Synthetic Data](#104-automated-pmx-ml-covariates--synthetic-data)
  - [10.5 ML/DL Prediction of Human PK & ADME](#105-mldl-prediction-of-human-pk--adme)
- [11. Open Clinical PK Datasets, Benchmarks & Awesome Lists](#11-open-clinical-pk-datasets-benchmarks--awesome-lists)
- [12. Multi-Lingual Open Textbooks & Workshops](#12-multi-lingual-open-textbooks--workshops)

---

## 1. Workflow, Editors & Orchestration

- [UUPharmacometrics/PsN](https://github.com/UUPharmacometrics/PsN) `(Perl)` — Core CLI toolkit automating NONMEM workflows (bootstrapping, SCM, VPC, SIR).
- [metrumresearchgroup/bbi](https://github.com/metrumresearchgroup/bbi) `(Go)` — Cross-platform, scheduler-agnostic CLI execution engine for NONMEM runs (local, Slurm, SGE).
- [metrumresearchgroup/bbr](https://github.com/metrumresearchgroup/bbr) `(R)` — R package for NONMEM run management, model ancestry tracking, and reproducible run logs.
- [metrumresearchgroup/bbr.bayes](https://github.com/metrumresearchgroup/bbr.bayes) `(R)` — Extends `bbr` to manage, execute, and summarize Bayesian pharmacometric models using Stan and NONMEM.
- [metrumresearchgroup/nmrec](https://github.com/metrumresearchgroup/nmrec) `(R)` — Low-level R parser and serializer for programmatically reading and editing NONMEM control streams.
- [metrumresearchgroup/mrgvalidate](https://github.com/metrumresearchgroup/mrgvalidate) `(R)` — Automates regulatory software validation documentation (plans, traceability matrices, test summaries) for R packages.
- [metrumresearchgroup/pkgr](https://github.com/metrumresearchgroup/pkgr) `(Go)` — CLI dependency manager for installing and curating reproducible, isolated R package environments.
- [NMautoverse/NMsim](https://github.com/NMautoverse/NMsim) `(R)` — Seamless R interface to run NONMEM simulations directly from existing estimation control streams without manual edits.
- [nlmixr2/babelmixr2](https://github.com/nlmixr2/babelmixr2) `(R)` — Cross-engine bridge translating `nlmixr2`/`rxode2` models to NONMEM, Monolix, PKNCA, and PopED.
- [nlmixr2/nonmem2rx](https://github.com/nlmixr2/nonmem2rx) `(R/C)` — Parses and converts NONMEM control streams and outputs into `rxode2` or `nlmixr2` models.
- [nlmixr2/monolix2rx](https://github.com/nlmixr2/monolix2rx) `(R/C)` — Imports and translates Monolix `.mlxtran` models and results into `rxode2`/`nlmixr2` objects.
- [UUPharmacometrics/assemblerr](https://github.com/UUPharmacometrics/assemblerr) `(R)` — Programmatically constructs pharmacometric models from R building blocks and compiles them into NONMEM control streams.
- [certara/R-Certara](https://github.com/certara/R-Certara) `(R)` — Meta-package and installer unifying Certara's open-source pharmacometric R packages and Shiny apps.
- [certara/R-RsNLME-Examples](https://github.com/certara/R-RsNLME-Examples) `(R)` — Scriptable tidyverse-style R interface for running the Phoenix NLME estimation engine.
- [MarcLavielle/Rsmlx](https://github.com/MarcLavielle/Rsmlx) `(R)` — Automates Monolix model building, statistical covariate search, and convergence assessment from R.
- [tsahota/NMproject](https://github.com/tsahota/NMproject) `(R)` — Turns RStudio into an integrated, script-based NONMEM model development environment with piped workflows.
- [dpastoor/nonmemutils](https://github.com/dpastoor/nonmemutils) `(Go)` — Fast Go CLI utilities for parsing NONMEM `.lst` output files and managing run submissions.
- [Robterheine/nmgui2](https://github.com/Robterheine/nmgui2) `(Python/PyQt6)` — Cross-platform PyQt6 desktop GUI (Pirana alternative) for browsing, comparing, and running NONMEM + PsN workflows.
- [a2-ai/slurmtools](https://github.com/a2-ai/slurmtools) `(R)` — R utilities for submitting, monitoring, and managing Slurm HPC jobs directly from R.
- [billdenney/Pharmacometrics-Docker](https://github.com/billdenney/Pharmacometrics-Docker) `(Docker)` — Community Dockerfiles for reproducible multi-version NONMEM and PsN deployments.
- [kinginsun/nonmem](https://github.com/kinginsun/nonmem) `(Docker/Shell)` — Cross-platform Docker setup and wrapper scripts for NONMEM, PsN, and MPICH parallel execution.
- [FelicienLL/runnonmem](https://github.com/FelicienLL/runnonmem) `(R)` — Lightweight R wrapper for invoking NONMEM directly from R scripts.
- [s0521/nonmem_cn](https://github.com/s0521/nonmem_cn) `(TS | Chinese)` — VS Code extension for NONMEM control files with syntax highlighting, snippets, and bilingual CN/EN tooltips.
- [vrognas/vrognas-nmtran](https://github.com/vrognas/vrognas-nmtran) `(TS)` — VS Code extension delivering language intelligence, diagnostics, and hover docs for NMTRAN/NONMEM.
- [UUPharmacometrics/vim-nonmem](https://github.com/UUPharmacometrics/vim-nonmem) `(Vim)` — Dedicated Vim/Neovim syntax highlighting plugin for editing NONMEM control streams.
- [nmusers/nm-mode](https://github.com/nmusers/nm-mode) `(Emacs Lisp)` — Minimalist Emacs major mode providing syntax highlighting and editing support for NONMEM.
- [TingjieGuo/MINGA](https://github.com/TingjieGuo/MINGA) `(Hugo/Shell | Chinese)` — Chinese-language installation guide and shell scripts for NONMEM, PsN, Pirana, and R PMx tools.
- [Slow-Walker66/PPK-workbench-assistance-demo](https://github.com/Slow-Walker66/PPK-workbench-assistance-demo) `(TS | CN/EN)` — Local-first PopPK workbench (Pirana alternative) for NONMEM+PsN with model lineage, diagnostics, and reporting.

---

## 2. Open-Source NLME & ODE Engines

- [nlmixr2/nlmixr2](https://github.com/nlmixr2/nlmixr2) `(R/C++)` — Open-source R framework for population PK/PD NLME modeling (FOCE-I, SAEM, nlme).
- [nlmixr2/rxode2](https://github.com/nlmixr2/rxode2) `(R/C/C++)` — High-speed C-compiled ODE solver and clinical trial simulator with NONMEM-style event tables.
- [nlmixr2/nlmixr2lib](https://github.com/nlmixr2/nlmixr2lib) `(R)` — Curated library of published clinical PopPK/PD and biologics/TMDD models for `nlmixr2` and `rxode2`.
- [nlmixr2/nlmixr2extra](https://github.com/nlmixr2/nlmixr2extra) `(R)` — Adds bootstrapping, stepwise covariate selection, and preconditioned fits to `nlmixr2`.
- [nlmixr2/lotri](https://github.com/nlmixr2/lotri) `(R/C)` — Concise DSL for specifying lower-triangular block covariance matrices (IIV/IOV) in `nlmixr2` and `rxode2`.
- [metrumresearchgroup/mrgsolve](https://github.com/metrumresearchgroup/mrgsolve) `(R/C++)` — Fast C++-compiled hierarchical ODE simulator in R with NONMEM-inspired syntax for PopPK/PBPK/QSP.
- [mrgsolve/depot](https://github.com/mrgsolve/depot) `(R/C++)` — Official companion repository of ready-to-run `mrgsolve` ODE templates including TMDD and PBPK models.
- [kylebaron/mrgsim.parallel](https://github.com/kylebaron/mrgsim.parallel) `(R)` — Accelerates large-scale `mrgsolve` simulations via chunked parallel execution with `parallel` or `future`.
- [metrumresearchgroup/mrgsim.ds](https://github.com/metrumresearchgroup/mrgsim.ds) `(R)` — Stores `mrgsolve` simulation outputs in Apache Arrow datasets to reduce memory overhead at scale.
- [InsightRX/PKPDsim](https://github.com/InsightRX/PKPDsim) `(R/C++)` — Compiled C++ ODE and analytical PK/PD simulator tailored for clinical precision dosing.
- [john-harrold/ubiquity](https://github.com/john-harrold/ubiquity) `(R)` — End-to-end R modeling framework generating simulations, estimates, Word/PPT reports, and Shiny apps.
- [pharmpy/pharmpy](https://github.com/pharmpy/pharmpy) `(Python)` — Python pharmacometrics library and Automated Model Development (AMD) tool across NONMEM and `nlmixr2`.
- [pharmpy/pharmr](https://github.com/pharmpy/pharmr) `(R)` — Official R wrapper around Pharmpy for automated model development and control-stream manipulation.
- [metrumresearchgroup/Torsten](https://github.com/metrumresearchgroup/Torsten) `(C++/Stan)` — Stan extension library providing pharmacometric compartmental/ODE solvers and NMTRAN events for Bayesian PopPK/PD.
- [iame-researchCenter/saemix](https://github.com/iame-researchCenter/saemix) `(R)` — Open-source R implementation of the SAEM algorithm for NLME population PK/PD modeling.
- [MarcLavielle/mlxR](https://github.com/MarcLavielle/mlxR) `(R)` — Longitudinal PopPK/PD simulation and visualization package interfacing with Monolix/Simulx.
- [LAPKB/Pmetrics](https://github.com/LAPKB/Pmetrics) `(R/Rust)` — Non-parametric and parametric PopPK/PD modeling and Bayesian dosing engine powered by Rust.
- [LAPKB/pharmsol](https://github.com/LAPKB/pharmsol) `(Rust)` — High-performance Rust library for PK/PD analytical/ODE/SDE simulation, NCA, and model DSLs.
- [LAPKB/PMcore](https://github.com/LAPKB/PMcore) `(Rust)` — Core Rust computational engine implementing non-parametric PopPK estimation algorithms (NPAG, NPOD, NPSA).
- [FeRx-NLME/ferx-core](https://github.com/FeRx-NLME/ferx-core) `(Rust)` — Open-source Rust NLME engine supporting FOCE/FOCEI, SAEM, importance sampling, and a `.ferx` DSL.
- [DavAug/chi](https://github.com/DavAug/chi) `(Python)` — Native Python framework for mechanistic ODE PK/PD, QSP, and hierarchical Bayesian MIPD inference.
- [MSDLLCpapers/cpk](https://github.com/MSDLLCpapers/cpk) `(Python)` — Nonlinear regression for 1- and 2-compartment IV/extravascular PK with AICc model selection and outlier detection.
- [gumgo91/PKPy](https://github.com/gumgo91/PKPy) `(Python)` — Automated Python PopPK framework with parameter initialization, 1-/2-compartment models, NCA, and GOF.
- [orlacchioresearch/pharmacokinetics-pkpd-toolkit](https://github.com/orlacchioresearch/pharmacokinetics-pkpd-toolkit) `(Python)` — Lightweight NumPy-only PK/PD toolkit for NCA, 1-compartment IV/oral fitting, and Emax modeling.
- [Down-To-Programme/PK_Model](https://github.com/Down-To-Programme/PK_Model) `(Python)` — Pip-installable compartmental PK library (`dtp-pkmodel`) with SciPy ODE solving and comparative plotting.
- [blakeaw/pysb-pkpd](https://github.com/blakeaw/pysb-pkpd) `(Python)` — Extends PySB rule-based modeling with domain macros for 1-, 2-, and 3-compartment PK/PD models.
- [shramish2057/NeoPKPD](https://github.com/shramish2057/NeoPKPD) `(Julia/Python)` — Multi-language (Julia core + Python API/CLI) platform for PK/PD simulation, NLME, NCA, and BE.
- [manuhuth/NoLimits.jl](https://github.com/manuhuth/NoLimits.jl) `(Julia)` — Open-source Julia NLME framework combining mechanistic ODEs, Markov models, Neural ODEs, and VPCs.
- [wahlquisty/FastPKSim.jl](https://github.com/wahlquisty/FastPKSim.jl) `(Julia)` — Lightweight, high-speed Julia simulator for multi-compartment PK under infusions and bolus dosing.
- [simkaryote/gPKPDSim](https://github.com/simkaryote/gPKPDSim) `(MATLAB)` — Open-source MATLAB SimBiology GUI app for PK/PD simulation, parameter scanning, fitting, and NCA.
- [benjaminrich/linpk](https://github.com/benjaminrich/linpk) `(R)` — Analytically simulates linear compartmental PK profiles and computes exact $C_{\max}$, $T_{\max}$, AUC, and $t_{1/2}$.
- [liucann/PKparmas1.0](https://github.com/liucann/PKparmas1.0) `(Python/Streamlit | Chinese)` — Lightweight Chinese Streamlit web app for interactive compartmental PK parameter fitting from Excel data.
- [peytoncchen/PK-Visualization](https://github.com/peytoncchen/PK-Visualization) `(JS/Wasm)` — Browser-based compartmental PK modeling and visualization app powered by WebAssembly (Pyodide).
- [SnowLeopard-io/ErgalicsStudio](https://github.com/SnowLeopard-io/ErgalicsStudio) `(TS/WebGPU | CN/EN)` — Browser-based WebGPU/Wasm scientific studio with built-in PK compartmental, DDI, and TDM simulation plugins.

---

## 3. Data Preparation, CDISC & QC

- [NMautoverse/NMdata](https://github.com/NMautoverse/NMdata) `(R)` — End-to-end NONMEM dataset prep, structural QC (`NMcheckData`), exclusion tracking, and output merging.
- [NMautoverse/NMcalc](https://github.com/NMautoverse/NMcalc) `(R)` — Lightweight essential pharmacometric calculations (trapezoidal AUC, CV%) for exploratory and simulation summaries.
- [metrumresearchgroup/mrgda](https://github.com/metrumresearchgroup/mrgda) `(R)` — Data assembly toolkit for consolidating clinical trial domains into modeling-ready PMx datasets.
- [metrumresearchgroup/yspec](https://github.com/metrumresearchgroup/yspec) `(R)` — YAML-based PMx dataset specification manager for automated validation, labeling, and `define.pdf` generation.
- [metrumresearchgroup/lastdose](https://github.com/metrumresearchgroup/lastdose) `(R/C++)` — Rapidly computes time after last dose (TAD) and most-recent dose amount across complex dosing records.
- [pharmaverse/admiral](https://github.com/pharmaverse/admiral) `(R)` — Modular pharmaverse toolbox for building CDISC ADaM datasets including `ADPC`, `ADPP`, and `ADPPK`.
- [kestrel99/pmxTools](https://github.com/kestrel99/pmxTools) `(R)` — Practical R utility suite for PMx data manipulation, closed-form PK math, and PsN output parsing.

---

## 4. NCA, Bioequivalence, IVIVC & Dissolution

- [humanpred/pknca](https://github.com/humanpred/pknca) `(R)` — Comprehensive R engine for dense and sparse NCA with unit conversion, imputation, and CDISC support.
- [pharmaverse/aNCA](https://github.com/pharmaverse/aNCA) `(R/Shiny)` — Interactive pharmaverse Shiny app for clinical NCA with visual $\lambda_z$ selection and reproducible R script export.
- [asancpt/NonCompart](https://github.com/asancpt/NonCompart) `(R | Korea)` — Industrial-strength R NCA package aligned with Phoenix WinNonlin formulas and CDISC SDTM conventions.
- [asancpt/ncar](https://github.com/asancpt/ncar) `(R | Korea)` — Regulatory-style PDF and RTF NCA report generator built on top of `NonCompart`.
- [asancpt/pkrshiny](https://github.com/asancpt/pkrshiny) `(R/Shiny | KR/EN)` — No-code interactive Shiny web interface for running noncompartmental PK analysis.
- [asancpt/BE](https://github.com/asancpt/BE) `(R | Korea)` — Bioequivalence statistical analysis and sample size estimation across crossover designs replicating SAS PROC GLM/MIXED.
- [asancpt/BE-apps](https://github.com/asancpt/BE-apps) `(R/Shiny | KR/EN)` — Interactive Shiny application integrating PK noncompartmental analysis with bioequivalence statistics.
- [cran/bear](https://github.com/cran/bear) `(R)` — Average bioequivalence (ABE) and comparative bioavailability statistical analysis for crossover and parallel designs.
- [Detlew/PowerTOST](https://github.com/Detlew/PowerTOST) `(R | DE/AT)` — Industry-standard R package for bioequivalence power and sample size calculations (TOST, RSABE, ABEL).
- [Helmut01/replicateBE](https://github.com/Helmut01/replicateBE) `(R)` — EMA-aligned ABEL bioequivalence evaluation package for replicate crossover designs of highly variable drugs.
- [juntotechnologies/bioeq](https://github.com/juntotechnologies/bioeq) `(Python)` — Pure-Python package for pharmacokinetic data processing and crossover/parallel bioequivalence statistics.
- [PharmCat/MetidaNCA.jl](https://github.com/PharmCat/MetidaNCA.jl) `(Julia)` — High-performance Julia NCA library suited for drug development and large-scale trial simulation post-processing.
- [PharmCat/MetidaBioeq.jl](https://github.com/PharmCat/MetidaBioeq.jl) `(Julia)` — Julia package for regulatory bioequivalence assessment using mixed-effects and generalized linear models.
- [matthiaskoenig/pkpdutils](https://github.com/matthiaskoenig/pkpdutils) `(Python | Germany)` — Pure-Python PK/PD analysis library supporting unit-aware NCA, NONMEM/ADNCA I/O, curve fitting, BE, and DDI.
- [Open-Systems-Pharmacology/IVIVC-with-particle-dissolution-module-in-OSP](https://github.com/Open-Systems-Pharmacology/IVIVC-with-particle-dissolution-module-in-OSP) `(R/PK-Sim)` — Mechanistic PBPK-based IVIVC workflow linking particle size distribution and dissolution kinetics to *in vivo* oral PK.
- [cran/Rivivc](https://github.com/cran/Rivivc) `(R)` — Performs Linear Level A IVIVC via numerical deconvolution and convolution handling unequal time grids.
- [vkaralis/ivivs-be](https://github.com/vkaralis/ivivs-be) `(Python)` — Python IVIVS framework combining GI dissolution, compartmental PK ODEs, and Monte Carlo trials to predict BE.
- [zhengguoxu/bootf2](https://github.com/zhengguoxu/bootf2) `(R)` — FDA/EMA-aligned dissolution profile comparison using similarity factor ($f_2$) and bootstrap $f_2$ 90% CIs.
- [piusdahinden/disprofas](https://github.com/piusdahinden/disprofas) `(R)` — Non-parametric dissolution profile similarity testing including $f_1$, $f_2$, bootstrap $f_2$, MCR, and $T^2$ tests.
- [Shipbuilder/Bioequivalence](https://github.com/Shipbuilder/Bioequivalence) `(Scripts | Chinese)` — Chinese-language statistical reference scripts for bioequivalence studies.

---

## 5. Diagnostics, Visualization & Automated Reporting

- [UUPharmacometrics/xpose](https://github.com/UUPharmacometrics/xpose) `(R)` — Modern `ggplot2`-based diagnostics framework for NONMEM/NLME goodness-of-fit and VPC plots.
- [UUPharmacometrics/xpose4](https://github.com/UUPharmacometrics/xpose4) `(R)` — Classic NONMEM model-building aid providing lattice-based GOF diagnostics, VPCs, and covariate screening plots.
- [nlmixr2/xpose.nlmixr2](https://github.com/nlmixr2/xpose.nlmixr2) `(R)` — Bridges `nlmixr2` fit objects into standard `xpose` databases (`xpdb`) for GOF diagnostics.
- [nlmixr2/nlmixr2plot](https://github.com/nlmixr2/nlmixr2plot) `(R)` — Native `ggplot2`-based diagnostic and visual predictive check plotting routines for `nlmixr2`.
- [ggPMXdevelopment/ggPMX](https://github.com/ggPMXdevelopment/ggPMX) `(R)` — Standardized ISoP-aligned GOF diagnostic plotting and reporting across Monolix, NONMEM, and `nlmixr2`.
- [metrumresearchgroup/pmplots](https://github.com/metrumresearchgroup/pmplots) `(R)` — Standardized, publication-ready exploratory and goodness-of-fit diagnostic plots for pharmacometrics.
- [certara/tidyvpc](https://github.com/certara/tidyvpc) `(R)` — Fast `data.table`-backed VPC engine supporting binned/binless (AQR/LOESS) VPCs, pcVPC, and BLQ censoring.
- [ronkeizer/vpc](https://github.com/ronkeizer/vpc) `(R)` — Flexible R package for continuous, categorical, and time-to-event Visual Predictive Checks across platforms.
- [UUPharmacometrics/ncappc](https://github.com/UUPharmacometrics/ncappc) `(R)` — Simulation-based posterior predictive check (PPC) evaluating PopPK/PD models via NCA exposure metrics.
- [pharmetheus/PMXForest](https://github.com/pharmetheus/PMXForest) `(R)` — Automated covariate forest plots with uncertainty directly from NONMEM `.cov`, PsN bootstrap, or SIR outputs.
- [metrumresearchgroup/pmforest](https://github.com/metrumresearchgroup/pmforest) `(R)` — Generates customizable covariate effect forest plots directly from model parameters and `mrgsolve` simulations.
- [certara/coveffectsplot](https://github.com/certara/coveffectsplot) `(R/Shiny)` — R package and Shiny app for producing standardized covariate-effect forest plots in PopPK/PD reports (see also [smouksassi/coveffectsplot](https://github.com/smouksassi/coveffectsplot)).
- [Novartis/xgxr](https://github.com/Novartis/xgxr) `(R)` — Novartis exploratory graphics (`ggplot2`) helpers for reproducible PK/PD and exposure-response plotting.
- [metrumresearchgroup/pmtables](https://github.com/metrumresearchgroup/pmtables) `(R)` — Publication- and submission-grade LaTeX summary table generator tailored for pharmacometric reports.
- [certara/pmxpartabc](https://github.com/certara/pmxpartabc) `(R)` — Parses NONMEM run directories and YAML specs to generate clean, report-ready parameter estimate tables.
- [NMautoverse/tracee](https://github.com/NMautoverse/tracee) `(R)` — Automates saving plots and tables with embedded source-script paths and timestamps for regulatory traceability.
- [kylebaron/mrgsim.sa](https://github.com/kylebaron/mrgsim.sa) `(R)` — Local and graphical parameter sensitivity analysis extension for `mrgsolve` PK/PD and QSP models.
- [nlmixr2/nlmixr2rpt](https://github.com/nlmixr2/nlmixr2rpt) `(R)` — YAML-driven automated Microsoft Word and PowerPoint report generator for `nlmixr2` model fits.
- [john-harrold/ruminate](https://github.com/john-harrold/ruminate) `(R/Shiny)` — Modular Shiny PMx workbench combining data wrangling, PKNCA, `rxode2` simulation, and Word/PPT/Excel reporting.
- [Genentech/gPKPDviz](https://github.com/Genentech/gPKPDviz) `(R/Shiny)` — Interactive `mrgsolve`-powered Shiny platform for real-time PopPK/PD simulation and virtual population exploration.
- [Boehringer-Ingelheim/MVPapp](https://github.com/Boehringer-Ingelheim/MVPapp) `(R/Shiny | Germany)` — Model Visualization Platform (Shiny) with live `mrgsolve` editing, NCA, sensitivity analysis, and NHANES demographics.
- [pipetcpt/2025-jscpt](https://github.com/pipetcpt/2025-jscpt) `(R/NONMEM | KR/JP)` — Automated publication-grade pharmacometric infographic generator from NONMEM IRT model outputs.

---

## 6. Regulatory ClinPharm, C-QTc, Dose-Finding, E-R & FIH

- [FDA/PKView](https://github.com/FDA/PKView) `(R/Shiny)` — U.S. FDA interactive clinical pharmacology review app ingesting CDISC SDTM/ADaM data for automated PK/safety reviews.
- [A2-ai/cqtkit](https://github.com/A2-ai/cqtkit) `(R)` — Streamlines Garnett white-paper Concentration-QTc (C-QTc) modeling: preprocessing, EDA, LME fitting, and diagnostics.
- [joannaparkinson/C-QTc-hands-on-tutorial](https://github.com/joannaparkinson/C-QTc-hands-on-tutorial) `(R)` — Reproducible hands-on C-QTc analysis tutorial implementing Garnett white-paper LME modeling and ΔΔQTc predictions.
- [FDA/CiPA](https://github.com/FDA/CiPA) `(R)` — Official U.S. FDA CiPA *in silico* cardiac safety suite for hERG kinetics, Bayesian Hill MCMC, and action potential simulations.
- [Novartis/OncoBayes2](https://github.com/Novartis/OncoBayes2) `(R/Stan)` — Bayesian Logistic Regression Models (BLRM) with EXNEX borrowing and EWOC for single/combination Phase I escalation.
- [openpharma/crmPack](https://github.com/openpharma/crmPack) `(R)` — Object-oriented framework for model-based Phase I dose-escalation including CRM, BLRM, and dual-endpoint designs.
- [brockk/escalation](https://github.com/brockk/escalation) `(R)` — Modular grammar to specify, chain stopping rules, and simulate BOIN, mTPI-2, CRM, and TITE-CRM dose-finding designs.
- [openpharma/DoseFinding](https://github.com/openpharma/DoseFinding) `(R/C)` — Regulatory-endorsed MCP-Mod methodology for planning, optimal design, and dose-response analysis in Phase II trials.
- [cran/BOIN](https://github.com/cran/BOIN) `(R)` — Bayesian Optimal Interval (BOIN) design for single-agent and combination Phase I trials under Project Optimus.
- [yamagubed/boinet](https://github.com/yamagubed/boinet) `(R)` — Model-assisted Phase I/II BOIN-ET designs jointly optimizing efficacy and toxicity to identify Optimal Biological Dose.
- [brockk/trialr](https://github.com/brockk/trialr) `(R/Stan)` — Collection of Bayesian clinical trial designs in RStan including CRM, TITE-CRM, and EffTox seamless Phase I/II.
- [mikesweeting/bcrm](https://github.com/mikesweeting/bcrm) `(R)` — One- and two-parameter Bayesian Continual Reassessment Method (CRM) designs and operating-characteristic simulations.
- [cran/dfcrm](https://github.com/cran/dfcrm) `(R)` — Foundational R package for Phase I dose-finding via CRM and Time-to-Event CRM (TITE-CRM).
- [cran/clinDR](https://github.com/cran/clinDR) `(R)` — Bayesian and maximum-likelihood Emax dose-response modeling tools tailored for Phase II dose-ranging analyses.
- [Genentech/BayesERtools](https://github.com/Genentech/BayesERtools) `(R/Stan)` — Bayesian exposure-response modeling toolkit over Stan for binary/continuous endpoints and decision forest plots.
- [metrumresearchgroup/confounded-exposure-metrics](https://github.com/metrumresearchgroup/confounded-exposure-metrics) `(R/NONMEM)` — Methodological simulation pipeline demonstrating exposure-metric confounding bias in oncology E-R and TTE analyses.
- [clay-good/onkos](https://github.com/clay-good/onkos) `(Python)` — Curated oncology TGI and E-R model library with transpilation to NONMEM, SBML, `rxode2`, and Pumas.
- [orlacchioresearch/tumor-growth-inhibition-modeling](https://github.com/orlacchioresearch/tumor-growth-inhibition-modeling) `(Python)` — Python toolkit for preclinical xenograft tumor growth curve fitting and TGI% / %T/C calculation.
- [campsisverse/campsis](https://github.com/campsisverse/campsis) `(R)` — Engine-agnostic clinical trial simulation (CTS) platform supporting both `rxode2` and `mrgsolve` backends.
- [andrewhooker/PopED](https://github.com/andrewhooker/PopED) `(R)` — Optimal experimental design for NLME models using the Fisher Information Matrix (FIM) to optimize sampling and dosing.
- [iame-researchCenter/PFIM](https://github.com/iame-researchCenter/PFIM) `(R | France)` — Population FIM optimal design package supporting covariates, IOV, and Fedorov-Wynn/PSO optimization.
- [phuse-org/toxSummary](https://github.com/phuse-org/toxSummary) `(R/Shiny)` — PHUSE Shiny app summarizing repeat-dose tox exposure margins and cross-species translation for FIH dose justification.
- [pipetcpt/DallphinAtoM](https://github.com/pipetcpt/DallphinAtoM) `(R | KR/EN)` — Allometric scaling and physiological animal-to-human PK parameter prediction tool for early FIH projection.
- [m-amanda/Analytical-Methods-Validation-with-R](https://github.com/m-amanda/Analytical-Methods-Validation-with-R) `(R/Shiny)` — Interactive Shiny app for bioanalytical method validation covering selectivity, linearity, homoscedasticity, and LOD/LOQ.
- [giovannisolarino/Methods-Validation-App-Web](https://github.com/giovannisolarino/Methods-Validation-App-Web) `(Python)` — Python web app for regulated bioanalytical labs to evaluate multi-day LC-MS calibration curves and validation metrics.

---

## 7. Clinical MIPD, TDM, Antimicrobial PTA & TCI

### 7.1 General MIPD Engines & Validation

- [sotalya/tucuxi-core](https://github.com/sotalya/tucuxi-core) `(C++ | CH/FR)` — Hospital-validated open-source Bayesian TDM/MIPD computing engine with CLI and REST server.
- [sotalya/tucuxi-gui](https://github.com/sotalya/tucuxi-gui) `(C++/Qt | CH/FR)` — Clinical desktop GUI for interpreting drug concentrations and computing individualized dosage adaptations via Tucuxi.
- [sotalya/tucuxi-drugs](https://github.com/sotalya/tucuxi-drugs) `(XML | CH/FR)` — Open XML repository of population PK drug models for narrow-therapeutic-index drugs used by Tucuxi.
- [sotalya/tucuxi-python](https://github.com/sotalya/tucuxi-python) `(Python/C++ | CH/FR)` — Python bindings for `tucuxi-core` enabling scripted PK predictions and batch retrospective TDM evaluation.
- [levenc/posologyr](https://github.com/levenc/posologyr) `(R | France)` — `rxode2`-based MIPD package for MAP-Bayesian estimation and target AUC/trough dose optimization.
- [FelicienLL/mapbayr](https://github.com/FelicienLL/mapbayr) `(R | France)` — Lightweight, fast MAP-Bayesian estimation engine built on `mrgsolve` PopPK models for clinical TDM.
- [FelicienLL/mapbayr-shiny](https://github.com/FelicienLL/mapbayr-shiny) `(R/Shiny | France)` — Ready-to-deploy R Shiny application templates for building `mapbayr`-powered Bayesian TDM calculators.
- [InsightRX/PKPDmap](https://github.com/InsightRX/PKPDmap) `(R)` — Modular MAP-Bayesian parameter estimation engine operating directly on `PKPDsim` models.
- [InsightRX/PKPDposterior](https://github.com/InsightRX/PKPDposterior) `(R/Stan)` — Full-Bayesian MCMC inference via Stan/Torsten quantifying posterior uncertainty in individualized dosing predictions.
- [InsightRX/clinPK](https://github.com/InsightRX/clinPK) `(R)` — Standardized clinical pharmacology equations for renal function, body weight descriptors, and basic PK math.
- [InsightRX/mipdeval](https://github.com/InsightRX/mipdeval) `(R)` — Evaluates predictive accuracy and bias of population PK/PD models on historical TDM datasets under Bayesian forecasting.
- [InsightRX/mipdtrial](https://github.com/InsightRX/mipdtrial) `(R)` — Simulates clinical PK/PD endpoints and target attainment metrics under adaptive MIPD trial protocols.
- [Martin-Umpierrez/exeval](https://github.com/Martin-Umpierrez/exeval) `(R)` — Reproducible external evaluation framework for benchmarking published PopPK/PD models on local hospital TDM cohorts.

### 7.2 Antimicrobial PK/PD, PTA/CFR & TDM

- [liangRXdev/vanco-auc-calc](https://github.com/liangRXdev/vanco-auc-calc) `(JS/PWA | ZH-TW/EN)` — Offline browser PWA for vancomycin AUC dosing with Sawchuk-Zaske, 2-compartment Bayesian MAP, and clinical alerts.
- [asancpt/shiny-vtdm](https://github.com/asancpt/shiny-vtdm) `(R/Shiny | KR/EN)` — Korean vancomycin TDM Shiny app implementing a 2-compartment PopPK Bayesian dosing model.
- [pipetcpt/tdm-vancomycin](https://github.com/pipetcpt/tdm-vancomycin) `(R/Shiny | KR/EN)` — Open-source Shiny app for vancomycin PopPK dosing simulation and TDM automation.
- [kpessa/vanco-auc](https://github.com/kpessa/vanco-auc) `(Excel/VBA)` — Hospital-deployed Excel/VBA toolkit for vancomycin empirical dosing and paired-level trapezoidal AUC24/MIC.
- [njrhodes/bds-app](https://github.com/njrhodes/bds-app) `(R/Shiny/Stan)` — Shiny-based Bayesian Dosing Simulator monorepo featuring meropenem and piperacillin-tazobactam MIPD modules.
- [cptbern/ShinyFlucloxacillin](https://github.com/cptbern/ShinyFlucloxacillin) `(R/Shiny | Switzerland)` — Interactive clinical TDM/MIPD Shiny web app (University of Bern) for personalized flucloxacillin dosing.
- [piranfar/caz-avi-evidence-composite-pkpd](https://github.com/piranfar/caz-avi-evidence-composite-pkpd) `(R/Python)` — Reproducible Monte Carlo PK/PD simulation workflow evaluating joint PTA and CFR for ceftazidime-avibactam.
- [shemtsai/Aminoglycoside-Calculator](https://github.com/shemtsai/Aminoglycoside-Calculator) `(HTML/JS)` — Lightweight browser-based non-trapezoidal aminoglycoside pharmacokinetic dosing calculator by an ID pharmacist.
- [joshcase/code-blue-gentamicin](https://github.com/joshcase/code-blue-gentamicin) `(Python/Web)` — Educational gentamicin dosing calculator demonstrating clinical pharmacokinetic dosing rules and safety checks.
- [727397883/Rifampicin-PopPK-Repository](https://github.com/727397883/Rifampicin-PopPK-Repository) `(R/Shiny | China)` — Open-source rifampicin PopPK model repository and interactive `mrgsolve` Shiny dosing simulator.
- [HassDhia/antibiosim](https://github.com/HassDhia/antibiosim) `(Python)` — Gymnasium-compatible simulation environments modeling antibiotic PK/PD target attainment and bacterial dynamics.

### 7.3 Immunosuppressant, NTI & Hospital Calculators

- [FelicienLL/BUSULFANAPP](https://github.com/FelicienLL/BUSULFANAPP) `(R/Shiny | France)` — `mapbayr`-powered Shiny application for model-informed precision dosing of busulfan in pediatric HSCT patients.
- [wojjy001/infliximab-bayes](https://github.com/wojjy001/infliximab-bayes) `(R)` — Bayesian forecasting and adaptive dosing simulation for infliximab maintenance therapy in IBD (see also [wojjy001/adaptive-infliximab](https://github.com/wojjy001/adaptive-infliximab)).
- [abusuraihsakhri/digoxin-therapeutic-level-estimator](https://github.com/abusuraihsakhri/digoxin-therapeutic-level-estimator) `(HTML/JS)` — Estimates digoxin plasma concentrations and therapeutic-range status from physiological variables and dosing history.
- [pharmot/multipurpose-calculator](https://github.com/pharmot/multipurpose-calculator) `(HTML/JS)` — Comprehensive hospital pharmacy calculator suite covering vancomycin AUC, aminoglycosides, phenytoin, heparin, and NICU TPN.
- [jeremy-steinberg/Paediatric-Dosing](https://github.com/jeremy-steinberg/Paediatric-Dosing) `(JS/HTML5)` — Zero-dependency client-side pediatric weight-based dosing calculator (mg and mL) based on NZF guidelines.
- [stalex444/CRRT_simulator](https://github.com/stalex444/CRRT_simulator) `(HTML/JS)` — Interactive ICU CRRT training simulator with real-time filtration fraction monitoring and integrated drug dosing calculator.
- [Londopy/Clinical_IQ](https://github.com/Londopy/Clinical_IQ) `(TS/Python)` — Full-stack clinical decision support web app bundling renal-adjusted weight dosing and IV infusion rate calculators.
- [cloveropen/pass](https://github.com/cloveropen/pass) `(Web | Chinese)` — Open-source clinical prescription automatic screening system (PASS) with tiered alerts and DDI checks.
- [yusuketakuma/pharma-free-tools](https://github.com/yusuketakuma/pharma-free-tools) `(HTML/JS | Japanese)` — Collection of ~24 browser-based clinical pharmacy tools for Japanese pharmacists including renal dosing calculators.
- [koikelab/medication_eq_R](https://github.com/koikelab/medication_eq_R) `(R | JP/EN)` — Automated calculation of psychotropic medication equivalent doses using Japanese psychiatric standards.
- [teezeit/medication-calculator](https://github.com/teezeit/medication-calculator) `(TS/React | Germany)` — Client-side SPA for bi-exponential pharmacokinetic calculations and Plotly multi-regimen curve comparisons.

### 7.4 Anesthesia TCI, Opioid Rescue & Glucose-Insulin PK/PD

- [vitaldb/tivatci](https://github.com/vitaldb/tivatci) `(Python | Korea)` — Open-source Python library for TIVA/TCI PK/PD modeling (Schnider, Marsh, Minto, Eleveld, Gepts) and LBM formulas.
- [luktinghin/simtiva](https://github.com/luktinghin/simtiva) `(JS/PWA)` — Offline PWA simulating TCI/TIVA for propofol and remifentanil with dual-drug PD interaction modeling.
- [BobAubouin/Python_Anesthesia_Simulator](https://github.com/BobAubouin/Python_Anesthesia_Simulator) `(Python)` — Multi-drug anesthesia PK/PD simulator (BIS, MAP, cardiac output) serving as a benchmark for closed-loop/RL control.
- [ManuMerlo/AReS-Anesthesia-Response-Simulator](https://github.com/ManuMerlo/AReS-Anesthesia-Response-Simulator) `(Python/MATLAB)` — Comprehensive TIVA patient response simulator modeling 4 drugs, TCI pumps, surgical stress, and fluid dynamics.
- [jarretrt/tci](https://github.com/jarretrt/tci) `(R)` — Implements TCI infusion-rate algorithms and closed-loop Bayesian updating for propofol and remifentanil PK/PD.
- [fra-mar/tci_simulator](https://github.com/fra-mar/tci_simulator) `(Python)` — Python multi-compartment PK simulator computing TCI pump infusion rates and plasma vs. effect-site curves.
- [seazuma/pkpd](https://github.com/seazuma/pkpd) `(JS/HTML | JP/EN)` — Offline browser-based 3-compartment anesthetic PK/PD and TCI simulator with variability bands and BIS prediction.
- [ysuzuki1978/rocuronium-pkpd-simulator](https://github.com/ysuzuki1978/rocuronium-pkpd-simulator) `(JS/PWA | JP/EN)` — Offline PWA simulating rocuronium PK and neuromuscular blockade (TOF) across 5 validated clinical models.
- [ysuzuki1978/remimazolam-tci-simulator](https://github.com/ysuzuki1978/remimazolam-tci-simulator) `(JS/HTML | JP/EN)` — Effect-site TCI simulator for remimazolam implementing the Masui (2022) PK model with CSV export.
- [ysuzuki1978/propofol-tci-simulator](https://github.com/ysuzuki1978/propofol-tci-simulator) `(JS/HTML | JP/EN)` — Interactive propofol effect-site TCI simulator built on the Eleveld (2018) PK/PD framework.
- [Clinical-Pharmacy-Saarland-University/pi_pumpsim](https://github.com/Clinical-Pharmacy-Saarland-University/pi_pumpsim) `(Python/Svelte | DE/EN)` — Interactive FastAPI + Svelte IV infusion pharmacokinetics simulation demo ("Dr. Dosis") with pump visualization.
- [FDA/Mechanistic-PK-PD-Model-to-Rescue-Opioid-Overdose](https://github.com/FDA/Mechanistic-PK-PD-Model-to-Rescue-Opioid-Overdose) `(R)` — U.S. FDA mechanistic PK/PD model simulating opioid-induced respiratory depression and naloxone rescue regimens.
- [practicefusion/mmecalculator](https://github.com/practicefusion/mmecalculator) `(C#)` — C# library and API parsing free-text prescription sigs to calculate maximum daily Morphine Milligram Equivalents (MME).
- [jxx123/simglucose](https://github.com/jxx123/simglucose) `(Python)` — Python implementation of the FDA-approved UVA/Padova Type 1 Diabetes glucose-insulin PK/PD simulator.
- [Perceptus/GlucoSym](https://github.com/Perceptus/GlucoSym) `(JS/Python)` — Simulates human glucose-insulin metabolic dynamics and insulin PK for closed-loop artificial pancreas testing.
- [1paulpo1/uva-padova-glucose-control-system](https://github.com/1paulpo1/uva-padova-glucose-control-system) `(C++/Python)` — Personalized UVA/Padova glucose-insulin PK/PD parameter identification and forecasting from CGM and pump logs.

### 7.5 Multi-Compartment Tracking & Dynamic Calibration

- [xingqimiao/Kira-HRT-Tracker](https://github.com/xingqimiao/Kira-HRT-Tracker) `(TS | CN/EN)` — Privacy-first PK tracker featuring 4 blood-level calibration estimators (MAP, EKF, OU-Kalman) and MCP integration.
- [LaoZhong-Mihari/HRT-Recorder-PKcomponent-Test](https://github.com/LaoZhong-Mihari/HRT-Recorder-PKcomponent-Test) `(Swift | CN/EN)` — Native Swift PK engine implementing 3-compartment, biphasic depot kinetics, and multi-route absorption models.
- [TransmtfTeam/Transmtf-HRT-Tracker](https://github.com/TransmtfTeam/Transmtf-HRT-Tracker) `(TS | CN/EN)` — Web PK tracker supporting flip-flop kinetics, 3-compartment cascade absorption, and Bayesian/EKF calibration.
- [meowhuan/Oyama-s-HRT-Tracker](https://github.com/meowhuan/Oyama-s-HRT-Tracker) `(TS | Multi-lingual)` — Multi-lingual local web simulator for real-time 3-compartment concentration-time curves and AUC visualization.
- [Trans-Prism/Trans-Prism](https://github.com/Trans-Prism/Trans-Prism) `(Flutter/JS | Chinese)` — Cross-platform Flutter offline toolkit with multi-compartment superposition PK curve simulation and dosing timeline.
- [WHSAH/estrannaise.js](https://github.com/WHSAH/estrannaise.js) `(JS)` — Client-side browser simulator for 3-compartment estradiol PK and Bayesian inference under arbitrary dosing regimens.

---

## 8. PBPK, IVIVE, DDI & Special Populations

- [Open-Systems-Pharmacology/PK-Sim](https://github.com/Open-Systems-Pharmacology/PK-Sim) `(C#/.NET | Germany)` — Flagship open-source whole-body PBPK modeling platform with adult, pediatric, and special-population physiology.
- [Open-Systems-Pharmacology/MoBi](https://github.com/Open-Systems-Pharmacology/MoBi) `(C#/.NET | Germany)` — Multiscale biosimulation and mechanistic QSP/PBPK tool complementing PK-Sim for custom reaction networks.
- [Open-Systems-Pharmacology/OSPSuite.Core](https://github.com/Open-Systems-Pharmacology/OSPSuite.Core) `(C#/.NET)` — Foundational core computational engine, data structures, and simulation kernel shared across the OSP Suite.
- [Open-Systems-Pharmacology/OSPSuite-R](https://github.com/Open-Systems-Pharmacology/OSPSuite-R) `(R/C++)` — Programmatic R interface for headless PK-Sim/MoBi batch simulations, parameter sweeps, and reporting.
- [Open-Systems-Pharmacology/Matlab-Toolbox](https://github.com/Open-Systems-Pharmacology/Matlab-Toolbox) `(MATLAB)` — Programmatic MATLAB interface for batch simulation and parameter identification of PK-Sim and MoBi models.
- [Open-Systems-Pharmacology/OSPSuite.ReportingEngine](https://github.com/Open-Systems-Pharmacology/OSPSuite.ReportingEngine) `(R)` — Automates standardized qualification workflows, diagnostics, and regulatory reports for OSP PBPK/QSP models.
- [Open-Systems-Pharmacology/OSPSuite.ParameterIdentification](https://github.com/Open-Systems-Pharmacology/OSPSuite.ParameterIdentification) `(R)` — Programmatic parameter estimation, optimization, and uncertainty analysis for PK-Sim and MoBi models.
- [Open-Systems-Pharmacology/TLF-Library](https://github.com/Open-Systems-Pharmacology/TLF-Library) `(R)` — Object-oriented R visualization framework (`tlf`) for standardized tables, listings, and qualification figures.
- [Open-Systems-Pharmacology/OSPSuite.RUtils](https://github.com/Open-Systems-Pharmacology/OSPSuite.RUtils) `(R)` — Shared utility package supplying validation, type-checking, and helper routines across OSP R packages.
- [Open-Systems-Pharmacology/OSP-PBPK-Model-Library](https://github.com/Open-Systems-Pharmacology/OSP-PBPK-Model-Library) `(PK-Sim/R)` — Peer-reviewed library of qualified open-source PBPK substance models and evaluation reports.
- [Open-Systems-Pharmacology/OSP-Qualification-Reports](https://github.com/Open-Systems-Pharmacology/OSP-Qualification-Reports) `(Markdown/R)` — Centralized repository auto-compiling platform-wide PBPK qualification reports (DDIs, pediatrics, transporters).
- [Open-Systems-Pharmacology/Qualification-DDI-CYP3A4](https://github.com/Open-Systems-Pharmacology/Qualification-DDI-CYP3A4) `(PK-Sim/R)` — Regulatory-grade PBPK qualification plan and datasets evaluating CYP3A4-mediated drug-drug interactions.
- [Open-Systems-Pharmacology/Pediatric_Qualification_Package_CYP3A4_Ontogeny](https://github.com/Open-Systems-Pharmacology/Pediatric_Qualification_Package_CYP3A4_Ontogeny) `(PK-Sim)` — Formal OSP qualification package validating pediatric scaling and CYP3A4 enzyme ontogeny from infants to adolescents.
- [Open-Systems-Pharmacology/Vancomycin-Model](https://github.com/Open-Systems-Pharmacology/Vancomycin-Model) `(PK-Sim/R)` — Whole-body PBPK model and evaluation report for vancomycin focusing on GFR-mediated renal clearance.
- [Open-Systems-Pharmacology/Voriconazole-Model](https://github.com/Open-Systems-Pharmacology/Voriconazole-Model) `(PK-Sim)` — Validated whole-body PBPK model of voriconazole capturing nonlinear metabolism and CYP2C19/CYP3A4 effects.
- [Open-Systems-Pharmacology/Voriconazole-Tacrolimus-DDGI](https://github.com/Open-Systems-Pharmacology/Voriconazole-Tacrolimus-DDGI) `(PK-Sim)` — Whole-body PBPK modeling of clinically critical drug-drug-gene interactions between voriconazole and tacrolimus.
- [Open-Systems-Pharmacology/Pregnancy-Models](https://github.com/Open-Systems-Pharmacology/Pregnancy-Models) `(PK-Sim/MoBi)` — Whole-body pregnancy PBPK framework incorporating gestational physiology and maternal-fetal placental transfer.
- [Open-Systems-Pharmacology/Lactation-PBPK-model](https://github.com/Open-Systems-Pharmacology/Lactation-PBPK-model) `(MoBi/SQLite)` — Lactation PBPK building blocks for simulating drug transfer into breast milk and infant systemic exposure.
- [Clinical-Pharmacy-Saarland-University/PBPK-Models](https://github.com/Clinical-Pharmacy-Saarland-University/PBPK-Models) `(PK-Sim/R | Germany)` — Peer-reviewed PBPK and DDI/DDGI model repository maintained by Saarland University.
- [Sanofi-Public/saemixPBPK](https://github.com/Sanofi-Public/saemixPBPK) `(R | France)` — Integrates SAEM NLME parameter estimation with OSP Suite whole-body PBPK/QSP models.
- [esqLABS/esqlabsR](https://github.com/esqLABS/esqlabsR) `(R)` — Standardized R workflow package managing multi-scenario OSP Suite PBPK/QSP projects via Excel templates.
- [certara/Simcyp-R-Scripts](https://github.com/certara/Simcyp-R-Scripts) `(R)` — Official Certara R scripts for programmatically controlling the Simcyp Simulator and parsing PBPK outputs.
- [mba16hk/Simcyp-R-Workflow](https://github.com/mba16hk/Simcyp-R-Workflow) `(R)` — High-throughput R workflow (`SimRFlow`) querying ChEMBL/PubChem properties for batch Simcyp PBPK runs.
- [USEPA/CompTox-ExpoCast-httk](https://github.com/USEPA/CompTox-ExpoCast-httk) `(R/C)` — High-throughput toxicokinetics (`httk`) package for generic PBPK modeling, partition coefficients, and IVIVE.
- [ScitoVation/plethem](https://github.com/ScitoVation/plethem) `(R/Shiny)` — Interactive Shiny platform (`PLETHEM`) integrating `httk` and `deSolve` for high-throughput PBPK, IVIVE, and reverse dosimetry.
- [metrumresearchgroup/PBPK_PC](https://github.com/metrumresearchgroup/PBPK_PC) `(R/mrgsolve)` — Implements and benchmarks tissue partition coefficient ($K_p$) methods (Rodgers & Rowland, Berezhkovskiy, etc.) in `mrgsolve`.
- [metrumresearchgroup/pbpk-qsp-mrgsolve](https://github.com/metrumresearchgroup/pbpk-qsp-mrgsolve) `(R/mrgsolve)` — Workshop repository providing hands-on `mrgsolve` code templates and case studies for whole-body PBPK and QSP.
- [metrumresearchgroup/cptpsp-tutorial-2019](https://github.com/metrumresearchgroup/cptpsp-tutorial-2019) `(R)` — Companion code for `mrgsolve` PBPK/QSP modeling including transparent Poulin & Theil $K_p$ calculation scripts.
- [metrumresearchgroup/BayesPBPK-tutorial](https://github.com/metrumresearchgroup/BayesPBPK-tutorial) `(Julia/Stan/R)` — Open-source Bayesian hierarchical PBPK modeling workflows using Julia (Turing.jl), Stan/Torsten, and R.
- [SystemsForecasting/ManchesterPBPK](https://github.com/SystemsForecasting/ManchesterPBPK) `(R)` — Open-source, code-first whole-body PBPK model (*PBPKedu*) written transparently in `rxode2`.
- [matthiaskoenig/sbmlsim](https://github.com/matthiaskoenig/sbmlsim) `(Python | Germany)` — Python simulation and reporting framework built on `libRoadRunner` for reproducible SBML PBPK models.
- [matthiaskoenig/glimepiride-model](https://github.com/matthiaskoenig/glimepiride-model) `(Python/SBML | Germany)` — Whole-body SBML PBPK model of glimepiride explicitly modeling renal impairment, cirrhosis, and CYP2C9 genetics.
- [matthiaskoenig/dapagliflozin-model](https://github.com/matthiaskoenig/dapagliflozin-model) `(Python/SBML | Germany)` — Coupled PBPK/PD SBML model of dapagliflozin evaluating hepatorenal impairment and urinary glucose excretion.
- [ahmedn12/oral-pbpk-model](https://github.com/ahmedn12/oral-pbpk-model) `(Python/R)` — Dual Python/R oral PBPK model capturing hepatic first-pass metabolism and protein-binding ($f_u$) sensitivity.
- [mathworks/Chemistry-Cheminformatics-Pharmacokinetics](https://github.com/mathworks/Chemistry-Cheminformatics-Pharmacokinetics) `(MATLAB/Python)` — Official MathWorks workflow bridging Python/RDKit descriptors with MATLAB SimBiology for oral absorption simulation.
- [qurit/PSMA-PBPK-Model-Matlab](https://github.com/qurit/PSMA-PBPK-Model-Matlab) `(MATLAB)` — MATLAB SimBiology/SBML whole-body PBPK model for PSMA-targeted radiopharmaceuticals.
- [pipetcpt/DallphinDDI](https://github.com/pipetcpt/DallphinDDI) `(R | KR/EN)` — Academic R-based physiological/PBPK modeling tool for simulating metabolic and transporter DDIs.

---

## 9. Biologics, TMDD, ADC, CAR-T, Immunogenicity & QSP

- [metrumresearchgroup/bioPBPK](https://github.com/metrumresearchgroup/bioPBPK) `(Julia/R)` — Code-first biologics/mAb whole-body PBPK models with FcRn recycling and lymphatics in Julia and R.
- [Open-Systems-Pharmacology/BAY794620-Model](https://github.com/Open-Systems-Pharmacology/BAY794620-Model) `(PK-Sim)` — Whole-body PBPK model for the antibody-drug conjugate (ADC) BAY-794620 capturing macromolecular disposition.
- [azelys/tce](https://github.com/azelys/tce) `(Julia/MATLAB)` — Mechanistic modeling of binding criteria, PK, identifiability, and optimal control for bispecific T-cell engagers (TCEs).
- [cosbi-research/PBPKmRNABiTE](https://github.com/cosbi-research/PBPKmRNABiTE) `(MATLAB | Italy)` — Multi-scale PBPK model for mRNA-encoded BiTE cancer therapy capturing trafficking, translation, and antibody PK.
- [cosbi-research/Campanile_et_al_PBPKmRNATherapeutics](https://github.com/cosbi-research/Campanile_et_al_PBPKmRNATherapeutics) `(MATLAB | Italy)` — SimBiology PBPK framework for lipid nanoparticle (LNP) delivery and mRNA-encoded antibody therapeutics.
- [RomanCohort/confluencia](https://github.com/RomanCohort/confluencia) `(Python | CN/EN)` — Small-sample circRNA discovery platform featuring the first 6-compartment mechanistic circRNA PK model (RNACTM).
- [maximvpolyakov/CAR-T-model](https://github.com/maximvpolyakov/CAR-T-model) `(C++/OpenMP)` — Spatiotemporal 3D coupled PDE simulator modeling CAR-T exhaustion, antigen escape, and hypoxia in solid tumors.
- [BioTender-max/CARTCellEngine](https://github.com/BioTender-max/CARTCellEngine) `(Python)` — Pure-Python ODE pipeline for CAR-T effector-target killing kinetics, T-cell exhaustion, and response prediction.
- [compiler-research/CARTopiaX](https://github.com/compiler-research/CARTopiaX) `(C++)` — High-performance agent-based platform modeling CAR-T trafficking, infiltration, and tumor-organoid killing.
- [FDA/TCPro](https://github.com/FDA/TCPro) `(MATLAB)` — U.S. FDA mechanistic tool predicting ex vivo T-cell proliferation and MHC-II immunogenicity/ADA risk for biologics.
- [singhharsh1708/QSPAtlas.jl](https://github.com/singhharsh1708/QSPAtlas.jl) `(Julia)` — Open-source Julia collection reconstructing and validating published PK/PD, QSP, and CAR-T cellular kinetics models.
- [BMSQSP/QSPToolbox](https://github.com/BMSQSP/QSPToolbox) `(MATLAB)` — BMS MATLAB toolbox standardizing SimBiology QSP workflows, global sensitivity analysis, and VPop calibration.
- [feigelman/gQSPsim-release](https://github.com/feigelman/gQSPsim-release) `(MATLAB)` — Genentech SimBiology GUI app enabling reproducible QSP model calibration, virtual population generation, and diagnostics.
- [pfizer-opensource/integrated-qsp-vpop-onco-efficacy-CPT-PSP](https://github.com/pfizer-opensource/integrated-qsp-vpop-onco-efficacy-CPT-PSP) `(MATLAB)` — Pfizer QSP virtual population framework with Metropolis-Hastings sampling and longitudinal oncology efficacy calibration.
- [popellab/QSPIO-TNBC](https://github.com/popellab/QSPIO-TNBC) `(MATLAB)` — Mechanistic multi-scale immuno-oncology QSP platform modeling tumor-immune interactions and checkpoint therapies.
- [NVIDIA-BioNeMo/nvQSP](https://github.com/NVIDIA-BioNeMo/nvQSP) `(C++/CUDA/Python)` — GPU-accelerated stiff ODE solver library from NVIDIA BioNeMo for ultra-fast, large-scale QSP VPop simulations.
- [SciML/Catalyst.jl](https://github.com/SciML/Catalyst.jl) `(Julia)` — Symbolic reaction network DSL compiling mechanistic QSP models into high-performance ODE/SDE/jump solvers.
- [pysb/pysb](https://github.com/pysb/pysb) `(Python)` — Rule-based Python framework for modular biochemical signaling and QSP models generating reaction networks and ODEs.
- [sys-bio/tellurium](https://github.com/sys-bio/tellurium) `(Python)` — Python systems biology and QSP environment combining Antimony model definitions with libRoadRunner SBML simulation.
- [copasi/COPASI](https://github.com/copasi/COPASI) `(C++)` — Open-source Complex Pathway Simulator supporting deterministic/stochastic simulation and parameter estimation for SBML QSP.

---

## 10. AI, ML, SciML & RL for ClinPharm & PMx

### 10.1 LLM Agents, MCP, RAG & Knowledge Mining

- [PeterBloomingdale/pmxagent](https://github.com/PeterBloomingdale/pmxagent) `(R/Python/Docker)` — Open-source agentic platform exposing R pharmacometrics functions as REST APIs and an MCP server for LLMs.
- [MomentumMetrix/PK_Claude](https://github.com/MomentumMetrix/PK_Claude) `(R/Claude Code)` — Integrates Claude Code into pharmacometrics workflows for AI-driven population PK analysis and scripting.
- [MomentumMetrix/RstudioMCP](https://github.com/MomentumMetrix/RstudioMCP) `(TS/R)` — MCP server for RStudio IDE allowing LLM agents to run R pharmacometrics scripts and capture diagnostic plots.
- [pharmacometricsai/nonmem-library](https://github.com/pharmacometricsai/nonmem-library) `(NONMEM/MD)` — Curated library of NONMEM PopPK/PD control streams co-developed and debugged with LLMs as a coding benchmark.
- [VirtualPatientEngine/AIAgents4Pharma](https://github.com/VirtualPatientEngine/AIAgents4Pharma) `(Python)` — Open-source LLM agent suite (including *Talk2BioModels*) for querying and simulating systems pharmacology models.
- [openpharma-org/fda-mcp](https://github.com/openpharma-org/fda-mcp) `(TS)` — MCP server connecting LLM agents directly to openFDA drug labels, FAERS, Orange Book, and Purple Book.
- [Slow-Walker66/PK-Sim-Mobi-RAG-Tool](https://github.com/Slow-Walker66/PK-Sim-Mobi-RAG-Tool) `(Python | CN/EN)` — Local RAG assistant indexing PK-Sim and MoBi technical documentation and building blocks for PBPK troubleshooting.
- [lfcypo/hrt-pk-mcp](https://github.com/lfcypo/hrt-pk-mcp) `(Python/MCP | Chinese)` — Standard Python MCP server wrapping multi-compartment PK algorithms for AI-agent dose logging and queries.
- [kimmingul/clinical-pharmacology-study-protocol-development](https://github.com/kimmingul/clinical-pharmacology-study-protocol-development) `(Claude Plugin | KR/EN)` — Claude Code plugin assisting clinical pharmacologists in drafting Phase 1 protocols (FIH, SAD/MAD, DDI) and ICFs.
- [QSong-github/DrugClaw](https://github.com/QSong-github/DrugClaw) `(Python)` — LangGraph agentic RAG runtime for evidence-grounded DDI, pharmacogenomics (PGx), ADR, and FDA label intelligence.
- [gadevito/LLMDDI](https://github.com/gadevito/LLMDDI) `(Python)` — Pipelines for knowledge extraction, LLM fine-tuning, and benchmarking for drug-drug interaction (DDI) prediction.
- [reddy-nithin/TruPharma-Clinical-Intelligence](https://github.com/reddy-nithin/TruPharma-Clinical-Intelligence) `(Python)` — Hybrid RAG app parsing official FDA drug labels and cross-referencing FAERS signals for clinical safety Q&A.
- [nikhilreddy00/pharma-agent](https://github.com/nikhilreddy00/pharma-agent) `(Python)` — Autonomous LangGraph + ChromaDB agentic RAG cross-referencing FDA labels, PubMed, and guidelines for DDI queries.
- [Genentech/CLADD](https://github.com/Genentech/CLADD) `(Python)` — Genentech's RAG-enhanced multi-agent LLM system querying biomedical knowledge bases for molecular property reasoning.
- [PKPDAI/PKDocClassifier](https://github.com/PKPDAI/PKDocClassifier) `(Python)` — NLP/ML binary text classifier automatically screening biomedical literature for *in vivo* PK parameter studies.
- [dueyama/pmda-pk-curve-viewer](https://github.com/dueyama/pmda-pk-curve-viewer) `(TS/Next.js | JP/EN)` — Parses official Japanese PMDA package insert XML files to extract PK parameters and plot estimated concentration curves.
- [pablosierrafernandez/FarmacoDB](https://github.com/pablosierrafernandez/FarmacoDB) `(Python | Spanish)` — LLM-assisted text mining pipeline standardizing multi-source PK data (>1,000 drugs) with half-life prediction models.
- [valentinnavalos/pharmawatch-api](https://github.com/valentinnavalos/pharmawatch-api) `(API | Spanish)` — Pharmacovigilance REST API providing prescription checking and PK drug-drug interaction analysis.
- [PharMolix/OpenBioMed](https://github.com/PharMolix/OpenBioMed) `(Python | CN/EN)` — Multimodal biomedical LLM and agent framework featuring built-in ADMET prediction and DDI analysis tools.
- [datamllab/CAi_copilot](https://github.com/datamllab/CAi_copilot) `(Python | CN/EN)` — Natural-language drug design agent integrating ADMET-AI for clearance, absorption, metabolism, and toxicity screening.

### 10.2 PINNs, Neural ODEs, UDEs & SciML

- [jameslu01/Neural_PK](https://github.com/jameslu01/Neural_PK) `(Python/PyTorch)` — Applies Neural ODEs to clinical PK forecasting across unseen dosing regimens, benchmarked against NLME and LSTM.
- [TommyGiak/pharmacoNODE](https://github.com/TommyGiak/pharmacoNODE) `(Python/PyTorch)` — Neural ODE codebase for longitudinal PK concentration-time prediction with patient covariates.
- [emotionor/UniPKModel](https://github.com/emotionor/UniPKModel) `(Python/PyTorch)` — Interpretable Neural ODE framework with pre-trained weights for generalizable data-driven PK curve forecasting.
- [FraunhoferChalmersCentre/neuralODEpopulation](https://github.com/FraunhoferChalmersCentre/neuralODEpopulation) `(Python)` — End-to-end population PMx pipeline combining Transformers, Neural ODEs, and VAE random effects with VPCs.
- [Janssena/DeepCompartmentModels.jl](https://github.com/Janssena/DeepCompartmentModels.jl) `(Julia)` — Deep Compartment Models combining compartmental ODE constraints with neural networks for covariate learning.
- [PumasAI-Labs/DeepPumas_workshop_2026_PAGE](https://github.com/PumasAI-Labs/DeepPumas_workshop_2026_PAGE) `(Julia)` — Official PAGE workshop demonstrating DeepPumas (DeepNLME) embedding Neural ODEs and UDEs in PopPK/PD models.
- [SCAI-BIO/MMPK-SciML](https://github.com/SCAI-BIO/MMPK-SciML) `(Python/Julia)` — Fraunhofer SCAI repository benchmarking SciML against mechanistic PopPK and classical ML for oncology PK prediction.
- [NazAhmadi/CMINNs](https://github.com/NazAhmadi/CMINNs) `(Python/JAX)` — Compartment Model-Informed Neural Networks (PINNs/fPINNs) capturing anomalous diffusion and time-varying PK/PD.
- [yapici/open-pk-pinn](https://github.com/yapici/open-pk-pinn) `(Python/PyTorch)` — Open, reproducible compartmental Physics-Informed Neural Network (CMT-PINN) benchmark on public *in vivo* PK data.
- [novainsilico/vpop-calibration](https://github.com/novainsilico/vpop-calibration) `(Python)` — Accelerates QSP virtual population calibration by coupling NLME inference with ML surrogate models.

### 10.3 RL & Deep Learning for Precision Dosing & TDM

- [hamilton-health-sciences/warfarin](https://github.com/hamilton-health-sciences/warfarin) `(Python/PyTorch)` — Offline deep RL (`smdbcq`) trained on COMBINE-AF trial data to optimize sequential warfarin dosing.
- [rudra2112/Warfarin-Dosage-Prediction](https://github.com/rudra2112/Warfarin-Dosage-Prediction) `(Python)` — Contextual multi-armed bandit (Linear-UCB) RL for individualized warfarin dosing with clinical and genotype features.
- [karneslab/warfarin-machinelearning](https://github.com/karneslab/warfarin-machinelearning) `(R)` — Machine learning scripts predicting stable warfarin maintenance doses using pharmacogenetic and clinical covariates.
- [lucis-e/PopPBPK-RL_Bnzpril](https://github.com/lucis-e/PopPBPK-RL_Bnzpril) `(Python/R)` — Integrates population PBPK with reinforcement learning to optimize benazepril dosing in renal-impaired cohorts.
- [FatemehRabie/chemotherapy](https://github.com/FatemehRabie/chemotherapy) `(Python)` — Couples a 3D tumor PDE simulator with Gymnasium/SB3 for physics-guided deep RL of personalized chemotherapy dosing.
- [ZhiGroup/PK-RNN](https://github.com/ZhiGroup/PK-RNN) `(Python)` — Recurrent neural network (PK-RNN-V) leveraging longitudinal EHR dosing/lab records for vancomycin TDM forecasting.
- [BingyuMao/vanco_2cm](https://github.com/BingyuMao/vanco_2cm) `(Python)` — Hybrid autoregressive RNN + mechanistic 2-compartment PK head (PKRNN-2CM) for interpretable vancomycin forecasting.
- [Yunwoolee17/Vancomycin_prediction_AI](https://github.com/Yunwoolee17/Vancomycin_prediction_AI) `(Python | Korea)` — ML pipeline with SHAP explainability predicting initial vancomycin doses to achieve target AUC (400–600 mg·h/L).
- [y-babdalla/tacrolimus_predictions](https://github.com/y-babdalla/tacrolimus_predictions) `(Python/PyTorch)` — End-to-end attention/time-aware LSTM pipeline with synthetic data augmentation for tacrolimus trough forecasting.
- [huiyum/tac_dose_adjustments](https://github.com/huiyum/tac_dose_adjustments) `(Python/Streamlit)` — Modular GRU deep learning pipeline and Streamlit app for tacrolimus trough prediction and dose adjustments.
- [sebboie/aptt-prediction](https://github.com/sebboie/aptt-prediction) `(Python)` — Recurrent neural network forecasting activated partial thromboplastin time (aPTT) trajectories during IV heparin therapy.

### 10.4 Automated PMx, ML Covariates & Synthetic Data

- [certara/pyDarwin](https://github.com/certara/pyDarwin) `(Python)` — Automates NONMEM/NLME PopPK/PD structural and covariate selection using GA, RF, GBRT, Gaussian Processes, and PSO.
- [gengbo-genentech/Pharm-AutoML](https://github.com/gengbo-genentech/Pharm-AutoML) `(Python)` — Genentech's *CPT:PSP* AutoML framework streamlining end-to-end modeling and interpretability for clinical pharmacology.
- [Janssena/pkSHAP](https://github.com/Janssena/pkSHAP) `(Python/Julia)` — Applies SHAP values to ML models to infer optimal mathematical functional forms of patient covariates in PK modeling.
- [AstraZeneca/Stochastic-gates-for-covariate-selection-in-population-pharmacokinetics-modelling-](https://github.com/AstraZeneca/Stochastic-gates-for-covariate-selection-in-population-pharmacokinetics-modelling-) `(Python)` — Uses differentiable Stochastic Gates neural feature selection to automate and accelerate PopPK covariate screening.
- [wahlquisty/learning-pharmacometric-covariate-structures](https://github.com/wahlquisty/learning-pharmacometric-covariate-structures) `(Julia)` — Neural symbolic regression prototype for automated pharmacometric covariate structure discovery.
- [iasiimwe/unite4tb_ml](https://github.com/iasiimwe/unite4tb_ml) `(R/Python)` — Benchmarks ML against traditional PMx/GWAS for high-dimensional SNP covariate imputation and selection in PopPK.
- [jbwoillard/synthetic_data_pharmacogenetics](https://github.com/jbwoillard/synthetic_data_pharmacogenetics) `(R/Python)` — Evaluates privacy-preserving synthetic patient data generators (Avatar, VAE, CTGAN) for clinical pharmacology cohorts.

### 10.5 ML/DL Prediction of Human PK & ADME

- [Novartis/DeepCt](https://github.com/Novartis/DeepCt) `(Python)` — Novartis deep learning framework predicting full plasma concentration-time profiles and compartmental PK from SMILES.
- [srijitseal/PKSmart](https://github.com/srijitseal/PKSmart) `(Python)` — Two-stage ML pipeline combining chemical descriptors and predicted animal PK to forecast human CL, Vdss, t1/2, and fu.
- [swansonk14/admet_ai](https://github.com/swansonk14/admet_ai) `(Python)` — Fast Chemprop-based GNN platform trained on TDC benchmarks predicting 40+ ADMET and PK properties at scale.
- [xli7654321/MMPK](https://github.com/xli7654321/MMPK) `(Python)` — Multimodal deep learning framework with substructure cross-attention predicting human oral PK (CL/F, Vz/F, t1/2, AUC, F).
- [xtalpi-xic/pk-model](https://github.com/xtalpi-xic/pk-model) `(Python)` — Combines GNNs (Chemprop/D-MPNN) and ensemble ML with PBPK workflows to predict human small-molecule PK.
- [dreadlesss/pharmacokinetic_prediction](https://github.com/dreadlesss/pharmacokinetic_prediction) `(Python)` — Gradient-boosted decision trees predicting human IV PK parameters (CL, Vd, t1/2, MRT, fu) from 1,352 compounds.
- [eugenebang/ADME-DL](https://github.com/eugenebang/ADME-DL) `(Python)` — Enriches molecular foundation models via sequential ADME PK-guided multi-task learning.
- [Sanofi-Public/DMPK-US-ML-mTPA](https://github.com/Sanofi-Public/DMPK-US-ML-mTPA) `(Python)` — Integrates minimal PBPK/TMDD with tree-based ML classifiers to evaluate early mAb target pharmacology and PK/PD feasibility.
- [UFPBPK/Nano-AI-PBPK-G1](https://github.com/UFPBPK/Nano-AI-PBPK-G1) `(Python/R)` — AI-assisted PBPK modeling framework predicting nanoparticle tumor delivery and tissue pharmacokinetics.
- [molecularinformatics/Computational-ADME](https://github.com/molecularinformatics/Computational-ADME) `(Python)` — Biogen's industrial benchmark code and datasets for prospective validation of ML/DL on *in vitro* ADME endpoints.
- [OpenADMET/openadmet-models](https://github.com/OpenADMET/openadmet-models) `(Python)` — Scalable open-science ML architectures and pipelines for reproducible ADMET and DMPK endpoint prediction.
- [abinittio/CYP450-Metabolism-Predictor](https://github.com/abinittio/CYP450-Metabolism-Predictor) `(Python)` — Multi-task GNN trained on ChEMBL predicting inhibition across 5 major CYP450 isoforms for DDI liability screening.
- [CDDLeiden/PK-in-generative-drug-design](https://github.com/CDDLeiden/PK-in-generative-drug-design) `(Python)` — Integrates the Lombardo human IV PK dataset with QSP/PK modeling pipelines for generative drug design.

---

## 11. Open Clinical PK Datasets, Benchmarks & Awesome Lists

- [matthiaskoenig/pkdb](https://github.com/matthiaskoenig/pkdb) `(Python/Django | Germany)` — FAIR open pharmacokinetics database (PK-DB) curating clinical PK curves, genotypes, and organ impairment via API.
- [Open-Systems-Pharmacology/Database-for-observed-data](https://github.com/Open-Systems-Pharmacology/Database-for-observed-data) `(Excel/CSV)` — Curated digitized clinical PK concentration-time profiles and DDI datasets from literature for PBPK qualification.
- [nlmixr2/nlmixr2data](https://github.com/nlmixr2/nlmixr2data) `(R)` — Standard benchmark and tutorial PopPK/PD datasets (1- and 2-compartment bolus/infusion) for `nlmixr2`/`rxode2`.
- [dpastoor/PKPDdatasets](https://github.com/dpastoor/PKPDdatasets) `(R)` — Curated ready-to-use pharmacokinetic and pharmacodynamic datasets for M&S benchmarking and education.
- [billdenney/PKdata](https://github.com/billdenney/PKdata) `(R)` — Real and simulated single-/multiple-dose PK datasets structured for validating NCA and PK software implementations.
- [mims-harvard/TDC](https://github.com/mims-harvard/TDC) `(Python)` — Standardized AI-ready ADME/PK benchmark datasets (CL, t1/2, Caco-2, PPB, CYP) with scaffold splits and leaderboards.
- [mindrank-ai/PharmaBench](https://github.com/mindrank-ai/PharmaBench) `(Python/Data)` — Cleaned, LLM-mined ADMET and PK property benchmark suite covering absorption, PPB, BBB, CYP, and clearance.
- [isop-phmx/awesome-pharmacometrics](https://github.com/isop-phmx/awesome-pharmacometrics) `(Markdown)` — ISoP-maintained directory of pharmacometrics university programs, journals, conferences, tutorials, and textbooks.
- [AIML-SIG/awesome-ai-ml-pharmacometrics](https://github.com/AIML-SIG/awesome-ai-ml-pharmacometrics) `(Markdown)` — Curated community list of AI/ML papers, tools, and resources for pharmacometrics, PBPK, and QSP.

---

## 12. Multi-Lingual Open Textbooks & Workshops

- [PumasAI-Labs/PumasIntroTutorial-ContinuousData](https://github.com/PumasAI-Labs/PumasIntroTutorial-ContinuousData) `(Julia/Quarto)` — Official PumasAI open tutorial covering clinical PK prep, FDA/EMA-aligned NCA, and continuous-data workflows in Julia.
- [asancpt/book-ncar](https://github.com/asancpt/book-ncar) `(Bookdown | Korean)` — Open-source Korean textbook teaching practical NCA and bioequivalence evaluation in R.
- [asancpt/nmw-nonmem](https://github.com/asancpt/nmw-nonmem) `(R/NONMEM | KR/EN)` — Educational code demonstrating NLME estimation algorithms (FO/FOCE/FOCE-I) bridging R and NONMEM.
- [AMC-CPT/PKwR](https://github.com/AMC-CPT/PKwR) `(R/Shiny | KR/EN)` — Companion repository for *Pharmacokinetics with R* with reproducible scripts and a vancomycin TDM Shiny app.
- [AMC-CPT/PMx](https://github.com/AMC-CPT/PMx) `(R/NONMEM | KR/EN)` — Companion repository for *Pharmacometrics with NONMEM and R* with verified NONMEM control streams and R code.
- [pipetcpt/basic](https://github.com/pipetcpt/basic) `(Bookdown/NONMEM | Korean)` — PIPET beginner pharmacometrics workshop covering NONMEM coding, dataset prep, covariates, and PK-PD linkage.
- [pipetcpt/pharmapk](https://github.com/pipetcpt/pharmapk) `(Bookdown | Korean)` — Open textbook explaining ADME, clearance, distribution, NCA, and compartmental PK for drug development.
- [pipetcpt/book-poppk](https://github.com/pipetcpt/book-poppk) `(Bookdown | Korean)` — Web-based compilation of Korea MFDS Population Pharmacokinetics regulatory guidelines and validation practices.
- [pipetcpt/capstone-qsp](https://github.com/pipetcpt/capstone-qsp) `(R/Shiny | KR/EN)` — Capstone projects demonstrating how to turn mechanistic QSP ODE models into interactive R Shiny dashboards.
- [matthiaskoenig/course-pharmacokinetic-modelling](https://github.com/matthiaskoenig/course-pharmacokinetic-modelling) `(Python/Jupyter | DE/EN)` — University-level interactive Jupyter Notebook course covering compartmental PK, PBPK, and dosing optimization.
- [Clinical-Pharmacy-Saarland-University/RTutorial](https://github.com/Clinical-Pharmacy-Saarland-University/RTutorial) `(R Markdown | DE/EN)` — Structured R tutorials for clinical pharmacy and pharmacometrics data analysis from Saarland University.
- [Kalo0m/pharmacocinetique](https://github.com/Kalo0m/pharmacocinetique) `(TS | French)` — French-language educational web app for learning and calculating fundamental pharmacokinetics concepts.
- [douglasufs/matematica-aplicada-ciencias-farmaceuticas](https://github.com/douglasufs/matematica-aplicada-ciencias-farmaceuticas) `(OER | Portuguese)` — Portuguese OER textbook covering pharmaceutical math, dilution, bioequivalence, and computational pharmacokinetics.

---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}

Integrating AI into Research Workflows: Resource Provisioning and AI-Driven Cyberinfrastructure
======
*Aug 2019 – Present*

Developed an AI-driven framework for optimizing resource allocation and scheduling in HPC and deep learning workflows, improving efficiency and reducing energy and time costs. Work conducted as part of the NSF ICICLE AI Institute and EAGER: Bridging the Last Mile projects under Dr. Rajiv Ramnath at The Ohio State University.

* **AI-Powered Cyberinfrastructure Tool for Researchers:** Streamlines preprocessing, tool exploration, and software optimization by leveraging past experiences and resources to support researchers in their workflows.
* **Smart Scheduler for Deep Learning Applications:** Framework for optimized resource allocation integrating SLURM to estimate job runtimes and enhance scheduling efficiency; tailored for TensorFlow and PyTorch frameworks.
* **HARP Framework for HPC Resource Prediction:** AI-driven system to predict HPC resource needs via historical data analysis, supporting FAIR principles for software generalization across cyberinfrastructures.
* **ML-Driven HPC Resource Allocation:** ML models to predict optimal resource allocation for applications like genome sequencing, reducing time and computational overhead in HPC environments.
* **DNN Resource Estimators:** Architecture-aware estimators leveraging XLA/HLO graph features for hardware-aware resource prediction, scaled across edge and center environments (latency, memory, power).
* **Rules Engine for Model Adaptation:** Rules-based decision framework integrating HARP and Smart Scheduler insights to autonomously trigger model retraining and fine-tuning across the computing continuum.
* **Agentic System Wrappers with LLM Interfaces (In Progress):** Extending frameworks into agentic, LLM-powered systems for natural language-driven workflow creation and self-updating orchestration.

AI-Driven Model Adaptation Framework for Edge Deployments in Computational Ecology
======
*Aug 2024 – Present*

Toolkit enabling field researchers in computational ecology to deploy and evaluate AI models directly on edge devices, supporting tasks such as intrusion detection and blank filtering in camera-trap imagery. Empowers non-ML experts to select suitable models under real-world hardware constraints (latency, memory, power) with minimal dependency on AI engineers. Architecture is generalizable to precision agriculture and environmental monitoring.

*My Role:* Requirement gathering with ecologists, training domain-centric ML models, testing with the Field Planner, and validating edge deployments using TACC's infrastructure.

* **ML Field Planner (TAPIS UI):** Guided interface for selecting a model, dataset, and target device; launches controlled benchmarks under edge constraints.
* **CKN Dashboard for Camera Traps:** Knowledge-network visualization for comparing runtime, memory utilization, latency, precision, and recall across experiments.
* **ML Edge Server:** Dockerized plug-and-play edge stack assembling configurable workflow stages (e.g., blank deletion, species-detection alerts).
* **CT-Controller (Edge Deployment Manager):** Control UI to deploy, manage, and verify models/workflows on edge devices; supports quick iteration and on-site validation.

Discovering Hypernyms for New Senses in WordNet (NLP — M.S. Research)
======
*Aug 2017 – May 2019*

Applied Hearst Patterns, regular expressions, and word2vec models to identify optimal insertion points for new word senses in WordNet; contributed to SemEval 2016 Task 14 and SemEval 2018 Task 9. Published peer-reviewed paper at SemEval@NAACL-HLT 2018.

* Applied pattern recognition algorithms (Hearst Patterns) and state-of-the-art vector space models (word2vec) for lexical hierarchy expansion.
* Demonstrated improved performance in automated WordNet updating without manual intervention.

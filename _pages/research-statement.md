---
layout: archive
title: "Research Statement"
permalink: /research-statement/
author_profile: true
---

{% include base_path %}

## The Policy Stakes: A Crisis of Waste, Access, and Governance

The United States has invested tens of billions of dollars in national supercomputing infrastructure — from the Ohio Supercomputer Center (OSC) to the Texas Advanced Computing Center (TACC) — on the premise that shared, high-performance computing (HPC) resources accelerate scientific discovery. HPC has delivered on that promise in extraordinary ways: large-scale simulations replaced underground nuclear testing, the Energy Exascale Earth System Model now informs IPCC climate policy, and supercomputers screened billions of compounds against SARS-CoV-2 proteins in days rather than years.

But this infrastructure is being used remarkably poorly.

My analysis of a local OSC cluster reveals a striking pattern: **GPU utilization rarely exceeds 50% and averages around 23%; GPU memory averages only 12%; CPUs are routinely left idle.** Researchers request full-node GPU allocations for jobs that need a fraction of one node. Jobs are terminated mid-run — losing all progress — because walltime was underestimated. Optimal CPU tuning could reduce job costs by roughly **30% with no increase in execution time**, yet it almost never happens. The root cause is not carelessness — it is the absence of tools that help researchers know what their jobs actually need before they submit them.

At the same time, AI is making this problem dramatically worse. Training a single large language model like GPT-3 consumed an estimated **5.4 GWh of electricity** — enough to power more than 500 American households for a year. AI-driven workloads are projected to **triple energy demand by 2030**. As AI moves from data centers to edge devices in homes, schools, hospitals, and field cameras, that footprint expands exponentially. The specialized hardware AI requires strains raw material supply chains. The environmental cost is real and growing.

Yet existing AI governance frameworks — the EU AI Act, IEEE Global Initiative on Ethics of Autonomous Systems, OECD AI Principles — focus almost entirely on transparency, privacy, and bias. **Almost none address the sustainability and efficiency of the cyberinfrastructure that makes AI possible.** This is a policy gap I am committed to closing through my research.

There is also an equity dimension. At major AI conferences such as NeurIPS and ICML, 40–50% of accepted papers are co-authored by researchers at industry labs with access to vast GPU clusters. Academic researchers, institutions in the Global South, ecologists with camera traps in remote field sites, and students at resource-constrained universities cannot compete — not because of a talent gap, but because of a **compute access gap**. When AI can only be meaningfully tested, validated, or challenged by those who own the infrastructure, accountability breaks down. The public cannot audit a model it cannot run.

My research addresses all three dimensions of this crisis — waste, sustainability, and access — by building the AI systems that make HPC resources smarter, more efficient, and more equitable.

---

## Broader Impact: What Responsible AI Infrastructure Enables

The policy vision motivating my work draws on a historical analogy: the World Wide Web flourished not because of raw technology, but because the World Wide Web Consortium (W3C) established open standards — consistency, accessibility, interoperability — that kept the web a democratic medium. AI and HPC need the equivalent: governance frameworks tied to **openness, sustainability, equity, and trust**.

My research contributes directly to this vision in four ways:

**Reducing waste in federally funded infrastructure.** By enabling researchers to accurately predict what their jobs need before submission, my frameworks reduce over-provisioning, shorten queue wait times, and cut computational costs. These are not abstract improvements — they translate directly into more science per dollar of public investment and lower energy consumption at national computing centers.

**Democratizing AI for domain scientists.** Ecologists, epidemiologists, conservation biologists, and agricultural scientists should not need a team of ML engineers to deploy AI models. My tools create pathways for non-experts to characterize, benchmark, and deploy AI on hardware they actually have — from Raspberry Pis in the field to shared HPC nodes.

**Informing AI sustainability policy.** My empirical data on real GPU utilization patterns and the cost of workload mischaracterization provides **evidence** for policy interventions: energy efficiency standards for compute infrastructure, evaluation guidelines for when AI-enabled alternatives are actually necessary, accountability frameworks for models running on shared national resources. Building policy without this data is building in the dark.

**Preparing the next generation.** I have mentored over 20 graduate and undergraduate students, managed the ICICLE NextGen student community of 280+ students, and launched outreach to middle and high school students. I believe fear of AI impedes its safe development. My outreach approach — demystifying the technology, building scientific literacy, creating trust — is itself a form of policy work.

---

## The Research: Making HPC and AI Self-Aware

My technical research builds the software infrastructure that closes the gap between _what a job needs_ and _what gets requested_. It spans three interconnected frameworks.

### HARP: Predicting HPC Resource Needs Before a Job Runs

The **HPC Application Resource Predictor (HARP)** is an AI-driven framework that generates application-specific estimates of walltime and resource requirements before job submission. HARP's key innovation is a three-stage pipeline: a _Generate_ component that uses scaled-down execution campaigns to create training data at a fraction of full-scale cost (reducing data collection overhead by a factor of 7); a _Build_ component that trains regression models with custom loss functions that asymmetrically penalize underestimation; and a _Predict_ component that selects the optimal model per application using policy-aware evaluation metrics (under-prediction percentage and over-estimation MAPE).

HARP addresses a fundamental challenge: there is no such thing as a "one model fits all" HPC resource estimator. Runtime is sensitive to application type (compute-bound vs. I/O-bound vs. memory-bound), input configuration, hardware generation, and CI policies that vary across centers. HARP's context-aware, application-specific models handle this diversity while adhering to FAIR principles for portability. I validated HARP on a representative spectrum of HPC workloads: Gray-Scott chemical diffusion simulations (compute-intensive), Trimmomatic genome sequencing preprocessing (I/O-intensive), and VGG16/ResNet50/InceptionV3 DNN training (memory-and-compute-intensive).

For **DNN workloads**, I extended HARP with architecture-aware white-box estimators that leverage High-Level Optimization (HLO) graphs generated by the XLA compiler. These graphs capture model structure at the operation level — node attributes, adjacency matrices, tensor shapes, tiling configurations — enabling Graph Neural Networks to predict GPU memory, training latency, and power draw across hardware generations (P100, V100, A100) without requiring full-scale executions. The dataset spans 20,000+ records across 17 model architectures and three OSC clusters.

_Key publications:_ PEARC 2022; IEEE ISPA/BDCloud 2022; **Best Paper — PEARC 2023** (Phil Andrews Award for Best Paper Overall); SC'25 WHPC Workshop; ISC-HPC 2025.

---

### Smart Scheduler: CI-Aware, Intelligent Job Orchestration

Knowing what a job needs is only useful if the scheduling system can act on that knowledge. The **Smart Scheduler (iScheduler)** framework integrates HARP's predictions with SLURM-based HPC scheduling through a **CI database** that encodes system configurations, queue limitations, billing policies, and feasibility constraints for multiple centers. The scheduler's _Intelligence Plane_ automates job submission, monitoring, rescheduling, and tracking — closing the loop between resource prediction and resource allocation.

The CI database is itself a research contribution: it combines scraped CI documentation with programmatically extracted SLURM data to encode the subtle but consequential policy differences between centers. At OSC, users can request partial nodes and the system dynamically assigns queues; at TACC, entire nodes must be reserved and queue selection is explicit. These differences profoundly affect what constitutes a "feasible" execution plan — and existing tools have no representation of them. The Smart Scheduler makes CI-awareness a first-class scheduling concern.

The Intelligence Plane exposes these capabilities through TAPIS APIs, enabling domain scientists to submit and monitor DNN training jobs through a unified, gateway-accessible interface without deep HPC expertise.

_Key publications:_ **Best Paper — PEARC 2025** (Phil Andrews Award for Best Paper Overall); PEARC 2024; Science Gateways 2023.

---

### ML Field Planner: Democratizing AI for Edge Deployments

A distinct thread of my research addresses the **last-mile access problem**: domain scientists who need to deploy AI models on edge devices for field research but lack the infrastructure or expertise to do so. In collaboration with TACC and the NSF ICICLE AI Institute, I co-developed the **ML Field Planner** — a toolkit that enables ecologists and conservation biologists to select, benchmark, and deploy computer vision models (for camera-trap blank filtering and intrusion detection) under real-world hardware constraints: latency budgets, memory limits, and power envelopes.

The Field Planner's core contribution is a _constrained model selection framework_ that translates hardware and deployment constraints into actionable model recommendations, backed by reproducible benchmark reports. This is generalizable beyond ecology — the same framework applies to precision agriculture sensor networks and environmental monitoring. My role included requirements elicitation with ecologists at TACC, training domain-adapted models on camera-trap imagery, and validating deployments on TACC's edge infrastructure.

_Key publications:_ **Best Paper — PEARC 2025** (co-author, Phil Andrews Award); PEARC 2024 (Human Powered Computing); Science Gateways 2025.

---

### Agentic AI: Toward Self-Managing Scientific Cyberinfrastructure

My current and future work extends the above frameworks into **agentic systems** — AI that autonomously perceives, reasons, and acts, with minimal human intervention. The **Intelligence Plane v2.0** reimagines the scheduler as an MLOps agent: it monitors model accuracy at the edge, detects out-of-distribution events via the Camera Knowledge Network (CKN), triggers retraining events, estimates resource requirements via HARP, selects the optimal HPC system from the CI database, submits jobs through TAPIS, tracks execution via a Job Monitoring Daemon, and updates Model Cards upon completion. The full cycle — from edge inference failure to retrained model deployment — is autonomous.

A key near-term goal is integrating **LLMs** into this agent loop: a conversational interface that lets scientists describe workflows in natural language ("retrain the blank-filter model on last month's camera trap data, keep it under 4 GPU-hours") and have the system decompose, validate feasibility, schedule, and report back. The **Unified Component API** (Science Gateways 2025) establishes the standardized middleware integration patterns that make cross-system interoperability — and therefore this kind of agent — possible.

_Key publications:_ PEARC 2025 (Beyond Automation: Agentic MLOps); Science Gateways 2025 (Unified Component API, ML Field Planner agentic extensions).

---

## Future Directions

My future research agenda is explicitly grounded in the policy imperatives above:

**Sustainability-aware scheduling.** Integrating carbon intensity signals and energy efficiency objectives directly into the Smart Scheduler's optimization function — moving beyond walltime minimization toward _sustainable science computing_. This would produce the empirical evidence needed to inform energy efficiency standards for national HPC centers.

**Foundation models for cross-institutional resource prediction.** Current HARP models are application- and cluster-specific. I plan to explore whether a foundation model pre-trained on multi-institution HPC log corpora can generalize resource predictions across centers with minimal fine-tuning — dramatically lowering the cost of deploying intelligent resource management at smaller or under-resourced institutions.

**Accountability infrastructure for AI on shared compute.** Building governance tooling — documentation standards, audit trails, and cost-attribution frameworks — that lets policymakers and resource administrators understand how AI workloads consume shared national infrastructure. AI needs its equivalent of a W3C, and that work starts with data.

---

_For the full list of publications, posters, and presentations, see the [Publications](/publications/) page._

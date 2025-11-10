---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}


Thesis Work
===========
• Ph.D. Thesis (In Progress): AI-Driven Resource Optimization for High-Performance Computing: A Comprehensive Framework (IHPCSS 2025 )
o Focus: Developing adaptive, user-centric frameworks that utilize AI to intelligently predict and allocate HPC resources, significantly reducing "time-to-science."
• M.S. Thesis: Hypernym Discovery over WordNet and English Corpora - using Hearst Patterns and Word Embeddings
o Focus: Foundational research in Natural Language Processing (NLP), applying Word Embeddings and pattern matching for semantic relation extraction (Hypernym Discovery).

Current Academic Research 
=========================
** Integrating Artificial Intelligence into Research Workflows: A Comprehensive Approach for Resource Provisioning and AI-Driven Cyberinfrastructure Development                      
Relevant Coursework: Artificial Intelligence (statistical models to build baselines for task-specific classifiers and regressors), Operating Systems (batch processing, hyper-parameters settings for performance optimizations), Advanced Computer Architecture, High-Performance deep neural network processing, and  Research project capstone (application of research methods and best practices in research; teamwork, written and oral communication)
Developed an AI-driven framework for optimizing resource allocation and scheduling in HPC and deep learning workflows, improving efficiency and potentially reducing energy and time costs.
• AI-Powered Cyberinfrastructure Tool for Researchers: Led a project to develop an AI-driven tool that streamlines pre-processing, tool exploration, and software optimization by leveraging past experiences and resources to support researchers in their workflows.
• Smart Scheduler for Deep Learning Applications: Designed a framework for optimized resource allocation in deep learning environments, integrating SLURM to estimate job runtimes and enhance scheduling efficiency, tailored for TensorFlow and PyTorch frameworks.
• HARP Framework for HPC Resource Prediction: Created an AI-driven system to predict HPC resource needs, supporting scientific workflows through historical data analysis, improving adherence to FAIR principles for software generalization across cyberinfrastructures.
• ML-Driven HPC Resource Allocation: Developed machine learning models to predict optimal resource allocation for applications like genome sequencing, reducing the time and computational resources needed to adjust system configurations in high-performance computing environments.
• DNN Resource Estimators: Developing DNN architecture-aware resource estimators that leverage XLA features—specifically drawn from HLO graphs—to incorporate hardware-aware characteristics influencing resource requirements, and scaling these estimators across edge and center environments to account for diverse resource constraints such as latency, memory, and power consumption.
• Rules Engine for Model Adaptation: Implemented a rules-based decision framework that integrates predictive insights from HARP and Smart Scheduler to autonomously trigger model retraining, fine-tuning, and estimator updates for edge and center deployments, enabling adaptive optimization based on dynamic workload, latency, and resource feedback across the computing continuum.
• Agentic System Wrappers with LLM Interfaces (Currently Exploring): Extending existing frameworks into agentic, LLM-powered systems that serve as interactive user interfaces for scientists—enabling natural language-driven workflow creation, adaptive scheduling, and self-updating orchestration across the computing continuum.

** AI-Driven Model Adaptation Framework for Edge Deployments in Computational Ecology         
Developed a toolkit to enable field researchers in computational ecology to deploy and evaluate AI models directly on edge devices, supporting tasks such as intrusion detection and blank filtering in camera-trap imagery. The project addresses a key challenge: ecologists often lack access to tools that test, compare, and fine-tune models under real-world hardware constraints such as latency, memory, and power. By bridging this gap, the toolkit empowers non-ML experts to select the most suitable model for their use case while minimising dependency on AI engineers. Although initially built for ecology, the framework’s architecture is generalizable to similar domains such as precision agriculture and environmental monitoring.
My Role: Conducted requirement gathering with ecologists, trained domain-centric ML models, and tested models with the Field Planner, and validated edge deployments using TACC’s infrastructure.
Core Components:
• ML Field Planner (TAPIS UI): Guided interface for selecting a model, dataset, and target device, then launching controlled tests to benchmark models under edge constraints.
• CKN Dashboard for Camera Traps: A knowledge-network visualization system that enables researchers to compare performance and efficiency metrics—including runtime, memory utilization, latency, precision, and recall—across experiments executed via the ML Field Planner..
• ML Edge Server: Plug-and-play edge software stack (Dockerized components) that assembles workflow stages—e.g., delete blanks only or delete blanks + alert authorities (via a near-edge laptop) when a target species is detected.
• CT-Controller (Edge Deployment Manager): Simple control UI to deploy, manage, and verify models/workflows on edge devices; supports quick iteration and on-site validation.



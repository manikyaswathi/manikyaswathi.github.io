---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Summary
======
7th-year Ph.D. candidate in Computer Science and Engineering at The Ohio State University, specializing in AI-integrated Cyberinfrastructure, with over 9 years of academic research experience and 4 years of professional software engineering experience. Graduate Research Assistant under Dr. Rajiv Ramnath on the NSF ICICLE AI Institute and EAGER: Bridging the Last Mile projects, designing and deploying AI-driven systems (HARP Framework, Smart Scheduler, ML Field Planner) to help researchers execute scientific workflows across the edge-to-center computing continuum. Current research explores integrating Large Language Models (LLMs) and agentic AI systems into cyberinfrastructure for autonomous workflow coordination. ICICLE NextGen Student Group Manager; advised and mentored over 20 graduate and undergraduate students and guided more than 200 undergraduates through teaching and summer capstone courses.

Education
======
* Ph.D. in Computer Science and Engineering, The Ohio State University, Aug 2019 – Present (GPA: 3.93/4.0)
* M.S. in Computer Science and Engineering, University of Minnesota Duluth, Aug 2016 – Jul 2018 (GPA: 3.95/4.0)
* B.Tech. in Computer Science and Engineering, VNRVJIET (JNTU-Hyderabad), Sept 2009 – May 2013 (GPA: 3.90/4.0)

Work Experience
======
* Aug 2019 – Present: Graduate Research Assistant
  * The Ohio State University, Columbus, OH
  * Academic Advisor: Dr. Rajiv Ramnath

* June 2025 – Aug 2025: SGX3 Summer Fellow
  * Texas Advanced Computing Center (TACC), University of Texas at Austin, Austin, TX
  * Supervisor: Dr. Joe Stubbs

* June 2024 – Aug 2024: SGX3 Summer Fellow
  * Texas Advanced Computing Center (TACC), University of Texas at Austin, Austin, TX
  * Supervisor: Dr. Joe Stubbs

* June 2023 – Aug 2023: SGX3 Summer Fellow
  * Texas Advanced Computing Center (TACC), University of Texas at Austin, Austin, TX
  * Supervisor: Dr. Joe Stubbs

* May 2022 – July 2022: Teaching Research Fellow (Summer India)
  * VNRVJIET, Hyderabad, Telangana, India

* June 2021 – Aug 2021: Research Intern
  * Oak Ridge National Laboratory (remote), Columbus, OH
  * Supervisor: Dr. Matthew Wolf

* Aug 2018 – July 2019: Web Application Developer
  * Spherexx.com, Tulsa, OK
  * Developed a full-stack voice bot application (C#, .NET MVC) with a Python ML classifier (NumPy, Pandas, Scikit-learn) for lease management lead generation and appointment booking.

* May 2017 – July 2017: IT Intern
  * CHART Industries, Tulsa, OK
  * Resolved bugs in ASP.NET in-house application CACHE; improved server-side performance and workflow automation.

* June 2013 – July 2016: Software Engineer (Associate until June 2015)
  * CA Technologies, Hyderabad, Telangana, India — Product: CA XCOM Gateway GA 2.0
  * Developed shippable deployments in Java/InstallAnywhere; implemented automated test suites with Selenium and TestNG; ensured cross-platform compatibility (Oracle, DB2, MySQL; Windows, UNIX, AIX); full Agile–Scrum lifecycle.

* Aug 2016 – May 2018: Graduate Teaching Assistant
  * Computer Science and Engineering, University of Minnesota Duluth

* Autumn 2019: Graduate Teaching Assistant
  * Computer Science and Engineering, The Ohio State University

Current Academic Research
======
**Integrating AI into Research Workflows: Resource Provisioning and AI-Driven Cyberinfrastructure** (Aug 2019 – Present)

Developed an AI-driven framework for optimizing resource allocation and scheduling in HPC and deep learning workflows.
* **AI-Powered Cyberinfrastructure Tool:** Streamlines preprocessing, tool exploration, and software optimization by leveraging past experiences and resources to support researchers in their workflows.
* **Smart Scheduler for Deep Learning:** Framework for optimized resource allocation integrating SLURM to estimate job runtimes; tailored for TensorFlow and PyTorch.
* **HARP Framework for HPC Resource Prediction:** AI-driven system to predict HPC resource needs via historical data analysis, supporting FAIR principles for software generalization across cyberinfrastructures.
* **ML-Driven HPC Resource Allocation:** ML models to predict optimal resource allocation for genome sequencing and similar applications.
* **DNN Resource Estimators:** Architecture-aware estimators leveraging XLA/HLO graph features for hardware-aware resource prediction, scaled across edge and center environments.
* **Rules Engine for Model Adaptation:** Rules-based decision framework integrating HARP and Smart Scheduler insights to autonomously trigger model retraining and fine-tuning across the computing continuum.
* **Agentic System Wrappers with LLM Interfaces (In Progress):** Extending frameworks into agentic, LLM-powered systems for natural language-driven workflow creation and self-updating orchestration.

**AI-Driven Model Adaptation Framework for Edge Deployments in Computational Ecology** (Aug 2024 – Present)

Toolkit enabling field researchers to deploy and evaluate AI models directly on edge devices for tasks such as intrusion detection and blank filtering in camera-trap imagery.
* **ML Field Planner (TAPIS UI):** Guided interface for selecting model, dataset, and target device; launches controlled benchmarks under edge constraints.
* **CKN Dashboard for Camera Traps:** Knowledge-network visualization for comparing runtime, memory, latency, precision, and recall across experiments.
* **ML Edge Server:** Dockerized plug-and-play edge stack assembling configurable workflow stages (e.g., blank deletion, species-detection alerts).
* **CT-Controller:** Control UI to deploy, manage, and verify models/workflows on edge devices.

**(Masters) Discovering Hypernyms for New Senses in WordNet** (Aug 2017 – May 2019)

Applied Hearst Patterns, regular expressions, and word2vec models to identify insertion points for new word senses in WordNet; contributed to SemEval 2016 Task 14 and SemEval 2018 Task 9; published peer-reviewed paper at SemEval@NAACL-HLT 2018.

Publications
======
* Hassan, A. Z., Vallabhajosyula, M. S., & Pedersen, T. (2018). UMDuluth-CS8761 at SemEval-2018 Task 9: Hypernym discovery using Hearst patterns, co-occurrence frequencies and word embeddings. *arXiv:1805.10271*.
* Vallabhajosyula, M. S., and Ramnath, R. "Towards Practical, Generalizable Machine-Learning Training Pipelines to build Regression Models for Predicting Application Resource Needs on HPC Systems." *PEARC 2022*, pp. 1–5.
* Vallabhajosyula, S. and Ramnath, R. "Establishing a Generalizable Framework for Generating Cost-Aware Training Data and Building Unique Context-Aware Walltime Prediction Regression Models." *IEEE ISPA/BDCloud/SocialCom/SustainCom*, Melbourne, Australia, 2022, pp. 497–506. doi: 10.1109/ISPA-BDCloud-SocialCom-SustainCom57177.2022.00070.
* **[BEST PAPER]** Vallabhajosyula, M. S., and Ramnath, R. "Insights from the HARP Framework: Using an AI-Driven Approach for Efficient Resource Allocation in HPC Scientific Workflows." *PEARC 2023*, pp. 341–344.
* Vallabhajosyula, M. S., Guzman, C., Ramnath, R., and Stubbs, J. "Demonstrating HARP (HPC Application Resource Predictor) Framework for Predicting Walltime for Single Node Applications."
* Vallabhajosyula, M. S., Budhya, S. S., and Ramnath, R. "Reference Implementation of Smart Scheduler: A CI-Aware, AI-Driven Scheduling Framework for HPC Workloads." *PEARC 2024*, pp. 1–4.
* **[BEST PAPER]** Stubbs, J., Balasubramaniam, S., Khuvis, S., Withana, S., Vallabhajosyula, S., Cardone, R., Garcia, C., Freeman, N., Guzman, C., Plale, B., Ramnath, R., and Berger-Wolf, T. "ML Field Planner: Analyzing and Optimizing ML Pipelines For Field Research." *PEARC 2024: Human Powered Computing*. 2025.
* Reddy, S., Davis, R., Vallabhajosyula, S., and Ramnath, R. "Building a Lab-scale Cyberinfrastructure for Fun and Profit." *PEARC 2024: Human Powered Computing*. 2025.
* Cliffel, N., Vallabhajosyula, M. S., Wang, J., Zhang, Z., and Ramnath, R. "Unified Component API: Supporting Standardized Middleware Integration and Flexible Interoperability in Cyberinfrastructure." *Science Gateways 2025 (SG25)*, Green Bay, WI.
* **[Extended Abstract – WHPC Workshop]** Vallabhajosyula, M. S., and Ramnath, R. "Predicting Resources for AI Workloads in HPC: Methods, Challenges, and Opportunities." *SC'25*, St. Louis, MI.

MS Thesis and Mentored Project Reports
======
1. *(MS Thesis)* "Hypernym Discovery over WordNet and English Corpora — using Hearst Patterns and Word Embeddings", S. Vallabhajosyula, T. Pedersen. <https://hdl.handle.net/11299/200144>
2. "Information Extraction from Gene Sequencing Scientific Documents", Rishabh Chanana, May 2021.
3. "Generating Knowledge Graphs on Scientific Execution Workspace", Akhilesh Gulati, December 2020.
4. "HARP – HPC Application Runtime Predictor", Prasanna, Saishree Miriyala, December 2022.
5. "Reference Implementation of Smart Scheduler: Configuring a pre-SLURM Database for Enabling Smart Scheduler", Akanksha Jain, May 2024.
6. "Reference Implementation of Smart Scheduler: Establishing a Smart Scheduler Framework Backend – Intelligence Plane", Sandeep Satish Budhya, May 2024.
7. "AI-Enabled Smart Scheduler for Optimizing Resource Utilization in HPC", Bhargavi Dwivedi (MS-ECE).
8. "Exploring and Building Profilers for HPC Environments" (Bachelor's), Maaz Baig.
9. "Parallelizing Training and Inferencing for Machine Learning Models: A Study on HLO Graphs for Network Optimization", Shashwat Rao.
10. "GPU Resource Prediction Dataset for DNN Workloads", Rahul Vaidhya.
11. "Exploring Different Regression Models for Runtime Prediction on Black-Box and White-Box Resource Profiles for DNN Training Time Estimation", Nachiappan Ramasamy.

Presentations and Posters
======
1. Vallabhajosyula, M. S. (2018): Identifying Hypernym for a New Sense in WordNet. figshare. <https://doi.org/10.6084/m9.figshare.22565089.v1>
2. Vallabhajosyula, M. S.; Ramnath, R. (2020): EAGER: Bridging the Last Mile. figshare. <https://doi.org/10.6084/m9.figshare.11777808.v3>
3. Vallabhajosyula, M. S.; Ramnath, R. (2021): Modeling A Framework To Estimate Resource Requirements For Scientific Workflows. figshare. <https://doi.org/10.6084/m9.figshare.22363183.v1>
4. Chanana, R.; Vallabhajosyula, M. S.; Ramnath, R. (2021): Using synthesized data to train machine learning models used in genome engineering pipeline. figshare. <https://doi.org/10.6084/m9.figshare.22565113.v1>
5. Vallabhajosyula, M. S.; Ramnath, R. (2022): Building an AI-powered Assistant for Computational Scientists. figshare. <https://doi.org/10.6084/m9.figshare.11777796.v1>
6. Vallabhajosyula, M. S.; Ramnath, R. (2023): Modeling A Framework To Estimate Resource Requirements For Scientific Workflows. figshare. <https://doi.org/10.6084/m9.figshare.22363183.v1>
7. Vallabhajosyula, M. S., and Ramnath, R. "Towards Characterizing DNNs to Estimate Training Time using HARP." *PEARC 2023*, pp. 483–485.
8. Vallabhajosyula, M. S., Ramnath, R., and Stubbs, J. "Custom Cost, Loss, And Reward Functions to Train Regression Models for Estimating Execution Resources using HARP." *Science Gateways 2023 (SG23)*, Pittsburgh, PA.
9. Vallabhajosyula, S., Budhya, S. S., Baig, M., Jain, A., and Ramnath, R. "Orchestrating a DNN training job using an iScheduler Framework: a use case." *PEARC 2024*.
10. Vallabhajosyula, S., Freeman, N., Garcia, C., Stubbs, J., and Ramnath, R. "Orchestrating End-to-End AI-Model Development using TAPIS and Smart Scheduler." *Science Gateways 2023 (SG23)*, Bozeman, MO.
11. Vallabhajosyula, M. S., Vaidhya, R., Ramasamy, N., and Ramnath, R. *Hybrid black-box and white-box approaches for efficient resource prediction for AI workloads in high-performance computing* [Project poster]. ISC-HPC 2025, Hamburg, Germany.
12. Vallabhajosyula, M. S., Tomko, K., and Ramnath, R. *Intelligence Plane: A framework for machine learning application life-cycle management* [Research poster]. ISC-HPC 2025, Hamburg, Germany.
13. Vallabhajosyula, M. S. *Motivated by challenges: Harnessing AI to revolutionize resource and workflow management in high-performance computing* [Women in HPC poster]. ISC-HPC 2025, Hamburg, Germany.
14. "AI-Driven Resource Optimization for High-Performance Computing: A Comprehensive Framework." *IHPCSS 2025*, Lisbon, Portugal.
15. Vallabhajosyula, S., Molakalmuru, G., Cliffel, N., and Ramnath, R. "Beyond Automation: Integrating Agentic Capabilities into MLOps with ICICLE Infrastructure." *PEARC 2025*.
16. Molakalmuru, G. G., Vallabhajosyula, M. S., Khuvis, S., Stubbs, J. F., and Ramnath, R. "Operational Considerations for Real-Time ML Pipelines on Edge Devices." *SG25*, Green Bay, WI.
17. Vallabhajosyula, M. S., Molakalmuru, G. G., Karthikeyan, N., Gamage, A. I., Khuvis, S., Freeman, N., Stubbs, J., Plale, B., and Ramnath, R. "Beyond Accuracy: The ML Field Planner's Framework for AI Model Selection in Conservation." *SG25*, Green Bay, WI.
18. [Portal] Vallabhajosyula, M. S., et al. "ML Field Planner with TAPIS: Configuring and Analyzing AI Models for Animal Ecology." *SG25*, Green Bay, WI.
19. [Doctoral Showcase] Vallabhajosyula, M. S., and Ramnath, R. "AI-Driven Resource Optimization for High-Performance Computing: A Comprehensive Framework." *SC'25*, St. Louis, MI.

Teaching
======
As a Graduate Teaching Assistant, assisted in the following courses:
* Programming: C++, Java
* Computing Ethics
* Natural Language Processing
* Web Technologies: HTML, CSS, JavaScript

During the undergraduate senior year, taught Android Programming to junior undergraduates. Guided more than 200 undergraduates through summer capstone courses.

Software Proficiency
======
* **Programming / Testing:** C, C++, C#, Core Java, J2EE, Python, Perl, Shell, Batch, TestNG, Selenium
* **Web Development:** HTML5, CSS, JavaScript, ASP.NET, ReactJS, VueJS, Node.js, REST APIs, Docker/Singularity, Kafka
* **Servers and Frameworks:** Tomcat, JBOSS, TAPIS API Framework, Flask, FastAPI, Selenium WebDriver
* **Operating Systems:** Windows Server, UNIX, AIX, Linux (Ubuntu/CentOS)
* **Profilers and HPC Tools:** NVIDIA-SMI, Nsight Systems, SLURM, TensorBoard, TAU
* **Databases:** MySQL, Oracle 11g/12c, DB2 LUW, DB2 z/OS, MS-SQL, MongoDB, PostgreSQL
* **AI / ML Frameworks:** TensorFlow, PyTorch, Keras, Horovod (Distributed Training), Hugging Face Transformers, Scikit-learn, Pandas, NumPy, OpenCV, NetworkX
* **Application Lifecycle Management:** Agile Scrum, Scrumban, Waterfall, CI/CD (GitHub Actions, Jenkins), MLOps (MLflow, Weights & Biases)

Awards, Certifications and Service
======
* **ICICLE NextGen Student Group Manager** (June 2023 – present): Collaborated with 280+ students from various universities; led K–12 AI literacy outreach as part of the HACK/IO series.
* **Academic Awards:**
  * Computer Science and Engineering (The OSU) Best Graduate Student Research Award, 2026
  * PEARC25 Best Paper: Systems & Applications Software Track and Phil Andrews Award for Best Paper Overall
  * PEARC23 Best Paper: Systems & Systems Software Track (Overall & Student Categories) and Phil Andrews Award for Best Paper Overall
  * Honorable Mention for Best Research, OSU College of Engineering, 2024
  * Honorable Mention for Best Research, CSE Annual Research Poster Exhibit
  * Undergraduate Third-Best Academic Project (CSE)
* **Professional Awards:** Above & Beyond, September 2014 and March 2016 @ CA Technologies (Broadcom)
* **Travel Awards:**
  * PEARC 2024 & 2025 Student Volunteer Travel Awards
  * Science Gateways 2023, 2024 & 2025 Travel Grants
  * Supercomputing (SC) 2025 SCinet Travel Grant
  * International HPC Summer School (IHPCSS) Grant, Lisbon, Portugal
  * SAIL Graduate Student Researcher Keynote Speaker and GSR Travel Grant, 2025
* **Invited Talks:** Summit of AI Institute Leadership (SAIL) Graduate Student Researcher Keynote Speaker
* **Scholarships:** Fully Funded Master's Program, University of Minnesota (full tuition and stipend for both M.S. years)
* **Soft Skill Certifications:** Leaders at All Levels @ CA Technologies; JAWS

Please find my latest resume [here](http://manikyaswathi.github.io/files/ManikyaSwathi_Vallabhajosyula_cv.pdf)

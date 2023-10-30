---
layout: archive
title: "Know Your Resource Needs: Using HARP to Estimate Resource Requirements for Running an Application"
permalink: /HARP_Portal/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

List of Contents
=====
1. HARP GitHub 
2. How much and How Long?
3. HARP - HPC Application Runtime Predictor
4. HARP Portal - In progress for Live - snapshots 
5. Publications and Presetations

# GitHub
The code for HARP and the contaner Images could be found here: https://github.com/ICICLE-ai/harp

# How much and How Long?
![Why HARP?](/images/HowWellYouKnowYourJob.png)

Scientific workflows rely on High-Performance Computing (HPC), where varying hardware and software requirements are critical. Choosing the correct execution environment is vital for optimal resource utilization. Yet, users frequently encounter difficulties with manual approaches, resulting in suboptimal allocation and underutilization. Maximizing HPC efficiency in research requires users to comprehend their workflows and execution environments. To accurately estimate resource needs, machine learning models with workflow-specific data are essential. This work highlights the challenges of manual workflow optimization and promotes the use of AI-driven frameworks for precise application resource estimation and optimal allocation recommendations.


# HARP - HPC Application Runtime Predictor

HARP stands for "HPC Application Resource (runtime) Predictor." It is a solution introduced in the context of high-performance computing (HPC) to help optimize resource allocation for scientific tasks. HARP utilizes prediction-based recommendations and aims to improve the efficient use of resources in HPC environments by considering specific resource requirements and batch queueing policies. HARP emulates scientific workflows, estimates resource requirements, and incorporates policy-driven resource management to optimize HPC utilization and improve efficiency.

![Why HARP?](/images/WhyHARP.png)

## Components of HARP
The HARP (HPC Application Resource Predictor) framework consists of several key components:

1. Workflow Emulation Module: This module is responsible for emulating scientific workflows, capturing how different tasks within a workflow interact with HPC resources. It profiles the usage requirements of workflows.

2. Resource Requirement Estimation Module: Using data gathered from the workflow emulation, this module estimates the resource requirements for future job executions. It utilizes regression models to predict memory and execution times accurately.

3. Policy-Driven Component: This component allows users to define and enforce policies for resource allocation. Users can customize rules for job prioritization, resource reservation, and other resource management aspects.

## Executing HARP from TAPIS
We've developed HARP containers for seamless integration with TAPIS. The HARP modules can run as TAPIS applications. The following Colab notebooks demonstrate the execution of HARP for profiling an example application (Euler Number) on both OSC and TACC systems:

* OSC Example: https://colab.research.google.com/drive/19GNHVNE6_b52JepLud1cpeVhg9ApgSlq
* TACC Example: https://colab.research.google.com/drive/1317dQqaKlGqcNULlOPP7i9i_vEvgYbWe

# HARP Portal - In progress for Live - snapshots 

Below are a couple pf screenshots from portal.

![Why HARP?](/images/Harp_portal1.png)

The above image shows the features corelation and the influence of features on Walltime

![Why HARP?](/images/Harp_portal2.png)

This is a sample cost-time output from the regression models results parsed to CI policied and billings. 

# Publications and Presetations
Publications
======
* Vallabhajosyula, Manikya Swathi, and Rajiv Ramnath. "Towards Practical, Generalizable Machine-Learning Training Pipelines to build Regression Models for Predicting Application Resource Needs on HPC Systems." Practice and Experience in Advanced Research Computing. 2022. 1-5.
* Vallabhajosyula and R. Ramnath, "Establishing a Generalizable Framework for Generating Cost-Aware Training Data and Building Unique Context-Aware Walltime Prediction Regression Models," 2022 IEEE Intl Conf on Parallel & Distributed Processing with Applications, Big Data & Cloud Computing, Sustainable Computing & Communications, Social Computing & Networking (ISPA/BDCloud/SocialCom/SustainCom), Melbourne, Australia, 2022, pp. 497-506, doi: 10.1109/ISPA-BDCloud-SocialCom-SustainCom57177.2022.00070.
* Vallabhajosyula, Manikya Swathi, and Rajiv Ramnath. " Insights from the HARP Framework: Using an AI-Driven Approach for Efficient Resource Allocation in HPC Scientific Workflows" http://camps.aptaracorp.com/ACM_PMS/PMS/ACM/PEARC23/70/3a84c88c-f988-11ed-b37c-16bb50361d1f/OUT/pearc23-70.html

  
Presentations and Posters
=====
* Vallabhajosyula, Manikya Swathi; Ramnath, Rajiv (2020): EAGER: Bridging the Last Mile. figshare. Poster. https://doi.org/10.6084/m9.figshare.11777808.v3
* Vallabhajosyula, Manikya Swathi; Ramnath, Rajiv (2021): Modeling A Framework To Estimate Resource Requirements For Scientific Workflows. figshare. Poster. https://doi.org/10.6084/m9.figshare.22363183.v1
* Vallabhajosyula, Manikya Swathi; Ramnath, Rajiv (2022): Building an AI-powered Assistant for Computational Scientists. figshare. Poster. https://doi.org/10.6084/m9.figshare.11777796.v1
* Vallabhajosyula, Manikya Swathi; Ramnath, Rajiv (2023): Modeling A Framework To Estimate Resource Requirements For Scientific Workflows. figshare. Poster. https://doi.org/10.6084/m9.figshare.22363183.v1
* Vallabhajosyula, Manikya Swathi; Ramnath, Rajiv (2023): Towards Characterizing DNNs to Estimate Training Time using HARP (HPC Application Resource (runtime) Predictor http://camps.aptaracorp.com/ACM_PMS/PMS/ACM/PEARC23/82/138a150e-f8dd-11ed-b37c-16bb50361d1f/OUT/pearc23-82.html


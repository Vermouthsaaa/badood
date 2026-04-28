---
title: "Bad-OOD: Discovering Harmful Synthetic Diffusion Outliers via Confidence Calibration"
conference: "**** ****"
summary: "Utilizing synthetic outlier samples has shown great promise in out-of-distribution (OOD) detection. In particular, impressive results have been achieved by employing diffusion models to generate synthetic outliers in the low-density manifold. However, guiding diffusion models to generate meaningful synthetic outliers remains challenging. The synthesized samples often fall either too close to the in-distribution (ID) data (risking overlap and ambiguity) or too far (leading to visually unrealistic results). Both extremes have been shown to degrade OOD detection performance. In this work, we propose a novel OOD synthesis framework that combines a pre-trained Representation Diffusion Model (RDM) with a simple yet effective classifier calibration strategy. RDM enables global semantic embedding generation without requiring auxiliary labels or text, producing diverse yet ID-relevant outliers, thereby facilitating a more compact ID-OOD decision boundary. To ensure the utility of these samples, we calibrate a binary classifier on both ID data and synthesized OODs to assign confidence-based anomaly scores. We find that mid-confidence outliers, i.e., those balancing realism and deviation, are most informative, and using them significantly boosts detection performance. Extensive experimental results validate the superiority of our calibrated OOD sampler over several strong baselines."
affiliations:
  - index: "1"
    name: "Beijing University of Posts and Telecommunications"
  - index: "2"
    name: "HAOHAN Data"
footnote: "*Corresponding author"
teaser: "pipeline.png"
authors:
  - name: "Donglin Ni"
    superscript: "1"
    url: "#"
  - name: "Zhixin Feng"
    superscript: "1"
    url: "#"
  - name: "Ke Li"
    superscript: "1"
    url: "#"
  - name: "Yue Zhang"
    superscript: "2"
    url: "#"
  - name: "Yonggang Qi"
    superscript: "1*"
    url: "https://qugank.github.io/"
links:
  - label: "Paper"
    url: "#paper"
  - label: "arXiv"
    url: "#"
  - label: "Code"
    url: "#"
  - label: "Project"
    url: ""
teaser_caption: "Overview of our proposed method Bad-OOD. Bad-OOD generates OOD samples via minority guidance, trains a detector, applies beta calibration to filter low/high-confidence OOD samples, and retrains the detector from scratch using the refined set."

results_image: "results.png"
results_caption: "OOD detection results for IMAGE-NET-100 and CIFAR-100 as the in-distribution data."

visual_image: "visual.png"
visual_images:
  - "visual.png"
  - "visual2.png"
  - "visual3.png"
visual_caption: "ID reference samples and synthetic OOD of class broccoli, candle, starfish and strawberry. The anomaly score is provided in the upper right of each sample."
visual_caption_secondary: "OOD samples of class candle and jeep. For OOD-II and OOD-III, the class predicted by CLIP is demonstrated under each image."

contributions:
  - "Calibration-aware OOD synthesis: We unify diffusion-based generation and confidence calibration to jointly improve outlier diversity and reliability."
  - "Minority-guided latent diffusion: We introduce a guidance strategy that drives sampling toward informative low-density regions while preserving semantic alignment."
  - "Two-stage training with outlier filtering: We show that selecting mid-confidence OOD samples leads to more compact decision boundaries and stronger detection performance."

bibtex: |
  @inproceedings{,
    title={Bad-OOD: Discovering Harmful Synthetic Diffusion Outliers via Confidence Calibration},
    author={},
    booktitle={},
    year={}
  }
---

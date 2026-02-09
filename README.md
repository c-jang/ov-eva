# Robust Vision-Language Alignment Using Multi-Modal Large Language Models for Open-Vocabulary Semantic Segmentation

[![Paper Status](https://img.shields.io/badge/Paper-Accepted-brightgreen)]([Link to Paper])
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This is the official PyTorch implementation of the paper: **"Robust Vision-Language Alignment Using Multi-Modal Large Language Models for Open-Vocabulary Semantic Segmentation"**.  
Authors: Cheolhun Jang, Seok Jun Youn, Issac Kang, Junhyeong Kwon, Daehyun JI, Jun Won Choi and Nam Ik Cho  
Accepted at IEEE Access.

> **🚧 Code Coming Soon 🚧**
>
> The code used in the paper is currently being cleaned up and will be uploaded soon. Thank you for your patience!

## Abstract

> Open-vocabulary semantic segmentation (OVSS) aims to segment objects without being constrained by a predefined set of categories. Recent advancements in OVSS have been driven by CLIP, a powerful vision-language model that enables segmentation through textual and visual feature matching. However, while visual features within a class exhibit significant diversity, their corresponding text features remain relatively limited in distribution. This discrepancy weakens the effectiveness of vision-language matching for OVSS. To address these challenges, we propose OV-EVA (Open-Vocabulary Semantic Segmentation with Enhanced Vision-Language Alignment), a novel training-free OVSS framework that leverages multi-modal large language models (MLLMs) to improve visual-language alignment and enhance segmentation robustness. Our method introduces an iterative vocabulary expansion strategy, where MLLMs generate a diverse and scene-relevant vocabulary set through a two-stage querying process. To ensure accurate segmentation, we incorporate a mask-guided score refinement mechanism, which enhances vocabulary terms closely aligned with the target mask while mitigating overly dominant terms across the entire image. Additionally, we introduce a top-$N$-based target class mapping strategy to improve the alignment between the generated vocabulary set and target class labels. The proposed OV-EVA achieves state-of-the-art performance across multiple benchmarks when using GPT-4o as the underlying MLLM. Furthermore, our approach demonstrates strong adaptability across different MLLMs, achieving competitive results with LLaVA and Janus-Pro. These findings suggest that leveraging generative reasoning from MLLMs offers a scalable pathway for robust zero-shot perception without task-specific training. Future work will focus on optimizing computational efficiency to facilitate real-time deployment in practical applications. The source code is available at https://github.com/c-jang/ov-eva.

## Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/woori21c/dfag.git](https://github.com/woori21c/ov-eva.git)
    cd dfag
    ```

2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
    *(Note: The `requirements.txt` file will be uploaded along with the source code.)*

## Usage

(This section will be updated once the code is uploaded.)

#### **Training**

To train the model, run the following command:
```bash
python train.py --config [path_to_config_file]

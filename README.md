# Graph Attention Network (GAT) Project

This repository contains my implementation of a **multi-head Graph Attention Network (GAT)** built for a Kaggle competition with a **17 million-row binding-affinity dataset**. Developed in **PyTorch Geometric**, it predicts molecular interactions, achieving **92.81% accuracy** and a **29% F1 score improvement** (0.61 → 0.79). Optimized for an RTX 4080 with VRAM constraints.

# Data Files
- Test and Train files can be found here: https://www.kaggle.com/competitions/leash-BELKA/data
- Files created by notebook (Such as gat model, graph strucutes, etc) not included as they are created by notebook.

## Overview
- **Duration**: May 2024 – September 2024  
- **Goal**: Predict binding affinity of molecules using graph-based ML on a massive dataset (~500K training graphs, 1.67M test molecules).  
- **Key Results**:  
  - Accuracy: **92.81%**  
  - F1 Score: Improved from 0.61 to **0.79** (+29%)  
  - Inference enabled on 1.67M test molecules via data chunking  

## Features
- **Multi-head GAT**: Leverages attention mechanisms for molecular graph modeling.  
- **Class Imbalance Handling**: Weighted loss and gradient clipping for stability.  
- **Memory Optimization**: Chunked dataset into 4 partitions (~418K graphs each) to fit RTX 4080 VRAM, hitting **90% utilization** without crashes.  

## Tech Stack
- **Languages**: Python  
- **Frameworks**: PyTorch, PyTorch Geometric, NumPy, Pandas  
- **Hardware**: NVIDIA RTX 4080  
- **Tools**: Git, Command Line  

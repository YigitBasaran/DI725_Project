# Remote Sensing Image Captioning with PaliGemma and LoRA

This project investigates the use of **Low-Rank Adaptation (LoRA)** for parameter-efficient fine-tuning of **PaliGemma**, a large vision–language model, for the task of **remote sensing image captioning (RSIC)**. The goal is to adapt a general-purpose model to the satellite imagery domain using minimal resources, demonstrating high performance with low computational cost.

## 🔍 Project Overview

- **Model**: PaliGemma (3B) from Google (vision–language transformer)
- **Fine-Tuning Method**: LoRA (Low-Rank Adaptation)
- **Dataset**: RISC — 44,521 satellite images with 5 captions each
- **Task**: Generate natural language captions for satellite images
- **Evaluation Metrics**: BLEU, METEOR, ROUGE-L
- **Outcome**: LoRA-1 configuration achieved the best performance with only ~0.077% of model parameters updated.

## 📁 Repository Structure

- `./notebooks`:  
  - `DataPreprocessing_Paligemma_Training_Validation_Testing.ipynb`:  
    Complete pipeline for data filtering, model preparation, LoRA integration, fine-tuning, and evaluation.
    
  - `ExplonatoryDataAnalysis.ipynb`:  
    Initial data exploration including caption length distribution, n-gram frequency, and duplication analysis.

- `./figures`: Contains figures of the project.

- `./data`:
  - `captions.csv`: Captions and related written data of the used dataset.
  - `./Resized`: The folder contains the image data.        

- `requirements.txt`:  
  Python dependencies required to run the notebooks and reproduce experiments.

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YigitBasaran/DI725_Project.git
cd DI725_Project


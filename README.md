# Whisper Fine-Tuning

A plug-and-play framework for fine-tuning OpenAI Whisper models for Automatic Speech Recognition (ASR), with support for both **LoRA fine-tuning** and **Full Fine-Tuning**.

The project is designed to make adapting Whisper to custom datasets and low-resource languages straightforward.

## Features

- **LoRA Fine-Tuning:** Parameter-efficient training with fewer trainable parameters and lower memory requirements. Recommended for low resource language when the dataset is not huge and have a limited VRAM of GPU. 
- **Full Fine-Tuning:** Update the model's parameters for greater flexibility when adapting to a target language or domain. This is recommended when the dataset is very huge, Lora is not improving the model generalization capability and have an ample amount of GPU or VRAM.  
- **Custom Datasets:** Adapt the pipelines to your own speech datasets.
- **Configurable Training:** Customize model selection, training parameters, and dataset paths.
- **ASR Evaluation:** Evaluate model performance using Word Error Rate (WER).

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Muhammadmudassir180/Whisper-Fine-Tuning.git
cd Whisper-Fine-Tuning
```

### 2. Install Dependencies

Dependencies will be automatically installed by running the 2nd cell of python notebook

### 3. Prepare Your Dataset

Configure your dataset paths and ensure your data matches the format expected by the selected training pipeline.

### 4. Configure Training

Update the relevant configuration settings, including:

- Pretrained Whisper model
- Dataset paths
- Output directory
- Batch size and gradient accumulation
- Learning rate and number of epochs

### 5. Start Fine-Tuning

Run the training script corresponding to your preferred approach


## Choosing a Pipeline

| Feature | LoRA | Full Fine-Tuning |
|---|---|---|
| Trainable parameters | Fewer | All model parameters |
| Memory requirements | Generally lower | Generally higher |
| Training flexibility | Parameter-efficient adaptation | Full model adaptation |
| Best suited for | Resource-efficient experiments | Full model adaptation |

## Customization

You can adapt the pipelines to different languages, domains, and speech datasets by updating the configuration and dataset preparation steps. Multiple languages are supported in this pipeline. 


**Contributions and feedback are welcome!**

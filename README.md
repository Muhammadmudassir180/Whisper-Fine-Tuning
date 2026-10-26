# Whisper Fine-Tuning

A plug-and-play framework for fine-tuning OpenAI Whisper models for Automatic Speech Recognition (ASR), with support for both **LoRA fine-tuning** and **Full Fine-Tuning**.

The project is designed to make adapting Whisper to custom datasets and low-resource languages straightforward.

## Features

- **LoRA Fine-Tuning:** Parameter-efficient training with fewer trainable parameters and lower memory requirements.
- **Full Fine-Tuning:** Update the model's parameters for greater flexibility when adapting to a target language or domain.
- **Custom Datasets:** Adapt the pipelines to your own speech datasets.
- **Configurable Training:** Customize model selection, training parameters, and dataset paths.
- **ASR Evaluation:** Evaluate model performance using Word Error Rate (WER).

## Getting Started

### 1. Clone the Repository

```bash
git clone <YOUR_REPOSITORY_URL>
cd <YOUR_REPOSITORY_NAME>
```

### 2. Install Dependencies

Create and activate a Python virtual environment, then install the required dependencies:

```bash
pip install -r requirements.txt
```

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

*Replace the script names with the actual filenames in your repository.*

## Choosing a Pipeline

| Feature | LoRA | Full Fine-Tuning |
|---|---|---|
| Trainable parameters | Fewer | All model parameters |
| Memory requirements | Generally lower | Generally higher |
| Training flexibility | Parameter-efficient adaptation | Full model adaptation |
| Best suited for | Resource-efficient experiments | Full model adaptation |

## Customization

You can adapt the pipelines to different languages, domains, and speech datasets by updating the configuration and dataset preparation steps.

## License

Check the licenses of the pretrained model, datasets, and dependencies before using this project. Add your repository's license here.

---

**Contributions and feedback are welcome!**

# IMAGE-GENERATION-USING-COMFY-UI-AND-STABLE-DIFFUSION

## AICTE Internship Project – AI: Transformative Learning with TechSaksham

This project explores the integration of Stable Diffusion and ComfyUI to generate images from text prompts. ComfyUI’s node-based interface offers a flexible and intuitive approach to designing complex image generation workflows, making Stable Diffusion more accessible and customizable.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
  - [Hardware](#hardware)
  - [Software](#software)
- [Installation](#installation)
- [Usage](#usage)

## Introduction
Stable Diffusion is a cutting-edge deep learning model designed to generate high-quality images based on textual inputs. ComfyUI enhances the user experience by providing a visual programming environment, enabling users to create custom image generation workflows. This project combines both tools to deliver a seamless and interactive image creation process.

## Features
- **Intuitive Visual Workflow**: Utilize ComfyUI’s node-based interface to design and manage image generation pipelines effortlessly.
- **Text-to-Image Capability**: Generate realistic images directly from textual descriptions.
- **Adjustable Parameters**: Fine-tune settings to achieve distinct artistic styles and enhance image quality.
- **Modular Workflow**: Easily add, remove, or modify nodes within ComfyUI to experiment with different configurations.
- **Real-time Preview**: (If supported) View live previews of images as parameters are adjusted, streamlining the creative process.
- **Expandable with Custom Scripts**: Integrate personalized Python scripts and nodes for advanced functionality.

## Requirements
### Hardware
- **Operating System**: Windows 10/11, macOS, or Linux (Linux recommended for optimal performance).
- **CPU**: Multi-core processor.
- **GPU**: NVIDIA GPU with at least 8GB VRAM (12GB+ recommended). AMD GPUs may require additional configuration and might have reduced performance.
- **RAM**: Minimum 16GB (32GB+ recommended).
- **Storage**: SSD with sufficient free space.

### Software
- **Python 3.8+** (Recommended: 3.10 or 3.11).
- **ComfyUI** (Download from the official repository).
- **Stable Diffusion Model Checkpoint** (Compatible .ckpt or .safetensors model file required).
- **Required Python Libraries** (Install via pip):
  ```bash
  pip install torch torchvision torchaudio transformers numpy Pillow Flask requests tqdm filelock gradio omegaconf
  ```
  *(Note: Ensure PyTorch installation matches your CUDA version if using an NVIDIA GPU. Refer to PyTorch documentation for details.)*

## Installation
1. **Install Python**: Make sure Python 3.8 or later is installed (preferably 3.10 or 3.11).
2. **Download and Install ComfyUI**:
   - Clone the GitHub repository:
     ```bash
     git clone <ComfyUI-Repository-URL>
     ```
   - Follow the repository’s setup instructions.
3. **Download Stable Diffusion Model**:
   - Obtain the `v1-5-pruned-emaonly-fp16` model from Hugging Face.
   - *(Provide the Hugging Face model link if applicable).*
4. **Place Model Checkpoint**:
   - Move the downloaded model file to:
     ```
     ComfyUI_windows_portable\ComfyUI\models\checkpoints
     ```
   - This location is necessary for ComfyUI to detect the model during initialization.
5. **Install Dependencies**:
   - Open a terminal/command prompt, navigate to the ComfyUI directory, and create a virtual environment:
     ```bash
     python3 -m venv .venv
     source .venv/bin/activate  # (Linux/macOS)
     .venv\Scripts\activate  # (Windows)
     ```
   - Install required libraries:
     ```bash
     pip install torch torchvision torchaudio transformers numpy Pillow Flask requests tqdm filelock gradio omegaconf
     ```
6. **Run ComfyUI**:
   - Launch ComfyUI following its documentation.
   - The model checkpoint should be automatically recognized upon startup if placed in the correct directory.

## Usage
1. **Launch ComfyUI**: Open ComfyUI as per its documentation.
2. **Load Workflow (Optional)**: Load a pre-configured workflow or create one from scratch.
3. **Enter Text Prompt**: Input the text description in the appropriate ComfyUI node.
4. **Modify Parameters**: Adjust various settings within the workflow to refine image output.
5. **Generate Image**: Execute the workflow to produce an image.
6. **View and Save Output**: Review the generated image within ComfyUI and save it as needed.

---

This README provides all essential information for setting up and using Stable Diffusion with ComfyUI. Feel free to update it with additional details or example images!



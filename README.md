# Practical No. 05: Image Generation using Pretrained Stable Diffusion

## Student Information

- **Name:** Mit Jangid
- **PRN:** 202401110072
- **Batch:** A1
- **Subject:** Generative AI

## Aim

To implement a pretrained Stable Diffusion model using the Hugging Face Diffusers library to generate images from text prompts and analyze the impact of inference steps, guidance scale, and different sampling methods on generated-image quality.

## Model Used

**DreamShaper 8 – `Lykon/dreamshaper-8`**

DreamShaper 8 is a Stable Diffusion 1.5-based fine-tuned model used for text-to-image generation.

The model is loaded using the Hugging Face Diffusers library and executed on a Google Colab Tesla T4 GPU using FP16 precision.

## Implementation Details

- Image resolution: 384 × 384 pixels
- Device: NVIDIA Tesla T4 GPU
- Precision: FP16 (half precision)
- Random seed: 42
- Library: Hugging Face Diffusers

## Experiments Performed

### 1. Effect of Inference Steps

The number of denoising steps is varied while keeping the prompt and guidance scale fixed.

- 10 steps
- 20 steps
- 30 steps

Generation time and image quality are compared.

### 2. Effect of Guidance Scale

The guidance scale is varied to analyze how strongly the generated image follows the text prompt.

- 4.0
- 7.5
- 10.0

### 3. Comparison of Sampling Schedulers

Three sampling methods are compared using the same prompt and random seed:

- PNDM
- DDIM
- Euler

### 4. Prompt Engineering

Different descriptive prompts are used to generate images based on:

- Eco-friendly architecture
- Coffee product photography
- Futuristic sustainable cities

### 5. Negative Prompt Comparison

Generated images are compared with and without negative prompts to study their effect on unwanted visual features.

## Technologies Used

- Python
- PyTorch
- Hugging Face Diffusers
- Transformers
- Accelerate
- Safetensors
- NumPy
- Pandas
- Matplotlib
- Google Colab

## Implementation Workflow

1. Install the required libraries.
2. Check GPU availability.
3. Load the pretrained DreamShaper 8 model.
4. Define a reusable image-generation function.
5. Generate an initial image from a text prompt.
6. Experiment with different inference steps.
7. Compare guidance scales.
8. Compare PNDM, DDIM and Euler schedulers.
9. Perform prompt engineering and negative-prompt experiments.
10. Save generated images and experimental results.

## Repository Contents

- `Mit_Jangid_Stable_Diffusion_Practical_05.ipynb` – Complete implementation with executed outputs.
- `README.md` – Practical documentation.

## Conclusion

A pretrained Stable Diffusion model was implemented using the Hugging Face Diffusers library for text-to-image generation. Experiments were conducted to understand the effects of inference steps, classifier-free guidance scale, sampling schedulers, prompt engineering and negative prompts on generated-image quality.

## Author

**Mit Jangid**  
TY AIML | Batch A1

\# Deep Learning: Generative Models



This repository contains deep learning experiments on generative models, image synthesis, semantic face editing, and speech enhancement. The project explores Variational Autoencoders (VAEs), Generative Adversarial Networks (GANs), StyleGAN2, InterfaceGAN, and STE-GAN.



\## Project Overview



The project is organized into three main parts.



\### 1. Variational Autoencoder (VAE) and UNet-VAE



\*\*Notebook:\*\* `dl\_hw3 (1).ipynb`



This section explores variational autoencoders for image reconstruction and generation using face images from the CelebA dataset.



Key activities:

\- Preprocessing and resizing face images to 64 × 64 pixels.

\- Converting images to RGB format and normalizing pixel values.

\- Implementing and training a Variational Autoencoder.

\- Studying latent-space representations and image reconstruction.

\- Exploring the effect of latent-space dimensionality.

\- Implementing a UNet-VAE architecture and comparing its performance with a standard VAE.

\- Evaluating model performance using reconstruction and validation losses.



\### 2. Semantic Face Editing with StyleGAN2 and InterfaceGAN



\*\*Notebook:\*\* `2\_1 (GAN).ipynb`



This section investigates semantic manipulation of facial images using pretrained generative models.



Key activities:

\- Using a pretrained pixel2style2pixel (pSp) encoder and StyleGAN2 generator.

\- Aligning facial images before processing.

\- Mapping real face images into the extended W+ latent space.

\- Extracting latent representations and reconstructing input images.

\- Applying an age-boundary direction obtained using InterfaceGAN.

\- Exploring age-related changes in generated faces through latent-space manipulation.

\- Visualizing the progression of facial appearance while attempting to preserve identity.



\### 3. STE-GAN for Speech Enhancement



\*\*Notebook:\*\* `2\_3,2\_4,2\_5(ste-gan).ipynb`



This section investigates an adversarial deep learning approach for speech enhancement.



Key activities:

\- Preparing clean and noisy speech data.

\- Implementing a generator and discriminator for speech enhancement.

\- Training the adversarial model and monitoring training and validation losses.

\- Analyzing generator and discriminator behavior during training.

\- Comparing clean and enhanced audio waveforms.

\- Examining residual error signals and spectrogram differences.

\- Evaluating enhancement performance using signal-based measures, including signal-to-noise ratio (SNR).



The notebook also includes experiments with an audio recording to examine the model's enhancement behavior.



\## Methods and Concepts



\- Variational Autoencoders (VAE)

\- UNet-VAE

\- Generative Adversarial Networks (GAN)

\- StyleGAN2

\- pixel2style2pixel (pSp)

\- InterfaceGAN and age-boundary manipulation

\- Latent-space extraction and semantic editing

\- Adversarial speech enhancement using STE-GAN

\- Training and validation loss analysis

\- Waveform and spectrogram analysis



\## Technologies and Libraries



The notebooks use Python and deep learning and data-processing libraries, including:



\- PyTorch

\- TorchVision

\- NumPy

\- OpenCV

\- Matplotlib

\- Pillow (PIL)

\- torchaudio

\- tqdm

\- Jupyter Notebook

\- Google Colab



Additional dependencies may be required for pretrained models and external repositories.



\## Datasets and Pretrained Models



The project relies on external datasets and pretrained resources.



\- \*\*CelebA:\*\* Used for face-image preprocessing and VAE experiments.

\- \*\*StyleGAN2 and pSp:\*\* Pretrained components used for face reconstruction and semantic editing.

\- \*\*InterfaceGAN age boundary:\*\* Used to manipulate age-related attributes in the latent space.

\- \*\*Speech datasets:\*\* Clean and noisy speech samples used for STE-GAN training and evaluation.



Datasets, pretrained weights, and supporting repositories may need to be downloaded separately. Their respective licensing terms and usage requirements should be followed.



\## Repository Structure



```text

Deep-Learning-Generative-Models/

├── dl\_hw3 (1).ipynb

├── 2\_1 (GAN).ipynb

├── 2\_3,2\_4,2\_5(ste-gan).ipynb

└── README.md

```



\## How to Run



1\. Clone or download this repository.

2\. Set up a Python environment with the required dependencies.

3\. Open the desired notebook using Jupyter Notebook or Google Colab.

4\. Download the required datasets and pretrained model weights.

5\. Update file paths and configuration settings for your environment.

6\. Execute the notebook cells in order.



GPU acceleration is recommended for deep learning training and inference.



\## Notes



\- Some notebooks depend on external datasets, pretrained checkpoints, or supporting code repositories.

\- File paths may need to be adapted when moving between Google Colab, Kaggle, and local environments.

\- Training time and results depend on the hardware, dataset, model configuration, and hyperparameters.

\- Large datasets, pretrained weights, and personal audio recordings should not be published without checking their size, privacy implications, and redistribution permissions.



\## Acknowledgment



This project was completed as part of a Deep Learning course assignment at Amirkabir University of Technology. It explores generative modeling, semantic image manipulation, and adversarial speech enhancement.




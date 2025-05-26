# HueNet 🎨 - Sketch-to-Art

HueNet is a **GAN-based sketch-to-art model** that transforms black-and-white sketches into vibrant colored artworks.  
It employs a **U-Net generator** with ResNet-style blocks, a **PatchGAN discriminator**, and **VGG perceptual loss** to boost realism.

## ✨ Overview  

- **Generator (U-Net)**: Converts sketches into colorful images.  
- **Discriminator (PatchGAN)**: Judges image patches for sharper, more detailed realism.  
- **VGG Feature Loss**: Enhances style and detail via high-level feature comparison.  
- **Training**:  
  - Uses adversarial and perceptual losses.  
  - Utilizes PyTorch’s **autocast** for faster mixed-precision training.  
  - Trained for 100 epochs; more data and epochs could improve results.

## 🏗️ Architecture Highlights  

- **Generator**: U-Net with encoder-decoder structure and residual-style conv blocks.  
- **Discriminator**: PatchGAN, focusing on local textures.  
- **Loss Functions**:  
  - Adversarial loss to guide realism  
  - L1/L2 pixel loss for structure  
  - VGG perceptual loss for style and detail  

## 🚀 Features  

- Effective **sketch-to-color** translation.  
- GAN-driven adversarial training for sharper outputs.  
- VGG perceptual loss ensures detailed and consistent colorization.  
- Mixed-precision training with autocast improves speed and memory efficiency.  

## Results  

![Image 1](images/13.png)  
![Image 2](images/11.png)  
![Image 3](images/12.png)  
![Image 4](images/8.png)  

More images available [here](https://github.com/Aryan-Palimkar/Hue-Net/tree/main/images)

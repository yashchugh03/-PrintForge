# Synthetic Fingerprint Generation for Medical Applications
## A Deep Convolutional Generative Adversarial Network Approach
### Project Overview
This project explores the application of Generative Adversarial Networks (GANs) for generating synthetic fingerprints tailored for medical applications. The goal is to create high-quality, realistic fingerprint images while preserving privacy and ensuring variability for research and practical use in medical diagnostics, access systems, and other health-related fields.

### Key Features
1. Deep Convolutional GAN (DCGAN) : Utilizes convolutional layers to ensure the generation of high-resolution, detailed fingerprints.
2. Synthetic Data for Privacy: Eliminates the need for real patient data, mitigating privacy concerns.
3. Medical Applicability: Designed to mimic variations critical in medical systems, such as minutiae patterns relevant to diagnostics or secure health access systems.
4. Customizability: The GAN architecture is flexible to generate fingerprint images with different resolutions and complexities.

### Motivation
Fingerprint data is widely used in medical and health-related biometric systems for patient identification and secure access. However, the use of real fingerprints raises significant privacy concerns. Synthetic fingerprints generated through GANs offer a solution by providing realistic data that preserves utility without compromising individual privacy.

### Methodology
#### 1. Model Architecture
![image](https://github.com/user-attachments/assets/10d8db65-e6af-4911-ad9f-20a9ff24bdc9)


#### 2. Training Process
##### Hyperparameters
+ batch_size = 128
+ image_size = 64 * 64 * 3
+ latent vector size for generator input(nz) = 100
+ feature size generator(ngf) = 64
+ feature size discriminator(ndf) = 64
+ num_epochs = 150
+ learning rate(lr) = 0.0002
+ param for Adam optimizer(beta1) = 0.5
  
##### Loss Functions:
    1. Binary Cross-Entropy Loss for adversarial classification.

#### 3. Dataset
##### SOCOFing Dataset:
A comprehensive fingerprint dataset containing over 6,000 images with both altered and unaltered samples.
Facilitates the training of GANs to produce diverse fingerprint patterns.

### Results and Evaluation
#### Generator and Discriminator Loss graph:
![image](https://github.com/user-attachments/assets/416b02d1-be06-42f9-a824-739147f546ca)

#### Visual Quality:
![image](https://github.com/user-attachments/assets/cbfb53ff-58c0-466d-90d5-48c8478f8e93)

Generated fingerprints resemble real patterns with intricate details.
#### Performance Metrics:
Inception Score (IS): 16.48

#### t-SNE 
![image](https://github.com/user-attachments/assets/aab54bcd-7b85-4d1c-bdcb-42dd7e38f820)

### Future Work
- Improve resolution and fine-grain patterns for advanced medical applications.
- Explore conditional GANs for generating targeted fingerprint variations.
- Release pre-trained models for broader accessibility.

### Contributors
1. Manas Vashisht
2. Medhansh Sharma
3. Smit Patel
4. Yash Chugh

### Acknowledgments
- Thanks to the creators of the SOCOFing Dataset for providing a robust foundation.
- Inspired by cutting-edge research in GANs and biometrics.


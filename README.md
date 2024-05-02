# GAN_FacialExpression
Generating different facial expressions.  
This project utilizes Generative Adversarial Networks (GANs) to generate lifelike facial images based on various expressions. This project employs two different types of GAN architectures: Conditional GANs (cGANs) and Auxiliary Classifier GANs (ACGANs), to create diverse and expressive faces.   
## Introduction  
Facial expression generation has long been a challenging task in the field of computer vision and artificial intelligence. We aim to overcome this challenge by leveraging the power of GANs, a class of machine learning algorithms that excel at generating realistic data samples.  
## Objective
The objective of this project is to utilize Generative Adversarial Networks (GANs), to generate synthetic facial images corresponding to different emotional expressions (e.g., happy, neutral, sad, angry, fear, surprised, disgust).  
1.Utilize Conditional Generative Adversarial Networks (CGANs) and Auxiliary Classifier Generative Adversarial Networks (ACGANs) to generate realistic black and white facial images.  
2.Incorporate specific emotion labels (happy, neutral, sad, angry, fear, surprised, disgust) to guide the generation process, enabling the creation of diverse facial expressions.  
3.Train the GAN models on the fer2013 dataset to develop a system capable of synthesizing expressive facial images corresponding to different emotions, advancing research in emotion recognition and synthesis.  
## Flowchart  
<img width="861" alt="Screenshot 2024-05-02 at 8 40 51 PM" src="https://github.com/PrishaGorakh/GAN-RMFC-Div-A-FacialExpression/assets/124128845/b45c1326-a309-4456-889e-f115da2f43a9">

## Architecture  
We have used two primary architectures for expression-based facial image generation:  
**Conditional GAN (cGAN):** In this architecture, the generator takes both a random noise vector and a conditional label representing the desired expression as input. The discriminator evaluates the generated images based on both their realism and whether they match the specified expression label.
<p align="center">
<img width="383" alt="Screenshot 2024-05-02 at 8 42 32 PM" src="https://github.com/PrishaGorakh/GAN-RMFC-Div-A-FacialExpression/assets/124128845/f4e42bc0-35b1-4966-a893-b1ff2e31da02"></p>

**Auxiliary Classifier GAN (ACGAN):** ACGAN extends the cGAN architecture by introducing an auxiliary classifier in the discriminator. This classifier not only distinguishes between real and fake images but also predicts the expression label associated with the generated images.  
<img width="383" alt="Screenshot 2024-05-02 at 8 43 27 PM" src="https://github.com/PrishaGorakh/GAN-RMFC-Div-A-FacialExpression/assets/124128845/c11ece85-7a08-4a3f-aba2-589a2612a2d9">

## Datasource:  
Dataset contain a CSV file of black and white labeled 48x48 images from the FER2013 dataset. Data contains 35,887 records from Fer2013:   
14,685 - Happy (29.63%) Emotion: 3  
13,066 - Neutral (26.36%) Emotion: 6  
6,345 - Sad (12.8%) Emotion: 4  
5,205 - Angry (10.5%) Emotion: 0  
5,142 - Fear (10.37%) Emotion: 2  
4,379 - Surprised (8.82%) Emotion: 5  
755 - Disgust (1.52%) Emotion: 1  
The CSV contains 3 columns Emotion, Pixels and Usage.  
(https://www.kaggle.com/datasets/nicolejyt/facialexpressionrecognition)

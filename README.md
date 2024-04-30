# GAN_FacialExpression
Generating different facial expressions.  
This project utilizes Generative Adversarial Networks (GANs) to generate lifelike facial images based on various expressions. This project employs two different types of GAN architectures: Conditional GANs (cGANs) and Auxiliary Classifier GANs (ACGANs), to create diverse and expressive faces.   
## Introduction  
Facial expression generation has long been a challenging task in the field of computer vision and artificial intelligence. We aim to overcome this challenge by leveraging the power of GANs, a class of machine learning algorithms that excel at generating realistic data samples.
## Architecture  
We have used two primary architectures for expression-based facial image generation:  
**Conditional GAN (cGAN):** In this architecture, the generator takes both a random noise vector and a conditional label representing the desired expression as input. The discriminator evaluates the generated images based on both their realism and whether they match the specified expression label.  
**Auxiliary Classifier GAN (ACGAN):** ACGAN extends the cGAN architecture by introducing an auxiliary classifier in the discriminator. This classifier not only distinguishes between real and fake images but also predicts the expression label associated with the generated images.  
## Datasource:
(https://www.kaggle.com/datasets/nicolejyt/facialexpressionrecognition)

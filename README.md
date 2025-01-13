# Faking Monets with a GAN

## Background
This project was made for Module 5 of the course *Introduction to Deep Learning* (DTSA-5511) at University of Colorado Boulder. The task is based on the Kaggle competition [I’m Something of a Painter Myself](https://www.kaggle.com/competitions/gan-getting-started).

## Description
The project employs **Generative Adversarial Networks (GANs)** to transform landscape photographs into paintings reminiscent of Claude Monet’s style. The model is trained on unpaired datasets of Monet paintings and landscape photos to learn the mapping between the two domains.

### Key Features:
* **CycleGAN Architecture**: Utilizes two generators and two discriminators to achieve bidirectional image translation between photographs and Monet-style paintings without the need for paired training examples.
* **Data Augmentation**: Applies various augmentation techniques to enhance the diversity of the training data, improving the model’s generalization capabilities.
* **Training Strategy**: Incorporates adversarial loss, cycle-consistency loss, and identity loss to ensure the generated images are both stylistically accurate and content-preserving.
* **Evaluation Metrics**: Assesses the quality of generated images using metrics such as the Fréchet Inception Distance (FID).

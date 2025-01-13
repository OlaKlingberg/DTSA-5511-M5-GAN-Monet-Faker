# Faking Monets with a GAN

## Background
This project was made for Module 5 of the course *Introduction to Deep Learning* (DTSA-5511) at University of Colorado Boulder. The task is based on the Kaggle competition [I’m Something of a Painter Myself](https://www.kaggle.com/competitions/gan-getting-started).

## Description
The project employs **Generative Adversarial Networks (GANs)** to transform landscape photographs into paintings reminiscent of Claude Monet’s style. The model is trained on unpaired datasets of Monet paintings and landscape photos to learn the mapping between the two domains.

### Data source
The dataset can be accessed from the page for the Kaggle competition [I'm Something of a Painter Myself](https://www.kaggle.com/competitions/gan-getting-started/data)

### Key Features:
* **CycleGAN Architecture**: Utilizes two generators and two discriminators to achieve bidirectional image translation between photographs and Monet-style paintings without the need for paired training examples.
* **Data Augmentation**: Applies various augmentation techniques to enhance the diversity of the training data, improving the model’s generalization capabilities.
* **Training Strategy**: Incorporates adversarial loss, cycle-consistency loss, and identity loss to ensure the generated images are both stylistically accurate and content-preserving.
* **Evaluation Metrics**: Assesses the quality of generated images using metrics such as the Fréchet Inception Distance (FID).

### Results
The trained model generates images which, when submitted to the Kaggle competition, received a decent MiFID score of 55.3. A manual inspection of a sample of the images reveals them to have a color scheme that is reminiscent of Monet's palette, but their graininess is a poor imitation of Monet's visible brushstrokes. The generated Monet-style images are unlikely to fool any human observer.

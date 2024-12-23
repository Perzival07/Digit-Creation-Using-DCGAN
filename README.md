# Digit-Creation-Using-DCGAN
This project demonstrates the implementation of a Generative Adversarial Network (GAN) to generate realistic handwritten digits, inspired by the MNIST dataset. It includes multiple test runs with varying configurations to explore the capabilities and scalability of GANs.



Installation

1.Clone the repository:
```python
git clone https://github.com/your-username/GAN-MNIST.git
cd GAN-MNIST
```

2.Install the required dependencies:
```python
pip install -r requirements.txt
```

3.Ensure TensorFlow is installed with GPU support (if using GPUs):
```python
pip install tensorflow-gpu
```



Usage

1.Preprocess the dataset by running the preprocessing script (if applicable):
```python
python preprocess.py
```

2.Start the GAN training process:
```python
python train.py --batch_size 128 --epochs 50
```
Optional flags include:
--batch_size: Define batch size (default: 128).
--epochs: Set the number of training epochs (default: 50).

3.View the generated images in the MNIST/figs/ directory.

4.To restore from a checkpoint and continue training:
```python
python train.py --restore_checkpoint path/to/checkpoint
```

5.Evaluate the trained model with the discriminator or generator independently (if supported).



The GAN-MNIST project implements a Generative Adversarial Network (GAN) to create realistic handwritten digits, inspired by the MNIST dataset. With custom-designed generator and discriminator models, it leverages TensorFlow's MirroredStrategy for multi-GPU training, ensuring scalability and performance. The project features dynamic image generation and visualization, periodic model checkpointing, and flexible configuration options for batch size, learning rate, and training epochs. Installation is straightforward with a requirements.txt file, and TensorFlow GPU support enhances training efficiency. Users can preprocess the dataset, train the GAN, monitor progress through generated images, and restore training from checkpoints effortlessly. The project's modular design and well-structured directories make it ideal for experimentation and research in generative modeling. Dive into the fascinating world of GANs and explore their potential with this project!

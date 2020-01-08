# Deep-Compression-with-autoencoder
 In addition to the implementation of deep encoder we will study the effect of different distorsions and noise on this model that is used in our case for <h3> compression </h3> <br>
 In our case we will deal with these type of distorsions: <br>
- Poisson noise <br>
- White  noise <br>
- Salt & pepper  noise <br>
- Speckle noise <br>
- Gaussian <br>
- Median 3x3 and 5x5 <br>
- Mean 3x3 and 5x5 <br>
<br>
For this we will use MNIST dataset (60000 for training et 10000 for test) <br> 
Images are in grayscale with 28x28 pixels

Now we will move to our model "Autoencoder"
<h1> Autoencoder </h1>

But first let's discover what is the "autoencoder" 

![in](https://user-images.githubusercontent.com/35869627/71977626-8ed33900-3219-11ea-94d2-ee019d02970c.png)
<br>
Autoencoder is an unsupervised artificial neural network that learns how to efficiently compress and encode data then learns how to reconstruct the data back from the reduced encoded representation to a representation that is as close to the original input as possible.
<br>
Autoencoder Components:

Autoencoders consists of 4 main parts: <br>

1- Encoder: In which the model learns how to reduce the input dimensions and compress the input data into an encoded representation. <br> 

2- Bottleneck: which is the layer that contains the compressed representation of the input data. This is the lowest possible dimensions of the input data.
<br>
3- Decoder: In which the model learns how to reconstruct the data from the encoded representation to be as close to the original input as possible.
<br>

4- Reconstruction Loss: This is the method that measures measure how well the decoder is performing and how close the output is to the original input.
<br>
The training then involves using back propagation in order to minimize the network’s reconstruction loss.
<br>
For more details about autoencoders why and why not just read this article: <br>
https://blog.keras.io/building-autoencoders-in-keras.html <br> 

<h1> Our Work</h1>
We will only use deep autoencoder and train our model with normal and noisy data and explain some facts.
<br> 

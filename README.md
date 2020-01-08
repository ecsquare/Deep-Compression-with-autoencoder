# Deep-Compression-with-autoencoder
 In addition to the implementation of deep encoder we will study the effect of different distorsions and noise on this model that is used in our case for <h3> compression </h3> <br>
 In our case we will deal with these type of distorsions: <br>
- Poisson noise <br>
- White  noise <br>
- Salt & pepper  noise <br>
- Speckle noise <br>
- Gaussian <br>
- Median 3*3 and 5*5 <br>
- Mean 3*3 and 5*5 <br>
<br>
For this we will use MNIST dataset (60000 for training et 10000 for test) <br> 
Images are in grayscale with 28x28 pixels

Now we will move to our model "Autoencoder"
<h1> Autoencoder </h1>
We build this model with respect to hyperparameter choice of this implementation: <br>
https://blog.keras.io/building-autoencoders-in-keras.html <br> 
But first let's discover what is the "autoencoder" <br>
![in](https://user-images.githubusercontent.com/35869627/71977626-8ed33900-3219-11ea-94d2-ee019d02970c.png)

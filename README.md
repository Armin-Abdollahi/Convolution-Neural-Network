# Convolution on CIFAR-10


To implement Convolution on the CIFAR-10 dataset, we first import the TensorFlow Framework and the necessary libraries, and then load the CIFAR-10 dataset.
After loading the dataset, we need to normalize our data. For this, by dividing by 255, our data will be a number between 0 and 1.

<img width="750" src="https://github.com/Armin-Abdollahi/Convolution-Neural-Network/assets/103449830/c9054734-3e93-4e3f-bcf0-6a3fcd568c9e">



The next step is to build the model, which we built in three convolution layers, each followed by a maximum integration layer and a final dense layer with SoftMax activation.
We trained the network twice, and in the first time, the layer activation function was "Relu" and in the second time, "Sigmoid", which you will see the results of in the following.

| Activation: Sigmoid | Activation: Relu |
| --- | --- |
|<img width="750" src="https://github.com/Armin-Abdollahi/Convolution-Neural-Network/assets/103449830/3a7544ca-5068-4c78-b8e9-240040e52115">|<img width="750" src="https://github.com/Armin-Abdollahi/Convolution-Neural-Network/assets/103449830/d812fbd9-a5ec-4387-9c7a-bb8477d1a7de">|
 


To compile the model, we chose the optimizer "adam" and to train the model, we set the number of epochs to 50 and the number of batch sizes to 4.

<img width="750" src="https://github.com/Armin-Abdollahi/Convolution-Neural-Network/assets/103449830/7a1eea17-2d2c-4183-9ffc-52dd296aef13">



Then we plot the results:

<img width="750" src="https://github.com/Armin-Abdollahi/Convolution-Neural-Network/assets/103449830/039ec0b3-cc39-4efb-9772-59e5a5611c28">



## Comparison:

|  | Activation: Relu | Activation: Sigmoid |
| --- | --- | --- |
| Loss | 0.6220 | 0.4688 |
| Accuracy | 0.7815 | 0.8346 |
| Val_loss | 1.1745 | 1.3413 |
| Val_accuracy | 0.6602 | 0. |
| Plot |![image](https://github.com/Armin-Abdollahi/Convolution-Neural-Network/assets/103449830/cd9ef6e2-bccf-4e25-9a42-e0fc063476db)|![image](https://github.com/Armin-Abdollahi/Convolution-Neural-Network/assets/103449830/76922907-acde-4d65-89fb-65f6b8345623)|

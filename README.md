# Quantization-of-semantic-segmentation
Here I train a U-net for salt segmentation and try to Quantize it.

The dataset can be downloaded from the following links <br />
Images https://drive.google.com/open?id=16TV2Y7SKS8is8nVutFCpr16jUAZDsqJw <br />
Masks https://drive.google.com/open?id=1N7kQjB8Gu-Pz-15rcOyO03A4r7nZr0NN  <br />

The Task is to identify the salt deposits in the given images.<br /> 

Read the jupyter notebook file "salt" to find the commented code. Here I train the model using two loss <br />
1) Binary crossentropy loss <br />
2) IOU loss (This is actually an approximation of the IOU) <br />

I get a IOU score of 69% on the semantic segmentation of the salt data set. Then I attempt to Quantize the network on a variable number of bits as specified by user. (This is still a work in progress)

### The U net
 ![](./Images/u-net-architecture.png)


### Quantization
   I am attempting to Quantize the net layer by layer, this is still a work in progress...... 

## Neural Network Prunning

As seen in most deep neural network architectures like ResNet, VGG and co, they exhibit a common charactersistics of having
very large number of parameters. These parameters is the cause of having the final model to be large in size. 
We can see that this poses a key disadvantage to deploying to low resource devices. Even though architectures like MobileNet 
attempts to solve this challenges, it still does not efficiently produce favourable model sizes.

The question that arise bring about new research field is; how do we leverage the large network architectures which have produced good results and make them of less parameters without loosing much accuracy. Based on Yann Le cunn work in 1990, we know that despite the  many parameters, some weights do not have much contribution to the final output of the model.

Hence, Neural network prunning is to remove the unnecessary parameters (neurons)  from the network and this results in a smaller and faster network. Several methods have been proposed on Neural Networks Prunning. You can get a full glimpse and a concise summary of the state of the art methods and code implementation of NN Prunning at this [github repository].

One key technique that has stayed for long is **ranking neurons** and the intuition is that for a given layer, we can rank the neurons in the network based on how much they contribute to the final performance and removing the low ranking neurons.

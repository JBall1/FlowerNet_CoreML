# FlowerNet_CoreML
Flower Net is built on top of mobilenetV2 with 1033 labels. The total custom dataset consits of approxamitely 80,000 images.


Coming Soon:
  There will soon be an update with mobilenetv3.
  
![Image of Loss Graph](https://github.com/JBall1/FlowerNet_CoreML/blob/master/Loss.png)
![Image of Accuracy Graph](https://github.com/JBall1/FlowerNet_CoreML/blob/master/accuracy.png)

Model Summary:

        _________________________________________________________________
        Layer (type)                 Output Shape              Param #   
        =================================================================
        mobilenetv2_1.00_224 (Model) (None, 7, 7, 1280)        2257984   
        _________________________________________________________________
        global_average_pooling2d_1 ( (None, 1280)              0         
        _________________________________________________________________
        activation_1 (Activation)    (None, 1280)              0         
        _________________________________________________________________
        dropout_1 (Dropout)          (None, 1280)              0         
        _________________________________________________________________
        dense_1 (Dense)              (None, 1033)              1323273   
        _________________________________________________________________
        activation_2 (Activation)    (None, 1033)              0         
        =================================================================
        Total params: 3,581,257
        Trainable params: 3,547,145
        Non-trainable params: 34,112
        _________________________________________________________________

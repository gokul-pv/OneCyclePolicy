# One Cycle Policy
> A custom ResNet architecture that uses One Cycle Policy to train the model 

The model is trained on CIFAR-10 dataset using a custom Resnet architecture as shown below

<p align="center" style="padding: 10px">
<img alt="Forwarding" src="https://github.com/gokul-pv/OneCyclePolicy/blob/main/Images/architecture.png?raw=true" width =500><br>
<em style="color: grey">Figure 1 : Resnet Architecture </em>
</p> 

The training is done using one cycle policy with following parameters
 - Total Epochs = 24
 - Max at Epoch = 5
 - LRMIN = FIND
 - LRMAX = FIND
 - NO Annihilation

The following image augmentations are done using Albumentation Library
 - RandomCrop 32, 32 (after padding of 4) 
 - FlipLR
 - CutOut(8, 8)


The **summary** of the model is shown below

<p align="center" style="padding: 10px">
<img alt="Forwarding" src="https://github.com/gokul-pv/OneCyclePolicy/blob/main/Images/model_summary.png?raw=true" width =500><br>
<em style="color: grey">Figure 2 : Model summary </em>
</p> 



**Result**

The training logs, loss and accuracy can be found [here](./OneCyclePolicy.ipynb)

<p align="center" style="padding: 10px">
<img alt="Forwarding" src="https://github.com/gokul-pv/OneCyclePolicy/blob/main/Images/learningrate.png?raw=true" width =500><br>
<em style="color: grey">Figure 3 : Plot for loss and accuracy </em>
</p> 

#### 不同优化器

建立带有五种优化器的网络，设定15个batch，在训练集上进行训练，并在每个batch中对测试集进行预测，记录每个batch中的loss及预测准确率，以下分别是1/5/10/15个batch相应结果：

```
[Optim SGD,Epoch 1] loss: 1.451
Accuracy of the network on the 10000 test images: 10 %
[Optim Momentum,Epoch 1] loss: 1.434
Accuracy of the network on the 10000 test images: 15 %
[Optim RMSprop,Epoch 1] loss: 0.901
Accuracy of the network on the 10000 test images: 47 %
[Optim Adam,Epoch 1] loss: 0.890
Accuracy of the network on the 10000 test images: 48 %
[Optim Adagrad,Epoch 1] loss: 1.163
Accuracy of the network on the 10000 test images: 34 %
```

```
[Optim SGD,Epoch 5] loss: 1.447
Accuracy of the network on the 10000 test images: 16 %
[Optim Momentum,Epoch 5] loss: 0.978
Accuracy of the network on the 10000 test images: 43 %
[Optim RMSprop,Epoch 5] loss: 0.632
Accuracy of the network on the 10000 test images: 60 %
[Optim Adam,Epoch 5] loss: 0.662
Accuracy of the network on the 10000 test images: 60 %
[Optim Adagrad,Epoch 5] loss: 1.056
Accuracy of the network on the 10000 test images: 39 %
```

```
[Optim SGD,Epoch 10] loss: 1.286
Accuracy of the network on the 10000 test images: 26 %
[Optim Momentum,Epoch 10] loss: 0.788
Accuracy of the network on the 10000 test images: 53 %
[Optim RMSprop,Epoch 10] loss: 0.551
Accuracy of the network on the 10000 test images: 62 %
[Optim Adam,Epoch 10] loss: 0.551
Accuracy of the network on the 10000 test images: 64 %
[Optim Adagrad,Epoch 10] loss: 0.977
Accuracy of the network on the 10000 test images: 41 %
```

```
[Optim SGD,Epoch 15] loss: 1.123
Accuracy of the network on the 10000 test images: 35 %
[Optim Momentum,Epoch 15] loss: 0.697
Accuracy of the network on the 10000 test images: 59 %
[Optim RMSprop,Epoch 15] loss: 0.525
Accuracy of the network on the 10000 test images: 63 %
[Optim Adam,Epoch 15] loss: 0.512
Accuracy of the network on the 10000 test images: 63 %
[Optim Adagrad,Epoch 15] loss: 0.977
Accuracy of the network on the 10000 test images: 43 %
```

根据每个batch绘制出的loss和acc图像如下所示：

![train_loss](train1/train_loss.png)

![train_acc](D:\5-1研一\新生培训\train1\train_acc.png)

#### 不同学习率

为了考虑学习率对网络的影响，建立了四种不同的学习率，在10个batch内记录每个网络的loss及预测准确率，下面是在1/5/10个batch得到的结果：

```
[learning_rate 0.001000,Epoch 1] loss: 1.443
Accuracy of the network on the 10000 test images: 15 %
[learning_rate 0.005000,Epoch 1] loss: 1.003
Accuracy of the network on the 10000 test images: 40 %
[learning_rate 0.010000,Epoch 1] loss: 0.942
Accuracy of the network on the 10000 test images: 44 %
[learning_rate 0.100000,Epoch 1] loss: 1.453
Accuracy of the network on the 10000 test images: 10 %
```

```
[learning_rate 0.001000,Epoch 5] loss: 0.927
Accuracy of the network on the 10000 test images: 45 %
[learning_rate 0.005000,Epoch 5] loss: 0.723
Accuracy of the network on the 10000 test images: 59 %
[learning_rate 0.010000,Epoch 5] loss: 0.640
Accuracy of the network on the 10000 test images: 61 %
[learning_rate 0.100000,Epoch 5] loss: 1.452
Accuracy of the network on the 10000 test images: 10 %
```

```
[learning_rate 0.001000,Epoch 10] loss: 0.836
Accuracy of the network on the 10000 test images: 52 %
[learning_rate 0.005000,Epoch 10] loss: 0.573
Accuracy of the network on the 10000 test images: 64 %
[learning_rate 0.010000,Epoch 10] loss: 0.522
Accuracy of the network on the 10000 test images: 62 %
[learning_rate 0.100000,Epoch 10] loss: 1.452
Accuracy of the network on the 10000 test images: 10 %
```

得到每个batch绘制loss和acc图像：

![learning_loss](D:\5-1研一\新生培训\train1\learning_loss.png)

![learning_acc](D:\5-1研一\新生培训\train1\learning_acc.png)

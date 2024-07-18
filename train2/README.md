将构造好的两个网络模型 net、unnet 进行15个epoch的训练，在第1/5/10/15个epoch中，loss及训练集上的Accuracy数据如下：

```
[epoch:1, net:net] Loss: 1.300 | Acc: 52.756% 
[epoch:1, net:unnet] Loss: 1.220 | Acc: 56.224% 
```

```
[epoch:5, net:net] Loss: 0.265 | Acc: 91.006% 
[epoch:5, net:unnet] Loss: 0.343 | Acc: 88.124% 
```

```
[epoch:10, net:net] Loss: 0.041 | Acc: 98.714% 
[epoch:10, net:unnet] Loss: 0.103 | Acc: 96.498% 
```

```
[epoch:15, net:net] Loss: 0.009 | Acc: 99.818% 
[epoch:15, net:unnet] Loss: 0.043 | Acc: 98.610% 
```

综合loss曲线和Accuracy曲线如下图所示：

![trainloss](https://github.com/aqqqaqqqq/2024-train/blob/main/train2/trainloss.png)

![trainacc](https://github.com/aqqqaqqqq/2024-train/blob/main/train2/trainacc.png)

在每个epoch训练后，将模型在测试集上进行预测，得到的两个网络模型在测试集上的综合Accuracy曲线如下图所示：

![testacc](https://github.com/aqqqaqqqq/2024-train/blob/main/train2/testacc.png)

对测试集中的每个类别单独计算Accuracy，得到的两个网络模型结果如下表所示：

| category | net（%） | unnet（%） |
| :------: | :------: | :--------: |
|  plane   |    81    |     84     |
|   car    |    86    |     90     |
|   bird   |    72    |     70     |
|   cat    |    59    |     66     |
|   deer   |    73    |     78     |
|   dog    |    66    |     69     |
|   frog   |    83    |     82     |
|  horse   |    83    |     83     |
|   ship   |    87    |     87     |
|  truck   |    84    |     86     |


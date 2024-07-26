将构造好的两个网络模型 LSTM、GRU 进行15个epoch的训练，在第1/5/10/15个epoch中，训练集及测试集上的loss如下（上面数据为LSTM，下面数据为GRU）：

```
Epoch 1/15, Train Loss: 0.4838, Test Loss: 0.3995
Epoch 1/15, Train Loss: 0.5499, Test Loss: 0.4423
```

```
Epoch 5/15, Train Loss: 0.0998, Test Loss: 0.4517
Epoch 5/15, Train Loss: 0.0733, Test Loss: 0.5088
```

```
Epoch 10/15, Train Loss: 0.0171, Test Loss: 0.8632
Epoch 10/15, Train Loss: 0.0127, Test Loss: 0.8966
```

```
Epoch 15/15, Train Loss: 0.0112, Test Loss: 1.0604
Epoch 15/15, Train Loss: 0.0043, Test Loss: 1.0651
```

LSTM和GRU的两个loss曲线如下图所示：

![trainloss](D:\5-1研一\新生培训\train3\lstmloss.png)

![trainacc](D:\5-1研一\新生培训\train3\gruloss.png)

对测试集中的每个类别单独计算Accuracy，得到的两个网络模型结果如下表所示：

| category | LSTM（%） | GRU（%） |
| :------: | :-------: | :------: |
| class 0  |   87.83   |  85.32   |
| class 1  |   77.42   |  83.44   |
|   all    |   82.62   |  84.38   |


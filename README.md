# code for my master's thesis, BatchRaCUN

## 1.Prerequisites
```
pip install -r requirements.txt
```

## 2.Training

- ```--model``` : ```resnet18``` / ```resnet50``` / ```resnet101```
- ```--dataset``` : ```CIFAR10``` / ```ImageNet```

#### Optional

- ```--react``` : Replaces the ReLU functions in ResNet with ReAct layers.
- ```--wandb``` : Enables the WandbLogger.
- ```--lr_scheduler``` : Uses the [OneCycleLR Scheduler](https://pytorch.org/docs/stable/generated/torch.optim.lr_scheduler.OneCycleLR.html)
<br/>

- ```--lr``` : Sets the learning rate (Default ```0.001```)
- ```--optimizer``` : Sets the optimizer: ```SGD``` / ```Adam``` / ```AdamW``` (Default ```Adam```)
- ```--batchsize``` : Sets the batch size (Default ```256```)
- ```--adv``` : Enables adversarial attacks.

#### UseAge
```python network_lightning.py --model resnet18 --dataset ImageNet --optimizer SGD```

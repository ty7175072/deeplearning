# 论文代码

## 项目结构
* net 存放所有网络模型结构
* params 存放所有权重文件
* 预测图像 存放由模型推理的图像
- train.py 训练脚本
- predict.py 预测脚本
- predict_more.py 预测脚本

> ## 操作
> ### 更换模型
> #### train.py脚本下
```
from net import *
net = deeplabv3_resnet50(num_classes=19)
```
> ### 训练
> #### train.py脚本下
>  `python3 train.py --num_classes=18 --data-path=../data/正位语义分割s4 --epochs=300`

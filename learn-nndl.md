#NNDL

[TOC]

##第一章
尽管人类在理解我们眼睛展示出来的信息上非常擅长,但几乎所有的过程都是无意识的.所以,我们通常并不能体会自身视觉系统解决问题的困难.
###1.1
* **感知机:**接收**几个**二进制输入,并产生**一个**二进制输出.
* **权重**,表示相应输入对于输出重要性的实数.
* **阈值**,threshold
* **偏置**,b=-threshold

```c
output = ((w .* x + b) <= 0) ? 0 : 1;
```

* 随着权重和阈值的变化,我们可以得到不同的决策模型.
* 
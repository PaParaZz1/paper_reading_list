### 7.29

Making Convolutional Networks Shift-Invariant Again(ICML2019)
https://arxiv.org/pdf/1904.11486.pdf

rethinking the value of network pruning
https://arxiv.org/abs/1810.05270v1

### 7.30

proxyless NAS
https://arxiv.org/abs/1812.00332

-   移动设备测速（实际测速cost太大，可以根据搜索空间准备架构数据，然后训练一个简易的测速估计模型）
-   搜索的结果结构，每次downsample之后MBConv会选择expand ratio大，kernel size大的block
-   其他NAS的搜索结果，权衡下来使用expand ratio=3的较多
-   整合latency的方法
    -   作为loss的正则化项
    -   像RL-based的NAS一样整合进reward
    -   进化算法来权衡accuracy和latency

train imagenet in 1 hour

https://arxiv.org/abs/1706.02677

-   调整学习率和调整梯度的步长
-   常数warmup和渐变（线性）warmup
-   多机多卡的bn如何计算，bn对于优化问题的影响，什么时候需要同步bn什么时候不需要
-   SGD的动量纠正
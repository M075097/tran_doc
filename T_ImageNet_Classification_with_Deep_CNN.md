ImageNet Classification with Deep Convolutional Neural Networks
使用深度卷积云神经网络对图片集进行分类

autor:Geoffrey Hinton 
Alex Krizhevsky
Ilya Sutskever 

##摘要
为了把ILSVRC-2010大赛中的120万张高清图片分为1000个不同的类别，我们训练了一个大型，深度的卷积神经网络。在测试数据上实现了TOP1和Top5分别为37.5%和17.0%的结果，而这个结果相比之前最好的数据结果还要好上很多。这个拥有6000万个数据特征和65万个神经元的神经网络由5个卷积层组成，这个神经网的一些层是按照最大池化层构建的，还有3层是全联通层（with a final 1000-way softmax）。为了使训练速度更快我们使用了非饱和神经元和一个高效的GPU来实现卷积运算。为了减少全联通网络的过度拟合我们使用了一项最新流行且被证明是有效的一种方法遗忘(“dropout”)。我们也在ILSVRC-2012赛事上使用了该模型的修正版本，并且得到了得到了top-5测试错误率为15.3%的成绩相比第二名的团队得到的成绩是26.2%。

原文地址：https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf
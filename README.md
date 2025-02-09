#开源的深度学习资料整理
####Last Update 2015.08.17
  
[![icon]](http://www.upc.edu.cn/)  
[icon]: http://www.upc.edu.cn/images/logo.jpg 
***

##

深度学习大火，将各个数据集的state of the art不断地刷新，在解决图像分类、语音识别等问题上获得了已知的最优结果，该系列算法越来越受到学术界和工业界的重视。何为深度学习？一个直观的解释是如果一个机器学习算法在建模的过程中使用了多层的自动特征表示，则该机器学习算法可以称之为深度学习算法，也就是该机器学习算法可以自动地计算特征的特征表示。

当前各类深度学习算法层出不穷，开源的工具库更是多如牛毛。选择太多比没有选择更令人痛苦。我们要感谢这些库的作者们，他们为领域的发展做出了卓越的贡献。这些工具库从使用的语言来分，大致可分为c++类、matlab类、python类和lua类。其中C++类的代表是caffe，难能可贵的是其还配有matlab和python接口，并且可以使用GPU加速，还提供预先训练好的模型，奠定了其在深度学习的领先地位。matlab类的代表是牛津的matconvnet，有GPU加速，上手快，还有精心准备的教程。python类的代表是theano、Keras和pylearn2，有UFLDL的强力支撑，想必一呼百应。lua类的代表是toch7，已经可以和caffe在CVPR2015上一较高下。

但是，我们更应该看到他们的不足。虽然上述这些库都可以跨平台使用，但是配置的难度缺差异很大。caffe依赖很多的第三方库，导致其安装十分繁琐，令很多初学者望而却步。欣喜的是电子科大的王峰博士提供了一键安装式的教程，大大方便了caffe的搭建，而华中科大的欧新宇博士/老师提供的caffe在ubuntu上的安装教程也让我信手拈来。theano在windows使用上的坑很多，之前使用python（x，y），怎么也编译不过theano，无奈放弃了使用theano这么简洁优雅的工具，甚是可惜。后来才发现要使用Anaconda，而且由于2.1后的版本取消了对MinGW的支持，只能选择2.1的版本。这些看似微不足道的细节使我们陷入泥沼，浪费了很多不必要的时间和精力。

一个很自然的想法就是如果有一个能给新手足够的参考资料，那么将会大大降低深度学习的门槛，使更多的研究者享受深度学习带来的福利。现在，这个梦想实现了。我皓首穷经，经过不断的尝试，去伪存真，略有小成，再也不用对着新放出的源码望洋兴叹了，相信你也可以做到。

具体包括深度学习的相关论文、教程、博客以及tricks，尤其是相关库的配置和使用，少部分的原理解析暂未放出。大部分的内容经过了我的验证，如果发现有错误之处，欢迎指正。

本文的资料来自于网上各位大神的无私奉献，版权归原作者所有。如果不经意间侵犯了您的正当权益，请联系我删除。
## TensorFlow数据类型介绍

&emsp;&emsp;本文主要介绍Tensorflow的基本操作技能，着重介绍TensorFlow中的数据类型。<br/>
&emsp;&emsp;在Python语音环境中常见的数据类型载体是list我们在list中可以增加任何类型的数据比如`int, double, string, tuple`等等并且可以随意的插入编辑，但是对于处理非常大的数据载体的时候放在内存中就比较不方便了，比如图片数据等等。这时候我们可以选用numpy.array，` np.array`就是为了解决同类型数据运算问题的数据载体，他可以很方便的存储很大的数据比如存储`[64, 224, 224, 3]`这样一个图片组，也可以很方便的做一下运算比如加减、转置等操作，但是numpy是在深度学习之前就已经设计好了的科学计算库那么他并没有很好地GPU支持也不能够自动求导。<br/>
&emsp;&emsp;这个时候TensorFlow就应运而生了，所以说从这个角度上看TensorFlow并没有那么神奇，在某些意义上跟numpy有一些对等只是神经网络方面相对于numpy来讲更突出一点，但是一些基本的操作比如拼接、分类等等的一些操作都是很numpy非常类似的，并且为了减少初学者的入门难度TensorFlow的一些API设计都是和numpy相近的甚至命名也是相近的。<br/>
&emsp;&emsp;Tensorflow中的数据载体是`tf.Tensor`，TensorFlow中用Tensor存储进行数据的存储和运算。
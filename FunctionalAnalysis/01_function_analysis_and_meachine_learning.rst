.. _01_function_analysis_and_meachine_learning:

泛函分析与机器学习 
================

在机器学习中，分类器可以看作一个函数，将样本x映射为标签y。其中x通常为一个向量，其各个分量成为特征。y通常为一个向量，代表类别。

通常我们认为存在这样一个函数f，其可以将x正确的映射到y。然而我们往往不知道这个函数的具体方程，甚至连这个函数大概长什么样子都不知道。我们只有训练集(一些x及对应的标签y),我们希望使用训练集学习一个映射，使这个映射逼近函数f。

举个例子，我们可以用一个多项式函数进行逼近。事先定义多项式函数的阶数，然后根据训练集，求解符合训练集的多项式参数。

这些与泛函分析有什么关系呢？

我们发现机器学习的关注点在于函数。对于向量，我们可以计算它们的和，积，它们的距离。而对于函数，如何计算它们的和，积，距离？如何去描述一列函数f逼近 :math:`f^*` ?

泛函分析给出了解决的思路。类似向量空间，我们可以将函数组成函数空间。函数空间中的元素就是单个函数，我们再定义函数空间中的度量，则可以衡量两个函数之间的距离，之后我们就能刻画收敛...... 

巴拿赫在泛函分析中的发现分为三个步骤。第一步，他考虑了抽象的线性空间，把函数当作其中的点或向量来处理，而作用于函数上的运算看作算子（如微分算子）。第二步，他对于这个抽象的线性空间引入范数，两个函数之间的距离即为 :math:`\|x-y\|` 。第三步，引入完备性的概念，即一个柯西序列会收敛到一个元素。


----
参考书：

.. [#] 普林斯顿数学指南 https://book.douban.com/subject/25817381/
.. [#] Pattern Recognition and Machine Learning https://book.douban.com/subject/2061116/ 

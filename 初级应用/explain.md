# 1、环境配置
## 1.1、LinearRegression.ipynb
主要需要配置以下内容，其余的缺啥补啥即可。
```python
pip install tensorflow==1.14.0
pip install numpy==1.17.0
pip install matplotlib
```
原作者使用的tensorflow1.x版本，然后Python使用的是2代而不是3代，我做出了一点改动。

## 1.2、LogisticRegression.ipynb
与1.1相同，不过要下载数据集，数据集已经存放在number_before_zip中，解压数据即可。

## 1.3、TensorflowTips.ipynb
```python
pip install scikit-learn==0.21.1
```
最后一个保存实现不了，其余基本上都可以。
难度是比较大的，比较恶心的。

# 2、其余解说：
## 2.1、LinearRegression.ipynb
实战一：线性回归
在这里面，由于我们只学习了基础的四大结构：**tensor、operation、graph、session**还有其余的一些设定值的方法：**constant、Variable、placeholder、init = tf.global_variables_initializer()** 等基础的操作，所以大致内容其实我们是不懂的，当然这些内容，之后会给我们详细介绍，在这里也不要太着急。

很明显，先传入tensor，
```python
train_X = numpy.asarray([3.3,4.4,5.5,6.71,6.93,4.168,9.779,6.182,7.59,2.167,
                         7.042,10.791,5.313,7.997,5.654,9.27,3.1])
train_Y = numpy.asarray([1.7,2.76,2.09,3.19,1.694,1.573,3.366,2.596,2.53,1.221,
                         2.827,3.465,1.65,2.904,2.42,2.94,1.3])
```
再进行operation
```python
pred = tf.add(tf.multiply(X, W), b)
```
graph的体现比较少，Session的体现在应用迭代之中。
设定值的一些方法也有体现，这就是这段代码的核心内容了。
完结。

## 2.2、LogisticRegression.ipynb
大致内容也差不多，只是多了读取数据集。
有图片和线性数据的区别。

## 2.3、TensorflowTips.ipynb
虽然学习了**梯度下降方法总结、自动求导autodiff、使用Optimizer**等方法，但这给我的感觉基本上等于没学。 
我只能说教的还是很差劲的。

## 深度学习比赛题目

​        因为别人的程序大多数不是代码文件的形式，是notebook的形式，而且在AIstudio平台上的可以直接拉过来运行，偷懒一下就不上传源码了。

​		人流密度检测基本思路有两种，1是直接估计（也就是用目标检测），2是间接估计（给图片预测密度图），直接估计在一些低密度且人头大小较为合适的情况下还是能得到不错的效果。但在密集人流或者透视变换严重的情况下基本无解。因此，此方法局限于低密度，弱透视的环境下。所以可能还是要用间接估计。

​		直接估计的代码

https://aistudio.baidu.com/aistudio/projectdetail/457200

​		但是几乎没有注释，真的看不懂……效果什么样也不清楚。

​		间接估计的代码

1.https://aistudio.baidu.com/aistudio/projectdetail/455827

2.https://aistudio.baidu.com/aistudio/projectdetail/456469

3.https://aistudio.baidu.com/aistudio/projectdetail/457048

4.https://aistudio.baidu.com/aistudio/projectdetail/382652

​		1和2使用的是cnn，有一点点区别，3使用的是ResNet，4使用的是VGG，其实除了神经网络外其他的地方（数据处理）都相同，我尝试过跑过的应该是1和4，得出结果感觉挺离谱的，几乎都是一个数值，没什么显著差别，但是也还能提交有个还可以的成绩的，有算力的话就试着跑跑改进一下吧。
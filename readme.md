
#### Reversi

实验设置：

* 使用 『Alpha-Beta 剪枝搜索』 实现 miniAlphaGo for Reversi（三种算法择一即可）。
* 使用 Python 语言。



Result：

实现 AIPlayer 类，采用 Alpha-Beta 剪枝搜索实现黑白棋 AI

下一步想法：可用『最小最大搜索』或 『蒙特卡洛树搜索算法』 实现，然后对比不一样算法的性能



#### Image_restoration

实验设置：

* 生成受损图像，函数接口 noise_mask_image
  * 受损图像是由原始图像添加了不同噪声遮罩（noise masks）得到的
  * 噪声遮罩仅包含 {0,1} 值。对原图的噪声遮罩的可以每行分别用 0.8/0.4/0.6 的噪声比率产生的，即噪声遮罩每个通道每行 80%/40%/60% 的像素值为 0，其他为 1。
* 使用区域二元线性回归模型，进行图像恢复。
* 评估误差为所有恢复图像与原始图像的 2-范数之和，此误差越小越好。



Result：

使用线性模型以 10 x 10 的区域为单位，进行像素预测，直到完成整张图片的像素预测，完成图像恢复



#### Waste_classification

实验设置：

* 利用深度学习模型完成垃圾分类
* 图片数据集来源：https://momodel.cn/explore/5d411ace1afd9427c236eab5?type=dataset



Result：

使用 PyTorch 自定义 7 层卷积神经网络加 2 层全连接层的分类模型

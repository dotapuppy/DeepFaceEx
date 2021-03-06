# DeepFaceEx
DeepFaceEx是一个与DeepFaceLab配合使用的插件

## 安装

下载后，在DeepFaceLab目录下解压
![](https://github.com/dotapuppy/DeepFaceEx/blob/master/Images/setup.png)

进入解压目录运行，第一次运行会自动执行安装步骤，安装完毕后，返回DeepFaceLab目录下，运行DeepFaceEx.exe即可
![](https://github.com/dotapuppy/DeepFaceEx/blob/master/Images/run.png)

如果无法运行，请安装.net framework 2.0

### 根据人脸相似度排序

在多个人脸的视频中，挑选出想要提取的人脸，例如：我们想快速提取出复仇者联盟中，所有黑寡妇的照片

    1.提取复仇者联盟里所有人脸，大概4万多张人脸
![](https://github.com/dotapuppy/DeepFaceEx/blob/master/Images/org.png)

    2.运行DeepFaceEx.exe，点击排序按钮，选择一张黑寡妇的照片
![](https://github.com/dotapuppy/DeepFaceEx/blob/master/Images/select.png)

    3.排序后，和所选照片越相似的人脸，会排在越前面。由于要考虑到运行速度，人脸特征值的算法并不是很强，所以还是有一些误检存在
![](https://github.com/dotapuppy/DeepFaceEx/blob/master/Images/sorted.png)

    4.往下拖动，越后面的图片，黑寡妇的图片越少。当大部分人脸都不是黑寡妇时，删除后面所有图片（大概只有前2000张有黑寡妇较多，后面3万多张很少）
![](https://github.com/dotapuppy/DeepFaceEx/blob/master/Images/sorted_1.png)

    5.手动删除不需要的人脸。此时也可以借助DeepFaceLab里其他脚本来处理，例如sort by similar histogram等，加快手动操作的效率。

### 精确标注人脸

开发中，使用更好的人脸标注算法，替代开源的人脸标注算法，争取达到在大多数情况下不再需要手动标注人脸。

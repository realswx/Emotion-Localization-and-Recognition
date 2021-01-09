# Emotion-Localization-and-Recognition
 
## 1、代码链接：
https://github.com/realswx/Emotion-Localization-and-Recognition

## 2、依赖：
（1）数据集链接：https://www.kaggle.com/deadskull7/fer2013 
（2）IDE：PyCharm
（3）Python版本：Python 3.6
（4）库：
    keras--------------2.2.4
    PyQt5-------------5.11.3
    tensorflow--------1.13.1
    pandas------------0.24.2
    scikit-learn--------0.21.2
    imutils-------------0.5.2
    opencv-python----4.10.25
    h5py----------------2.9.0
    matplotlib----------3.2.1
    安装方法：二选一
    （1）手动安装：PyCharm进入file--Settings--Project:Emotion Localization and Recognition--Python Interpreter中配置Python Interpreter并添加上述Package
    （2）链接下载后将venv文件夹放到项目根目录 链接：https://pan.baidu.com/s/19GiAve85biw7f2EVHlkOvA  提取码：1gdc 

## 3、运行步骤：
（1）系统程序：运行runMain.py程序。界面中模型可选可不选（有默认模型），可点击开启摄像头或者上传图片进行定位识别。
（2）训练模型：运行train_classifier.py程序
（3）混淆矩阵：运行plot_confusion_matrix.py程序

## 4、程序简要说明：
（1）runMain.py：程序界面入口，运行它可借助选择的模型使用摄像头或者上传图像进行表情识别。
（2）video_me.py：负责对（1）中摄像头或上传图像功能进行处理
（3）LocalizationNRecognition.py：使用PyQt5制作程序界面，并生成LocalizationNRecognition_UI.ui
（4）train_classifier.py：配置训练模型
（5）load_and_process.py：载入数据集进行预处理再个（4）进行训练
（6）models/cnn.py：mini_Xception网络代码
（7）plot_confusion_matrix.py：计算生成混淆矩阵和识别准确率，结果在项目根目录生成图confusion_matrix.png

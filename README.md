# NER
基于tensorflow深度学习的地理位置的命名实体识别
# 说明
本文介绍的命名实体识别技术，起源于识别地理位置，但其实词模型是一个通用模型，只要有指定的实体列表并且有对应的tag就可以；
另一个需要注意的是TensorFlow的版本，此模型是使用的最新的alpha版本，未必使用这个版本，但是最好使用比较新的版本，安装命令如下
pip install tensorflow==2.0.0-alpha0
# 如何调用脚本
1.首先需要生成文本的embedding向量，可以使用word2vec/glove/fasttext等等任意一种都可以，最终保存为vec.txt文件格式
2.通过gendata.py文件来划分数据为train/dev/test三部分数据
3.最终执行main.py文件完成训练和模型评估，训练和模型评估使用命令行参数--train True/False来区分

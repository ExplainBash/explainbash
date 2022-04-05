# 软件学报文章：基于双重信息检索的Bash代码注释自动生成方法

这里是软件学报论文“基于双重信息检索的Bash代码注释自动生成方法”的数据集与源代码

## 语料库

数据集是来自NL2Bash研究共享的预料库与NLC2CMD竞赛的官方数据，其中存在重复数据，我们删除重复数据后构建了包含10592个数据的语料库。包括train.csv，test.csv和valid.csv。

## 如何运行代码

- 下载该项目
- 我们的项目包含了两个文件夹：IR_Code和dataset，其中IR_Code是实验所需的代码，dataset是实验所需的数据集。
- IR_Code文件中包含了两个文件：explainBash.py和Information_Retrival.py。explainBash.py为主方法，也是运行的入口，在这里我们需要确认读取的训练集和测试集（信息检索方法不需要验证集）的路径是否正确。Information_Retrival.py是检索方法的具体代码，explainBash.py调用Information_Retrival.py的方法检索出测试集的所有代码注释，然后将生成的代码注释和真实注释进行评价指标计算。


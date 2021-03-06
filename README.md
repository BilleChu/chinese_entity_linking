# chinese_entity_linking
基于CN-DBpedia的短文本实体链接测试数据   
CN-DBpedia：http://kw.fudan.edu.cn/cndbpedia  
知识工厂实体链接服务： http://shuyantech.com/api/entitylinking/  
知识工厂实体链接api：http://shuyantech.com/api/entitylinking/cutsegment  
  
数据集的文本由1037条人工标注的短文本语料组成。其中大约70%来自新闻语料，包括新闻标题和内容，比如“英超-桑切斯4分钟内梅开二度阿森纳3-2五轮不败”；大约20%来自人工构建的基于歧义实体的语料，比如“红楼梦的演员有哪些”；大约10%来自问答语料中的简单问句，比如说“岳阳有哪些旅游景点”。   
  
数据标注的格式如下。每个样本的标注格式包括3个部分：语料，mention和实体，用制表符‘\t’分隔；其中mention为语料中指代实体的子段，多个用“|||”分隔；实体部分为各mention对应的实体，多个用“|||”分隔，数量应与mention一致。比如，“李娜拿过澳网冠军吗\t李娜|||澳网\t李娜（中国女子网球名将）|||澳大利亚网球公开赛”。   
  
目前，我们的实体识别与链接技术在该数据集上能达到很好的效果。其中实体识别部分的准确率为91.0%，召回率为89.4%，F1分数为90.2%；实体链接部分的准确率为94.5%（实体识别后单独计算的实体链接准确率）；针对实体识别与链接任务的准确率为86.1%，召回率为84.5%，F1分数为85.3%。   


If you want to cite our work, please use this publication:  
Bo Xu, Yong Xu, Jiaqing Liang, Chenhao Xie, Bin Liang, Wanyun Cui, and Yanghua Xiao. CN-DBpedia: A Never-Ending Chinese Knowledge Extraction System. In International Conference on Industrial, Engineering and Other Applications of Applied Intelligent Systems, pp. 428-438. Springer, Cham, 2017.
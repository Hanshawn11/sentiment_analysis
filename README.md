# NLP-level1
This is a note for me and anyone who are interested in NLP.
「情感极性分析」是对带有感情色彩的主观性文本进行分析、处理、归纳和推理的过程。按照处理文本的类别不同，可分为基于新闻评论的情感分析和基于产品评论的情感分析。其中，前者多用于舆情监控和信息预测，后者可帮助用户了解某一产品在大众心目中的口碑。
目前常见的情感极性分析方法主要是两种：基于情感词典的方法和基于机器学习的方法。

需要的数据：
1 情感词典及对应分数，BosonNLP数据 情感词典，来源于社交媒体文本，所以词典适用于处理社交媒体的情感分析。
1.1 否定词词典
1.2 程度副词词典
1.3 停用词词典

eg： 我非常讨厌害说谎
seg --> 我/非常/讨厌/说谎
非常 adv ， 讨厌 not word,  说谎 senti word

finalSentiScore = (-1) ^ (num of notWords) * degreeNum * sentiScore
finalScore = sum(finalSentiScore)

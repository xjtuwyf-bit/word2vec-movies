## 项目目的

学习如何使用Word2Vec来对文本文件进行处理。

## 来源

这个笔记是基于Kaggle比赛：[Bag of words meets bags of popcorn](https://www.kaggle.com/c/word2vec-nlp-tutorial)。打开页面后可以看到有关于NLP的相关教程，于是我把Part1~3用中文做了三个笔记。

因为年代比较久远，有些库的API失效了，我重新用python3实现的过程中填了不少坑，都是可以正常运行的。

## 内容

- [Part 1 For Beginners Bag of Words（初学词袋）](http://nbviewer.jupyter.org/github/BrambleXu/word2vec-movies/blob/master/Part%201%20For%20Beginners%20Bag%20of%20Words%EF%BC%88%E5%88%9D%E5%AD%A6%E8%AF%8D%E8%A2%8B%EF%BC%89.ipynb)
- [Part 2 Word Vectors（词向量）](http://nbviewer.jupyter.org/github/BrambleXu/word2vec-movies/blob/master/Part%202%20Word%20Vectors%EF%BC%88%E8%AF%8D%E5%90%91%E9%87%8F%EF%BC%89.ipynb)
- [ Part 3 More Fun With Word Vectors（词向量的更多用法）](http://nbviewer.jupyter.org/github/BrambleXu/word2vec-movies/blob/master/Part%203%20More%20Fun%20With%20Word%20Vectors%EF%BC%88%E8%AF%8D%E5%90%91%E9%87%8F%E7%9A%84%E6%9B%B4%E5%A4%9A%E7%94%A8%E6%B3%95%EF%BC%89.ipynb)

## Dependencies

以下库全基于python3.5.2:

- pandas==20.3
- scikit-learn==0.19.0
- numpy==1.13.1
- jupyter==1.0.0

## 计划

因为这个笔记里的内容只是kaggle项目上给出的教学部分，实际得分最好也只有0.84，所以充其量只能是一个了解word2vec的教程，内容本身并不深入。

于是我找到了这个项目：[sentiment-analysis](https://github.com/pangolulu/sentiment-analysis)，作者写了三个模型，前两个在教程中出现过了，第三个使用Ensemble的方法把前两个模型组合了起来，最后得分能到0.96。而且作者代码组织得也不错，可以用来学习如何写一个完整的项目，而不是仅仅在Jupyter Notebook上写。

不过因为作者用的是python2，而且很多包的API变了，我打算用pytohn3重写一下，一边学习一边分享出来。项目地址在这里：[sentiment-analysis](https://github.com/BrambleXu/sentiment-analysis)

## 推荐读物

- [ NLP 秒懂词向量Word2vec的本质](https://zhuanlan.zhihu.com/p/26306795)：这篇文章做了一个word2vec学习路径，总结得很棒
- [基于神经网络的词和文档语义向量表示方法研究](http://licstar.net/archives/687)：这篇博士论文把各种词嵌入方法做了个梳理，很全面，而且中文看起来也容易一些，作者的博客里也非常推荐，有很多不错的文章。

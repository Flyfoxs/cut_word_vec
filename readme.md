## 解决如下几个问题

### 腾讯词向量的可视化

具体code可参考[Jupyter Notebook] (https://github.com/Flyfoxs/cut_word_vec/blob/master/notebook/visual.ipynb)

![Word Vec Screenshot](https://raw.githubusercontent.com/Flyfoxs/cut_word_vec/master/imgs/word_vec.png)


### 腾讯词库的定制:
具体code可参考[Jupyter Notebook]( https://github.com/Flyfoxs/cut_word_vec/blob/master/notebook/word_split.ipynb)

- 裁剪词库: 
	
开源词库特别大,加载慢,如何根据当前的任务裁剪. 因为字典表非常大,比如腾讯开源的词库有8,824,330个词, 解压后有16G. 针对当前的训练数据往往只是很小一部分,在训练时完全加载这么大的数据集是完全没有必要的,可以提前准备一个mini的字典.
	
	
- 减少oov的大小:
	
因为中文有分词的问题, 这样分词结果可能和字典表不匹配,导致oov,但是可以通过变通的办法取近似值. 比如"2019年年底",可以通过"2019" 和 "年底"来取平均值 





# 腾讯词向量下载地址

- https://ai.tencent.com/ailab/nlp/data/Tencent_AILab_ChineseEmbedding.tar.gz



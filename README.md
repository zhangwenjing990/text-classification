1，简单的词向量平均模型：

$${\bf{h}}_{avg}=\frac{1}{|\boldsymbol{x}|}\displaystyle\sum_{t}emb(x_{t})$$

正面情感的概率为：

$$\sigma({\bf{h}}_{avg}{\bf{w}}^{\rm{T}})$$

2，Attention 加权平均模型

词向量权值：$$\alpha_{t}=softmax(cosin({\bf{u}}, emb(x_{t})))$$

句子encoder: $${\bf{h}}_{att}=\displaystyle\sum_{t}\alpha_{t}emb(x_{t})$$

正面情感的概率为：

$$\sigma({\bf{h}}_{att}{\bf{w}}^{\rm{T}})$$

3，Self Attention模型


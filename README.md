# RSpapers
### 我整理的一些推荐系统相关的论文

主要是跟我研究相关的论文

---

* **Tag-aware RS：** 基于标签的推荐系统，使用标签来提高推荐准确率等
* **Attention Based RS：** 采用Attention机制的论文
* **realtime RecSystem：**  实时推荐系统


## Tag-aware RS
#### 1-liang2018-TRSDL Tag-Aware Recommender System
#### 2- Towards A Standardized Tag Recommender Benchmarking Framework 
[http://www.dominikkowald.info](http://www.dominikkowald.info/)
[github](https://github.com/learning-layers/TagRec)
发现了tag领域同道中人的github ，万岁！！o(*≧▽≦)ツ┏━┓
## Attention Based RS
#### 1-  NAIS: Neural Attentive Item Similarity Model for Recommendation.
[code](https://github.com/AaronHeee/Neural-Attentive-Item-Similarity-Model)
item similarity 
#### 2-MTNet:Neural Approach for Cross-Domain Recommendation with Unstructured Text
cross domain
#### 3-Neural Collaborative Filtering
[论文导读](https://www.paperweekly.site/papers/notes/390)
[pytorch实现](https://towardsdatascience.com/paper-review-neural-collaborative-filtering-explanation-implementation-ea3e031b7f96)
这篇论文导读给我一种“这才是论文导读的感觉啊”，一篇论文的正确读法：
* 动机
* 模型
* 实验
* 评价（读者的）

而不是翻译一篇论文，看别人的翻译不如自己看原文
>取代MF的一个基础模型
#### 4-Next Item Recommendation with Self-Attention
[论文导读](https://zhuanlan.zhihu.com/p/48069398)
> **本文提出了一种基于 self-attention 的基于序列的推荐算法**，利用**self-attention**来为用户短期行为模式的依赖关系和重要性建模。同时该模型也保留了用户的长久兴趣。整个网络在 **metric learning** 的框架下，是**第一次将 self-attention 和 metric learning的结合的尝试。**
#### 5-**Attention-based Transactional Context Embedding for Next-Item Recommendation**
[paper](http://203.170.84.89/~idawis33/DataScienceLab/publication/AAAI18-Wang.pdf)
[论文导读](https://blog.csdn.net/Zhongsigen/article/details/81704545)
>作者提出一个推荐算法，这个算法不仅考虑当前交易中所有的observed items，而且还要用不同的relevance(相关性)对它们进行加权，以建立一个attentive context(注意力上下文)，以高概率输出正确的下一个项目。模型——基于注意的事务嵌入模型（ATEM），用于上下文嵌入，以在不假定顺序的情况下对每个观察到的项目进行加权。


这篇导读对模型的介绍几乎没有，需要补全
$$Attention(Q,K,V)=Attention(Q, Q, Q)$$

### 6-self-attention 
[介绍博客-self attention in NLP](http://www.cnblogs.com/robert-dlut/p/8638283.html)

#### 7-Attentive collaborative filtering
Multimedia recommendation with item-and component-level attention
[论文导读](https://zhuanlan.zhihu.com/p/32787606)
利用多媒体内容特征学习component-level attention网络， 然后再利用该网络的结果学习item-level attention网络，其实就是嵌套了两层网络。

#### 8- A^3NCF: An Adaptive Aspect Attention Model for Rating Prediction
paper weekly 推荐的一篇论文
https://www.paperweekly.site/papers/2560 
[代码](https://github.com/hustlingchen/A3NCF)
>本文是新加坡国立大学发表于IJCAI 2018的工作，论文**基于评论文本**对用户偏好和商品特征进行抽取，提出了一种自适应注意力模型用于用户评论的智能排序，不断学习用户对商品在不同关注点方面的权重，进而提升推荐效果。本文解决了已有方法忽视不同用户对商品不同侧面关注点不同的缺陷，并且在Amazon Product Review和Yelp 2017这两个大规模推荐系统数据库上取得了领域内最好效果。

[](https://www.jianshu.com/p/46d36caa9688)
#### 9-Attention-based Group Recommendation
paper weekly 推荐的一篇论文
https://www.paperweekly.site/papers/2561
>本文来自南洋理工大学。作为个体的用户和群组成员的行为是不同的，作者基于用户评级历史的深度学习技术，提出了一个注意力群体推荐模型来解决群体推荐问题，模型自动学习群组中的每个用户的影响权重并根据其成员的权重偏好为群组推荐项目。虽然基于图和概率的模型已经得到了广泛的研究，但本文是第一个将Attention机制应用到群体推荐中的。

## 实时推荐系统
#### 1-StreamRec: a real-time recommender system ACM2011
#### 2-Streaming recommender systems
[paper](https://dl.acm.org/citation.cfm?id=3052627)
#### 3- RecSys'15 Tutorial on "Real-Time Recommendation of Streamed Data"
tutorial 不是论文
[地址](https://www.slideshare.net/fraho/recsys15-tutorial-on-realtime-recommendation-of-streamed-data)

## 交叉推荐
#### 1-Man, Tong et al. Cross-domain recommendation: an embedding and mapping approach. IJCAI, 2017.
[导读](https://zhuanlan.zhihu.com/p/30621349)

## 时序漂移
#### 1-Collaborative filtering with temporal dynamics
#### 2- taste over time: the temporal dynamics of user preferences
[paper](http://www.cs.cornell.edu/~jlmo/ismir13.pdf)

提出了一个动态嵌入概率模型，将用户和歌曲都嵌入一个d维欧几里得ko
<!--stackedit_data:
eyJoaXN0b3J5IjpbNzAyMzM0MzU4LDgzNDkwMDkwOSw5ODkxNT
YzNDcsLTY1NDkxMzcyNiwtMTg2MzA5NTMwNywtMTMxNjk2ODk1
MCwtMTgzMzA3ODY2MSwxMzQwMTM1NTI5LDE1MTU3NDk5NDAsMT
c0OTUyMzgzNiw0MzYxMzk1MDAsNDY3NDM1MzEsMTc2ODk0MTU5
NiwxNjIzODkzMjQwLC0xOTM2MzY2Mjk1LC0xOTAwNzk2NjExLD
ExMjA0MDg1NDAsOTQ3NTUyODg5LDE3NjY5MjIyMTcsLTE2OTkx
MTI2ODJdfQ==
-->
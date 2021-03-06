## 贝叶斯网络与EM算法

周志华机器学习第七章学习笔记。

- 贝叶斯网络 Bayes Nets

  > 1. 贝叶斯网又称信念网，一个刻画属性之间依赖关系的有向无环图（DAG)。一个贝叶斯网由结构G和参数Θ组成，记作B=< G, Θ >。描述如下，若两个属性有直接依赖关系，就将他们用一条边连接起来，并且参数Θ定量的描述其依赖关系，Θ一般用条件概率表来表示，在连续属性是条件概率表变为条件概率密度函数。
  >
  > 2. 从贝叶斯网结构中找到变量间的条件独立性。
  >    - 道德图 moral graph
  >
  > 3. 首要任务，通过训练数据集找到最恰当的贝叶斯网结构G
  >    - 定义评分函数：常用的评分函数基于信息论准则，将寻找最恰当的结构这一学习过程看作数据压缩任务，目标是找到一个用最短编码长度来描述训练数据的结构。
  >
  >      ![bayes-net-costfunction](../pics/bayes-net-costfunction.PNG)
  >
  >      上式是给定数据集*D*，贝叶斯网*B*=< G, Θ >在*D*上的评分函数。其中，*f(θ)*贝叶斯网络的每一个参数用多少字节表示；|*B*|代表贝叶斯网参数的个数；*LL*代表log likelihood function，也就是计算贝叶斯网*B*所对应的概率分布![bays-net-probablistic-distribution](../pics/bays-net-probablistic-distribution.PNG)对数据集*D*描述的有多好。
  >
  >      - 当 *f(θ)* = 1，得到**AIC**评分函数；Akaike Information Criterion
  >
  >
  >      - 当 *f(θ)* = (1/2)* log(m)，得到**BIC**评分函数；Bayesian Information Criterion
  >
  >
  >      - 当 *f(θ)* =0，不计算网络进行编码的长度，评分函数退化为对数似然，相应的学习任务退化成极大似然估计；
  >
  >    - 由于在某个贝叶斯网结构上的最优参数可以很方便的在训练集上通过计数获得，所以问题转换成在所有可能的网络结构空间中搜寻最优的贝叶斯网络结构。然而这个问题确实一个**NP难**问题，周志华老师列出了两种在有限时间内求得近似解的策略：**贪心法**和施加约束。
  >
  > 4. 推断 Inference
  >
  >    ​
  >
  > ​

- Representing joint distributions with conditional independence assumptions

- Inference

- Learning from fully observed data

- Learning from partially observed data

- 期望最大化算法 EM

- 半监督学习 Semi-supervised learning

- 高斯混合聚类 Mixture of Gaussian clustering

- K-means clustering
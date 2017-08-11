## 贝叶斯网络与EM算法

- 贝叶斯网络 Bayes Nets

  > 1. 贝叶斯网又称信念网，一个刻画属性之间依赖关系的有向无环图（DAG)。一个贝叶斯网由结构G和参数Θ组成，记作B=< G, Θ >。描述如下，若两个属性有直接依赖关系，就将他们用一条边连接起来，并且参数Θ定量的描述其依赖关系，Θ一般用条件概率表来表示，在连续属性是条件概率表变为条件概率密度函数。
  > 2. 从贝叶斯网结构中找到变量间的条件独立性。
  >    - 道德图 moral graph
  > 3. 首要任务，通过训练数据集找到最恰当的贝叶斯网结构G
  >    - 定义评分函数
  > 4. 推断 Inference
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
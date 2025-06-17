# Lora

在机器学习中，我们通常使用一个矩阵来表示一个全连接层，但是这个全连接层往往是[过参数化](https://zhida.zhihu.com/search?content_id=235586149\&content_type=Article\&match_order=1\&q=%E8%BF%87%E5%8F%82%E6%95%B0%E5%8C%96\&zhida_source=entity)的，这意味着我们可以通过计算这个矩阵的秩来确定哪些特征是重要和相关的。换句话说，我们试图找到原始特征空间（或矩阵）中少数维度的（线性）组合，能够捕捉数据集中大部分的信息且一旦我们找到了足够解决问题的参数空间，再增加这个参数空间的大小并不会显著提升模型的性能。**所以只要调整这一部分的参数可以达到调整所有参数同样的效果同时减少GPU使用量**

<figure><img src="../.gitbook/assets/屏幕截图 2025-06-17 221547.png" alt=""><figcaption><p>原理图</p></figcaption></figure>

**原理:**

在大模型的矩阵$W\in R^{d\times k}$ 旁插入多一个$\Delta W$ 但是由于可以低秩分解于是可以分解成$AB=\Delta W$ ,其中$A \in R^{d \times r}$ ,$B \in R^{r \times k}$ ,然后我们只要训练$A$ 和$B$ 即可最后把$AB$ 加到$W$ 中即可。

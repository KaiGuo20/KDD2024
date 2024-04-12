# KDD2024
**To review 1** 

**Novelty:** 5: Above Average    

**Technical Quality:** 4: Average

Q1: "In contrast, we observe that the linear classification layer tends to compromise graph OOD generalization capability." I think this part is relatively not well supported. More insight would be helpful.

A1: Thanks for your question. In addition to the results presented in section 3.4 of our paper, which indicates that GCN without an additional linear classifier performs better, we also conducted experiments on GAT. Table 1 and 2 still demonstrate that GAT without an additional linear classifier performs better. The reason is that the the additional linear layer introduces more parameters to the model architecture, which increases the risk of overfitting. This could potentially hinder performance when faced with OOD distribution shifts. By omitting this layer, we amplify the graph’s intrinsic structure, leading to improved OOD generalization.
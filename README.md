# AG_News_Classification

最佳結果: 在7600筆測試集(test.csv中的全部)取的94.7%的acc

使用的預訓練模型是"bert-base-uncased"  
訓練過程中，learning_rate一開始設1e-5逐步降到1e-7

training set: 120000筆(train.csv中全部的data)
test set: 7600筆(test.csv中全部的data)

做的測試&實作過程:
一開始Data只用Title沒有用Description，train出來的結果最佳在test set可以取的90.1%的acc
再來換Data只用Description沒有用Title，train出來的結果最佳在test set可以取的93.6%的acc
以上可以大概得知Description的資訊可以比Title多很多，最後用Title +Description進去跑，train出來的結果最佳在test set可以取的94.7%的acc。


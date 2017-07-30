# Sphereface-model
This is the pre-trained model of SphereFace : Deep Hypersphere Embedding for Face Recognition.
This model is trained on Webface and the accuracy on LFW is **99.13%**. I set the lambda=5 firstly and only got a accuracy of 98.8%， which is much lower than the paper claimed(**~99.26%**). Then, I decreased the lambda and continue training. Fortunately, I found the accuracy is increasing.

I think the performance can still be further improved by carefully fine-tuning. Feel free to use this model.
# Experiment Results
Train 28000(lambda=3.6, batch_size=170):

|Original | With PCA | With mirror trick| With mirror trick and PCA |
|:---------:|:---------:|:---------------:|:-----------------:|
| 99.86%  |  99.13%   |    98.85%       |99.12%           |

Here is the model:   http://pan.baidu.com/s/1miietDm

## Reference
https://github.com/wy1iu/sphereface

https://github.com/happynear/NormFace/blob/master/MirrorFace.md

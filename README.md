# Sphereface-model
This is the pre-trained model of SphereFace : Deep Hypersphere Embedding for Face Recognition.
This model is trained on Webface and the accuracy on LFW is **99.18%**. I set lambda=5 firstly and only got an accuracy of 98.8%， which is much lower than the paper claimed(**~99.26%**). Then, I decreased the lambda and continue training. Fortunately, I found the accuracy is still increasing.

I think the performance can still be further improved by carefully fine-tuning. Feel free to use this model.
# Experiment Results
Train 22000(lambda=3.6, batch_size=170).

![Feature distribution](https://github.com/goodluckcwl/Sphereface-model/hist.jpg)


|Original | With PCA | With mirror trick| With mirror trick and PCA |
|:---------:|:---------:|:---------------:|:-----------------:|
| 98.88%  |  99.13%   |    98.98%       |**99.18%**           |

Here is the model:   https://pan.baidu.com/s/1pL0pmll

**LFW** evluation code can be found in [https://github.com/happynear/FaceVerification]. 

## Reference
https://github.com/wy1iu/sphereface

https://github.com/happynear/NormFace/blob/master/MirrorFace.md

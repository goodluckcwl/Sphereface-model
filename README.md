# Sphereface-model
This is the pre-trained model of SphereFace : Deep Hypersphere Embedding for Face Recognition.
This model is trained on CASIA-Webface and the accuracy on LFW is **99.18%**. 
- Training on Webface with the default setting only got an accuracy of 98.5%， which is much lower than the paper claimed(**~99.26%**). 
- Fixed lambda = 5, kept on training, and got an accuracy of 98.8%.
- Decreased the lambda. Final accuracy is 99.18%.

I think the performance can still be further improved by carefully fine-tuning. Feel free to use this model.
# Experiment Results
Train 22000(lambda=3.6, batch_size=170).

The distribution of features on LFW:

![Feature distribution](https://github.com/goodluckcwl/Sphereface-model/raw/master/hist-cos.jpg)

The roc curve:

![ROC](https://github.com/goodluckcwl/Sphereface-model/raw/master/roc.jpg)

Accuracy on LFW:

|Original | With PCA | With mirror trick| With mirror trick and PCA |
|:---------:|:---------:|:---------------:|:-----------------:|
| 98.88%  |  99.13%   |    98.98%       |**99.18%**           |

Here is the model:   https://pan.baidu.com/s/1pL0pmll

**LFW** evaluation code can be found in [https://github.com/happynear/FaceVerification]. 

# Update
- Accuracy on LFW 99.18%  2017.07.31

## Reference
https://github.com/wy1iu/sphereface

https://github.com/happynear/NormFace/blob/master/MirrorFace.md

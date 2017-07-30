# Sphereface-model
This is the pre-trained model of SphereFace : Deep Hypersphere Embedding for Face Recognition. The accuracy on LFW is 99.13%. I set the lambda=5 firstly and only got a accuracy of 98.8%， which is much lower than the paper claimed(~99.26%). Then, I decreased the lambda and continue training. Fortunately, I found the accuracy is increasing.
I think the accurracy can still be further improved by carefully fine-tuning. Feel free to use this model.
# Experiment Results
Train 28000:

|Original | With PCA | With mirror trick| With mirror trick and PCA |
|---------|:---------:|:---------------:|-----------------:|
| 99.86%  |  99.13%   |    98.85%       |99.12%           |


## Reference
https://github.com/wy1iu/sphereface

https://github.com/happynear/NormFace/blob/master/MirrorFace.md

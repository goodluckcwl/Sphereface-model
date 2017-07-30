# Sphereface-model
This is the pre-trained model of SphereFace : Deep Hypersphere Embedding for Face Recognition. The accuracy on LFW is 99.08%. I set the lambda=5 firstly and only got a accuracy of 98.8%. Then, I decreased the lambda and continue finetuned. Fortunately, I found the accuracy is increasing.
# Experiment Results
|Original | With PCA | With mirror trick |
|---------|:---------:|-----------------:|
| 99.01%  |  99.08%   | 99.08%           |


## Reference
https://github.com/wy1iu/sphereface
https://github.com/happynear/NormFace/blob/master/MirrorFace.md

# 2022 - 2 HUFS 기계학습 텀 프로젝트
- 학과 : 수학과
- 이름 : 김인겸

#### [About project]
Tensorflow 샘플 내에서 볼 수 있는 기본적인 데이터인 MNIST Dataset을 이용하여 각 모델들을 구현했습니다.
<br>
4장 내 생성 모델인 GAN(generative adversarial network)과 6장 내 Autoencoder의 유사한 점과, 다른 점에 대하여 직접 구현해 보고 알아보았습니다.
<br>


#### [Source code] / GAN.ipnyb & Autoencoder.ipnyb

- Simple GAN 구현 : Pytorch 를 통해 구현했습니다.
- Autoencoder 구현 : Tensorflow 를 통해 구현했습니다.

#### 참고자료
[Goodfellow2014](https://arxiv.org/pdf/1406.2661.pdf)
<br>
[Autoencoder구현](https://github.com/ExcelsiorCJH/Hands-On-ML/blob/master/Chap15-Autoencoders/Chap15-Autoencoders.ipynb)

#### +) Pytorch에서 MNIST Dataset 불러오기
```
import torch
import torch.nn as nn
import torch.nn.functional as F
import torch.optim as optim
import torchvision.utils as utils
import torchvision.datasets as dsets
import torchvision.transforms as transforms

from torchvision import datasets
import torchvision.transforms as transforms
from torch.utils.data import DataLoader
from torchvision.transforms.functional import to_pil_image
import matplotlib.pylab as plt
```


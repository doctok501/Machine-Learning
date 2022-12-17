# 2022 - 2 HUFS 기계학습 텀 프로젝트
- 학과 : 수학과
- 이름 : 김인겸

#### [About project]
Tensorflow 샘플 내에서 볼 수 있는 MNIST Dataset을 이용하여 각 모델들을 구현했습니다.
<br>
4장 내 생성 모델인 GAN(generative adversarial network)과 6장 내 Autoencoder의 유사한 점과, 다른 점에 대하여 직접 구현해 보고 알아보았습니다.
<br>
#### [프로젝트 내용과 결과 설명]

GAN 과 오토인코더 모두 딥러닝을 이용하여 가상의 이미지를 만듭니다.
<br>
그러나, GAN이 세상에 없는 완전한 가상의 것을 만들어 내는 것과는 달리,
<br>
오토인코더는 입력데이터가 주어졌을때, 이 특징을 잡아내어 이를 이용한 가상의 이미지를 생성해 낸다는 점에서 차이가 있습니다.
<br>
 [GAN](https://github.com/doctok501/Machine-Learning/blob/main/GAN%20vs%20Autoencoder/GAN.ipynb)에서 마지막 결과 이미지 확인 부분을 보면, 새로운 손글씨가 생성됨을 알 수 있습니다. 
<br>
    그러나, [Autoencoder](https://github.com/doctok501/Machine-Learning/blob/main/GAN%20vs%20Autoencoder/Autoencoder.ipynb)에서 결론 부분을 보면, 위의 입력된 데이터를 이용하여 새로운 가상의 이미지를 만들어낸다는 것을 알 수 있습니다.



#### [Source code] / GAN.ipnyb & Autoencoder.ipnyb

- Simple GAN 구현 : Pytorch 를 통해 구현했습니다.
- Autoencoder 구현 : Tensorflow 를 통해 구현했습니다.

#### [참고자료]
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



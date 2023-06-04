# Siamese neural network One-shot learning Paper model
> Siamenetwork 구조를 적용한 모델 학습 프로젝트이다.

> AT&T dataset을 활용하여 한쌍의 숫자 이미지에 대한 유사도를 판별한다.


# 데이터셋 AT&T
![Alt text](https://4.bp.blogspot.com/-_289WYEeNks/WMC3wZ7SjHI/AAAAAAAAAz0/be3-bvMYwKYBVq8DzPh_ZLwJ4qMzTBhowCLcB/s1600/ATT.png)

> 40명의 사람들에 대한 다양한 표정으로 찍힌 얼굴 사진이 각각 10장씩 포함되어 있는 데이터셋이다.


# 모델
### 1. Siamese network 논문
> https://www.cs.cmu.edu/~rsalakhu/papers/oneshot1.pdf


### 2. What is Siamese network?
> 두 개의 입력 이미지를 비교하여 유사도를 측정하는 모델 구조이다.

> 새로운 이미지에 대한 유사성을 예측할 수 있다.

> 두 개의 동일한 네트워크 공유 가중치로 구성되며 각 네트워크는 입력 이미지를 임베딩 하는 역할을 수행한다.

> 각각의 입력 이미지는 네트워크를 통과한 후 이미지의 핵심 특징을 나타내는 임베딩 벡터로 변환된다.

> 두 임베딩 벡터의 유클리디란 거리를 계산 후, 거리의 값이 작을수록 두 이미지가 유사하다고 판단한다.

> Siamese Network는 손실 함수를 통해 학습된다.
>> Training label에는 이미지 쌍의 유사성(유사할 경우1, 다른 경우 0)이 포함된다. 모델은 입력 이미지 쌍을 임베딩 하여 거리를 계산하고, 이를 기반으로 유사성을 예측한다. 손실 함수는 예측된 label과 실제 label의 차이를 최소화하기 위해 모델의 가중치를 조정한다.


# 사이트
### 1. link
> 두명의 사진을 입력받고, 두 사진속 인물의 얼굴 유사도를 퍼센테이지로 보여주는 사이트이다.

> http://3.35.4.129/

### 2. github
> https://github.com/YoonHyunWoo/A.child
> https://github.com/MyungSub0519/A.child



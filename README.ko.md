# 딥러닝 연습장

딥러닝과 다양한 뉴럴 네트워크 구현을 주피터 노트북과 파이썬을 이용해 연습한 내용입니다. 내용은 대부분 영어로 작성되었습니다.

다른 머신러닝 방법들이나 강화학습에 대한 내용은 다른 리포지토리에 저장했습니다.

저는 이 프로젝트가 딥러닝과 신경망에 이론과 실용에 대한 좋은 참고자료가 되었으면 합니다.

* Read this in other language: [English](README.md)

## 실행환경
- Python3.6
    - requirement.txt 안에 모든 파이썬 패키지가 들어있습니다.
    - 패키지 설치:  
        - cpu만 이용하는 경우  

        ```
        $ pip install -r requirements.txt
        ```

        - gpu를 같이 이용하는 경우  

        ```
        $ pip install -r requirements_gpu.txt
        ```

    - 패키지 설치는 파이썬 가상환경(virtualenv) 안에서 하는걸 추천합니다.
    - 주로 케라스(Keras)와 텐서플로(TensorFlow)를 이용해 작성했습니다.
    - 텐서플로를 GPU(그래픽카드)와 함깨 사용하려면 requirement.txt 안에 tensorflow 패키지를 tensorflow-gpu 로 바꾸면 됩니다.
- TensorFlow 1.5.0


## 목차

### 지도학습 (Supervised Learning)    
0. 신경망 이론
    1. 뉴런과 퍼셉트론  
    2. 활성화함수
    3. 경사하강법
    4. __Back Propagation__
        1. __Stochastic Gradient Descent__
        2. __Adam__
1. 회귀
    1. 간단한 선형 회귀
        1. 경사하강법 구현연습
    2. 최소제곱법
    3. 다층 뉴럴 네트워크 회귀 연습
    4. 보스턴 집값 데이터를 이용한 회귀 모델
    - 활성화함수
2. 비전 w/ __Keras__  
    1. 간단한 분류기 연습  
    2. MNIST 이미지 분류 - 단일 전연결 계층  
        1. Single Dense Layer w/ Visualization  
    3. MNIST 이미지 분류 - 이중 전연결 계층  
    4. 다중 전연결 신경망  
    5. 합성곱 필터  
        1. 풀링 계층  
        2. MNIST 이미지 분류 - 합성곱+전연결 네트워크  
        3. CIFAR10 이미지 분류 - 합성곱+전연결 네트워크  
        4. fashion_MINST 이미지 분류 - 합성곱+전연결 네트워크  
    6. MNIST 이미지 분류 - VGG 16,19 네트워크 예제  
    7. CIFAR10 이미지 분류 - ResNet 네트워크 예제  
3. 문장과 시계열  
    1. IMDB 댓글 분류기 - 일차원 합성곱 네트워크  
    2. IMDB 댓글 감정 분류기 - LSTM 네트워크  
    3. 이진 가산기 - 단순 순환네트워크  
    4. Airline - 단순 순환네트워크  
    5. Power Consumption - LSTM 활용 예측기
    6. 십진 가산기 - LSTM 활용 예측기

### 비지도학습 (Unsupervised Learning)
4. 자동 부호화기 (Autoencoder)
    1. MNIST - Autoencoder Fully Connected
    2. MNIST - Autoencoder CNN
    3. CIFAR10 - UNET Color Restoration
5. Generative Adversarial Networks
    1. Probabilistic Distribution - Fully Connected GAN
    2. MNIST - CNN GAN

* 기울림 글씨는 아직 미완성된 노트라는 의미입니다.

## Miscellaneous Notes

- 유용한 기능
    - 케라스 (Keras)
        - 저장과 불러오기 Save/Load Model
        - 이미지 프로세싱 Preprocessing Image (Augmented Image Generator)
    - 텐서플로 (TensorFlow)
        - 문법 Basic Grammer
        - 저장과 불러오기 Save, Load
        - 텐서보드 Tensorboard

## 참조

Some data was brought from https://github.com/Jpub/TensorflowDeeplearning jupyter_tfbook

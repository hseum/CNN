# CNN 실습

<aside>
<img src="https://www.notion.so/icons/command-line_pink.svg" alt="https://www.notion.so/icons/command-line_pink.svg" width="40px" />

**학습목표**

- 핵심 이론으로 감잡고 빠르게 구현하기
- 시각적으로 보기
- 엔비디아는 왜 떡상했는가?
</aside>

<aside>
<img src="https://www.notion.so/icons/command-line_pink.svg" alt="https://www.notion.so/icons/command-line_pink.svg" width="40px" />

**Contact**

[hseum - Overview](https://github.com/hseum)

[www.linkedin.com](https://www.linkedin.com/in/hyeonsik-eum-1993272a6/)

[Instagram (@hyeonsik.eum)](https://www.instagram.com/hyeonsik.eum/)

</aside>

# Datasets

[[python/AI] MNIST란? MNIST 데이터 개념 / 컴퓨터 비전 / 인공신경망](https://cobinding.tistory.com/16)

# CNN

- 이론적 배경

[[Deep Learning 101] 합성곱신경망 CNN, Convolutional Neural Network](https://www.youtube.com/watch?v=lDqn1UNwgrY&t=356s)

- 실습예시

[[Deep Learning 101] 나만의 CNN을 만들어보자](https://www.youtube.com/watch?v=zjuc3ogUYmM&t=1415s)

<aside>
<img src="https://www.notion.so/icons/command-line_pink.svg" alt="https://www.notion.so/icons/command-line_pink.svg" width="40px" />

**visualization**

[Convolutional Neural Network (CNN) Visualization](https://youtu.be/enjnRVUoH9g?feature=shared)

[Convolutional Neural Networks Explained (CNN Visualized)](https://www.youtube.com/watch?v=pj9-rr1wDhM)

</aside>

# colab

[https://github.com/hseum/CNN](https://github.com/hseum/CNN)

# GPU

```python
# GPU 사용 가능 여부 확인
import torch

if torch.cuda.is_available():
    device = torch.device("cuda")
    print("GPU 사용 가능")
else:
    device = torch.device("cpu")
    print("GPU 사용 불가능 - CPU 사용")

print(f"Using device: {device}")

# 모델을 GPU로 이동
model = SimpleCNN().to(device)
```
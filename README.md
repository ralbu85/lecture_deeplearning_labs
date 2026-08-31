# 딥러닝 — 코딩 실습 노트북

부경대학교 시스템경영공학부 **딥러닝** (담당: 이지환) 코딩 실습 노트북입니다.
강의 사이트의 실습 페이지에서 자동 생성되며, 배지를 누르면 **Google Colab**에서 바로 열립니다.

| 주차 | 실습 | Colab |
|:---:|---|:---:|
| 1 | 데이터를 행렬로 — 벡터와 행렬 다루기 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ralbu85/lecture_deeplearning_labs/blob/main/lab01.ipynb) |
| 2 | 퍼셉트론을 쌓아 신경망 만들기 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ralbu85/lecture_deeplearning_labs/blob/main/lab02.ipynb) |
| 3 | 학습 루프를 직접 만든다 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ralbu85/lecture_deeplearning_labs/blob/main/lab03.ipynb) |
| 4 | 진짜 표 하나를 끝까지 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ralbu85/lecture_deeplearning_labs/blob/main/lab04.ipynb) |
| 5 | 이미지를 텐서로, 콘볼루션을 코드로 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ralbu85/lecture_deeplearning_labs/blob/main/lab05.ipynb) |
| 6 | CNN 구조 만들고 학습시키기 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ralbu85/lecture_deeplearning_labs/blob/main/lab06.ipynb) |
| 7 | 전이학습 — 사진 몇백 장으로 학습시키기 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ralbu85/lecture_deeplearning_labs/blob/main/lab07.ipynb) |
| 9 | 객체탐지 — IoU와 NMS를 직접 구현하기 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ralbu85/lecture_deeplearning_labs/blob/main/lab09.ipynb) |
| 10 | 텍스트를 숫자로 — 토큰화와 임베딩 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ralbu85/lecture_deeplearning_labs/blob/main/lab10.ipynb) |
| 11 | 어텐션을 손으로 만들기 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ralbu85/lecture_deeplearning_labs/blob/main/lab11.ipynb) |
| 12 | Transformer 블록과 언어모델 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ralbu85/lecture_deeplearning_labs/blob/main/lab12.ipynb) |

## 사용법

- 실습은 **채점하지 않는 연습장**입니다. 직접 타이핑하며 따라 실행하고, 숫자를 바꾸어 결과를 확인합니다.
- `✏️ 직접 채워 보세요` 셀은 스스로 작성한 뒤, 바로 아래 정답 셀과 맞춰 봅니다.
- 데이터는 모두 인터넷에서 바로 내려받으므로 별도 준비가 필요 없습니다.
- 이론 설명은 강의 사이트에 있습니다.

## 만드는 것과 배우는 부품

| 주차 | 완성하는 것 | 그 주에 새로 배우는 PyTorch 부품 |
|:---:|---|---|
| 1 | 표·사진·문장을 각각 행렬로 만들고, 행렬 곱으로 예측 | `Tensor` · `shape`/`dtype` · 인덱싱·마스크 · `dim`/`keepdim` · `reshape`/`.T`/`unsqueeze` · 브로드캐스팅 · `@` |
| 2 | 마력→연비, 세 모형 비교 (선형 / 활성화 없음 / ReLU) | `nn.Linear` · 활성화 모듈 · `nn.Sequential` · `TensorDataset` · `DataLoader` · `torch.optim` |
| 3 | 펭귄 3종 분류 (학습 루프를 직접 작성) | `CrossEntropyLoss` · `requires_grad`/`backward` · `torch.optim` |
| 4 | 자동차 9변수→연비 (분할·미니배치·조기 종료) | `batch_size`/`shuffle` · `train()`/`eval()` · `state_dict` |
| 5 | 옷 3종 분류 (파라미터 235개 CNN) | `Conv2d` · `transforms` · `ImageFolder` 이전 단계 |
| 6 | CIFAR-10 3종 분류 (Flatten vs GAP) | `MaxPool2d` · `AdaptiveAvgPool2d` · `nn.Module` 서브클래싱 |
| 7 | 개미·벌 397장 (처음부터 / 동결 / 미세조정) | `ImageFolder` · `models.resnet18` · `requires_grad=False` |
| 9 | 물체 위치 예측 (박스 회귀, IoU 평가) | `box_iou` · `nms` · 회귀 헤드 |
| 10 | 네이버 영화 리뷰 감성 분류 | `nn.Embedding` · HuggingFace 토크나이저 · 패딩·마스크 |
| 11 | 같은 과제를 어텐션으로 (본 단어 시각화) | `softmax` 마스킹 · `MultiheadAttention` |
| 12 | Transformer 블록 조립 + GPT-2 검산·생성 | `LayerNorm` · 잔차 · `AutoModelForCausalLM` |

랩은 **PyTorch 표준 부품만** 씁니다. 편의를 위한 별도 헬퍼 함수(`fit()` 같은)는 만들지 않습니다 —
학습 루프는 2주차부터 12주차까지 같은 네 줄이 그대로 반복됩니다.

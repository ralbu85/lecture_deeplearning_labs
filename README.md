# 딥러닝 — 코딩 실습 노트북

부경대학교 시스템경영공학부 **딥러닝** (담당: 이지환) 코딩 실습 노트북입니다.
강의 사이트의 실습 페이지에서 자동 생성되며, 배지를 누르면 **Google Colab**에서 바로 열립니다.

| 주차 | 실습 | Colab |
|:---:|---|:---:|
| 1 | 펭귄의 몸무게를 맞히는 첫 모형 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ralbu85/lecture_deeplearning_labs/blob/main/lab01.ipynb) |
| 2 | 층을 쌓아 직선을 벗어나기 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ralbu85/lecture_deeplearning_labs/blob/main/lab02.ipynb) |
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

## 각 주차가 만드는 것

| 주차 | 완성하는 학습 |
|:---:|---|
| 1 | 펭귄 치수 → 몸무게 회귀 (경사하강법 = 수학적 정답 확인) |
| 2 | 자동차 마력 → 연비 (선형 / 활성화 없음 / ReLU 세 모형 비교) |
| 3 | 펭귄 3종 분류 (학습 루프를 직접 작성) |
| 4 | 자동차 9개 변수 → 연비 (미니배치 · 조기 종료 · 진단) |
| 5 | 옷 사진 3종 분류 (파라미터 235개 CNN, 학습된 커널 시각화) |
| 6 | CIFAR-10 3종 분류 (Flatten vs GAP 비교) |
| 7 | 개미·벌 사진 397장 (처음부터 / 동결 / 미세조정 비교) |
| 9 | 물체 위치 예측 (박스 회귀, IoU로 평가) |
| 10 | 네이버 영화 리뷰 감성 분류 (임베딩 + 마스크 평균) |
| 11 | 같은 과제를 어텐션으로 (모형이 본 단어 시각화) |
| 12 | Transformer 블록 조립 + GPT-2 파라미터 검산 · 문장 생성 |

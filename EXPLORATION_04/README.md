# EXPLORATION_04

4. 작사가 인공지능 만들기
### 멋진 작사가 만들기
---

**Step 1. 데이터 다운로드**

- [Song Lyrics](https://www.kaggle.com/paultimothymooney/poetry/data)에서 다운로드

**Step 2. 데이터 읽어오기**
- glob 를 활용하여 모든 txt 파일을 읽어온 후, raw_corpus 리스트에 문장 단위로 저장

**Step 3. 데이터 정제**
- 토큰화 했을 때 토큰의 개수가 15개를 넘어가는 문장을 학습 데이터에서 제외하기를 권장

**Step 4. 평가 데이터셋 분리**
- 단어장의 크기는 12,000 이상 으로 설정하고 총 데이터의 20%를 평가 데이터셋으로 사용

**Step 5. 인공지능 만들기**
- 모델의 Embedding Size와 Hidden Size를 조절하며 10 Epoch 안에 val_loss 값을 2.2 수준으로 줄일 수 있는 모델을 설계

**"i love"로 시작하는 모델이 생성한 가사 한 줄을 제출하세요.**

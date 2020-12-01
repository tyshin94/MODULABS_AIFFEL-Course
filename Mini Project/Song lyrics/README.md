# Song lyrics project
## 작사가 만들기

### Step 1. Data 다운로드
---

### Step 2. Data 읽어오기
---

### Step 3. Data 정제
---

### Step 4. 평가 데이터셋 분리
---

### Step 5. 인공지능 만들기
---

### 정리
- Batch Normalization를 활용하여 성능을 더 좋게 만들 수 있었음
    - BN을 layer에 두 번 활용할 경우 Overfitting이 더 자주 일어남
    - BN을 한 번은 LSTM_2과 Dense 레이어 사이에 넣어서 실행
    - 나머지 한 번은 LSTM_1과 LSTM_2 레이어 사이에 넣어서 실행
- 전체 단어의 개수는 1201개 이상 진행할 시 쉽게 Overfitting이 일어남
    - Word 수를 줄일 수록 더 좋은 모형을 드러냄

 ```결론```
 - word = 1200, batch 1 (LSTM_1 ~ LSTM_2 layer), embedding size = 256, learning rate = 0.001
 - **val_loss: 2.0889**
 - 요구하는 val_loss 2.2 이하 맞춤

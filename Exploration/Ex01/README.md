# AIFFEL Campus Online Code Peer Review Templete
- 코더 : 이호창
- 리뷰어 : 이치오

# PRT(Peer Review Template)
- [x]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요?**
    - 문제에서 요구하는 최종 결과물이 첨부되었는지 확인
        - 중요! 해당 조건을 만족하는 부분을 캡쳐해 근거로 첨부
        - 프로젝트 1의 회귀모델 예측정확도가 기준 이상 높게 나왔는가? (MSE 손실함수값 3000 이하를 달성)
        - ![image](https://github.com/user-attachments/assets/49f9412a-6a5f-4f07-90d6-4c0bbc02c45e)
        - 프로젝트 2의 회귀모델 예측정확도가 기준 이상 높게 나왔는가? (RMSE 값 150 이하를 달성)
        - ![image](https://github.com/user-attachments/assets/a010cbae-9548-4cf1-97c7-998fe90f148e)
        - 시각화 요구사항이 정확하게 이루어졌는가? (각 프로젝트 진행 과정에서 요구하고 있는 데이터개수 시각화 및 예측결과 시각화를 모두 진행하였다.)
        - ![image](https://github.com/user-attachments/assets/719a26a2-00bb-41fd-935c-86712ff763fd)
        - ![image](https://github.com/user-attachments/assets/12da6a40-abb1-4bd7-ab2d-f0fa9c95fde9)
        - ![image](https://github.com/user-attachments/assets/de04d4fb-0a4e-4cff-acc4-cd284268e111)
    
- [ ]  **2. 전체 코드에서 가장 핵심적이거나 가장 복잡하고 이해하기 어려운 부분에 작성된 
주석 또는 doc string을 보고 해당 코드가 잘 이해되었나요?**
    - 해당 코드 블럭을 왜 핵심적이라고 생각하는지 확인
    - 해당 코드 블럭에 doc string/annotation이 달려 있는지 확인
    - 해당 코드의 기능, 존재 이유, 작동 원리 등을 기술했는지 확인
    - 주석을 보고 코드 이해가 잘 되었는지 확인
        - 중요! 잘 작성되었다고 생각되는 부분을 캡쳐해 근거로 첨부
        
- [x]  **3. 에러가 난 부분을 디버깅하여 문제를 해결한 기록을 남겼거나
새로운 시도 또는 추가 실험을 수행해봤나요?**
    - 문제 원인 및 해결 과정을 잘 기록하였는지 확인
    - 프로젝트 평가 기준에 더해 추가적으로 수행한 나만의 시도, 
    실험이 기록되어 있는지 확인
        - 중요! 잘 작성되었다고 생각되는 부분을 캡쳐해 근거로 첨부
        - ![image](https://github.com/user-attachments/assets/27c98952-83de-453d-b5f9-6a73f4586784)

- [ ]  **4. 회고를 잘 작성했나요?**
    - 주어진 문제를 해결하는 완성된 코드 내지 프로젝트 결과물에 대해
    배운점과 아쉬운점, 느낀점 등이 기록되어 있는지 확인
    - 전체 코드 실행 플로우를 그래프로 그려서 이해를 돕고 있는지 확인
        - 중요! 잘 작성되었다고 생각되는 부분을 캡쳐해 근거로 첨부
        
- [x]  **5. 코드가 간결하고 효율적인가요?**
    - 파이썬 스타일 가이드 (PEP8) 를 준수하였는지 확인
    - 코드 중복을 최소화하고 범용적으로 사용할 수 있도록 함수화/모듈화했는지 확인
        - 중요! 잘 작성되었다고 생각되는 부분을 캡쳐해 근거로 첨부
        - ![image](https://github.com/user-attachments/assets/291fb4e9-4508-488e-a770-627a1a616ca6)

# 회고(참고 링크 및 코드 개선)
```
# 리뷰어의 회고를 작성합니다.
# 원래 주어진 코드를 행렬곱 연산자를 이용해 가독성을 향상시켰다.
def my_model(X, W, b): 
    predictions = 0
    predictions = X @ W
    predictions += b
    return predictions

def ori_model(X, W, b):
    predictions = 0
    for i in range(10):
        predictions += X[:, i] * W[i]
    predictions += b
    return predictions
# 코드 리뷰 시 참고한 링크가 있다면 링크와 간략한 설명을 첨부합니다.
# 코드 리뷰를 통해 개선한 코드가 있다면 코드와 간략한 설명을 첨부합니다.
```


### Hi there 👋

<!--
**mingyu3619/mingyu3619** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

# Pretrain 모델과 커스텀 모델을 이용한 마스크 착용 판별

코로나 19로 인해 마스크가 생필품이 되면서, 이걸을 사람이 아닌 컴퓨터 비전 기술을 이용하여 마스크 착용 여부를 알 수 있게하는 프로젝트.

사용 모델: CNN, Resnet50 

# 데이터 수집

크롤링.ipynb 파일을 통해 크롤링
colab을 통해 키워드 '마스크'와 키워드 '얼굴'을 통해 마스크를 쓴 사람과 안쓴 사람의 이미지 수집.

# 실험 

cnn에 모델의 epoch에 따른 성능

![image](https://user-images.githubusercontent.com/86222639/146324198-5535e33a-1c77-4cee-b667-4f889242287f.png)

Resnet50의 사전에 설정된 weights 여부에 따른 성능

![image](https://user-images.githubusercontent.com/86222639/146324246-d5d9324d-38f5-4d37-aedb-7a335f86a245.png)

--> resnet50은 overffiting된 모습이다.

# 결과
실험결과를 토대로 성능이 더 우수한 커스텀 cnn을 이용해 마스크 인식 여부 예측

label / 예측

![image](https://user-images.githubusercontent.com/86222639/146322810-9e22b061-1678-4e41-ab97-fc95db9218fd.png)

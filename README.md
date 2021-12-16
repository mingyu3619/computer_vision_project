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
cnn에 모델의 epoch에 따란 성능
![image](https://user-images.githubusercontent.com/86222639/146323343-8b534697-89d9-42be-a7e8-9520ac18c2e9.png)

Resnet50의 사전에 설정된 weights 여부에 따른 성능
![image](https://user-images.githubusercontent.com/86222639/146323504-85f9464e-8367-4abd-9e5d-8cd150e5285f.png)

![image](https://user-images.githubusercontent.com/86222639/146323892-742a5384-f887-4b72-82ea-3e745e7aff78.png)
![image](https://user-images.githubusercontent.com/86222639/146323900-6bcfe99e-a700-4819-84f2-46392c795863.png)

--> resnet50은 overffiting된 모습이다.

# 결과
성능이 더 우수한 커프텀 cnn을 이용해 마스크 인식 여부 
label / 예측
![image](https://user-images.githubusercontent.com/86222639/146322810-9e22b061-1678-4e41-ab97-fc95db9218fd.png)

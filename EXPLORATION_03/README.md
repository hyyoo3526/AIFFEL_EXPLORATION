# EXPLORATION_03

3. 카메라 스티커앱 만들기 첫걸음
### 고양이 수염 스티커 만들기
---

**Step 1. 스티커 구하기 or 만들기**

- [고양이 수염 이미지](https://www.flaticon.com/free-icon/cat-whiskers_24674?term=cat%20nose&page=1&position=1)에서 다운로드

**Step 2. 얼굴 검출 & 랜드마크 검출 하기**
- dlib을 이용해서 얼굴의 bounding box 위치와 landmark의 위치 찾기

**Step 3. 스티커 적용 위치 확인하기**
- 고양이 수염이 적용 될 볼 위치를 landmark를 사용해서 계산하기
 
![image](https://user-images.githubusercontent.com/60082623/126982245-aecb5059-a7c9-4d58-8872-0a5ec6f6eca9.png)

**Step 4. 스티커 적용하기**
-  np.where 를 사용해서 스티커를 적용
-  스티커 뒤로 원본 이미지가 같이 보이도록 만들 것(opencv 의 cv2.addWeighted())

**Step 5. 문제점 찾아보기**
- 다양한 각도에서 촬영하면서 스티커를 반복해서 적용할 것
- 문제점을 해결하기 위한 방법하기

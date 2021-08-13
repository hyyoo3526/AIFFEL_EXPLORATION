# EXPLORATION_08

8. 인물사진을 만들어 보자
### 인물 모드 문제점 찾기
---

**Step 1. 인물모드 직접 해 보기**

- 최소 3장 이상의 인물모드 사진을 만들어보자.
- 귀여운 고양이에 대한 아웃포커싱 사진도 만들어 보자.
- 배경을 blur하는 인물모드 사진이 아니라 배경사진을 다른 이미지로 교체하는 크로마키 배경 합성을 시도해보자  

**Step 2. 해결 방법을 제안해 보기**
- 인물 영역에 포함되어 blur되지 않고 나온다던가 하는 경우 등 이상한 점을 찾아보자.  
- 만들어 낸 인물 모드 사진 중 하나에서도 이상한 위치를 찾아 사진에 표시한 이미지를 포함하여 제출하자.  

**Step 3. 데이터 정제**
- 이 DeepLab 모델의 Semantic Segmentation 이 만들어 낸 Mask 영역에 어떻게 적용되어 문제점을 보완하게 되는지의 메커니즘이 포함된 솔루션을 제시해보자.   

>- **세그멘테이션의 한계:**    
   피사계심도를 이용한 보케(아웃포커싱) 효과는 섬세하나 이를 따라 한 semantic segmentation 모듈은 완벽히 구현하기 어렵다.  
>- **피사계 심도 이해하기:**    
  [피사계심도의 개념](https://ggyul.tistory.com/12)을 이해해보자.  
>- **3D Depth Camera 활용하기:**  
  카메라 1대가 찍은 영상에서 semantic segmentation 시도했을 때 결과가 정확하지 않았다.  
  요즘 스마트폰의 카메라는 [렌즈가 여러개인 이유](https://m.blog.naver.com/panoptics/221336152952)를 이해해보자.  
>- **깊이 영상(Depth image) 활용하기:**  
  Struct2Depth 라는 기법을 소개한다.  
  depth에 따른 물체인식을 보여 주는데, LiDAR가 없이도 아주 정확한 segmentation을 동반한 depth sensor가 가능하다.  
  [Recognizing Depth in Autonomous Driving](https://towardsdatascience.com/depth-prediction-autonomous-driving-18d05ff25dd6)  
  [Unsupervised Learning of Depth and Ego-Motion: A Structured Approach](https://sites.google.com/view/struct2depth)  
>- **IR(적외선)을 활용한 사례:**   
  구글 pixel4에 IR 카메라는 보다 멋진 [3d depth sensing](https://ai.googleblog.com/2020/04/udepth-real-time-3d-depth-sensing-on.html)이 가능하다.  
 - 가능하면 순서도(Flow Chart)를 활용한 솔루션을 설명해보자.  
   


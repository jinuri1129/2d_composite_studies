# 2d_composite_studies
# keying
키잉은 영상의 일부분을 투명하게 하여 해당 영상을 다른 영상과 합성하는데 사용하는 영상기법이다.

<img src="https://cdn.elearningindustry.com/wp-content/uploads/2017/02/chroma-key-technology-in-elearning-utilizing-virtual-studios-to-create-effective-training.jpg" width="400">

위 사진처럼 초록색 크로마키를 이용해서 촬영을 하면 배경을 분리 해 줄 수 있다.


크로마키를 깔끔하게 따 내기 위해서 크로마키쪽에도 조명을 쬐어서 그림자를 최대한 없애주고, dispill을 활용해서 빛 때문이거나 모션블러 때문에 초록색이 묻은 부분도 수정해주고, 그마저도 완성이 되지 않는다면 로토스코핑으로 일일히 잡아 주어야 한다.
<img src="https://luismpla.com/wp-content/uploads/2016/05/Despilling_sample.jpg" width="400">

위 사진은 디스필을 활용해서 영역을 침범한 녹색 부분을 제거해 주었다.

https://wikidocs.net/30096



# 딥러닝을 이용한 이미지 프로세싱

애니메이션 배경을 직접 그리기도 하지만, 요즘은 시간 단축이나 디테일을 위해서 사진을 찍어서 합성하는 경우가 많다.
사진을 일러스트 처럼 보이기 위해서 사진을 찍은 뒤 포토샵에서 그림처럼 보이게 하는 과정이 필요하다.


사진을 그림처럼 보이게 포토샵 작업을 하는 영상

https://www.youtube.com/watch?v=hO2mnKqAgKw


이미지 딥러닝을 통해 비슷한 이미지를 컴퓨터가 학습해서 프로세싱 해주는 코드를 발견해서 테스트를 해보았다 

<img src="https://user-images.githubusercontent.com/76280155/137619891-a2f74820-389b-4556-a235-6488f5d9a60c.jpg" width="600">

↑원본이미지

<img src="https://user-images.githubusercontent.com/76280155/137619896-9000c6f1-3194-4596-9620-67054683726f.jpg" width="600">
↑지브리 작풍을 학습한 결과물

<img src="https://user-images.githubusercontent.com/76280155/137619897-ff4a95b5-6900-404b-96ea-b36151759d9f.jpg" width ="600">
↑파프리카 작풍을 학습한 결과물

<img src="https://user-images.githubusercontent.com/76280155/137619900-3693ae2b-078c-4725-9f27-cebf40d53212.jpg" width ="600">
↑신카이 마코토 작풍을 학습한 결과물

직접 그린것 만큼의 퀄리티는 나오지 않지만 어느정도 그림처럼 보이게 프로세싱이 되었다.
여기서 리터칭을 해서 작업한다면 작업시간을 단축 시킬수 것 같다.

그림과 사진을 합성할때 유용하게 사용할 수 있을것같다.

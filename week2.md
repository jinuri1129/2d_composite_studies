# 2d_composite_studies
# Gamma
감마는 화면상의 나타나는 영상의 휘도간 상관관계를 결정하는 수치이다.
모니터는 원래의 이미지보다 좀더 어둡게 표현하는 경향이 있다. 그래서 이미지가 원래 모습 그대로 보이게 하려면 본 이미지 보다 좀더 밝게 저장을 해야 모니터에서 정상적으로 나온다.
이렇게 감마를 조절하는 과정을 비선형인 감마를 선형으로 만든다고 "리니어 워크플로우" 라고 한다.



<img src="http://rapapa.net/wp/wp-content/uploads/2018/06/i2eZj9U.png" width="400">
리니어 워크플로우


https://blog.daum.net/trts1004/12109543
http://rapapa.net/?p=3406

# aces
aces 는 Academy Color Encoding System 의 약자이다
카메라 필름에서 나오는 소스에 대한 색상 관리 체계를 정립하기 위해서 설계되었다.


밝고 어두운 부분의 영역을 사람이 인지하는 색 공간 이상의 영상에 담고 표현하려는 노력이 이뤄지고 있다. 한 프로그램에서 많은 카메라 장비가 사용되고 그에 따른 장비마다 가지고 있는 또는 담을 수 있는 색 공간이 다르며, 각각의 제조사에서 담고 있는 컬러 스펙트럼의 차이가 나타나게 될 수밖에 없다. 그러므로 여러 가지의 색 공간을 하나의 색 공간으로 만드는 작업이 필요로 하게 되고, 기존의 ACES 시스템을 이용하는 워크플로가 각광을 받고 현장에서 사용되고 있다. 

<http://journal.kobeta.com/%EC%B0%B8%EA%B4%80%EA%B8%B0-aces-%EC%8B%9C%EC%8A%A4%ED%85%9C/>


즉, 다른 색공간에서 찍힌 소스들을 통일시켜 색감이 달라지는 문제점을 보완하기 위함이다.


<img src="https://i1.wp.com/schoolofcolor.org/wp-content/uploads/2018/11/Post_HDTV_Workflow_Part_II_04.jpg?resize=768%2C585" width="600">


https://en.wikipedia.org/wiki/Academy_Color_Encoding_System


# straight & PreMultiplication
<img src="https://limnu.com/wp-content/uploads/2016/06/premult-vs-straight.jpeg" width="600">

스트레이트 방식은 rgb 값에 상관없이 모양틀로 알파를 단순하게 뚫어버리는 것이다.
프리멀트는 rgb 값에다 alpha 값을 곱해서 알파를 표현한다.

스트레이트는 알파가 한번 저장되면 이미지를 다시 원래돼로 돌릴 수 없지만, 프리멀트 방식은 rgb 에다 alpha 를 곱해서 표현한 것이기 때문에, 알파의 값이 변해도 상관없다.

포토샾에서 지우개로 이미지를 지우고 투명하게 만든 이미지를 저장하고 나중에 다시 그 파일을 열었을때 원본 이미지로 되돌릴 수 없지만,
프리멀트로 알파를 곱해서 이미지를 투명하게 만들었을때는 알파를 다시 나눠주면 원본이미지가 생길것이다.

이렇게 알파와 rgb 간 계산을 해서 이미지를 만들 수 있기 때문에 다양한 블랜딩 모드를 사용할 수 있다. (3주차 참조)

https://limnu.com/webgl-blending-youre-probably-wrong/

https://en.wikipedia.org/wiki/Alpha_compositing


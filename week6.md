# Tracking

트래킹은 영상의 픽셀의 움직임을 추적하는 기능이다 이를 활용하여 2d영상을 3D상의 공간으로 만들 수도 있고, 로토의 수고를 덜 수도 있다.

## 1점 tracking
<img src="https://user-images.githubusercontent.com/76280155/140642813-021e8bc7-59a6-486c-9af5-fdb02d81f2d3.jpg" width="600">

한점을 따라가는 트래킹을 이용하면 인물의 점이나 멀리있는 배경을 손쉽게 로토를 딸 수 있다.

1점 tracking은 위치에 대한 정보만 필요할때 유용하다

## 2점 tracking
<img src="https://i.ytimg.com/vi/a8Cs80rz4zk/maxresdefault.jpg" width="600">

2점 tracking 은 위치와 회전값을 알 수 있어서 좌우로 회전하는 카메라의 움직임을 잡아내기 용이하다.
크로마키의 트래킹포인트를 이용해서 회전하는 배경을 집어넣을 수도 있다.

## 다중 트래킹
<img src="https://user-images.githubusercontent.com/76280155/140643060-aeb8c290-ab71-41cf-a8e8-9b1c4e8e4013.jpg" width="600">

tracking 포인트가 많아 질수록 더 정교한 형태를 계산할 수 있다. 4점 부터는 너비를 쉽게 추적할 수 있다.

## 카메라 트래킹
<img src="https://i.ytimg.com/vi/YifeHwCEUwo/maxresdefault.jpg" width="600">
카메라 트래킹은 많은 트래킹 점들을 이용하여 점들의 움직임 속도를 계산한다.
속도 차이를 이용해서 멀리 있는 점과 앞에 있는 점을 추적해내고 이를 토대로 3d 카메라를 만들어 낸다.

2d 이미지와 3d 카메라가 똑같이 움직이게 되었다면, 3d 공간에 물체를 집어넣어 합성을 진행 할 수 있다.

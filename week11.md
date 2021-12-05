# deep compositing



![image](https://user-images.githubusercontent.com/76280155/144751691-e89ed743-e56e-44a4-86a9-c0d6a973a665.png)
2d 이미지와 딥의 차이점

2d 이미지는 픽셀에 rgba 의 채널을 가질 수 있다
딥은 픽셀 하나하나의 공간 데이터를 가진다.

![image](https://user-images.githubusercontent.com/76280155/144751802-74f6fe3d-3a8b-4773-a10b-8e0759d72ada.png)
픽셀 하나하나가 공간 데이터를 가지기 때문에 이런 볼륨메트릭한 이미지 연기나 불 폭발과 같은 이미지들이 가려지는 부분과 보이는 부분이 자연스럽게 나타난다

![image](https://user-images.githubusercontent.com/76280155/144751840-ee84aee5-fefd-47be-a4bc-1439659ef31b.png)
딥 체널로 가면 위와 같은 이미지를 볼 수 있는데 진할수록 앞에 있고 연할수록 멀리있다는 의미이다.


![image](https://user-images.githubusercontent.com/76280155/144751873-efb8e3b6-22a2-4418-b8df-6c1a5feb49b2.png)

zdepth 와 deep 의 차이점

zdepth 는 카메라에서 얼마나 멀리 떨어져 있는지를 계산 하는 것이다
deep 도 카메라에서 얼마나 멀리 떨어져 있는지 도 나타나지만, 픽셀하나하나의 거리 데이터가 다 담겨있다
![image](https://user-images.githubusercontent.com/76280155/144751945-0ddce814-4a77-4af8-82d5-fd17e6b0503b.png)
deep 을 사용하는 이유

zdepth는 패스 자체에 안티 얼라이어싱이 적용되어 있기 때문에 외곽선이 자연스럽지 못하게 처리되는 경우가 생긴다

특히 반투명하거나, 모션블러, 초점이 맞지않은 것과 합성할때 문제가 생긴다

딥을 사용하면 이러한 문제를 해결할 수 있다

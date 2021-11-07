# open EXR
OpenEXR은 ILM에서 개발한 HDR 이미지 포맷이다. 자유 소프트웨어 라이선스로 공개되었다. 채널당 16비트 이상의 컬러를 사용할 수 있으며, 비손실 압축 기법을 지원한다. 2003년 발표되었고, 주로 영화업계에서 사용되고 있다.

이것은 잠재적으로 다른 픽셀 크기의 다중 채널을 지원하는 것은 주목할만한 특징이다. 또한 임의의 채널을 가질 수 있으며 왼쪽 및 오른쪽 카메라 이미지와 같은 여러 시점을 인코딩할 수 있기에 입체적인 기술을 지원하는 그래픽 포맷이다.

예를 들면, 기존의 이미지 처리에서는 컬러에대한 정보만을 주로 다루었지만, 조지 루카스는 이미지정보에 컬러뿐만 아니라, 현장 요구에 부응하는 알파채널이나 카메라 앵글에 대한 정보를 담는 파일 포맷을 필요로 했고 이를 개발해냈다. 
(위키 백과 설명 https://ko.wikipedia.org/wiki/OpenEXR)

CG 소프트 웨어 영상을 보다보니 EXR 이라는 파일포맷이 CG에서 많이 사용 되었다 이육가 궁금해서 조사해 보았다.

## HDR
exr 에서는 HDR 을 지원한다고 한다.
HDR 은 high dynamic range image 의 약자로 아주 넓은 범위의 밝기를 표현할 수 있는 이미지를 말한다.

<img src="https://ww.namu.la/s/f714c821d1e60cbc34ef6ca1a6ba8c765b1d8adcfefc526336979ddf19bc19fdd26774191af28ab126f061edf19fbeff1d25f7dc23b34d8f2fd065cc5d24d05fb0b0075f335b02ad3cdb0648accf66b4c44fb79460971cacd32ba3422e063eb1" width="300">


<img src="https://w.namu.la/s/399483d3a38775d964d7d9e1152e8b3a3a772706a94a9bfce276cfd4dc06bd40b2b49d1f34934d7be1da353290c908dd2d569ca83e191d7b854664194a671783f85e9d1a8e4330d7c8547cec147f7c6ce9be2940c32533c0ffdf865a94f81c5ad08c905dee6a2fa33f249a315049308b" width="600">

한 이미지 안에 다양한 노출값이 담겨있다.

다양한 노출을 저장할 수 있기때문에 3D 에서 조명으로서 사용되기도 한다.

![hdr](https://user-images.githubusercontent.com/76280155/140640088-fa06dd23-6e57-494f-9b8e-133bc9c73618.jpg)
낮은 노출부터 높은 노출을 찍어서 하나의 이미지로 만들어져 있다.
(위키 백과 설명 https://ko.wikipedia.org/wiki/%ED%95%98%EC%9D%B4_%EB%8B%A4%EC%9D%B4%EB%82%B4%EB%AF%B9_%EB%A0%88%EC%9D%B8%EC%A7%80_%EC%9D%B4%EB%AF%B8%EC%A7%95)

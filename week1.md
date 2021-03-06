# Week1

## Color
컴퓨터에서 색깔은 red green blue 의 색깔을 조합해서 표현된다.

<img src="https://user-images.githubusercontent.com/76280155/134163040-485d22b5-adbf-4271-9366-49c153f13839.png" width="220" align = "left">
<img src="https://upload.wikimedia.org/wikipedia/commons/8/89/Nexus_one_screen_microscope.jpg" width="300">



위 사진처럼 빛의 삼원색을 이용해서 색깔을 만들어 내기 때문에, 색깔이 있는 이미지는 최소한 3개의 채널이 있어야 색깔을 표현 할 수 있다.

각각의 채널의 비트수에 따라서 표현될수 있는 색깔수가 결정된다.

8비트에서는 채널당 256가지의 색이 있어 조합하면 256 * 256 * 256 = 16,777,216 가지의 색상표현이 가능하다.
이정도 색이면 사람눈으로 구별해 내기 힘들 만큼 많은 색이지만, 컴퓨터 이미지 합성을 하면서 손실되는 색들이 많기 때문에 이미지 합성을 할때는 더 높은 비트의 사진을 사용한다 

(비트 이미지에 대한 블로그 글 https://m.blog.naver.com/PostView.naver?isHttpsRedirect=true&blogId=master_cyma&logNo=130145038232)

## Alpha

<img src="https://previews.123rf.com/images/s4rt4/s4rt42005/s4rt4200500198/149737729-transparent-pattern-background-simulation-alpha-channel-png.jpg" width="300">

매트 정보의 저장을 위한 알파 채널의 개념은 1970년대 말 앨비 레이 스미스(Alvy Ray Smith)가 처음 선보였고 1984년에 토머스 포터(Thomas Porter)와 톰 더프(Tom Duff)에 의해 백서를 통해 완전히 개발되었다.

알파채널은 색깔이 없는 투명한 부분을 나타내는 채널이다, 포토샾에서 opacity를 조절하거나 마스크를 사용한다면 이 알파채널을 사용한 이미지 합성이다.
기존의 rgb 와 alpha 채널을 합해서 rgba 채널이라고도 부른다.

알파채널이 지원되는 대표적인 파일 포맷은 png 와 tga 가 있다



(alpha 위키: https://ko.wikipedia.org/wiki/%EC%95%8C%ED%8C%8C_%EC%B1%84%EB%84%90)


## Bit Depth
<img src="https://mblogthumb-phinf.pstatic.net/20130105_64/phominator_1357367209369pHqV8_JPEG/bitdepth1.jpg?type=w2" width="300">
https://mblogthumb-phinf.pstatic.net/20130105_64/phominator_1357367209369pHqV8_JPEG/bitdepth1.jpg?type=w2

색 깊이는 화소 하나 즉 픽셀 하나가 가질수 있는 정보값을 말하는데 비트의 크기에 따라서 표현할 수 있는 색의 위가 넓어진다.
높은 비트를 가진 이미지는 많은 정보를 가지고 있기 때문에 이미지 프로세싱을 많이 거치더라도 정보의 손실을 잘 버틸 수 있다.

(위키백과 https://ko.wikipedia.org/wiki/%EC%83%89_%EA%B9%8A%EC%9D%B4)
(비트심도에 관한 블로그 글 : https://m.blog.naver.com/PostView.naver?isHttpsRedirect=true&blogId=phominator&logNo=110155856769)
## Colorspace
<img src="https://upload.wikimedia.org/wikipedia/commons/1/1e/CIE1931xy_gamut_comparison.svg" width="300">
색 영역은 아래의 이미지에서 표현한는 색상 (Color) 범위를 2차원으로 표현하는 X값과 Y값이 있고(수평 면), 여기에 선형 함수 또는 EOTF에 근거하여 휘도 (Luminance, 밝기 범위)를 표현하는 Z값 (수직 축)이 추가된 원뿔 모양의 3차원 벡터로 정의된다.

색깔을 표현할수 있는 범위에 따라 color Gamut이 정해진다

### Srgb
대표적으로 srgb 색영역이 있다
srgb는 ntsc 72%의 색영역을 가지고 있다. 
ntsc 에서 정한 색 규격의 72%를 표현하는 색영역이다. 사람의 눈으로 인식할 수 있는 색상의 33.3%정도 된다.
(ntsc는 national television system committee 의 약자)


### Adobe RGB
adobe 사에서 만든 색영역 srgb가 나올 당시 기술적 타협을 보고 나왔기 때문에 그것을 커버하기 위해 나오게 되었다
srgb에서 표현하지 못했던 cyan 과 green 영역이 확장된 색영역을 가졌다.


색영역을 크게 잡고 작업을 하고 색영역을 작게 표현하는 디스플레이에 가져간다면 색이 다르게 보일 것이다. 작업할때 어떤곳에서 영상을 상영할지 생각하고 색영영을 선택해야한다.




나무위키https://namu.wiki/w/%EC%83%89%20%EC%98%81%EC%97%AD#s-1

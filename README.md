* # Explanation

파이썬 코드 기반으로 아두이노 자동차를 

원격으로 조종하는 GUI 프로그램을 만들었습니다.

자동차에 부착된 카메라 화면을 실시간으로 표시하였고

마우스 클릭이나 키보드 입력을 통한 기본적인 수동 조종과 속도설정,

얼굴 객체 검출기능, 그리고 자율주행 기능등을 사용할 수 있습니다.

**PyQt5, opencv, yolo5, numpy** 를 사용하여 개발하였습니다.



---

* # How to use?

1. 먼저 3.10 버전의 파이썬 프로그램과 마이크로소프트에서 지원하는 Visual Studio code 프로그램을 깔아준뒤 코드를 복사해줍니다.
 
2. 폴더를 만들고 VSCODE로 열고 난 뒤 터미널에서 
**py -3.10 -m venv venv, .\venv\Scripts\activate** 두개의 명령어를 입력하고
가상환경을 구성합니다.

3. **ctrl+shift+p** 를 눌러서 인터프리터선택->가상환경으로 선택해줍니다.

4. pip install opencv-contrib-python numpy PyQt5 yolo5
위 코드를 입력해서 필요한 모듈들을 다운받아줍니다.

5. **https://github.com/opencv/opencv/tree/master/data/haarcascades**
해당주소에서 **haarcascade_frontalface_default.xml**을 폴더에 다운받아줍니다.

6. 원격연결이 가능한 아두이노 자동차를 윈도우 모바일 핫스팟을 통해 연결시킨 뒤
표시되는 IP의 주소를 복사해서 코드에있는 ip주소에 넣어줍니다.


---


* # Version log

첫 단계에서는 화면송출과 수동조종이 가능한 부분까지만 기능을 만들었습니다.

그 뒤에 Haar를 통한 얼굴객체 검출 기능을 추가하였고 

라인트레이싱을 통한 자율주행 기능을 추가하였습니다.

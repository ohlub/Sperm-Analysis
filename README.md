# CASA를 이용한 AI기반의 정자 운동성 패턴 분석 시스템
email: dud991212@naver.com
### Preview image
![image](https://github.com/ohlub/Sperm-Analysis/assets/129753604/1868e9dd-57b7-43cb-a03a-eec0fe42ecd7) ![image](https://github.com/ohlub/Sperm-Analysis/assets/129753604/8826dd04-a7dc-4774-8e64-71aac19011a5)


## Introduction
(Computer Assisted Semen Analysis)CASA는 컴퓨터 정액 분석 시스템으로, 고해상도 비디오카메라가 정액 시료 분석을 실시하면, 
비디오카메라로 촬영된 영상 및 이미지가 분석 소프트웨어 프로그램에 의해 자동으로 분석해 주는 시스템이다. 
CASA를 사용하여 추출한 데이터를 AI와 결합하여 정자 운동성 패턴 분석 시스템을 제작하였다.

CASA 장비로 추출한 데이터 영상에는 활발히 움직이는 정자, 활발하진 않지만 움직이는 정자, 운동성이 없는 정자 등 정자의 운동성을 표시할 수 있다. 
이 시스템은 그중 활발히 움직이는 정자를 분석하고, 전문가의 도움을 받아 정의한 4가지 형태로 운동성을 구분하여 이를 각각 A(Active), B(Semi-Active), C(In-Active), D(Non-Active) 클래스로 분류한다.
검사 결과로는 분류된 정자의 운동성 패턴 정보, 속도, 객체의 이동 거리를 나타내는 유클리드 거리와 맨해튼 거리, 개수 정보를 얻을 수 있다.


## Development Environment
- Window 11
- Jupyter Notebook
- Tensorflow
- Keras
- Resnet50
- Python
 
## Test
1. Python 라이브러리 설치<br>
pip(conda) install opencv-python<br>
pip(conda) install pyqt5<br>
pip(conda) install tensorflow==2.11.0<br>
pip(conda) install pyautogui<br>
pip(conda) install scipy


2. GUI_BASE.ui, GUI_BASE2.ui, model.h5 파일을 주피터 노트북 경로에 저장

3. System.ipynb 파일을 사용자의 주피터 노트북 경로에 저장, 주피터 노트북 환경에서 실행 

4. 실행하면 처음 나오게 되는 메인 화면에서 CASA 영상 5개를 업로드, 분석 시작 ( 만약 Kernel died. 오류가 발생하면 Kernel Restart 진행 )

5. 분석 결과 확인

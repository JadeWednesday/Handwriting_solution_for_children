# :pencil2: 아동 AI 손 글씨 학습 솔루션 제작 (수정중)
<img src="https://user-images.githubusercontent.com/96769060/176324023-bdc8dceb-e1d1-41bc-a759-fd4d3653d724.png" width="750">  
[2022년 KDT 해커톤 출품작(예선 통과)] 아동 기초 언어 능력 향상을 위한 AI 손 글씨 학습 솔루션

본 프로젝트는 디지털 뉴딜 2.0 정책 중 '교육 인프라 디지털화' 및 '비대면 산업 육성' 방향에 초점을 맞추어 기획되었습니다.

※ 전체 발표 영상과 PPT 자료(PDF)는 아래 링크를 참고 부탁드립니다.  
:movie_camera: [`YouTube 발표 영상 (Ctrl+클릭)`](https://youtu.be/h0gBjF3WwHs)  
:bookmark_tabs: [`전체 PPT 자료 (Ctrl+클릭)`](https://github.com/JadeWednesday/CAKD5_3rd_Project/blob/main/%EB%8F%99%EA%B7%B8%EB%A6%AC_PPT.pdf)

<br>

## 프로젝트 세부사항
  - 수행 기간: 22/05/09 ~ 22/06/10 (총 5주)
  - 수행 인원: KDT 수강생 6명 ([`이동연`](https://github.com/movingkite) [`김기연`](https://github.com/kimkeee) [`용지영`](https://github.com/djy00) [`김재경`](https://github.com/rmadmswk) [`정현우`](https://github.com/HyeonuJeong) [`최지원`](https://github.com/JadeWednesday))
  - 수행 역할: (개인) 프로그램 기획, 사전조사 및 실사용 데이터 수집, 동화 이미지 데이터셋 제작, 이미지 출력 파트 담당  
  - 개발 환경: <img src ="https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=python&logoColor=white"/> <img src ="https://img.shields.io/badge/Google Colab-F9AB00.svg?style=flat&logo=Google Colab&logoColor=white"/> <img src ="https://img.shields.io/badge/VS Code-007ACC.svg?style=flat&logo=Visual Studio Code&logoColor=white"/> <img src ="https://img.shields.io/badge/Flask-282828.svg?style=flat&logo=Flask&logoColor=white"/> <img src ="https://img.shields.io/badge/HTML-E34F26.svg?style=flat&logo=HTML5&logoColor=white"/> <img src ="https://img.shields.io/badge/JS-F7DF1E.svg?style=flat&logo=JavaScript&logoColor=282828"/> <img src ="https://img.shields.io/badge/CSS-1572B6.svg?style=flat&logo=CSS3&logoColor=white"/> <img src ="https://img.shields.io/badge/Kakao OCR-FFCD00.svg?style=flat&logo=Kakao&logoColor=282828"/>
<br>

## 목차
[1. 프로젝트 기획 배경]()
<br>
[2. 데이터 분석 및 모델 개발]()
<br>
[3. 기대가치 정리]()
<br>
[4. 프로그램 사용 방법]()




### 1. 프로젝트 기획 배경
<img src="https://user-images.githubusercontent.com/96769060/176325014-8b0587d2-d6ba-4115-aee4-abc3addb37a1.png" width="425"> <img src="https://user-images.githubusercontent.com/96769060/176325105-35da1815-954f-49bf-8cc7-55ab9ddf2ceb.png" width="425">  





### 2. 데이터 분석 및 모델 개발
<img src="" width="750">  


<img src="" width="750">  


<img src="" width="750">  


### 3. 기대가치 정리

<img src="" width="750">  



### 4. 프로그램 사용 방법
※ 본 프로그램은 Chrome 브라우저 기반으로 제작되었습니다.  
Chrome 브라우저의 `다운로드 설정`(chrome://settings/downloads)에서 '다운로드 전에 각 파일의 저장 위치 확인' 옵션을 꺼 주셔야 정상 작동합니다.
1. 프로젝트를 다운로드 하여 압축을 푼 뒤, 'donggri_solution' 폴더를 C 드라이브 하위로 옮깁니다.
2. main.py와 function.py 내부의 경로를 로컬 PC에 맞게 수정합니다. 수정하는 경로는 총 2가지입니다.  
  - 브라우저에서 자동으로 다운로드 되는 '다운로드' 폴더 (C:\Users\user\Downloads)
  - 다운로드 받은 손 글씨 이미지가 이동하는 static 하위 'sorce' 폴더의 Paint.jpg 파일 (C:\donggri_solution\static\sorce\Paint.jpg)
3. (웹 구동) 가상환경을 세팅한 후 pip install -r requirements.txt 명령어를 입력해 필요한 라이브러리를 설치합니다.
4. python main.py 명령어를 입력하여 프로그램을 실행합니다.  
:sound: 배경음과 효과음이 출력되오니 스피커를 켜 주시면 원활한 감상이 가능합니다.

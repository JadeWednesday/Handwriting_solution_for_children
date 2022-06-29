# :pencil2: 아동 AI 손 글씨 학습 솔루션 제작
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
[1. 기획 배경]()
<br>
[2. 개발 과정]()
<br>
[3. 기대가치]()
<br>
[4. 프로그램 사용 방법]()




### 1. 기획 배경
<img src="https://user-images.githubusercontent.com/96769060/176325014-8b0587d2-d6ba-4115-aee4-abc3addb37a1.png" width="375"> <img src="https://user-images.githubusercontent.com/96769060/176325105-35da1815-954f-49bf-8cc7-55ab9ddf2ceb.png" width="375">  

현재 코로나 19로 인한 양질의 교육 기회 감소, 전자기기와 각종 영상 매체에 노출되는 비중이 커지는 등 여러 요인들로 인해 어린 세대에서 학업 성취도가 크게 낮아지고 있습니다.  
저희 동그리 팀은 글을 접할 기회가 많지 않은 아이들이 쓰기와 읽기에 대한 즐거움을 느낄 수 있도록 해 문해력 저하 현상을 초기에 예방하고, 기초적인 언어 능력을 향상시키는 것에 중점을 두고 솔루션의 방향을 결정했습니다.



### 2. 개발 과정
<img src="https://user-images.githubusercontent.com/96769060/176356900-7d1fd34f-20cb-425f-8259-bbd27a9451ed.png" width="750">  

솔루션은 2가지 단계로 구성되어 있습니다.
  - [LEVEL 1] 간단한 명사로 구성된 선택지를 고르며 아동의 사고력을 키우는 참여형 동화 (만 5~6세 추천)
  - [LEVEL 2] 자유롭게 일기를 작성하면 문장에서 명사만을 추출해 명사와 매칭되는 그림을 출력하고,  
출력된 그림을 자유롭게 배치하여 꾸미는 그림일기 (만 7~8세 추천)

각각의 솔루션은 손글씨를 텍스트로 인식하는 OCR 알고리즘을 공유하며, 이렇게 전환된 텍스트는 솔루션에 따라 처리하는 과정이 달라집니다.

<img src="https://user-images.githubusercontent.com/96769060/176365321-89c43b98-2c44-4d89-a6bf-0008b86b510c.png" width="375"> <img src="https://user-images.githubusercontent.com/96769060/176365595-bf13c12d-b4cc-4aef-9d31-8e300c651d15.png" width="375">  

#### :clipboard: 동그리 솔루션의 주요 활용 기술
  - `OCR(광학문자인식)` Web 내의 그림판에 작성한 손 글씨 이미지를 텍스트로 변환
  - `KoNLPy를 활용한 자연어 처리` (그림일기) 작성한 문장을 형태소 분석하고 9가지 품사에 맞춰 태깅 → 명사(noun)만 추출하여 이미지 데이터셋과 매칭


### 3. 기대가치

<img src="https://user-images.githubusercontent.com/96769060/176365810-86d5d053-a542-4f2d-9c2c-e7a62dfcd24c.png" width="750">  

#### :pencil: 동그리 솔루션을 활용함으로써 얻을 수 있는 기대 효과
  - `문해력 저하 예방` 글쓰기, 스스로 생각하기에 익숙한 환경을 이른 시기부터 구축
  - `능동적인 학습 태도 함양` 여러 흥미 요소를 삽입, 산만해지기 쉬운 아동도 자발적으로 학습하도록 유도
  - `성취감 달성` 하나의 창작물을 완성하는 과정에서 아동은 성취감과 자기효능감을 얻음
  - `공부도 놀이처럼 재밌게` 자기표현 능력 기르기 활동은 아동의 관심을 집중시켜 적극적인 의사 표현력의 증진으로 이어짐



### 4. 프로그램 사용 방법
※ 본 프로그램은 Chrome 브라우저 기반으로 제작되었습니다.  
Chrome 브라우저의 `다운로드 설정` (chrome://settings/downloads)에서 '다운로드 전에 각 파일의 저장 위치 확인' 옵션을 꺼 주셔야 정상 작동합니다.
1. 프로젝트를 다운로드 하여 압축을 푼 뒤, 'donggri_solution' 폴더를 C 드라이브 하위로 옮깁니다.
2. main.py와 function.py 내부의 경로를 로컬 PC에 맞게 수정합니다. 수정하는 경로는 총 2가지입니다.  
  - 브라우저에서 자동으로 다운로드 되는 '다운로드' 폴더 (C:\Users\user\Downloads)
  - 다운로드 받은 손 글씨 이미지가 이동하는 static 하위 'sorce' 폴더의 Paint.jpg 파일 (C:\donggri_solution\static\sorce\Paint.jpg)
3. (웹 구동) 가상환경을 세팅한 후 pip install -r requirements.txt 명령어를 입력해 필요한 라이브러리를 설치합니다.
4. python main.py 명령어를 입력하여 프로그램을 실행합니다.  
:sound: 배경음과 효과음이 출력되오니 스피커를 켜 주시면 원활한 감상이 가능합니다.

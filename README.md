# 2020Data_Creator_Camp
## 2020 데이터 크리에이터 캠프 (최우수상 수상)

### 공모전 안내
* 대회명 : 2020 데이터 크리에이터 캠프
* 주최/주관 : 과학기술정보통신부/한국정보화진흥원
* 목적 : 고등학생 및 대학(원)생에게 실생활에서 직면할 수 있는 문제를 빅데이터 및 지능정보기술로 해결해 나가는 지식 공유의 장 마련
* 진행방법 : 예선 - 2시간 동안 기초 강의 후 3시간 동안 문제 해결 / 본선 - 3시간 동안 문제 해결 (문제는 당일 공개)
* 참고 링크 : https://m.onoffmix.com/event/224467

### 팀 소개
* 데이터사나이 : 김윤환,박대한, 박준민, 이재상, 정규형(연세대학교 응용통계학과)

### 예선
* 대회 일정 : 2020년 11월 14일(토)
* 문제 : 3시간 동안 긍정 부정 라벨링 된 영화 리뷰 data를 군집화하여 마케팅 전략팀이 유용하게 쓸 수 있도록 분석하기
* 문제 해결 : </br>
  - 군집화의 성능을 높이기 위해 stop words를 설정해주었다.
  - 제공받은 data는 전처리 과정에서 띄어쓰기를 제거하고 형태소 분석기를 사용하였다. </br>하지만 형태소 분석기를 사용할 때, 띄어쓰기가 있는 것이 더욱 성능이 좋다는 것을 알고 있어, 띄어쓰기를 포함하도록 다시 전처리하였다.</br>
  - 또한, 한국어에서 의미를 가지고 있는 것은 동사, 명사, 형용사이기에 모든 형태소를 쓰는 대신, 동사, 명사, 형용사만 사용하였다. (KoNLPy 사용)
  - K-Means, DBSSCAN, HDBSCA,K-Mdoids 등을 사용하여 성능 비교하려 했지만 시간 제약의 문제로 인해 K-Means 사용하여 군집화
  - 군집화 결과를 Word Cloud를 활용하여 시각화
* 결과 : 1등으로 본선 진출 (띄어쓰기 활용이 출제의도의 핵심이었고 우리 팀이 유일했다.)
 
 ### 본선
* 대회 일정 : 2020년 11월 28일(토)
* 문제 : 3시간 동안 국산 차량 이미지를 통해 차량 클래스를 구분하는 모델 만들기
* 문제 해결 : </br>
  - 총 24,916개의 이미지 데이터가 30*30*3 픽셀값과 클래스로 제공되었다. (24,916행, 2701열)
  - 샘플 모델 Logistic Regression, SVC, Perceptron 제공되었다.
  - 소나타 YF, 소나타 뉴라이즈 등의 클래스를 소나타 클래스 하나로, 아반떼 XD, 아반떼MD 등을 아반떼 하나로 통일하여 클래스 갯수 축소
  - 제한된 시간으로 인해 학습 시간을 줄이기 위해 많은 상위 n개의 클래스만 활용
  - 더 좋은 성능을 위해 CNN을 사용하기로 하였고 출제자에게 이미지 파일을 받아 CNN을 위한 파일 정렬
* 결과 : 최우수상 수상 (딥러닝 기법을 활용한 팀은 우리 팀 포함 두 팀이었고 학습까지 성공한 팀은 우리 팀이 유일했다.)

### 결과
최종 최우수상 수상

### 분석 툴
* Python

#### 기타 세부사항은 보고서 및 ppt 참고바랍니다.


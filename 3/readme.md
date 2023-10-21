# 3차 미니프로젝트

## Part 1
<br/>
# 문제 정의
  주제: 차량 공유업체의 차량 파손 여부 분류서비스 개발
  Data 출처 : KT 자체 제작 (DLLL-E)
  Data 구분 : Image
  문제 유형 : Classification
  중점 사항 : Tensorflow Keras를 통한 CNN 모델 설계
  성능개선(Data Augmentation, Transfer Learning)
<br/>
# 프로젝트 수행
  1. 데이터 전처리
     1) 데이터 분할
     2) 데이터 복사(모델링1) 및 이동
        (기존 폴더는 (모델링 2)에 사용)
  2. CNN 모델링
     1) 이미지 데이터 array화
     2) 클래스 생성 및 구분
     3) 모델 구조 설계
     4) 모델 학습
     5) 예측값생성
     6) 성능 평가
 3. Data Augmentation + Transfer Learning
    1) Keras의 ImageGenerator을 이용하여 증강
    2) VGG16함수로부터 basemodel 저장, 연결구조설계
    3) 모델 학습
    4) 예측값 생성
    5) 성능 평가
<br/>
## Part 2
<br/>
# 문제 정의
  주제: '시각장애인' 및 '저시력자' 등 시각의 보조가 필요한 사용자들에게 스마트폰 카메라를 통해 화폐 정보를 알려주는 AI모델 개발
  Data : 화폐정보 데이터
  Data 출처 : 셀렉스타
  Data 구분 : Image, Json
  문제 유형 : Classification
  중점 사항 : 화폐 앞 뒤를 구별하여 학습
<br/>
# 프로젝트 수행
  1. 데이터 전처리
     1) annotation 정보 추출
        - 위치정보, 박스정보, 클래스 정ㅂ ㅗ추출
        - 화폐 앞뒷면을 하나의 클래스로 <b>통합</b>
        - 이미지는 1/4로 축소
        - 모델 형식에 맞춰 위치정보 변경
     2) dataset 정보파일 생성
  2. 모델링
     1) 가중치 파일 다운로드
     2) 모델 학습
     3) 직접찍은 화폐사진을 탐지 과정에서 사용
     4) 성능 비교
<br/>

# AIFFEL_HACKATHON_1 [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FHRPzz%2FAIFFEL_HACKATHON_1&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)

AIFFEL DAEGU 1 TEAM 3

---

# 제 1차 해커톤: 데이터톤(Datathon)

## CALENDAR (2022.03.08 ~ 2022.03.11)

### March, 2022  (3 days)

>| Week | Sun | Mon | Tue | Wed | Thu | Fri | Sat |
>|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
>| **1** | - | - | **1** | **2** | **3** | **4** | **5** |
>| **To Do** | - | - | - | - | - | - | - |
>| **2** | **6** | **7** | **8** | **9** | **10** | **11** | **12** |
>| **To Do** | - | - | H-01<br>팀플 진행 | - | H-01<br>팀플 진행 | [H-01](%5BH-01%5D%20Team03_Datathon.ipynb)<br>전시 발표 | - |
>| **3** | **13** | **14** | **15** | **16** | **17** | **18** | **19** |
>| **To Do** | - | - | - | - | - | - | - |
>| **4** | **20** | **21** | **22** | **23** | **24** | **25** | **26** |
>| **To Do** | - | - | - | - | - | - | - |
>| **5** | **27** | **28** | **29** | **30** | **31** | - | - |
>| **To Do** | - | - | - | - | - | - | - |

## 소개

### 아이펠 여러분의 천생연분을 찾아드립니다!

![intro img](https://img1.daumcdn.net/thumb/R800x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FI5CHm%2FbtqNVS1OFZh%2FTKFhrpy49sdTxlXzwUwHP1%2Fimg.png)

안녕하세요? 저희 조는 전력사용량 데이터셋을 새로운 시각으로 분석하고자 노력했습니다. 주어진 데이터셋을 활용하여 팀원끼리 협동하여 재미있고 흥미로운 주제로 프로젝트를 진행하고자 했습니다.

부족하지만 가벼운 마음으로 즐겁게 봐주세요!

## 대구3조

- 조원: [박혜령](https://github.com/HRPzz), [이봄](https://github.com/bom-Lee), [허준호](https://github.com/nidolight), [권민호](https://github.com/kwonminho8314)
- 협업 툴 사용

>|번호|항목|링크|용도|
>|:---:|---|:---:|:---:|
>|1|Gather Town|-|만남, 소통|
>|2|Figma|[🔗](https://www.figma.com/file/fvseqWDBu9KVL02yCtXK1d/H-01_3%EC%A1%B0?node-id=0%3A1)|자료 정리|
>|3|Google Shared Drive|[🔗](https://drive.google.com/drive/folders/1BTrydJv_zhqTk7zyQS8pjf4NgPnFfsCC?usp=sharing)|파일 공유|
>|4|Colab Jupyter Notebook|[🔗](https://colab.research.google.com/drive/1lU_jVPNErtE1wvx5NGM_VsNSk6o9Ag-F)|코드 및 마크다운 작성|

## 선택한 데이터셋

- [전력사용량 예측 AI 경진대회](https://dacon.io/competitions/official/235736/data)
  - 시계열 | SMAPE | 한국에너지공단 | 전력
  - 대회 안내
    - 배경
      - 전력 수요 예측 시뮬레이션을 통한 효율적인 인공지능 알고리즘 발굴
      - 전력 융합 신서비스 발굴 및 비즈니스 모델 개발 활용
      - 디지털 뉴딜의 성공을 위한 인공지능(AI)의 융합, 확산을 촉진
    - 목적
      - 건물 정보와 기후 정보를 활용한 전력사용량 예측
    - 주최 / 주관
      - 주최 : 한국에너지공단
      - 주관 : 데이콘
- 데이터 설명
  - train.csv (122400, 10)
    - train 데이터 : 60개 건물들의 2020년 6월 1일 부터 2020년 8월 24일까지의 데이터
    - 1시간 단위로 제공
    - 전력사용량(kWh) 포함
    - columns: num, date_time, 전력사용량(kWh), 기온(°C), 풍속(m/s), 습도(%), 강수량(mm), 일조(hr), 비전기냉방설비운영, 태양광보유
  - test.csv (10080, 9)
    - test 데이터 : 60개 건물들의 2020년 8월 25일 부터 2020년 8월 31일까지의 데이터
    - 3시간 단위로 제공(강수량의 경우 6시간 단위로 제공,  예보데이터)
    - 전력사용량(kWh) 미포함
    - columns: num, date_time, 기온(°C), 풍속(m/s), 습도(%), 강수량(mm,  6시간), 일조(hr,  3시간), 비전기냉방설비운영, 태양광보유

## EDA (Exploratory Data Analysis)

- 데이터 **시각화** 를 통한 분석 진행 과정
  - 시간에 따른 전력 사용량 패턴 분석으로 건물의 MBTI 정하기
  - 대구 캠퍼스 교육생 MBTI 설문조사
  - MBTI 궁합으로 알맞은 건물 추천하기
- **INSIGHT: 대구 캠퍼스 수강생 MBTI 에 어울리는 건물 추천하기**

## 전시 및 발표

>|장소|날짜 및 시간|
>|:---:|:---:|
>|ZEP<br>Session 5|22.03.11.금<br>14:10 ~ 14:30|
>|![ZEP 미니맵](https://user-images.githubusercontent.com/44178037/158010804-031ebd70-3854-4355-bc5b-e49a636d9363.png)|![발표 순서](https://user-images.githubusercontent.com/44178037/158010806-d5af5557-eec1-4e86-9cf0-5135d28f0bbd.png)|

## 평가 및 시상

- 평가 표(절대평가)

>|번호|항목|배점|
>|:---:|---|:---:|
>|1|**EDA 및 시각화** 가 적절하게 이루어졌는가?|15|
>|2|데이터 분석을 통한 **인사이트가 도출** 이 잘 되었는가?|15|
>|3|도출한 인사이트를 통해 설득력이 충분하였는가?|20|
>|4|팀원들이 협업을 통해 프로젝트를 수행하고 발표를 진행하였는가?|25|
>|5|발표시간을 준수하였는지?|25|
>|6|가점: 교육생 여러분들의 평가 (참신해요, 흥미있어요, 좋아요)|-|

- 시상 조에게는 **[평가기준]** 에 1단계/2단계 기준 충족시, 따라 소정의 상품과 시상이 진행될 예정입니다. (상품미정)
  - 1단계: 총점 100점 **만점 기준 50점 이상** 달성
  - 2단계: 총점 100점 **만점 기준 75점 이상** 달성
- 평가 결과: 2단계 통과

## 참고자료

- LMS
  - EXPLORATION
    - E-02. Iris 의 세 가지 품종, 분류해볼 수 있겠어요?
    - E-05. 나의 첫 번째 캐글 경진대회, 무작정 따라해보기
  - FUNDAMENTALS
    - F-09. Data 어떻게 표현하면 좋을까? 배열(array)과 표(table)
    - F-10. 다양한 데이터 전처리 기법
    - F-11. 데이터를 한 눈에! Visualization
    - F-12. 사이킷런으로 구현해보는 머신러닝
    - F-15. 가랏, 몬스터볼! 전설의 포켓몬 찾아 삼만리
- Dacon
- Kaggle

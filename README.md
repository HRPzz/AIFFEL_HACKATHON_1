# AIFFEL_HACKATHON_1 [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FHRPzz%2FAIFFEL_HACKATHON_1&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)

AIFFEL DAEGU 1 TEAM 3

---

# 제 1차 해커톤: 데이터톤(Datathon)

## CALENDAR (2022.03.08 ~ 2022.03.11)

### March, 2022 (3 days)

>| Week | Sun | Mon | Tue | Wed | Thu | Fri | Sat |
>|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
>| **1** | - | - | **1** | **2** | **3** | **4** | **5** |
>| **To Do** | - | - | - | - | - | - | - |
>| **2** | **6** | **7** | **8** | **9** | **10** | **11** | **12** |
>| **To Do** | - | - | 팀플 진행 | - | 팀플 진행 | 전시 발표 | - |
>| **3** | **13** | **14** | **15** | **16** | **17** | **18** | **19** |
>| **To Do** | - | - | - | - | - | - | - |
>| **4** | **20** | **21** | **22** | **23** | **24** | **25** | **26** |
>| **To Do** | - | - | - | - | - | - | - |
>| **5** | **27** | **28** | **29** | **30** | **31** | - | - |
>| **To Do** | - | - | - | - | - | - | - |

## 대구3조

- 조원: [박혜령](https://github.com/HRPzz), [이봄](https://github.com/bom-Lee), [허준호](https://github.com/nidolight), [권민호](https://github.com/kwonminho8314)
- 협업 툴 사용

>|번호|항목|용도|
>|:---:|---|:---:|
>|1|Gather Town|만남, 소통|
>|2|[Figma](https://www.figma.com/file/fvseqWDBu9KVL02yCtXK1d/H-01_3%EC%A1%B0?node-id=0%3A1)|자료 정리|
>|3|[Google Shared Drive](https://drive.google.com/drive/folders/1BTrydJv_zhqTk7zyQS8pjf4NgPnFfsCC?usp=sharing)|파일 공유|

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
  - 각 건물별 성격(mbti) 정하기
  - 대구 캠퍼스 교육생 mbti 설문조사
  - mbti 궁합으로 알맞은 건물 추천하기
- **Insight: 대구 캠퍼스 수강생 mbti 에 어울리는 건물 추천하기**

## 전시 및 발표

- 장소
  - ZEP
  - Session 5
  - ![ZEP 미니맵](https://user-images.githubusercontent.com/44178037/158010804-031ebd70-3854-4355-bc5b-e49a636d9363.png)
- 날짜 및 시간
  - 22.03.11.금
  - 14:10 ~ 14:30
  - ![발표 순서](https://user-images.githubusercontent.com/44178037/158010806-d5af5557-eec1-4e86-9cf0-5135d28f0bbd.png)

## 평가 표(절대평가)

>|번호|항목|배점|
>|:---:|---|:---:|
>|1|데이터 전처리, 모델학습, 예측의 전체 과정을 거쳐 캐글 submission까지 진행되었다.|15|
>|2|데이터 분석을 통한 인사이트가 도출이 잘 되었는가?|15|
>|3|도출한 인사이트를 통해 설득력이 충분하였는가?|20|
>|4|팀원들이 협업을 통해 프로젝트를 수행하고 발표를 진행하였는가?|25|
>|5|발표시간을 준수하였는지?|25|

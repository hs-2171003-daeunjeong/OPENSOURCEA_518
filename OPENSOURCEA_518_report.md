<div align="center" style="text-align:center">

# MZ세대를 위한 맛집 추천 서비스 OPENSOURCEA_518
1971142 박주용 / 2191214 박준서 / 1771115 박형선 / 1971324 전희연 / 2171126 정다빈 / 2171003 정다은
</div>
<br/><br/><br/>

## 서비스 설명

**추진배경**
![https://github.com/hs-2171003-daeunjeong/OPENSOURCEA_518/blob/heeyeonjeon/%EC%84%9C%EB%B9%84%EC%8A%A4%EC%86%8C%EA%B0%9Cimg.png?raw=true](https://github.com/hs-2171003-daeunjeong/OPENSOURCEA_518/blob/heeyeonjeon/%EC%84%9C%EB%B9%84%EC%8A%A4%EC%86%8C%EA%B0%9Cimg.png?raw=true)

2021.12월에 건강의료전문미디어 매경헬스에서 최근 1년 내에 일주일 간 국내여행을 한 번이라도 가본 전국 거주 만 19세 이상 남녀 1,349명을 대상으로 여행 중 맛집 음식점 방문 행태를 조사하였다.

현지 맛집 음식점에 방문하는 이유는 맛있는 음식을 먹기 위해서라는 답이 63.4%로 가장 컸다. 이처럼 최근 MZ세대 사람들의 약속이나 모임에 맛있는 음식을 먹고 싶어서 맛집을 방문한다는 이유처럼 맛집에 대한 수요가 높아지고 중요성 또한 커지고 있기 때문에 이 주제를 선택하게 되었다.

<br/>

**서비스 소개**

맛집을 고르기 위해 검색해보고 어떤 곳을 갈지 고민하며 찾는 데에 시간을 쓴 경험이 다들 한번쯤 있을거라 생각한다. 우리는 이런 시간을 줄여 맛집을 선택하는 데에 도움이 될 수 있는 맛집 추천 서비스의 필요성을 느껴 고안하게 되었다.

MZ세대를 위한 맛집 추천 서비스는 맛집 데이터베이스를 기반으로 리뷰 정보를 분석하여 사용자의 정보와 사용자로부터 입력받은 검색어를 토대로 맛집을 추천해주는 서비스이다.

오픈소스 소프트웨어를 이용하여 사용자로부터 검색어를 입력받으면 검색된 단어를 기반으로 맛집 정보 데이터베이스에서 평점이 우수한 맛집을 추천해주고 사용자의 정보(나이, 성별, 자주먹는 음식 등)와 사용자의 위치를 받아와 사용자 주변의 맛집을 사용자 취향을 고려하여 추천해준다.

<br/><br/>

## GUI
<div align="center" style="text-align:center">
<img src="https://github.com/hs-2171003-daeunjeong/OPENSOURCEA_518/blob/main/GUI1.jpg?raw=true"  width="200" height="400"/><img src="https://github.com/hs-2171003-daeunjeong/OPENSOURCEA_518/blob/main/GUI2.jpg?raw=true"  width="200" height="400"/>
</div>

<br/><br/>

## 유사 서비스 분석

(내용)
<br/><br/>

## DFD
**DFD 데이터 흐름도**
![https://github.com/hs-2171003-daeunjeong/OPENSOURCEA_518/blob/main/5_18%20DFD.jpg?raw=true](https://github.com/hs-2171003-daeunjeong/OPENSOURCEA_518/blob/main/5_18%20DFD.jpg?raw=true)

<br/><br/>

## 각 오픈소스 소프트웨어 설명

### 박주용 - Scrapy

![https://scrapy.org/img/scrapylogo.png](https://scrapy.org/img/scrapylogo.png)

**python으로 작성된 오픈소스 웹 크롤링 프레임워크 (BSD 라이센스)**

웹 사이트를 탐색하고 구조화된 데이터를 추출하기 위한 애플리케이션 프레임워크 데이터 마이닝, 정보처리 또는 이력 아카이브와 같은 유용한 애플리케이션에 사용할 수 있다.

원래 웹 스크랩용으로 설계되었지만 API(Amazon Associates Web SErvice 등)를 사용하거나 범용 웹 크롤러로 데이터를 추출하는 데도 사용할 수 있다.

#### 스크래핑을 쉽고 효율적으로 하기 위해 사용하는 기능

- 확장 CSS 셀렉터 및 XPath 식을 사용
  - HTML/XML 소스에서 데이터를 선택 및 추출할 수 있으며 정규 표현을 사용하여 추출하는 도우미 메서드가 내장되어 있음
- CSS 및 XPath 식을 사용하여 데이터를 스크래핑하기 위한 인터랙티브셸 콘솔(IPython 인식).
  - 스파이더 쓰기 또는 디버깅 시 매우 편리함
- 여러 형식(JSON, CSV, XML)으로 피드 내보내기를 생성
  - 여러 백엔드(FTP, S3, 로컬 파일 시스템)에 저장할 수 있는 내장 지원

<br/><br/>

### 박준서 - scikit-learn

<img src = "https://scikit-learn.org/stable/_static/scikit-learn-logo-small.png"/>

**python을 대표하는 머신러닝 라이브러리  (BSD 라이센스)**
- 예측 데이터 분석을 위한 간단하고 효율적인 도구
- 모든 사람이 액세스 가능
- 다양한 상황에서 재사용이 가능
- NumPy, SciPy 및 matplotlib 기반
#### 기능
- 분류 (Classification)
  - 개체가 속한 범주를 식별 (스팸 감지, 이미지 인식)
- 회귀 (regression)
  - 객체와 관련된 연속 값 속성 예측 (약물 반응, 주가)
- 클러스터링 (clustering)
  - 유사한 개체를 세트로 자동 그룹화 (고객 세분화, 실험결과 그룹화)
- 차원 감소 (dimensionality reduction)
  - 고려할 무작위 변수의 수 감수 (시각화, 효율성 향상)

<br/><br/>

### 박형선 -

<br/><br/>

### 전희연 - Apache Mahout

![https://mahout.apache.org/assets/mahout-logo-blue.svg](https://mahout.apache.org/assets/mahout-logo-blue.svg)

**수학자, 통계학자 및 데이터 과학자가 자신의 알고리즘을 신속하게 구현할 수 있도록 설계된 분산 성형 대수학 프레임워크이자 수학적으로 표현한 Scala DSL (Apache 라이선스 V2.0)**

- 권장되는 즉시 사용 가능한 분산 백엔드 or 다른 분산 백엔드로 확장 가능 - 다중 분산 백엔드 지원
- CPU, GPU, CUDA 가속을 위한 모듈식 네이티브 솔버
- 기계 학습으로 이루어짐, but 많은 기능이 있어 통계학, 알고리즘, 수학 공식을 들여다 보지 않아도 필요한 비즈니스 시나리오에 활용 가능.

#### Mahout의 구성도
![https://cafeptthumb-phinf.pstatic.net/MjAxOTEwMDFfMjM1/MDAxNTY5OTE1Mzk1OTE5.jRCCrYg8u-Ko0zTQgf4YPOqdYEbj7K0p9stkI5STDRkg._37dPysPAB8POnjwaSvYVQoyiva4SC4wTD5T7cT9Zfcg.PNG/Mahout%EA%B5%AC%EC%84%B1%EB%8F%84.png?type=w800](https://cafeptthumb-phinf.pstatic.net/MjAxOTEwMDFfMjM1/MDAxNTY5OTE1Mzk1OTE5.jRCCrYg8u-Ko0zTQgf4YPOqdYEbj7K0p9stkI5STDRkg._37dPysPAB8POnjwaSvYVQoyiva4SC4wTD5T7cT9Zfcg.PNG/Mahout%EA%B5%AC%EC%84%B1%EB%8F%84.png?type=w800)

#### 기능

#### 1. 협업 필터링 (Collaborative Filtering)

사용자 정보(ex 등급, 클릭 수 등)를 활용하여 사용자에게 추천 항목을 제공하는 기술 

##### **추천 방법** 

- 사용자 기반 : 유사한 사용자를 찾아서 항목을 추천
- 항목 기반 : 항목 간의 유사성을 계산하여 항목을 추천
- Slope-One : 부울 연산자를 사용한 선호도가 아니라 사용자가 등급을 지정할 때 적용 가능한 매우 빠르고 간단한 항목 기반의 추천 방식
- 모델 기반 : 사용자와 등급으로 구성된 모델을 기반으로 추천 항목을 제공

#### 2. 클러스터링 (Clustring)

비교사 학습 (사전에 데이터와 그들 간의 관계에 대한 정보 X) 

##### **클러스터링 알고리즘** 

- Canopy : 빠른 클러스터링 알고리즘이며 다른 클러스터링 알고리즘의 초기 시드를 작성하는 데도 사용
- k-Means(및 fuzzy k-Means) : 이전 반복의 중심 또는 중앙으로부터 항목이 떨어져 있는 거리를 기반으로 항목을 k개의 클러스터로 클러스터링
- Mean-Shift : 클러스터 수를 미리 알 필요가 없으며 임의 형태의 클러스터를 생성할 수 있는 알고리즘
- Dirichlet : 가능성이 있는 여러 모델을 기반으로 하는 클러스터가 제공되므로 특정 클러스터 보기를 조기에 결정하지 않다도 된다는 장점이 있음

##### **클러스터링 단계** 

1. 입력을 준비한다. 텍스트를 클러스터링하는 경우에는 텍스트를 숫자 표현으로 변환해야 한다. 
2.  Mahout에 있는 여러 Hadoop-ready 드라이버 프로그램 중 하나를 사용하여 클러스터링 알고리즘을 실행한다. 
3. 결과를 평가한다. 
4. 필요한 경우 위 단계를 반복한다.

*클러스터 - n 차원 공간에서 제품을 점으로 찍음 -> 유사한 장소에 있는 것을 그룹이라 하고 그룹들의 점을 클러스터라 부름

#### 3. 분류 (Classification or Categorization)

교사학습 (사전에 데이터와 그들 간의 관례에 대한 정보를 가지고 있음) 

일반적으로 미리 정의된 결과 값과 함께 샘플 입력 값이 주어지고 훈련을 통해 하나의 모델이 만들어짐, 이 모델은 다른 데이터 들을 입력 받아서 카테고리로 분류함.

- Naïve Bayes 분류기 데이터에 대한 매우 단순한 가정이 완전히 독립되어 있음에도 불구하고 빠르면서도 상당히 정확
- Complementary Naïve Bayes 단순성과 속도를 유지하는 동시에 Naïve Bayes 방법과 관련된 일부 문제를 해결하려고 시도

<br/><br/>

### 정다빈 - Apache Solr

![img](https://blog.kakaocdn.net/dn/b3nwrp/btqEk3ketov/NdkOyh7FkRBe398ojgHRzk/img.png)



#### 오픈 소스 엔터프라이즈 검색 플랫폼

- 프로그래밍 언어 : Java
- 라이선스 : Apache 2.0



#### 기술 용어

- **클러스터(Cluster)** : 하나 이상의 노드로 이루어진 가장 큰 시스템 단위- 독립적인 형태로 유지
- **스키마**(Schema) : 색인할 문서의 필드, 필드 타입 정의
- **인덱스 복제**(Index Replication): 마스터 인덱스의 전체 복사본을 하나 이상의 슬레이브 서버로 배포 및 업데이트하는 것 - 대규모 볼륨에 대한 분산 처리
- **샤드(Shard)** : 데이터를 분산하여 저장하는 단위



#### 기능



##### **1. 색인 / 검색**

색인은 HTTP 프로토콜 상에서 XML을 통해서 색인, 검색은 HTTP GET으로 쿼리를 보낼 수 있으며 XML의 형태로 값을 얻음 

##### **2. 분산 처리**

솔라는 인덱스 복제(Index Replication)라는 기술을 활용한다. 복제 및 분산처리를 통해 Solr는 대규모 검색 볼륨에 대한 쿼리에 적절한 대응력을 제공함.

##### **3. 접근성**

솔라 검색서버 URL을 사용하기에 인터넷을 통해 파일을 질의, 인덱스하는 어느 곳에서나 접근 가능

<br/><br/>

### 정다은 - Geopy
<img src="https://geopy.readthedocs.io/en/stable/_images/logo-wide.png" width="600" height="300"/>  

**지오코딩 웹 서비스를 위한 Python 클라이언트 (MIT 라이선스)**

- 지오코더 및 기타 데이터 소스를 사용하여 전 세계의 주소, 도시, 국가 및 랜드마크의 좌표를 쉽게 찾을 수 있음
- Geopy와 함께 Python의 Folium 모듈을 사용하여 지도에 마커 표시 가능 (GUI 예시 참조)
#### 기능
#### 1. 거리 측정 기능
geodesic distance(측지선 거리) 또는 great-circle distance(대원 거리)를 사용하여 두 지점 사이의 측지 거리를 계산  
- 측지 거리: 두 점 사이의 최단 경로 거리
- 곡면상의 두 점을 이루는 곡선의 거리를 계산하여, 구의 형태인 지구에서도 적용시켜볼 수 있음
- 지구는
**'이상적인 구'**
로 간주하고 계산  
##### 참고
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/38/Law-of-haversines.svg/220px-Law-of-haversines.svg.png" width="300" height="300"/>  

측지 거리를 계산할 때 지구를
**'이상적인 구'**
로 간주하여 계산한다는 것은, 약간의 오차가 발생한다.  
왜냐하면 실제로 지구는 완전한 구가 아니기 때문이다.  
따라서 Haversine distance 대신, WGS-84 좌표 시스템을 사용하는 Vincenty distance를 사용하는 것이 실제로 더 정확할 것이라고 한다.  
- Haversine distance: 구에서 두 점 사이의 거리를 계산할 때 사용되는 공식인 '하버사인 공식'으로 구한 거리
- Vincenty distance: '경위도 연산'으로 구한 거리
#### 2. 지오 코딩 기능
주소나 장소 이름과 같은 위치에 대한 텍스트 기반 설명을 취하고 지리적 좌표(종종 위도/경도 쌍)를 반환하여 지구의 위치를 식별  
우편 및 행정 경계와 함께 주소 지점, 거리/도로 네트워크의 컴퓨터 표현에 의존
- 지오 코딩(Geocoding): 주소 혹은 지명 등의 고유명사를 통해, 위도와 경도로 이루어진 좌표값을 얻는 것
- 위도, 경도 좌표를 통해 주소를 얻을 수 있는
**'역지오 코딩'**
도 가능

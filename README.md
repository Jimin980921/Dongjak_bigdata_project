# 2020 동작구 빅데이터 정책 연구 공모전 기획안(2020.03.16~05.01) 
![공모전 포스터](https://user-images.githubusercontent.com/57060127/78499818-d7a17c00-778d-11ea-8e32-f5acd57de15f.jpg)
* 프로젝트 목적: 동작구 여가/문화 유적지 활성화 정책 제안: 문화유산이란 그 나라의 역사와 문화를 반영하고 있는 공간이다. 5000년의 역사를 자랑하는 대한민국에는 가치있는 역사 관광지가 매우많음. 빅데이터 분석을 통해 문화유산 관광지 주변 부흥 요인을 밝혀 동작구에 있는 문화유적지 활성화에 기여할 수 있다.

#### 1 단계: '대한민국 구석구석 관광지'목록 크롤링(인기순으로 정렬 후, 상위 1000곳 저장)
<p align="center"> 
<img src="https://user-images.githubusercontent.com/57060127/84516317-95099c00-ad08-11ea-8081-51b2c587bc84.JPG" width="300" height="350">
</p>

#### 2 단계: 문화유산지명+'주변'+ [음식점, 숙박, 대중교통, 공원, 술집 등] 자동 검색 ('주변'의 기준은 반경 2km이내)   
#### 해당 문화유산지의 리뷰수와 [음식점, 숙박, 대중교통, 공원, 술집 등] 각각의 이름을 크롤링(크기: 약 11MB)
<p align="center"> 
<img src="https://user-images.githubusercontent.com/57060127/84516870-617b4180-ad09-11ea-83a3-76ed008f1de7.JPG" width="300" height="350">
</p>

#### 3 단계: 빅데이터 전처리 및 정리
#### 문화유산지주변 [음식점, 숙박, 대중교통, 공원, 술집 등] 크롤링결과를 전처리(null값 삭제, duplicate값 삭제 등) 후,갯수를 count한다.
<p align="center"> 
<img src="https://user-images.githubusercontent.com/57060127/84518088-1eba6900-ad0b-11ea-83be-06197dbd589b.JPG" width="200" height="300">
</p>

#### 4 단계: 빅데이터 분석
#### 주변 부흥 요인 총 10가지(공원,관광명소,교통,쇼핑,술집,음식점 등)와 리뷰와의 관계를 다중 선형회귀분석을 진행한다.
<p align="center"> 
<img src="https://user-images.githubusercontent.com/57060127/84518639-f7b06700-ad0b-11ea-8439-b3946369ff03.JPG" width="400" height="200">
</p>
#### 이전에 상위 10%에 해당하는 문화유산지의 data를 이용해 리뷰와 각 부흥요인의 상관관계 분석을 진행한다. 그 결과 [공원, 화장실]은 상관계수값이 낮아 회귀분석 특징에서 제거한다.

><data: 데이터>

><pdf: 완성결과>



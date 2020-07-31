# 2020 동작구 빅데이터 정책 연구 공모전 기획안(2020.03.16~05.01) 
![공모전 포스터](https://user-images.githubusercontent.com/57060127/78499818-d7a17c00-778d-11ea-8e32-f5acd57de15f.jpg)
* __프로젝트 목적__ : 동작구 여가/문화 유적지 활성화 정책 제안  
문화유산이란 그 나라의 역사와 문화를 반영하고 있는 공간 => 5000년의 역사를 자랑하는 대한민국에는 가치있는 역사 관광지가 매우 많음
빅데이터 분석을 통해 문화유산 관광지 주변 부흥 요인을 밝혀 동작구에 있는 문화유적지 활성화에 기여할 수 있음

-----------------------------------------------------------------------------------------------------------------
## 개발 단계  
__1 단계:__'대한민국 구석구석 관광지'목록 크롤링(인기순으로 정렬 후, 상위 1000곳 저장) 
<p align="center"> 
<img src="https://user-images.githubusercontent.com/57060127/84516317-95099c00-ad08-11ea-8081-51b2c587bc84.JPG" width=30%>
</p>
<br>
<br>


__2 단계:__ 문화유산지명+'주변'+ [음식점, 숙박, 대중교통, 공원, 술집 등] 자동 검색 ('주변'의 기준은 반경 2km이내)   
해당 문화유산지의 리뷰수와 [음식점, 숙박, 대중교통, 공원, 술집 등] 각각의 이름을 크롤링(크기: __약 11MB__)
<p align="center">
<img src="https://user-images.githubusercontent.com/57060127/84516870-617b4180-ad09-11ea-83a3-76ed008f1de7.JPG" width=40%>
</p>
<br>
<br>



__3 단계:__ 빅데이터 전처리 및 정리  
문화유산지주변 [음식점, 숙박, 대중교통, 공원, 술집 등] 크롤링결과를 전처리(결측값 삭제, duplicate값 삭제 등) 후, 갯수를 count
<p align="center"> 
<img src="https://user-images.githubusercontent.com/57060127/84596101-b7312480-ae96-11ea-9ff9-f5c50aa6965f.JPG" width=80%>
</p>
<br>
<br>

__4 단계:__ 빅데이터 분석  
주변 부흥 요인 총 10가지(공원,관광명소,교통,쇼핑,술집,음식점 등)와 리뷰와의 관계를 다중 선형회귀분석을 진행
<p align="center"> 
<img src="https://user-images.githubusercontent.com/57060127/84518639-f7b06700-ad0b-11ea-8439-b3946369ff03.JPG" width=70%>
</p>
<br>

이전에 상위 10%에 해당하는 문화유산지의 data를 이용해 리뷰와 각 부흥요인의 __상관관계 분석__ 진행  
그 결과 [공원, 화장실]은 상관계수값이 낮아 회귀분석 특징에서 제거  
상관계수값이 낮은 특징을 제거하고 회귀분석을 진행한 결과, p-value값이 낮은 요소는 [교통,숙소,술집]으로 분석됨  
교통과 숙소가 리뷰와 양의 관계, 술집과는 음의 관계를 보임  
<p align="center"> 
<img src="https://user-images.githubusercontent.com/57060127/84519277-d603af80-ad0c-11ea-9afe-016623223b96.JPG" width=60%>
</p>
<br>
<br>



__5 단계:__ 동작구 주변요소와 빅데이터분석결과와 비교  
활성화에 영향을 미치는 주변 3가지요소[교통,숙소,리뷰]의 갯수를 비교한 결과,  
전체적으로 교통 편의성은 상위 문화유산지의 평균치이지만, 숙박시설의 보충이 필요하고, 술집의 갯수는 3배이상이므로 단속이 필요
<p align="center"> 
<img src="https://user-images.githubusercontent.com/57060127/84519526-32ff6580-ad0d-11ea-869d-5a040d39ac32.JPG" width=40%>
</p>
<br>
<br>


* data: 데이터 


* pdf: 결과발표자료


[네이버 쇼핑 리뷰 크롤링 프로젝트](https://github.com/Jimin980921/text_mining)  
[유튜브 크롤링](https://github.com/Jimin980921/youtube_crawling)


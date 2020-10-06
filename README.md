# 2020 동작구 빅데이터 정책 연구 공모전 기획안(2020.03.16~05.01)  
![공모전 포스터](https://user-images.githubusercontent.com/57060127/78499818-d7a17c00-778d-11ea-8e32-f5acd57de15f.jpg)  
<br>


(자세한 설명: [발표 pdf](https://github.com/Jimin980921/Dongjak_bigdata_project/blob/master/%EB%8F%99%EC%9E%91%EA%B5%AC%202020%20%EB%B9%85%EB%8D%B0%EC%9D%B4%ED%84%B0%20%ED%99%9C%EC%9A%A9%20%EC%95%84%EC%9D%B4%EB%94%94%EC%96%B4%20%EB%B6%84%EC%84%9D%20%EC%84%A4%EB%AA%85%EC%84%9C.pdf))  

-----------------------------------------------------------------------------------------------------------------
## 프로젝트 개요  
<img src="https://user-images.githubusercontent.com/57060127/95219399-4be9d480-0830-11eb-83e5-d55c9c5e7560.JPG">
<img src="https://user-images.githubusercontent.com/57060127/95219408-4db39800-0830-11eb-812c-92bcf99dfda2.JPG">
<img src="https://user-images.githubusercontent.com/57060127/95219412-4ee4c500-0830-11eb-8413-a0ae9e021c4d.JPG">
<img src="https://user-images.githubusercontent.com/57060127/95219414-4ee4c500-0830-11eb-8129-35caca930826.JPG">
<img src="https://user-images.githubusercontent.com/57060127/95219416-4f7d5b80-0830-11eb-8a8b-9b471ad5fab0.JPG">
<br>


## 빅데이터 수집  
<img src="https://user-images.githubusercontent.com/57060127/95219774-bdc21e00-0830-11eb-96a6-6b806565d579.JPG">
<img src="https://user-images.githubusercontent.com/57060127/95219782-bf8be180-0830-11eb-9402-dd963a1b51eb.JPG">
<img src="https://user-images.githubusercontent.com/57060127/95219784-c0247800-0830-11eb-8104-b0dc75c8941b.JPG">
<img src="https://user-images.githubusercontent.com/57060127/95219781-bef34b00-0830-11eb-9b0d-6b361acfcff5.JPG">
<img src="https://user-images.githubusercontent.com/57060127/95219783-c0247800-0830-11eb-8447-98f35b87f6fa.JPG">
<br>



## 빅데이터 분석  
- 빅데이터 전처리  
<img src="https://user-images.githubusercontent.com/57060127/95220334-522c8080-0831-11eb-801b-144daf0e60ca.JPG">
- 상관분석 & 회귀분석  
<img src="https://user-images.githubusercontent.com/57060127/95220409-65d7e700-0831-11eb-9304-8654068e43c3.JPG">
<img src="https://user-images.githubusercontent.com/57060127/95220391-63758d00-0831-11eb-86a0-9591df1a3f0d.JPG">
<img src="https://user-images.githubusercontent.com/57060127/95220406-64a6ba00-0831-11eb-9d39-b84623fe10ee.JPG">
<br>


## 빅데이터 분석결과  

## 결론 및 정책제안  



__3 단계:__ 빅데이터 전처리 및 정리  
문화유산지주변 [음식점, 숙박, 대중교통, 공원, 술집 등] 데이터 전처리(결측값 삭제, duplicate값 삭제 등) 후, 갯수 count  

   - [데이터 전처리](https://github.com/Jimin980921/Dongjak_bigdata_project/blob/master/data/All.csv)  
<p align="center"> 
<img src="https://user-images.githubusercontent.com/57060127/84596101-b7312480-ae96-11ea-9ff9-f5c50aa6965f.JPG" width=80%>
</p>
<br>
<br>

__4 단계:__ 빅데이터 분석   
주변 부흥 요인 총 10가지(공원,관광명소,교통,쇼핑,술집,음식점 등)와 리뷰와의 관계를 __다중 선형회귀분석__ 진행  
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

--------------------------------------------------------------------------------------------------

## 분석 결과  
__활성화에 영향을 미치는 주변 3가지요소[교통,숙소,리뷰] 요소 비교__  
=> 전체적으로 교통 편의성은 상위 문화유산지의 평균치이지만, 숙박시설의 보충이 필요, 술집의 갯수는 3배이상이므로 단속이 필요
<p align="center"> 
<img src="https://user-images.githubusercontent.com/57060127/84519526-32ff6580-ad0d-11ea-869d-5a040d39ac32.JPG" width=40%>
</p>
<br>
<br>


- 유사 프로젝트  
   - [네이버 쇼핑 리뷰 크롤링 프로젝트](https://github.com/Jimin980921/text_mining)  
   - [유튜브 크롤링](https://github.com/Jimin980921/youtube_crawling)


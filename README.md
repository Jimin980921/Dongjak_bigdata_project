# 2020 동작구 빅데이터 정책 연구 공모전 기획안(2020.03.16~05.01) 
![공모전 포스터](https://user-images.githubusercontent.com/57060127/78499818-d7a17c00-778d-11ea-8e32-f5acd57de15f.jpg)

<main: 완성본>

<data: 데이터>

<memory: 개발 과정>

0413= 검색되지 않는 문화유산지는 -1로 채우기(성공)
이후 과제: 3page이후에서는 돌아가지않고 에러남, 세부주소저장, '문화유산지, 종류, 이름, 주소'형태로 csv에 저장, 세부주소이용하여 위도,경도 추출, 문화유산지와의 거리 비교, 2km이내가 아니면 탈락시킴.


0415= 위도,경도 코드 성공


0416=csv저장 코드 성공, 이후 과제: 에러나지않게 데이터 가져오는 것

0417=csv에 내 데이터 저장해보기("문화유산지, 이름, 종류, 위치") 형태로

0419= 구글맵은 '문화유산지'+'주변'+'서비스시설'로 검색했을때, 주변이 아닌 멀리떨어진 지역((예) '경복궁 주변 쇼핑몰'을 검색했을때, 김포공항 롯데몰 출력됨)까지 검색결과로 출력되어, 모든 상점을 클릭하여 세부주소를 가져와 위도,경도를 출력하는 코드(위도,경도.ipynb)를 사용하여 엑셀 거리계산함수를 사용하여 2km이상인 지역을 탈락시키려고 했으나, 비효율적이고 시간이 오래걸려 주변시설이 정확하게 나오는 네이버지도로 변경하기로 하였다. 

0424= 구글에서 크롤링하던 특징값 list로 저장완료. 이후과제:csv로 옮기기, 리뷰수 저장하기

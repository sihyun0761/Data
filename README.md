### 데이터 크롤링 하기
***

##### 크롤링 프로그램 설치
    git clone https://github.com/YoongiKim/AutoCrawler

    cd AutoCrawler
 - 윈도우애서 링크(https://github.com/YoongiKim/AutoCrawler) 다운로드한 후 앞축 풀기
##### 크롤링에 필요한 패키지 설치

    pip install -r requirements.txt
    
##### 다운로드할 키워드 입력

 - AutoCrawler-master 폴더 안의 keywords.txt을 연다.

 - 검색하고 자 하는 키워드를 한 줄에 한 개씩 쓴 후 저장한다.

##### 크롤링 실행

    python main.py
    
20개로 제한해서 하기

    python main.py --limit 20
##### 데이터 정제하기

데이터 정제를 하는 이유는 한 사진에 내가 입력한 키워드가 2개 이상 들어가 있을 수 있기 때문이다. 만약 동시에 있다면 클래스를 2개가 아닌 하나로만 설정할 수 있다.

    multi-labelclassification

얘로 해결 가능하지만 우리는

    single-labelclassification

으로 하나의 클래스만 있게하고 나머지는 삭제해 버렸다.



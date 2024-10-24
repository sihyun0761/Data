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

![R1280x0](https://github.com/user-attachments/assets/825acf9e-0494-4483-9e66-8face6779243)

##### 크롤링 실행

    python main.py
    
20개로 제한해서 하기

    python main.py --limit 20
##### 크롤링 결과 확인
 - download 폴더에 한 검색어설정한 수만큼의 사진이 다운받아 진 것을 확인한다.
기다리면 download 폴더에 클래스 별로 폴더가 만들어진다.

![R1280x0](https://github.com/user-attachments/assets/105906c2-37f8-43c0-9bcf-5be109dd4c48)
***
![R1280x0](https://github.com/user-attachments/assets/d7d7a39f-170f-4ddf-a8e8-274fc6f5fc91)
***
##### 데이터 정제하기

데이터 정제를 하는 이유는 한 사진에 내가 입력한 키워드가 2개 이상 들어가 있을 수 있기 때문이다. 만약 동시에 있다면 클래스를 2개가 아닌 하나로만 설정할 수 있다.

    multi-labelclassification

얘로 해결 가능하지만 우리는

    single-labelclassification

으로 하나의 클래스만 있게하고 나머지는 삭제해 버렸다.



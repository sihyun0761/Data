
### 데이터 크롤링 하기
***

##### 크롤링 프로그램 설치
    git clone https://github.com/YoongiKim/AutoCrawler

    cd AutoCrawler
##### 크롤링에 필요한 패키지 설치
    pip install -r requirements.txt
##### 다운로드할 키워드 입력
AutoCrawler-master 폴더 안의 keywords.txt을 연다.
검색하고 자 하는 키워드를 한 줄에 한 개씩 쓴 후 저장한다.
##### 크롤링 실행
    python main.py
20개로 제한해서 하기
    python main.py --limit 20


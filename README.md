## 동아리 활동

### 제슨나노 시작하기
***
     1. Jetson Nano Setting 준비물
  
        - jetson nano 4gb
  
        - c type power adapter
  
        - 와이파이 동글
  
        - 웹캠(USB Camera), 또는 CSI Camera (라즈베리파이 V2)
  
        - 64기가 이상 마이크로sd카드
  
        - 그외 쿨링펜, lcd, 또는 모니터. hdmi
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

### yolo 가상환경 만들기
***
##### yolo 가상환경 만들기
    uname -a
    wget https://github.com/Archiconda/build-tools/releases/download/0.2.3/Archiconda3-0.2.3-Linux-aarch64.sh
    sudo chmod 755 Archiconda3-0.2.3-Linux-aarch64.sh
    ls
##### 결과

  Archiconda3-0.2.3-Linux-aarch64.sh Pictures Desktop Public Documents Templates Downloads Videos examples.desktop yolov8_4gb Music

     ./Archiconda3-0.2.3-Linux-aarch64.sh
실행 중 선택이라 뜨면
yes---> enter ---> yes in your /home/ldh/.bashrc ? [yes|no] [no] >>> yes
이렇게 한다.

    conda env list
    conda activate base
    jetson_release 

    
### python 3.8 가상환경 만들기
***
base가 아닌 native에서 실행
    conda create -n yolo python=3.8 -y
    conda env list

    conda activate yolo

 

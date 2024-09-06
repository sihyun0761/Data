## 동아리 활동

### 제슨나노 시작하기
***

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
    ###### result 
ldh@ldh-desktop:~$  ./Archiconda3-0.2.3-Linux-aarch64.sh

Welcome to Archiconda3 0.2.3

In order to continue the installation process, please review the license
agreement.
Please, press ENTER to continue
>>> q
Copyright (c) 2016-2017 Jonathan J. Helmus
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are
met:

    * Redistributions of source code must retain the above copyright
       notice, this list of conditions and the following disclaimer.

    * Redistributions in binary form must reproduce the above
       copyright notice, this list of conditions and the following
       disclaimer in the documentation and/or other materials provided
       with the distribution.

    * Neither the name of the developers nor the names of any
       contributors may be used to endorse or promote products derived
       from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.


Do you accept the license terms? [yes|no]
[no] >>> 
Please answer 'yes' or 'no':'
>>> yes

Archiconda3 will now be installed into this location:
/home/ldh/archiconda3

  - Press ENTER to confirm the location
  - Press CTRL-C to abort the installation
  - Or specify a different location below

[/home/ldh/archiconda3] >>> 
PREFIX=/home/ldh/archiconda3
installing: python-3.7.1-h39be038_1002 ...
Python 3.7.1
installing: ca-certificates-2018.03.07-0 ...
installing: conda-env-2.6.0-1 ...
installing: libgcc-ng-7.3.0-h5c90dd9_0 ...
installing: libstdcxx-ng-7.3.0-h5c90dd9_0 ...
installing: bzip2-1.0.6-h7b6447c_6 ...
installing: libffi-3.2.1-h71b71f5_5 ...
installing: ncurses-6.1-h71b71f5_0 ...
installing: openssl-1.1.1a-h14c3975_1000 ...
installing: xz-5.2.4-h7ce4240_4 ...
installing: yaml-0.1.7-h7ce4240_3 ...
installing: zlib-1.2.11-h7b6447c_2 ...
installing: readline-7.0-h7ce4240_5 ...
installing: tk-8.6.9-h84994c4_1000 ...
installing: sqlite-3.26.0-h1a3e907_1000 ...
installing: asn1crypto-0.24.0-py37_0 ...
installing: certifi-2018.10.15-py37_0 ...
installing: chardet-3.0.4-py37_1 ...
installing: idna-2.7-py37_0 ...
installing: pycosat-0.6.3-py37h7b6447c_0 ...
installing: pycparser-2.19-py37_0 ...
installing: pysocks-1.6.8-py37_0 ...
installing: ruamel_yaml-0.15.64-py37h7b6447c_0 ...
installing: six-1.11.0-py37_1 ...
installing: cffi-1.11.5-py37hc365091_1 ...
installing: setuptools-40.4.3-py37_0 ...
installing: cryptography-2.5-py37h9d9f1b6_1 ...
installing: wheel-0.32.1-py37_0 ...
installing: pip-10.0.1-py37_0 ...
installing: pyopenssl-18.0.0-py37_0 ...
installing: urllib3-1.23-py37_0 ...
installing: requests-2.19.1-py37_0 ...
installing: conda-4.5.12-py37_0 ...
installation finished.
Do you wish the installer to initialize Archiconda3
in your /home/ldh/.bashrc ? [yes|no]
[no] >>> yes

Initializing Archiconda3 in /home/ldh/.bashrc
A backup will be made to: /home/ldh/.bashrc-archiconda3.bak


For this change to become active, you have to open a new terminal.

Thank you for installing Archiconda3!
이건 결과임. 이렇게 뜨면 성공
    conda env list
    conda activate base
    jetson_release 

    
### python 3.8 가상환경 만들기
***
base가 아닌 native에서 실행
    conda create -n yolo python=3.8 -y
    conda env list

    conda activate yolo

 

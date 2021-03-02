# Image Downloader

## 해당 프로젝트는 영어로 된 프로젝트를 한글로 옮겨 놓은것임. 원래 프로젝트는 아래 URL 참고

## [원본](https://github.com/sczhengyabin/Image-Downloader)

## 1. 소개

Selenium, python3, PyQt5를 이용하여 이미지를 다운로드하는 프로젝트

## 2. 주요 특징

+ 검색 엔진: Google, Bing, Baidu
+ 키워드 여러개로된 파일 또는 키워드 입력
+ 여러개의 쓰레드로 다운로드 가능
+ 조건부 검색 가능
+ 구글 안전모드로 스위치 가능
+ 프록시 설정 (socks, http).
+ CMD와 GUI 모두 지원.

## 3. 설치

### 3.1 Python3.5이상 설치 및 다운로드

+ 파이썬3.5이상 다운로드 [다운로드](https://www.python.org/downloads/)

### 3.2 크롬드라이버 셋팅(필수) [recommend]

+ Chrome 또는 Chromium 브라우저가 설치되어있어야함
+ 우측 링크로 크롬드라이버 다운로드. [다운로드](https://chromedriver.chromium.org/downloads)
+ 다운로드 받은 크롬 드라이버를 ${project_directory}/bin/ 경로에 두거나 환경변수에 위치 추가. 
+ ex) Image-Downloader/bin/chromdriver.exe

+ 크롬 브라우저 버전이 안맞는다는 오류가 뜰경우, 크롬 부라우저 버전에 맞는 크롬드라이버 다운로드.

### 3.3 파이썬 패키지 설치

```bash
pip3 install -r requirements.txt
```

## 4. Usage

### 4.1 GUI

Run `image_downloader_gui.py` script to yank GUI:
```bash
python image_downloader_gui.py
```

![GUI](/GUI.png)

### 4.2 CMD

```bash
usage: image_downloader.py [-h] [--engine {Google,Bing,Baidu}]
                           [--driver {chrome_headless,chrome,phantomjs}]
                           [--max-number MAX_NUMBER]
                           [--num-threads NUM_THREADS] [--timeout TIMEOUT]
                           [--output OUTPUT] [--safe-mode] [--face-only]
                           [--proxy_http PROXY_HTTP]
                           [--proxy_socks5 PROXY_SOCKS5]
                           keywords
```

## License

+ MIT License
+ 996ICU License

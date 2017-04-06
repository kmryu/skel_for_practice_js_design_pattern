# skel_for_practice_js_design_pattern
이 저장소는 김태웅이 디자인 패턴 학습 결과를 제출하는 방식을 설명하기위해 만들어졌으며 아래와 같은 목적을 함께 이루고자 만들어졌습니다.

## Goal
* 학습 결과 제출 및 확인
* 학습 결과 공유
* Git 기반의 개발 프로세스에 대한 이해

## 디렉토리 구조 및 네이밍 규칙
* 상위 폴더는 학습 일차를 입력. d1, d2, d3, .... 와 같은 형식이다.
* 폴더를 생성하기 위한 최소한의 조건은 디자인 패턴중 하나의 학습이 완료되었을때 생성 한다.
* 폴더 아래엔 다음과 같은 파일을 생성 한다.
    ** d1.html
    ** README.md
* html 파일에는 해당 일차에 학습했던 디자인 패턴 예제를 실행 해 볼 수 있도록 작성 한다.
* README.md 파일에는 해당 일차에 학습했던 디자인 패턴에 대한 설명을 간략히 작성 한다.
* 예제가 여러개일 경우 해당 학습 일차의 폴더내에 d1-1.html, d1-2.html ... 과 같은 형식으로 추가 한다.

## 학습 결과의 실행 방법에 대한 설명
python을 설치하고 학습 디렉토리로 이동 한 후 아래의 명령을 실행 한다.

```
> python -m SimpleHTTPServer
Serving HTTP on 0.0.0.0 port 8000 ...
```

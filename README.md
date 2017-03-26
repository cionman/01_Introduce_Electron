# Electron 소개

<img src="ASSETS/electron.png" alt="JavaScript">

## Electron은 무엇인가?

[**Electron**](https://electron.atom.io/)은  **HTML, css, javascript**을 사용하여 **크로스 플랫폼**을 지원하는 **데스크탑 어플리케이션**을 제작할 수 있는 프레임워크입니다. 

[**Electron**](https://electron.atom.io/)은 [Chromium](https://www.chromium.org/)과 [Node.js](https://nodejs.org/)를 하나의 런타임으로 결합하여 실행되며, Mac, Windows 및 Linux 용으로 패키지화 할 수 있습니다.

## Electron으로 만들어진 프로그램

### Atom - [https://atom.io/](https://atom.io/)

<img src="ASSETS/atom.png" alt="JavaScript">

### Visual Studio Code - [https://code.visualstudio.com/](https://code.visualstudio.com/)

<img src="ASSETS/visualstudiocode.png" alt="JavaScript">

### Slack - [https://slack.com/](https://slack.com/)

<img src="ASSETS/slack.png" alt="JavaScript">

### Kaku Music player - [http://kaku.rocks/](http://kaku.rocks/)

<img src="ASSETS/kaku.jpeg" alt="JavaScript">

### WebTorrent - [https://webtorrent.io/](https://webtorrent.io/)

<img src="ASSETS/webtorrent.png" alt="JavaScript">

## Electron 설치

---
1. Node 설치 - [https://nodejs.org](https://nodejs.org) 에서 Node를 설치합니다.
2. Electron 설치<br/> 
```
     npm install -g electron
```
   >※ Mac이나 리눅스의 경우는 권한에 따라서 npm 명령어 앞에 sudo를 적어주어야 합니다.**
---
## Electron 실행 구조

Electron은 Main Process와 Renderer Process라고 불리는 2개의 실행 구조를 가집니다.
1. Main Process : 이 프로세스는 Electron의 주 프로세스이며, BrowserWindow api 인스턴스를 통해 창을 생성하고 웹페이지를 읽어옵니다. Browser process 라고도 불립니다.<br/><br/>
 대표 API 소개
    - [app](https://electron.atom.io/docs/api/app/) : 어플리케이션의 생명주기를 다루는 모듈
    - [BrowserWindow](https://electron.atom.io/docs/api/browser-window/) : 창을 생성하고 컨트롤하는 모듈
    - [Menu](https://electron.atom.io/docs/api/menu/) : 어플리케이션의 네이티브 메뉴를 생성하는 모듈
    - [dialog](https://electron.atom.io/docs/api/dialog/) : 네이티브 시스템 다이얼로그 창을 생성하는 모듈(file, alert 등)
    - [ipcMain](https://electron.atom.io/docs/api/ipc-main/) : Main Process에서 Renderer Process로 비동기적으로 통신하는 모듈
    - [Tray](https://electron.atom.io/docs/api/tray/) : 
    시스템의 알림영역에 아이콘 및 컨텍스트 메뉴를 추가하는 모듈
2. Renderer Process : Main Process의 BrowserWindow가 표시하는 웹페이지 내의 프로세스 입니다. 각각의 웹페이지는 개별적인 Renderer Process를 가집니다.<br/></br>
일반 브라우저는 시스템의 고유 리소스 접근을 허용하지 않지만, Electron은 Node.js API를 통해 OS와 상호작용을 가능하게 합니다.<br/><br/>
대표 API 소개
    - [webFrame](https://electron.atom.io/docs/api/web-frame/) : 현재 웹페이지의 렌더링을 커스터마이징하는 모듈
    - [remote](https://electron.atom.io/docs/api/remote/) : Renderer Process에서 Main Process의 모듈을 사용이 가능하게 해주는 모듈
    - [ipcRenderer](https://electron.atom.io/docs/api/ipc-renderer/) : Renderer process에서 Main Process로 비동기적으로 통신하는 모듈
    



## 모던 자바스크립트 라이브러리/프레임워크

모던 자바스크립트를 사용하여 라이브러리/프레임워크를 활용 방법 학습

<img src="ASSETS/JS.gif" alt="JavaScript">


---

### 정규교육과정 소개

- JavaScript 작성 시, 피해야 할 코딩 습관, 좋은 코딩 습관 학습
- 라이브러리 [jQuery](https://jquery.com/), [ScrollMagic](http://scrollmagic.io/), [GSAP](https://greensock.com/) 등을 통해 실무에 활용 가능한 예제 실습
- 프레임워크 [Vue.js](https://vuejs.org/) 입문

---

1. JavaScript를 짜임새있게 짤 수 있는 방법을 다뤄보면서 피해야할 안좋은 코딩 습관을 살펴봅니다.
1. [ECMAScript 6](http://www.ecma-international.org/ecma-262/6.0/)를 살펴보면서 [Node.js](http://nodejs.org/) 환경의 JavaScript도 가볍게 다뤄봅니다.
1. 실무에서 자주 사용되는 UI 컴포넌트를 jQuery 버전으로 작성해봅니다.
1. 애니메이션 라이브러리를 사용하여 스크롤 기반의 인터랙션 페이지를 제작해봅니다.
1. Vue.js 프레임워크가 지향하는 컴포넌트 단위 개발 방법에 대해 다뤄봅니다.

※ 본 과정은 과정 시작 전, 수강생 수준 테스트 후 평균 학습 능력에 따라 커리큘럼이 변동될 수 있습니다.<br>
요컨대 수강생 수준이 부족하다 판단될 경우 JavaScript 기본기 다지는 교육으로 변경 진행합니다.

---

### 정규교육과정 개요

#### 목적

- JavaScript 활용 능력 증진
- 라이브러리 및 프레임워크 학습/활용

#### 참여 대상

- JavaScript를 사용 중인 실무자
- 라이브러리 및 프레임워크를 학습 방법을 익히고자하는 실무자
- 프론트엔드 라이브러리/프레임워크 개념 정리가 부족한 실무자

#### 참여 불가능 대상

- HTML/CSS로 페이지 뷰 구현이 가능하지 않으면 이 과정은 적합하지 않습니다.
- JavaScript를 모르거나, 잘 사용하지 않는다면 이 과정은 적합하지 않습니다.

---

### 정규교육과정 프로그램

#### DAY 1. JavaScript __Good/Anti Pattern__

- Anti Pattern
- Good Pattern
- ECMAScript 6

#### DAY 2. JavaScript __Library__

- jQuery API
- ScrollMagic API
- GSAP API

#### DAY 3. JavaScript __Framework__

- Vue.js API
- Vuex


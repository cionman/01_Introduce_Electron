# Electron 소개

<img src="ASSETS/electron.png" alt="JavaScript">

## Electron은 무엇인가?

[**Electron**](https://electron.atom.io/)은  **HTML, css, javascript**을 사용하여 **크로스 플랫폼**을 지원하는 **데스크탑 어플리케이션**을 제작할 수 있는 프레임워크입니다. 

[**Electron**](https://electron.atom.io/)은 [Chromium](https://www.chromium.org/)과 [Node.js](https://nodejs.org/)를 하나의 런타임으로 결합하여 실행되며, Mac, Windows 및 Linux 용으로 패키지화 할 수 있습니다.


<br/><br/>
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

<br/><br/>
## Electron 설치

---
1. Node 설치 - [https://nodejs.org](https://nodejs.org) 에서 Node를 설치합니다.
2. Electron 설치<br/> 
```
     npm install -g electron
```
   >※ Mac이나 리눅스의 경우는 권한에 따라서 npm 명령어 앞에 sudo를 적어주어야 합니다.**
---
<br/><br/>
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
    




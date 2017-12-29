---?image=assets/image/patrick-tomasso.jpg

# React 튜토리얼

---?image=assets/image/daniel-ghio.jpg

## 목차
- 준비
- 개요 
- 상태변경 
- 히스토리 저장

<br>
---?image=assets/image/daniel-ghio.jpg

### 준비 

- 개발결과 보기 
- 사전준비
- 개발 환경

-@fa[microphone gp-tip](Press S for Speaker Notes)
<br><br>

----?image=assets/image/daniel-ghio.jpg
---?code=src/go/server.go&lang=golang&title=Golang File

### 개요 
- React란?
- 시작하기 
- Props를 통한 Data전달
- Interactive 구성요소
- 개발도구 

-## Template Features
---?image=assets/image/daniel-ghio.jpg

### 상태변경 

- Immutability의 중요성
- 기능요소
- 다음순번 처리 
- 우승자 선정

---?code=src/go/server.go&lang=golang&title=Golang File

### 히스토리 저장
- Moves 보여주기
- Keys
- 시간순서로 실행하기 
- 정리하기 

---?image=assets/image/simon-matzinger.jpg

@title[JavaScript Block]

<p><span class="slide-title">JavaScript Block</span></p>

```javascript
// Include http module.
var http = require("http");

// Create the server. Function passed as parameter
// is called on every request made.
http.createServer(function (request, response) {
  // Attach listener on end event.  This event is
  // called when client sent, awaiting response.
  request.on("end", function () {
    // Write headers to the response.
    // HTTP 200 status, Content-Type text/plain.
    response.writeHead(200, {
      'Content-Type': 'text/plain'
    });
    // Send data and end response.
    response.end('Hello HTTP!');
  });

// Listen on the 8080 port.
}).listen(8080);
```

@[1,2](You can present code inlined within your slide markdown too.)
@[9-17](Displayed using code-syntax highlighting just like your IDE.)
@[19-20](Again, all of this without ever leaving your slideshow.)

---?gist=onetapbeyond/494e0fecaf0d6a2aa2acadfb8eb9d6e8&lang=scala&title=Scala GIST

@[23](You can even present code found within any GitHub GIST.)
@[41-53](GIST source code is beautifully rendered on any slide.)
@[57-62](And code-presenting works seamlessly for GIST too, both online and offline.)

---?image=assets/image/daniel-ghio.jpg

## Template Help

- [Code Presenting](https://github.com/gitpitch/gitpitch/wiki/Code-Presenting)
  + [Repo Source](https://github.com/gitpitch/gitpitch/wiki/Code-Delimiter-Slides), [Static Blocks](https://github.com/gitpitch/gitpitch/wiki/Code-Slides), [GIST](https://github.com/gitpitch/gitpitch/wiki/GIST-Slides) 
- [Custom CSS Styling](https://github.com/gitpitch/gitpitch/wiki/Slideshow-Custom-CSS)
- [Slideshow Background Image](https://github.com/gitpitch/gitpitch/wiki/Background-Setting)
- [Slide-specific Background Images](https://github.com/gitpitch/gitpitch/wiki/Image-Slides#background)
- [Custom Logo](https://github.com/gitpitch/gitpitch/wiki/Logo-Setting), [TOC](https://github.com/gitpitch/gitpitch/wiki/Table-of-Contents), and [Footnotes](https://github.com/gitpitch/gitpitch/wiki/Footnote-Setting)

<br><br>

---?image=assets/image/gitpitch-audience.jpg

### <span class="white">Template Versions</span>

- #### [Base Template  @fa[external-link gp-download]](https://gitpitch.com/gitpitch/templates/brick)
- #### [Code Maximized @fa[external-link gp-download]](https://gitpitch.com/gitpitch/templates/brick?p=codemax)
- #### [Speaker Notes @fa[external-link gp-download]](https://gitpitch.com/gitpitch/templates/brick?p=speaker)

---?image=assets/image/daniel-ghio.jpg

### Questions?

<br>

@fa[twitter gp-contact](@gitpitch)

@fa[github gp-contact](gitpitch)

@fa[medium gp-contact](@gitpitch)

---?image=assets/image/gitpitch-audience.jpg

@title[Download this Template!]

### <span class="white">Get your presentation started!</span>
### [Download this template @fa[external-link gp-download]](https://gitpitch.com/template/download/brick)


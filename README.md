# RactTutorial

## 준비
### 개발결과 보기 
* [tic-tac-toe 게임](https://codepen.io/gaearon/pen/gWWZgR?editors=001)
### 사전준비 
* 사전지식은 HTML, JavaScript이다.
* JavaScript 요약 [가이드](https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript)를 확인하라. 
* ES6 문법 : arrow functions, classes, let, const 
 
### 따라하기 
* 개발 완료 하기 위한 방법 두가지가 있다.
#### 웹브라우저상에서 개발
* [Starter code](https://codepen.io/gaearon/pen/oWWQNa?editors=0010)
#### 로컬 PC에서 개발
* [Node.js](https://nodejs.org/en/) 다운받기
* [이곳에서](https://reactjs.org/docs/installation.html#creating-a-new-application) 새로운 프로젝트 생성하기 

## 개요 
### React란?
* 선언적이고 효과적이며 유연한 JavaScript 라이브러리이다.
* React.Componet 서브클래스로 시작 할 것이다. 


```javascript
class ShoppingList extends React.Component {
  render() {
    return (
      <div className="shopping-list">
        <h1>Shopping List for {this.props.name}</h1>
        <ul>
          <li>Instagram</li>
          <li>WhatsApp</li>
          <li>Oculus</li>
        </ul>
      </div>
    );
  }
}
// Example usage: <ShoppingList name="Mark" />

ReactDOM.render(
  <ShoppingList />,
  document.getElementById('root')
);
```
### 시작하기
* [예제링크](https://codepen.io/gaearon/pen/oWWQNa?editors=0010)
* 3개의 구성
  * Square
  * Board
  * Game

### Props을 통한 Data 전달
* Board의 구성요소 데이터를 Square 구성요소로 보내는 것을 해보자.

 * Board안에 있는 renderSquare method코드는 value prop를 Square로 보내기위해 변환한다. 
```javascript
class Board extends React.Component {
    renderSquare(i) {
        return <Square value = {i}/>;
    }
}

class Square extends React.Component {
    render () {
        return (
        <button className ="square">
        {this.props.value}
        </button>
        );
    }
}

```
### Interactive 구성요소
* 사각형안을 클릭하면 구성요소를 "X"로 채워넣는 것을 만들어 보자
 * render() 함수안에 있는 변환하는 버튼태크를 되돌렸다 아래의 코드를 참고 하라


```javascript
class Square extends React.Component {
    render() {
        return (
            <button className="square" onClick = {() => alter('click')}>
              {this.props.value}
            </button>
        );
    }
}
```
사각형을 클릭했다면, 브라우저에서 alter를 가지고 있어야 한다.
onClick 함수는 자바스크립트 새로운 문법이며 버튼을 클릭 하는 대신에 즉각적으로 주의를 준다.

React 구성요소는 this.state 상태를 갖을수 있지만 private 구성요소를 고려해야 한다.
최근 사각형안의 상태들을 저장하고, 그 사각형이 클릭되면 변환하자. 

* 첫번째는 클래스 상태를 초기화 한다.
 ```javascript
 class Square extends React.Component {
     constructor(props) {
         super(props);
         this.state = {
             value: null,
         };
     }

     render() {
         return (
             <button className ="square" onClick={() => alter('click')}>
                {this.props.value}
             </button>
         );
     }
 }
```
* 자바스크립트안에서 서브클래스 설계자가 super(); 호출를 정의 할 때 명확히 해야한다.
* 사각형 render method를 최근 상태의 값을 나타내기 위해서 그리고 토글을 클릭하기 위해서 바꾼다. 
 * <button>태그안의 this.props.value를 this.state.value로 대체한다. 
 * () => alter()를 () => this.setState({value: 'X'})로 대체 한다 

 ```javascript
 class Square extends React.Compnent {
     constructor(props) {
         super(props);
         this.state = {
             value: null,
         };
     }

     render() {
         return (
             <button className="square" onClick= {() => this.setState({value: 'X'})}>
             {this.state.value}
             </button>
         );
     }
 }  
 ```

### 개발도구

## State 상태변경 
### Immutability의 중요성 
### 기능요소 
### 다음순번 처리 
### 우승자 선정

## 히스토리 저장
### Moves 보여주기 
### keys
### 시간순서로 실행하기 
### 정리하기 





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
* React.Componet 서브클래스를 시작 할 것이다. 


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
### Interactive 구성요소
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





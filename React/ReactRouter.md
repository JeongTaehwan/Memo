# React Router 🕵️‍♂️

## 설명

**React Router란?** 
> 새로운 페이지를 로드하지 않고 하나의 페이지(SPA) 안에서 필요한 데이터만 가져오는 형태이다.

**SPA란?** 🕵️‍♂️
> SPA란 `Single Page Application` 의 약자로 말 그대로 페이지가 하나인 어플리케이션을 말한다. 기존의 웹 어플리케이션의 구조는, 여러 페이지로 구성되어 있어 속도면에서 SPA 보다 더욱 느린 모습을 보인다.

---

## 설치 및 기본적인 사용법 
 > 먼저 프로젝트를 만든 후 라우터 관련 라이브러리를 설치 한다.

```javascript
$ cd router-tutorial
$ yarn add react-router-dom
```
> 라우터를 적용할 땐 `index.js` 에서 `BrowserRouter` 라는 컴포넌트를 사용하여 적용한다.

```javascript
import React from 'react';
import ReactDOM from 'react-dom';
import { BrowserRouter } from 'react-router-dom'; // BrowserRouter 를 불러옴
import './index.css';
import App from './App';
import * as serviceWorker from './serviceWorker';

// App 을 BrowserRouter 로 감쌈
ReactDOM.render(
  <BrowserRouter>
    <App />
  </BrowserRouter>,
  document.getElementById('root')
);

serviceWorker.unregister();
```

---

## 파라미터와 쿼리 

> 페이지 주소를 정의할 때, 유동적인 값을 전달해야 할 수 있다. 이 때 파라미터와 쿼리로 나눠질 수 있다.

```
파라미터: /profiles/velopert
쿼리: /about?details=true
```
- 파라미터 : 특정 id나 이름을 가지고 조회를 할 때 사용
- 쿼리 : 특정 키워드를 검색하거나, 요청을 할 때 필요한 옵션을 전달할 때 사용

---

## 서브 라우트 

>  서브 라우트는 라우트 내부의 라우트를 만드는 것을 의미한다. 간단하게 컴포넌트를 만들어 그 안에 또 `Route` 컴포넌트를 렌더링 하면 된다.

---

## useReactRouter 

> `Router` 를 `Hook` 을 이용하여 구현할 수 있는데 `useReactRouter` 를 이용하여 구현할 수 있다.

```
$ yarn add use-react-router
```

---

**출처 : 패스트캠퍼스 강의 - 벨로퍼트와 함께하는 React Router**
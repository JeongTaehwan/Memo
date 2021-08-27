# Styled-Components 💅

## Styled-Components란? 
> Styled-Components란 `CSS in JS`로 css를 react의 component 내부에서 사용할 수 있게 만든 가장 인기있는 라이브러리 입니다.

## Styled-Components 사용법 
> `styled-components`를 사용할 react 폴더에 `yarn add styled-components`를 해주세요.

```javascript
import styled from 'styled-components';

const Circle = styled.div`
  width: 5rem;
  height: 5rem;
  background: black;
  border-radius: 50%;
`;

function App() {
  return <Circle />;
}
```
> 이런식으로 코드를 작성하면 `Circle`이라는 `styled-components`를 사용한 것이다. 코드의 윗부분에서 `import styled from 'styled-components';`로 불러와 사용할 수 있다.

---
  
**출처 : 패스트캠퍼스 강의 - 벨로퍼트와 함께하는 리액트 컴포넌트 스타일링하기**
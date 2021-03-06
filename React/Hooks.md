# Hooks

리액트 v16.8에 새로 도입된 기능인 Hooks 덕분에 함수 컴포넌트에서도 state와 여러 React 기능을 사용할 수 있게 되었습니다. Hook은 함수 컴포넌트에서 state와 lifecycle 기능을 연동할 수 있게 해줍니다. 클래스 안에서는 동작하지 않습니다.

<br>

## 1. Motivation

리액트 공식 문서에서는 Hooks의 개발 동기로 기존 클래스형 컴포넌트의 문제점들을 제시하였습니다.

- 컴포넌트 사이에서 상태 로직 재사용이 어렵다.
- 복잡한 컴포넌트들은 이해하기 어렵다.
- 클래스는 사람과 기계 모두를 헷갈리게 만든다.

이같은 문제점 덕분에 react를 배우는 데에 클래스가 큰 진입장벽이 되었으며, react의 최신 기술들이 클래스형 컴포넌트에 효과적으로 적용되지 않았습니다.

따라서 함수 컴포넌트에 Hooks를 이용해 react 개념에 좀 더 직관적인 API를 제공하기로 합니다.

<br>

## 2. Hook을 사용해야 하는 이유

- 컴포넌트로부터 state 관련 로직을 추상화할 수 있고 독립적인 테스트, 재사용이 가능하다.
- 서로 비슷한 것을 하는 작은 함수의 묶음으로 컴포넌트를 나눌 수 있다.
- 코드가 최적화 가능한 경로에서 유지될 가능성이 높다.(코드의 최소화, 핫 리로딩을 비교적 신뢰 가능)

<br>

## 3. 내장 Hook

- useState : 컴포넌트 상태관리
- useEffect : 렌더링될 때마다 특정 작업 수행
- useReducer : useState보다 다양한 상태관리
- useMemo : 컴포넌트 내부 연산 최적화
- useCallback : 렌더링 성능 최적화
- useRef : 함수 컴포넌트에서 ref을 쉽게 사용할 수 있도록 함

<br>

## 4. Hook 사용 규칙

- <b>최상위</b>에서만 Hook을 호출해야 한다.
- React 함수 컴포넌트 내에서만 Hook을 호출해야 한다. (일반 js 함수에서 호출 금지, custom Hook 내에서는 가능)

<br>

## Reference

- React : https://ko.reactjs.org/docs/hooks-intro.html
- 리액트를 다루는 기술, 김민준

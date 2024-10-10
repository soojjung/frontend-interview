# 프론트엔드 기술 면접

### 프론트엔드 예상 기술 면접 질문

질문에 대한 답만 외우는 것이 아닌 해당 내용에 대한 공부를 우선적으로 하며, 기술 면접에서도 잘 대답할 수 있도록 준비합니다.

<img src="./images/main.png" alt="메인" />

## JavaScript

- [호이스팅에 대해서 설명해주세요.](notes/javascript/hoisting.md)
- [클로저에 대해서 설명해주세요.](notes/javascript/closure.md)
- [JavaScript는 어떤 언어인가요?](notes/javascript/javascript-language.md)
- [Event Loop에 대해 알고 있으신가요?](notes/javascript/eventloop.md)
- [마이크로태스크 큐와 태스크 큐에 대해서 말씀해주세요.](notes/javascript/microtaskqueue-taskqueue.md)
- [이벤트 버블링과 캡처링에 대해서 말씀해주세요.](notes/javascript/event-bubbling-capturing.md)
- [실행 컨텍스트에 대해서 설명해주세요.](notes/javascript/execution-context.md)
- [null, undefined, undeclared, NaN 에 대해 설명해주세요.](notes/javascript/null-undefined-NaN.md)
- [얕은 비교와 깊은 비교의 차이](notes/javascript/shallow-deep-comparison.md)
- [Prototype과 Prototype Chaining이란?](notes/javascript/prototype-chaining.md)
- [콜백함수란?](notes/javascript/callback-function.md)
- [Promise란?](notes/javascript/promise.md)
- [async-await란?](notes/javascript/async-await.md)
- [OOP 특징](notes/javascript/object-oriented-programming.md)
- [화살표 함수와 일반 함수의 차이점](notes/javascript/arrow-function.md)
- [‘==’과 ‘===’의 차이점](notes/javascript/‘==’-‘===’.md)
- [event.target과 event.currentTarget의 차이점](notes/javascript/event-current-target.md)
- [Map과 Set 설명 및 차이점](notes/javascript/map-set.md)

## CSS

- [CSS에서 margin과 padding에 대해서 설명해주세요.](notes/css/margin-padding.md)
- [CSS에서 position을 어떻게 사용하는지 설명해주세요.](notes/css/position.md)
- [Flex 속성 설명해주세요.](notes/css/flex.md)
- [Box model에 대해 설명해주세요.](notes/css/box-model.md)
- [Display에 대해 설명해주세요.](notes/css/display.md)
- [CSS 애니메이션과 JS 애니메이션의 차이점](notes/css/css-animation-js-animation.md)

## 브라우저 / 네트워크

- [브라우저의 렌더링 원리에 대해 설명해주세요.](notes/browser-network/browser-rendering.md)
- [Reflow와 Repaint가 실행되는 시점에 대해 말씀해주세요.](notes/browser-network/reflow-repaint.md)
- [주소창에 google.com을 입력하면 일어나는 일에 대해 말씀해주세요.](notes/browser-network/google.com.md)
- [브라우저 저장소의 차이점에 대해 설명해주세요. (LocalStorage,SessionStorage,Cookie)](notes/browser-network/web-storage.md)
- [CORS란? 대응 방법은?](notes/browser-network/cors.md)
- [RESTful API란?](notes/browser-network/restful-api.md)
- [OAuth란? OAuth의 동작 방식은?](notes/browser-network/o-auth.md)
- [JWT방식과 Session방식의 차이](notes/browser-network/jwt-session.md)
- [HTTP와 HTTPS 통신의 차이](notes/browser-network/http-https.md)
- [SEO란?](notes/browser-network/seo.md)
- [크로스 브라우징이란?](notes/browser-network/cross-browsing.md)
- [CSR과 SSR의 차이점](notes/browser-network/csr-ssr.md)
- [DOM과 가상 DOM 이란?](notes/browser-network/virtual-dom.md)

## React

- [React는 라이브러리인가요 프레임워크인가요?](notes/react/library-framework.md)
- [리액트의 특징을 설명해주세요. (리액트를 사용한 이유)](notes/react/why-react.md)
- [Suspense에 대해서 설명해주세요.](notes/react/suspense.md)
- [JSX 를 알고있나요?](notes/react/jsx.md)
- [리액트에서 JSX가 어떻게 작동하나요?](notes/react/how-jsx-works.md)
- [리액트에서 JSX 사용 시 주의해야 할 점이 있을까요?](notes/react/jsx-considerations.md)
- [React에서 화면 변경 과정을 설명해주세요. (가상 DOM을 이용한 업데이트)](notes/react/how-virtualdom-works.md)
- [컴포넌트의 key 에 대해 설명해주세요.](notes/react/key.md)
- [SPA 장점과 단점을 설명해주세요.](notes/react/spa.md)
- [SEO(검색엔진최적화) 가 뭔가요?](notes/react/seo.md)
- [TTV, TTI를 알고 있나요? (time-to-view, time-to-interect)](notes/react/ttv-tti.md)
- [함수 컴포넌트와 클래스 컴포넌트의 차이가 무엇인가요?](notes/react/class-component.md)
- [컴포넌트 라이프 사이클에 대해 설명해주세요.](notes/react/life-cycle.md)
- [props와 state에 대해 설명해주세요.](notes/react/props-state.md)
- [Props Drilling 이란 무엇인가요?](notes/react/props-drilling.md)
- [리액트 state의 불변성에 대해 설명해주세요.](notes/react/immutability.md)
- [스프레드 연산자의 단점에 대해 설명해주세요.](notes/react/spread-operator.md)
- [리액트에서 자식 컴포넌트에서 부모 컴포넌트로 데이터를 전달할 수는 없나요?](notes/react/pass-data-from-child-to-parent.md)
- [훅이란 무엇인가요?](notes/react/hooks.md)
- [useState 훅을 설명해주세요.](notes/react/useState.md)
- [useEffect 훅을 설명해주세요.](notes/react/useEffect.md)
- [useLayoutEffect 훅을 설명해주세요.](notes/react/useLayoutEffect.md)
- [useMemo와 useCallback 훅의 공통점과 차이점을 설명해주세요.](notes/react/useMemo-useCallback.md)
- [componentDidMount, componentDidUpdate 등 클래스 컴포넌트에서 사용되던 생명주기 메소드를 함수 컴포넌트에서는 어떻게 구현하나요?](notes/react/life-cycle-methods.md)

# 리액트에서 JSX 가 어떻게 작동하나요?

### 1. **JSX의 기본 동작**

JSX 자체는 브라우저에서 직접 이해되지 않기 때문에, React 프로젝트에서 사용하기 위해서는 **트랜스파일러**(예: Babel)가 필요합니다. 이 트랜스파일러가 JSX를 순수한 JavaScript 코드로 변환합니다.

### 2. **React.createElement() 함수**

JSX 코드를 변환한 결과인 `React.createElement()` 함수는 **React 요소(React Element)**를 반환하는 함수입니다. 이 함수는 컴포넌트나 HTML 태그, 그리고 해당 태그의 속성(props), 자식 요소들을 입력받아 **React Element**라는 객체를 생성합니다.

### 3. **가상 DOM (Virtual DOM)과의 연계**

JSX에서 변환된 `React.createElement()` 함수는 React 요소를 정의하는데, 이 React 요소는 가상 DOM에 추가됩니다. 가상 DOM은 메모리 상에서의 DOM 트리 복사본으로, 실제 DOM과는 별개로 관리됩니다. React는 이 가상 DOM을 사용하여 효율적으로 DOM 업데이트를 관리합니다.

- JSX로 작성된 React 요소들이 가상 DOM에 반영됩니다.
- React는 가상 DOM을 실제 DOM과 비교(이 과정은 **"diffing"**이라고 불림)하여 변경된 부분만 실제 DOM에 업데이트합니다.

이 방식 덕분에 React는 불필요한 DOM 조작을 줄이고 성능을 최적화할 수 있습니다.

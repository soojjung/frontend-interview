# 리액트에서 JSX 사용 시 주의해야 할 점이 있을까요?

1. 최상단 단일 루트 요소로 감싸기

2. `class` 대신 `className` 사용
   JSX는 JavaScript이기 때문에, `class`는 JavaScript의 예약어입니다. 따라서 HTML의 `class` 속성을 JSX에서 사용할 때는 `className`으로 작성해야 합니다.

3. 컴포넌트 이름은 반드시 대문자로 시작
   JSX에서 소문자로 시작하는 태그는 HTML 태그로 인식되고, 대문자로 시작하는 태그는 React 컴포넌트로 인식됩니다.

4. JavaScript 표현식은 중괄호 `{}`로 감싸기
5. JSX에서 내용이 없는 태그는 반드시 self-closing 태그로 작성해야 합니다.
6. JSX에서 배열이나 리스트를 렌더링할 때는 반드시 고유한 `key` 속성을 지정해야 합니다. `key`는 React가 리스트의 항목을 식별하고, DOM 업데이트를 최적화하는 데 사용됩니다.

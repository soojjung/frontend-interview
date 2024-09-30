# null, undefined, undeclared, NaN 에 대해 설명해주세요.

**null**

- 빈 값
- null이라는 빈 값을 할당했을 때, 생기는 타입입니다.
- typeof ‘object’인데, 이는 자바스크립트의 버그이다.

**undefined**

- 정의되지 않음
- `var` 선언문의 경우, 호이스팅 되었을 때, 변수 선언과 초기화가 동시에 일어나기 때문에, 변수가 `undefined` 됩니다.(타입 결정 안됨)

```
console.log(data); // undefined
const data = 'data';
```

**undeclared**

- 선언되지 않음
- `let`, `const` 선언문의 경우, [호이스팅](https://github.com/Esoolgnah/Frontend-Interview-Questions/blob/main/Notes/important-4/null-undefined-undeclared-nan.md#gear-%ED%98%B8%EC%9D%B4%EC%8A%A4%ED%8C%85) 되었을 때, 변수 선언과 초기화가 따로 이루어지기에, 변수가 `undeclared`되어 에러가 생깁니다.

```
console.log(data); // error
let data = 'data';
```

**NaN**

- 표현 불가능한 수치형 결과입니다.

`typeof 1 / 0; // NaN`

```jsx
console.log(typeof NaN); // 'number'
console.log(NaN === NaN); // false
```

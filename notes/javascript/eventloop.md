# Event Loop에 대해 알고 있으신가요?

Event Loop는 **Web API를 사용하면 자바스크립트 런타임에서 자동으로 Event Loop와 Event Queue가 돌아갑니다**.

Call Stack과 Event Queue의 상태를 주기적으로 체크하고, Call Stack이 빈 상태가 되면 Event Queue의 첫 번째 callback function을 Call Stack에서 실행시킵니다.

만약 예시처럼 코드가 작성되어 있다면

```jsx
setTimeout(() => {
  console.log(5);
}, 1000);
```

콜스택에 `setTimeout` 함수가 쌓이고, 이 `setTimeout` 함수가 pop 되면서 실행되고, 외부 Web API에서 1초의 타이밍이 돌고 난 다음에 콜백함수인 콘솔로그가 Event Queue에 들어가게 됩니다. Event Loop가 콜스택과 Event Queue를 확인하고, 콜스택이 비어있기 때문에 콘솔로그가 콜스택에 들어가고, pop되면서 실행되어 5를 뱉어냅니다.

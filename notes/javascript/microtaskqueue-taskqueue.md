# 마이크로태스크 큐와 태스크 큐에 대해서 말씀해주세요.

자바스크립트에서 마이크로태스크 큐와 태스크 큐는 **비동기 작업을 처리**하는 두 가지 메커니즘으로, **이벤트 루프가 관리**하는 개념입니다.

### 태스크 큐

태스크 큐는 자바스크립트의 비동기 작업(**setTimeout, setInterval, 이벤트 핸들러**)이 완료되었을 때, 그 콜백을 저장하는 큐입니다.

### 마이크로태스크 큐

마이크로태스크 큐는 보다 우선적으로 처리되는 비동기 작업을 관리하는 큐입니다. 여기에는 주로 **Promise**의 콜백, **MutationObserver** 등이 들어갑니다.

콜 스택이 비어 있을 때, 이벤트 루프는 먼저 마이크로태스크 큐를 모두 처리하고, 그 다음에 태스크 큐의 작업을 처리합니다.

```jsx
console.log("Start");

setTimeout(() => {
  console.log("Task Queue");
}, 0);

Promise.resolve().then(() => {
  console.log("Microtask Queue");
});

console.log("End");
```

```jsx
Start
End
Microtask Queue
Task Queue
```

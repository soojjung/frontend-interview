# Promise란?

Promise는 비동기 연산이 종료된 이후에 결과값이나 실패 사유를 처리하기 위한 것이고, Promise를 이용하면 동기 메서드처럼 값을 반환할 수 있습니다. Promise는 resolve와 reject를 파라메터로 받고 있는데 비동기 작업이 성공하면 resolve 함수를 호출하고, 실패하면 reject 함수를 호출합니다.

### **Promise 사용 (then, catch, finally)**:

`Promise` 객체는 비동기 작업이 완료되었을 때 실행할 콜백 함수를 연결할 수 있도록 **`then`**, **`catch`**, **`finally`** 메서드를 제공합니다.

- **`then`**: `resolve`가 호출되면 실행되는 **이행 성공** 콜백을 처리합니다.
- **`catch`**: `reject`가 호출되면 실행되는 **거부** 콜백을 처리합니다.
- **`finally`**: Promise의 **성공/실패와 상관없이** 마지막에 실행되는 콜백을 처리합니다.

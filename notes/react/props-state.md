# props와 state에 대해 설명해주세요.

- 상태(state)는 컴포넌트 내부에서 관리되는 데이터이며, 컴포넌트가 스스로 변경할 수 있습니다.
- props는 부모 컴포넌트가 자식 컴포넌트로 전달하는 데이터로, 자식 컴포넌트는 props를 수정할 수 없습니다.
- 상태는 동적 데이터, props는 정적 데이터를 다룰 때 주로 사용됩니다.

## 컴포넌트가 언제 다시 렌더링 되나요?

- 다시 호출되면서 props가 변경되거나,
- 컴포넌트 내부의 state가 변경되거나,
- 부모 컴포넌트가 다시 렌더링 되거나,
- 클래스 컴포넌트의 `forceUpdate` 메소드가 호출되었을 때 발생합니다.

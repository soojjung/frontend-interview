# 리액트에서 자식 컴포넌트에서 부모 컴포넌트로 데이터를 전달할 수는 없나요?

기본적으로 리액트에서 컴포넌트 사이 데이터 전송은 props로 이루어집니다.

리액트는 단방향 바인딩이기 때문에 props는 부모 컴포넌트에서 자식 컴포넌트로만 넘겨줄 수 있습니다.

하지만 자식 컴포넌트에서 부모 컴포넌트로 데이터를 전달하기 위한 방법으로 **함수를 사용**할 수 있습니다. props로 부모 컴포넌트의 상태를 변경하는 함수를 전달하고, 자식 컴포넌트에서 props로 넘겨받은 함수를 호출해서 부모 컴포넌트의 상태를 변경할 수도 있습니다.

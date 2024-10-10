# componentDidMount, componentDidUpdate 등 클래스 컴포넌트에서 사용되던 생명주기 메소드를 함수 컴포넌트에서는 어떻게 구현하나요?

클래스 컴포넌트에서 사용되던 생명주기 메서드인 `componentDidMount`, `componentDidUpdate`, `componentWillUnmount`는 함수 컴포넌트에서는 **`useEffect` 훅**을 통해 구현할 수 있습니다. `useEffect`는 컴포넌트의 마운트, 업데이트, 언마운트 시점에 맞춰 특정 로직을 실행할 수 있도록 해줍니다.

### 1. **`componentDidMount` → `useEffect`**

`componentDidMount`는 **컴포넌트가 처음 마운트(렌더링)된 후에 한 번 실행**되는 생명주기 메서드입니다. 함수 컴포넌트에서는 **빈 의존성 배열([])**을 `useEffect`에 전달하여 컴포넌트가 마운트될 때 한 번만 실행되도록 설정할 수 있습니다.

### 2. **`componentDidUpdate` → `useEffect`**

**설명**: `useEffect`의 의존성 배열에 **`value`**를 넣으면, `value`가 변경될 때마다 `useEffect`가 실행됩니다. 이는 `componentDidUpdate`와 동일한 동작입니다.

### 3. **`componentWillUnmount` → `useEffect`의 cleanup 함수**

`componentWillUnmount`는 **컴포넌트가 언마운트되기 직전에 호출**되어, 타이머 제거나 이벤트 리스너 해제 등의 정리 작업을 수행하는 생명주기 메서드입니다. 함수 컴포넌트에서는 `useEffect` 내에서 `cleanup 함수`를 반환하여 컴포넌트가 언마운트될 때 정리 작업을 수행할 수 있습니다.

`useEffect`에서 반환된 **cleanup 함수**는 컴포넌트가 **언마운트될 때** 실행됩니다. 이는 `componentWillUnmount`와 동일한 역할을 합니다.

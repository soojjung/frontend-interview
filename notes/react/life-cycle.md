# 컴포넌트 라이프 사이클에 대해 설명해주세요.

React에서 **컴포넌트 라이프사이클**(Component Lifecycle)은 **컴포넌트가 생성되고, 업데이트되고, 소멸되기까지의 일련의 과정(생명 주기)을 의미합니다.** 각각의 단계에서 React는 특정 메서드(또는 함수)를 호출하여, 개발자가 그 단계에서 필요한 작업을 수행할 수 있도록 합니다.

React 컴포넌트의 라이프사이클은 크게 **세 가지 단계**로 나눌 수 있습니다:

1. **마운트(Mount)**: 컴포넌트가 생성되어 DOM에 삽입되는 단계
2. **업데이트(Update)**: 컴포넌트의 상태나 props가 변경될 때 다시 렌더링되는 단계
3. **언마운트(Unmount)**: 컴포넌트가 DOM에서 제거되는 단계

# 스프레드 연산자의 단점에 대해 설명해주세요.

스프레드 연산자는 얕은 복사만 수행합니다. 즉, 스프레드 연산자는 객체나 배열의 1차적인 속성만 복사하고, 중첩된 객체나 배열은 그대로 참조합니다. 이는 깊은 구조의 객체를 다룰 때 문제가 될 수 있습니다.

객체 안에 객체가 있는 등 깊이가 있는 객체들을 복사할 때, 내부에 있는 객체는 참조값이 복사되게 됩니다.
그래서 복사 로직이 복잡해 질 수 있고, 간단하게 해결하기 위해서 immer 라이브러리 등을 사용할 수 있습니다.

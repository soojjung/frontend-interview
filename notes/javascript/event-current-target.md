# event.target과 event.currentTarget의 차이점

`event.target`은 이벤트가 **실제로 발생한 요소**를 가리킵니다. 즉, 사용자가 클릭하거나 상호작용한 **가장 하위의 요소**를 반환합니다.

`event.currentTarget`은 **이벤트 핸들러가 등록된 요소**를 가리킵니다. 즉, 이벤트가 현재 처리되고 있는 **요소 자체**를 나타냅니다.

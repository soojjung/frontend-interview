# 브라우저의 렌더링 원리에 대해 설명해주세요.

브라우저는 화면에 나타내는 요소를 렌더링 할 때, 웹킷(Webkit)이나 게코(Gecko) 같은 렌더링 엔진을 사용합니다. 렌더링 엔진은 웹 페이지 리소스를 파싱하여 화면에 표시하는데, 다음 단계들로 이루어집니다.

## 브라우저의 렌더링 과정

1. 서버로 받은 **HTML 문서를 파싱** 후, **DOM 트리**를 구축
2. HTML 파싱 중 CSS 링크 또는 스타일 태그를 만나면, CSS를 파싱 후 **CSSOM 트리**를 구축
3. 자바스크립트 파싱 및 실행 (HTML 파싱 도중 `<script>` 태그가 발견되면 브라우저는 HTML 파싱을 중단하고, 자바스크립트를 다운로드하고 실행)
4. DOM과 CSSOM을 조합하여 **렌더 트리**를 구축
5. Layout(Reflow): 뷰포트 기반으로 노드의 정확한 위치와 크기를 계산
6. Paint(Repaint): 모든 요소의 레이아웃이 결정되면, 텍스트, 색상, 그림자 등 스타일 속성에 따라 요소들을 화면에 렌더링

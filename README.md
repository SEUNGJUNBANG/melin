 # ✨ Portfolio Website

    반응형 웹사이트 제작
    기술 : HTML, CSS, JAVASCRIPT, JQUERY, Swiper Slide, GSAP
    프로그램 : 피그마, 비주얼스튜디오코드
    링크 : https://seungjunbang.github.io/melin/


---

## 🔍 Self Review

### 📁 1. 파일 구조 및 구성

- [x] 역할별로 디렉토리 분리 (`/css`, `/js`, `/images`)
- [x] 인라인 스타일, 스크립트 제거 → 외부 파일로 분리 완료
- [x] 파일/폴더 네이밍 일관성 유지

---

### 🧱 2. HTML 리뷰

```html
<div id="header"></div>
<div id="main">
<div id="smoother-wrapper">
<div id="smoother-content">

```
- [ ]  의미론적 태그를 적절히 사용이 부족함 (`<article>`, `<section>`, `<header>`, `<main>`, `<nav>` 등)
- `div id="main"` 의 `div`대신 `main`태그 사용이 필요함
- [ ]  heading 태그는 순차적으로 구조화 진행 (`<h1>` `<h2>` `<h3>` ..)
- [x] 모든 이미지에 `alt` 속성 적용
- [x] 폼 요소에 `label` 연결 완료
- [ ] `<h1>`이 여러 번 사용됨 → 하나만 사용하도록 구조 변경 예정
- [ ] 링크(<a>)안에 버튼(<button>) 태그 사용  a태그만 사용 예정

---

### 🎨 3. CSS 리뷰

- [x] 중복 스타일 최소화 및 공통 클래스 추출
- [x] 반응형 웹 완성 (미디어 쿼리 사용)
- [ ] 초기값, 공통된 요소 하나의 페이지에서 모두 작성 → reset.css, common.css분리하여 정리 예정

---

### ⚙️ 4. JavaScript 리뷰

```javascript
var $main_visual = $(".main_visual .main_slider");
var $visualList = $(".main_visual .main_slider .slide_box > div");
var $visual_length = $visualList.length;
var _visualNum = 0;

```
- $(function () {
            var swiper = new Swiper(".content-Swiper", {
                slidesPerView: 5.2,
                spaceBetween: 16,
                pagination: {
                    el: ".swiper-pagination",
                    clickable: true,
- [x] 자바스크립트와 제이쿼리 구분을 위해 변수명 앞에 $ 추가함
- [x] 메뉴 토글, 스크롤 애니메이션 등 기능 구현 완료
- [ ] 함수 네이밍 일부 추상적 (예: `handle1()`) → 의미 있는 이름으로 리팩토링 예정
- [x] 코드 모듈화 완료 (기능별 함수 분리)
- [ ] 반복되는 선택자 변수화 필요 및 on('change') 사용 권장
```javascript

```
- 
---


### 🎯 5. UX/UI 측면

- [x] 인터랙션 요소에 호버 및 포커스 스타일 제공
- [x] 모바일 환경에서 메뉴가 터치로 작동함
- [x] 디자인 시각적 계층 구조 명확함
- [ ] PPL과 영상 보러갈 수 있도록 링크 추가

---

## 🛠️ 개선 계획 (To-Do)

- [ ] <h1> 태그 구조 개선 → SEO 및 접근성 향상
- [ ] JavaScript 함수명 구체화 (handle1() → toggleMenu() 등)
- [ ] 로딩 애니메이션 추가하여 UX 개선
- [ ] 불필요한 webfont 파일 정리
- [ ] 의미론적 태그로 구조 재구성 (<main>, <section> 등)
- [ ] reset.css, common.css 분리 적용
- [ ] 콘텐츠 영역에 실제 영상, 링크 추가
- [ ] 반복되는 jQuery 선택자 변수화 처리


---

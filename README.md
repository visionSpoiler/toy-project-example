# toy-project-example

HTML / CSS / JavaScript 로 진행하는 토이 프로젝트 예제 저장소입니다.

## 구조

```
.
├── .gitignore
├── README.md
├── index.html
├── css/
│   ├── main.css
│   └── components.css   (선택)
├── js/
│   ├── main.js
│   ├── app.js           (선택)
│   └── utils.js         (선택)
├── assets/
│   ├── images/
│   ├── fonts/
│   └── icons/
└── scripts/             (선택)
```

## 폴더별 사용법

### 루트
- `index.html` : 진입점. 필요하면 페이지가 여러 개일 때 `pages/` 또는 루트에 추가.
- `.gitignore` : node_modules, 환경변수, OS/IDE 파일 등 저장소에 올리면 안 되는 것 제외.
- `README.md` : 프로젝트 설명, 실행 방법, 의사결정 메모.

### css/
- 전역/베이스 스타일은 `main.css` 에.
- 컴포넌트별 스타일은 별도 파일(`components.css` 등)로 분리.
- 변수는 `:root` 에 미리 정의해두면 나중에 테마/리팩토링이 쉬움.

### js/
- `main.js` : 초기화/진입점. DOMContentLoaded 이후 앱 시작.
- `app.js` : 핵심 로직.
- `utils.js` : 자주 쓰는 헬퍼 함수.
- 규모가 커지면 기능 단위로 파일을 나누고, 필요하면 모듈 방식(타입스크립트 없이 ES 모듈)으로 전환 가능.

### assets/
- 이미지, 폰트, 아이콘 등 정적 자원을 넣는다.
- 이미지는 `images/`, 아이콘은 `icons/` 처럼 용도별로 나눠두면 찾기 쉽다.

### scripts/ (선택)
- 배포나 생성 보조 스크립트(빌드, 압축, 이미지 리사이징 등)를 넣을 수 있다.
- 토이 프로젝트 초기에는 거의 안 쓸 수 있으니 비워둬도 된다.

## 실행 방법

브라우저에서 `index.html` 을 열면 바로 확인할 수 있습니다.

로컬 서버로 열고 싶으면 아무 HTTP 서버나 사용하면 됩니다.

```bash
# 예: Python
python3 -m http.server 8000
```

## 다음 단계

1. `index.html` 에 필요한 마크업 추가
2. `css/main.css` 에 스타일 추가
3. `js/main.js` 에서 기능 구현
4. 필요하면 컴포넌트/기능별로 파일 분할

---

이 저장소는 EXAMPLE 용으로 만든 템플릿입니다. 필요하면 구조를 그대로 가져다 쓰고, 불필요한 폴더는 삭제/축소해도 됩니다.

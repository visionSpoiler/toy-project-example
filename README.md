# toy-project-example

HTML / CSS / JavaScript 로 진행하는 토이 프로젝트 예제 저장소입니다.

## 구조

```
.
├── .gitignore
├── README.md
├── index.html
├── css/
│   └── main.css
├── js/
│   └── main.js
├── assets/
│   └── images/
└── notes/
    ├── README.md
    └── index.md
```

## 폴더별 사용법

### 루트
- `index.html` : 진입점.
- `.gitignore` : node_modules, 환경변수, OS/IDE 파일 등 제외.
- `README.md` : 프로젝트 설명, 실행 방법.

### css/
- 전역/베이스 스타일은 `main.css` 에.

### js/
- `main.js` : 초기화/진입점.

### assets/
- 이미지, 폰트, 아이콘 등 정적 자원.

### notes/
- 프로젝트를 진행하면서 배운 것을 정리하는 학습 노트 전용 폴더입니다.
- 영역(서비스/개발/데이터)을 폴더로 나누지 않고, 필요하면 노트 파일 안에서 섬션으로만 구분합니다.
- 새 노트를 추가하는 방법은 `notes/README.md` 참고.

## 실행 방법

브라우저에서 `index.html` 을 열면 바로 확인할 수 있습니다.

```bash
python3 -m http.server 8000
```

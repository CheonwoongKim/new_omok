# 오목 게임 (New Omok)

간단하고 직관적인 웹 기반 오목 게임입니다.

## 🎮 게임 특징

- **반응형 디자인**: 모바일과 데스크톱 모두 지원
- **실시간 게임**: 두 플레이어가 번갈아 가며 진행
- **승부 판정**: 5개 연속으로 놓으면 승리
- **게임 초기화**: 새 게임 시작 버튼

## 🚀 배포 방법

### Cloudflare Pages로 배포

1. **Cloudflare Dashboard**에서 Pages 프로젝트 생성
2. GitHub 저장소 연결
3. 배포 설정:
   - **Framework preset**: None
   - **Build command**: 비워두기
   - **Build output directory**: `/`

### 로컬 실행

```bash
# 간단한 HTTP 서버로 실행
python -m http.server 8000
# 또는
npx serve .
```

브라우저에서 `http://localhost:8000`으로 접속

## 📁 프로젝트 구조

```
new_omok/
├── index.html          # 메인 게임 파일
├── _headers           # Cloudflare Pages 보안 설정
├── prd.md            # 프로젝트 요구사항
├── superdesign/      # 디자인 파일들
└── README.md         # 이 파일
```

## 🎯 게임 규칙

1. 흑돌부터 시작
2. 번갈아 가며 돌 놓기
3. 가로, 세로, 대각선으로 5개 연속이면 승리
4. 게임 종료 후 "새 게임" 버튼으로 재시작

## 🔧 기술 스택

- **HTML5** & **CSS3**
- **Vanilla JavaScript**
- **Tailwind CSS** (CDN)
- **Cloudflare Pages** (배포)

---

🤖 Generated with [Claude Code](https://claude.ai/code)
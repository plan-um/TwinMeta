# WARP.md

이 파일은 WARP (warp.dev)가 이 저장소에서 코드를 작업할 때 참고할 가이드를 제공합니다.

## 프로젝트 개요

**TwinMeta 사용자 시나리오 흐름도** 프로젝트는 Web3 커뮤니티 플랫폼 TwinMeta의 사용자 여정을 시각화하는 정적 웹사이트입니다. 다크 테마 UI와 반응형 디자인을 통해 6가지 주요 사용자 시나리오를 설명합니다.

## 아키텍처

### 핵심 기술 스택
- **HTML5** 시맨틱 마크업
- **Tailwind CSS** 유틸리티 기반 스타일링
- **Noto Sans KR** 한글 웹폰트
- **GitHub Pages** 정적 사이트 호스팅

### 디자인 시스템
- **다크 테마**: 메인 배경 `#0A0F1C`, 카드 배경 `#1A2035`
- **컬러 팔레트**: 시나리오 그룹별 구분 색상 (cyan, fuchsia, emerald, yellow, rose, blue)
- **타이포그래피**: Noto Sans KR 폰트 패밀리
- **레이아웃**: 컨테이너 기반 반응형 그리드

### 주요 컴포넌트
- **시나리오 카드**: 각 사용자 여정을 담는 컨테이너
- **플로우 스텝**: 타임라인 형태의 단계별 시각화
- **코드 하이라이트**: 페이지 코드 참조를 위한 인라인 스타일

## Development Commands

### Setup & Local Development
```bash
# 로컬에서 파일 열기
open user_scenarios.html

# 또는 간단한 HTTP 서버 실행 (Python)
python3 -m http.server 8000

# Node.js의 경우
npx http-server
```

### GitHub Pages 배포
```bash
# Git 초기화 (최초 1회)
git init

# 파일 추가
git add .

# 커밋
git commit -m "Initial commit: TwinMeta user scenarios"

# GitHub 원격 저장소 연결
git remote add origin https://github.com/USERNAME/REPOSITORY.git

# 메인 브랜치 푸시
git push -u origin main
```

### 콘텐츠 업데이트
```bash
# 변경사항 확인
git status

# 파일 스테이징
git add user_scenarios.html

# 커밋
git commit -m "Update scenario content"

# 배포
git push origin main
```

## 파일 구조

### 메인 파일
- `user_scenarios.html`: 메인 시나리오 흐름도 페이지
- `WARP.md`: 프로젝트 가이드 (현재 파일)
- `README.md`: 프로젝트 설명서

### 콘텐츠 구조
```
TwinMeta/
├── user_scenarios.html    # 메인 페이지
├── WARP.md               # Warp 가이드
├── README.md             # 프로젝트 문서
└── .gitignore           # Git 무시 파일
```

## 시나리오 그룹 구성

### 그룹 1: 신규 방문 및 가입 (Cyan)
- 1-1. 서비스 가치 인지 및 회원가입
- 1-2. 기존 회원 로그인

### 그룹 2: 프로젝트 탐색 및 참여 (Fuchsia)
- 2-1. 얼리버드 참여
- 2-2. NFT 구매

### 그룹 3: NFT 및 활동 관리 (Emerald)
- 3-1. NFT 확인 및 실물 인증
- 3-2. 활동 내역 및 포인트 확인

### 그룹 4: 트윈코드 활용 (Yellow)
- 4-1. 실물 티셔츠 스캔 및 포인트 획득

### 그룹 5: 수익 창출 및 관리 (Rose)
- 5-1. 트윈커의 프로젝트 생성
- 5-2. TD의 프로젝트 참여 및 수익화

### 그룹 6: 커뮤니티 기여 및 확산 (Blue)
- 6-1. 레퍼럴 보상 시스템

## 스타일 가이드

### CSS 클래스 네이밍
- `.scenario-card`: 시나리오 컨테이너
- `.flow-step`: 플로우 단계 요소
- `code`: 인라인 코드 참조

### 컬러 시스템
```css
:root {
  --bg-primary: #0A0F1C;      /* 메인 배경 */
  --bg-secondary: #1A2035;     /* 카드 배경 */
  --border: #2A314E;           /* 테두리 */
  --accent: #00D4FF;           /* 강조색 */
  --text-primary: #E0E0E0;     /* 주요 텍스트 */
  --text-secondary: #9CA3AF;   /* 보조 텍스트 */
}
```

### 반응형 브레이크포인트
- **Mobile**: 기본 (320px+)
- **Tablet**: md (768px+)
- **Desktop**: lg (1024px+)
- **Wide**: xl (1280px+)

## GitHub Pages 설정

### 저장소 설정
1. GitHub에서 새 public 저장소 생성
2. Settings > Pages에서 Source를 "Deploy from a branch" 선택
3. Branch를 "main"으로 설정
4. 루트 폴더 `/` 선택

### 커스텀 도메인 (선택사항)
```
# CNAME 파일 생성
echo "your-domain.com" > CNAME
git add CNAME
git commit -m "Add custom domain"
git push origin main
```

## 사용자 경험 최적화

### 성능
- **폰트 최적화**: Google Fonts preconnect 사용
- **CSS 최적화**: Tailwind CSS CDN 활용
- **이미지 최적화**: 현재 아이콘만 사용 (이모지)

### 접근성
- **시맨틱 HTML**: 적절한 heading 구조
- **컬러 대비**: WCAG AA 준수 색상 조합
- **키보드 네비게이션**: 포커스 관리

### SEO
```html
<meta name="description" content="TwinMeta Web3 커뮤니티 플랫폼의 사용자 시나리오 흐름도">
<meta name="keywords" content="TwinMeta, Web3, NFT, 사용자여정, UX">
<meta property="og:title" content="트윈메타 사용자 시나리오 흐름도">
```

## 업데이트 가이드

### 콘텐츠 수정 시
1. `user_scenarios.html` 파일 직접 편집
2. 브라우저에서 로컬 확인
3. Git 커밋 후 푸시하여 GitHub Pages 자동 배포

### 새로운 시나리오 추가 시
1. 기존 구조를 복사하여 새로운 시나리오 그룹 생성
2. 적절한 색상 클래스 적용 (border-COLOR-400)
3. flow-step 구조로 단계별 내용 구성

### 스타일 변경 시
1. Tailwind CSS 클래스 활용 권장
2. 커스텀 CSS는 `<style>` 태그 내부에 추가
3. 반응형 고려하여 모든 디바이스에서 테스트

## 배포 자동화

GitHub Actions를 통한 자동 배포는 이미 GitHub Pages에서 기본 제공되므로 별도 설정 불필요. `main` 브랜치로 푸시하면 자동으로 사이트가 업데이트됩니다.
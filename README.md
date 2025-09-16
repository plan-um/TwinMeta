# TwinMeta 사용자 시나리오 흐름도

![TwinMeta Logo](https://img.shields.io/badge/TwinMeta-Web3%20Community-00D4FF?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-327FC7.svg?style=for-the-badge&logo=github&logoColor=white)

## 📖 프로젝트 소개

**TwinMeta 사용자 시나리오 흐름도**는 Web3 커뮤니티 플랫폼 TwinMeta의 사용자 여정을 시각적으로 설명하는 인터랙티브 웹사이트입니다. 

현실과 가상을 연결하는 TwinMeta 플랫폼의 6가지 핵심 사용자 시나리오를 단계별로 상세히 제시하여, 서비스의 전체적인 사용자 경험을 이해할 수 있도록 구성되었습니다.

## 🌟 주요 특징

- **📱 반응형 디자인**: 모든 디바이스에서 최적화된 사용자 경험
- **🎨 다크 테마 UI**: 현대적이고 세련된 인터페이스 디자인
- **🔄 플로우 시각화**: 타임라인 형태로 사용자 여정을 직관적으로 표현
- **🎯 시나리오별 색상 구분**: 6개 그룹을 색상으로 명확히 구분
- **📖 상세한 설명**: 각 단계별 구체적인 행동과 결과 제시

## 🛠️ 기술 스택

- **Frontend**: HTML5, Tailwind CSS, JavaScript
- **Font**: Noto Sans KR (한글 최적화)
- **Hosting**: GitHub Pages
- **Design**: 다크 테마, 컴포넌트 기반 디자인

## 📋 시나리오 구성

### 🔷 그룹 1: 신규 방문 및 가입
- **1-1**: 서비스의 가치를 처음 접하고 회원가입까지 완료
- **1-2**: 기존 회원이 다시 방문하여 로그인

### 🔶 그룹 2: 프로젝트 탐색 및 참여 (일반 사용자)
- **2-1**: 마음에 드는 프로젝트를 발견하고 '얼리버드'에 참여
- **2-2**: 얼리버드 참여 후, NFT를 구매

### 🟢 그룹 3: NFT 및 활동 관리 (보유자)
- **3-1**: 구매한 NFT를 확인하고 실물을 인증
- **3-2**: 자신의 활동 내역과 포인트를 확인

### 🟡 그룹 4: 트윈코드 활용
- **4-1**: 다른 사용자의 실물 티셔츠를 스캔하고 포인트를 획득

### 🔴 그룹 5: 수익 창출 및 관리 (트윈커 & TD)
- **5-1**: 크리에이터(트윈커)가 새로운 프로젝트를 생성
- **5-2**: 디자이너(TD)가 프로젝트에 참여하고 수익 옵션을 설정

### 🔵 그룹 6: 커뮤니티 기여 및 확산
- **6-1**: 친구를 초대하여 레퍼럴 보상을 받기

## 🚀 로컬 개발 환경 설정

### 1. 저장소 클론
```bash
git clone https://github.com/YOUR_USERNAME/TwinMeta-User-Scenarios.git
cd TwinMeta-User-Scenarios
```

### 2. 로컬에서 실행
```bash
# 브라우저에서 바로 열기
open user_scenarios.html

# 또는 HTTP 서버 실행
python3 -m http.server 8000
# 브라우저에서 http://localhost:8000 접속
```

## 📦 배포

이 프로젝트는 GitHub Pages를 통해 자동 배포됩니다.

### GitHub Pages 설정
1. GitHub에서 저장소 생성 (Public)
2. **Settings** > **Pages**로 이동
3. Source: **Deploy from a branch**
4. Branch: **main** 선택
5. Folder: **/ (root)** 선택

### 배포 명령어
```bash
git add .
git commit -m "Update user scenarios"
git push origin main
```

## 🎨 디자인 시스템

### 컬러 팔레트
```css
/* 메인 컬러 */
--bg-primary: #0A0F1C;      /* 다크 배경 */
--bg-secondary: #1A2035;    /* 카드 배경 */
--border: #2A314E;          /* 테두리 */
--accent: #00D4FF;          /* 강조색 (사이언) */

/* 시나리오 그룹별 컬러 */
--cyan: #22D3EE;           /* 그룹 1 */
--fuchsia: #E879F9;        /* 그룹 2 */  
--emerald: #34D399;        /* 그룹 3 */
--yellow: #FDE047;         /* 그룹 4 */
--rose: #FB7185;           /* 그룹 5 */
--blue: #60A5FA;           /* 그룹 6 */
```

### 반응형 브레이크포인트
- **모바일**: 기본 (320px+)
- **태블릿**: 768px+
- **데스크톱**: 1024px+
- **와이드**: 1280px+

## 📱 모바일 최적화

- 터치 친화적인 인터페이스
- 스와이프 제스처 지원
- 모바일 우선 반응형 디자인
- 최소 44px 터치 영역 보장

## ♿ 접근성

- **WCAG 2.1 AA 준수**: 색상 대비 비율 4.5:1 이상
- **시맨틱 HTML**: 스크린 리더 호환성
- **키보드 네비게이션**: Tab 키를 통한 순차 접근
- **포커스 관리**: 명확한 포커스 표시

## 🔧 커스터마이징

### 새로운 시나리오 추가
1. 기존 시나리오 카드 구조 복사
2. 새로운 색상 클래스 적용
3. `flow-step` 구조로 단계 구성

### 스타일 수정
1. Tailwind CSS 클래스 활용 권장
2. 커스텀 CSS는 `<style>` 태그에 추가
3. 모든 디바이스에서 테스트 필수

## 📈 성능 최적화

- **폰트 최적화**: Google Fonts preconnect 활용
- **CSS 최적화**: Tailwind CSS CDN 사용
- **이미지 최적화**: 이모지 아이콘으로 경량화
- **로딩 최적화**: 최소한의 JavaScript 사용

## 🤝 기여하기

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 라이선스

이 프로젝트는 MIT 라이선스를 따릅니다. 자세한 내용은 [LICENSE](LICENSE) 파일을 확인해주세요.

## 📞 연락처

프로젝트에 대한 질문이나 제안사항이 있으시면 언제든 연락주세요.

- **이메일**: your.email@example.com
- **GitHub**: [@yourusername](https://github.com/yourusername)

---

<div align="center">

**🔮 TwinMeta - 현실과 가상을 연결하는 Web3 커뮤니티 플랫폼**

Made with ❤️ by [Your Name](https://github.com/yourusername)

</div>
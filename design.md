# 김에디터 포트폴리오 웹사이트 디자인 가이드 (Design System & Specs)

## 1. 컨셉 & 톤앤매너 (Concept & Mood)
- **에디토리얼 테크 (Editorial-Tech):** 종이 매거진의 정제된 타이포그래피 품격과 실리콘밸리 테크 프로덕트의 현대적이고 기능적인 UI의 조화.
- **키워드:** `Precision (정확함)`, `Warmth (온기)`, `Density (밀도)`, `Clarity (명료함)`.
- **디자인 모드:** 다크 모드(기본) & 라이트 모드 토글 지원 (사용자 OS 테마 감지 및 로컬 스토리지 저장).

## 2. 컬러 시스템 (Color Palette)

### [Dark Mode (Default)]
- **Background Primary:** `#0d1117` (Deep Obsidian Charcoal)
- **Background Secondary / Surface:** `#161b22` / `#1c2128` (Subtle Elevated Surface)
- **Text Primary:** `#f0f6fc` (Soft High-Contrast Off-White)
- **Text Secondary / Muted:** `#8b949e` / `#6e7681` (Refined Slate Gray)
- **Accent Primary (Editorial Amber):** `#f59e0b` / `#fbbf24` (따뜻한 지적 에너지)
- **Accent Secondary (Teal Cyan):** `#06b6d4` (데이터 & 디지털 감각)
- **Border / Divider:** `rgba(255, 255, 255, 0.08)`
- **Glassmorphism:** `background: rgba(22, 27, 34, 0.75); backdrop-filter: blur(12px);`

### [Light Mode]
- **Background Primary:** `#f8fafc` (Warm Clean Paper Tone)
- **Background Secondary / Surface:** `#ffffff` (Pure Card Surface with Gentle Shadow)
- **Text Primary:** `#0f172a` (Deep Slate Black)
- **Text Secondary:** `#475569` (Charcoal Slate)
- **Accent Primary:** `#d97706` (Deep Warm Amber)
- **Border / Divider:** `rgba(15, 23, 42, 0.08)`

## 3. 타이포그래피 (Typography)
- **한글 본문 & UI:** `Pretendard`, -apple-system, BlinkMacSystemFont, system-ui, sans-serif
- **영문 헤더 & 포인트:** `Newsreader` / `Playfair Display` (클래식 저널리즘 감성)
- **코드 & 데이터 지표:** `JetBrains Mono`, `Fira Code`, monospace
- **행간(Line-height):** 본문 1.75~1.85 (완독성을 높이는 넉넉하고 편안한 줄 간격)

## 4. UI 컴포넌트 & 인터랙션 설계
1. **Global Navigation Bar (GNB):**
   - 상단 고정, 사파이어 & 오션 블루 글래스모피즘 (`#0f2a5e` / `#1d4ed8`) 적용
   - 실시간 읽기 진행률 표시 바 (Scroll Progress Bar)
   - 섹션 바로가기 네비게이션 및 다크/라이트 테마 스위처
   - 화이트 텍스트 및 스카이블루 액센트로 최적화된 시인성
   - 모바일 햄버거 메뉴 및 오버레이 드로어
2. **Hero Section:**
   - 임팩트 있는 타이포그래피와 상태 뱃지 ("🟢 Currently exploring new challenges")
   - 실시간 숫자 카운터 애니메이션 (경력 8년, 오픈율 42.8%, 온보딩 +28.4% 등)
   - 이메일 복사 원클릭 버튼 및 토스트 알림
3. **UX 라이팅 Before & After 인터랙티브 비교기:**
   - 탭 또는 슬라이더 방식으로 원본 문구와 개선 문구, 전환율 지표를 즉각 비교
4. **Editorial Process & Timeline:**
   - 6단계 워크플로우를 시각화한 대화형 인터랙티브 카드
5. **Interactive FAQ:**
   - 부드러운 아코디언 애니메이션
6. **동료 추천사 (Testimonials) 슬라이더 / 그리드:**
   - 신뢰감을 주는 인용구 카드 디자인
7. **Contact Drawer / Modal & Quick Copy:**
   - 즉시 커피챗을 신청할 수 있는 메일 링크 및 클립보드 복사 피드백

## 5. GitHub Pages 배포 고려사항
- 순수 정적 웹사이트 (Pure HTML5, CSS3, Vanilla JS ES6+)
- 모든 에셋 및 링크는 상대 경로 (`./`) 사용
- 외부 의존성은 신뢰할 수 있는 CDN (Google Fonts, Pretendard, FontAwesome/Lucide 아이콘)
- 별도 번들러/빌드 과정 없이 `git push` 즉시 동작

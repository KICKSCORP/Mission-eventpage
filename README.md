# KICKS Mission App

킥스 미션 애플리케이션 - 카페 방문 미션을 통한 리워드 시스템

## 📱 기능

- 프로필 입력 및 개인정보 동의
- 미션 안내 및 시작
- Kakao 지도 기반 네비게이션
- QR 코드 스캔
- 미션 완료 화면
- 리워드 쿠폰 교환

## 🚀 배포

Vercel을 통해 배포됩니다.

### 로고 및 아이콘 변경 방법

#### 1. KICKS 로고 변경
`index.html`의 Screen 1에서:
```html
<!-- Line ~90 근처 -->
<svg width="180" height="80" viewBox="0 0 180 80" fill="none" xmlns="http://www.w3.org/2000/svg">
    <text x="90" y="55" font-family="Arial, sans-serif" font-size="48" font-weight="bold" fill="#E91E63" text-anchor="middle">Kicks</text>
</svg>
```
**변경 방법:**
- 이미지 사용: `<img src="./logo.png" alt="KICKS" style="width: 180px; height: 80px;">`
- 또는 로고 SVG로 교체

#### 2. 킥보드 아이콘 변경
진행 상황 바 위의 킥보드 아이콘 (🛴) 변경:
- Screen 3, 4, 6에서 찾아서 변경
- 다른 이모지 사용: `🎯`, `🚀`, `⚡` 등
- SVG 아이콘 사용 가능

#### 3. 로고 이미지 추가
로고 이미지를 사용하려면:
1. `public` 폴더 생성
2. 로고 이미지 파일 저장 (예: `logo.png`)
3. HTML에서 `./logo.png` 또는 `./public/logo.png`로 참조

## 📁 파일 구조

```
kicks-mission-vercel/
├── index.html          # 메인 애플리케이션
├── vercel.json         # Vercel 설정
├── public/
│   ├── logo.png        # KICKS 로고 (선택사항)
│   └── icon.png        # 기타 아이콘 (선택사항)
└── README.md           # 이 파일
```

## 🔧 로컬 테스트

브라우저에서 `index.html`을 열어 테스트할 수 있습니다.

## 📝 Vercel 배포 순서

1. GitHub에 저장소 생성
2. 파일 업로드
3. Vercel에서 GitHub 저장소 연결
4. 자동 배포

## 💡 커스터마이징 가능 부분

- **색상**: #E91E63 (핑크) → 다른 색상으로 변경
- **로고**: SVG 또는 이미지 파일로 교체
- **아이콘**: 이모지 또는 SVG 아이콘으로 변경
- **텍스트**: 한글 전체 수정 가능
- **카페 정보**: Screen 3의 카페 정보 수정

---

**마지막 수정일**: 2024년 12월 10일

# Portfolio

두 개의 포트폴리오가 동일한 GitHub 저장소에서 관리되며, Vercel에서 독립적으로 배포됩니다.

## 폴더 구조

```
portfolio/
├── company-a/           # 기존 회사용 포트폴리오
│   └── index.html
├── fnf/                 # F&F 지원용 포트폴리오 (여러 페이지 웹사이트)
│   ├── index.html       # 홈: 소개 · 경력 · 주요 프로젝트 · 기술 · 학력
│   ├── projects/        # 프로젝트별 상세 페이지 3개
│   ├── css/style.css
│   ├── assets/          # 그래프 이미지, 논문 PDF
│   └── vercel.json      # cleanUrls (/projects/vlm-qa)
└── README.md
```

## Vercel 배포 방법

### 기존 회사 포트폴리오

1. Vercel 계정에 로그인
2. "New Project" 버튼 클릭
3. 이 GitHub 저장소 연결
4. Project Settings에서 **Root Directory를 `company-a`로 설정**
5. Deploy

### F&F 포트폴리오

1. Vercel 계정에 로그인
2. "New Project" 버튼 클릭
3. 동일한 GitHub 저장소 연결
4. Project Settings에서 **Root Directory를 `fnf`로 설정**
5. Deploy

## 주요 특징

- 단일 GitHub 저장소 유지
- 각 포트폴리오는 독립적인 Vercel 프로젝트로 배포
- 각 폴더는 완전히 독립적으로 작동 (외부 의존성 없음)
- company-a는 단일 HTML(Base64 내장), fnf는 HTML/CSS/에셋 분리 구조 (폰트는 Pretendard CDN)

# Portfolio

두 개의 포트폴리오가 동일한 GitHub 저장소에서 관리되며, Vercel에서 독립적으로 배포됩니다.

## 폴더 구조

```
portfolio/
├── company-a/           # 기존 회사용 포트폴리오
│   └── index.html
├── fnf/                 # F&F 지원용 포트폴리오
│   └── index.html
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
- 모든 스타일과 이미지는 Base64 인코딩 또는 CDN을 통해 제공

# KDH PM TO-DO LIST

번역 프로젝트 관리를 위한 PM용 TO-DO LIST 앱입니다.

## 기능

- **전체 프로젝트**: 모든 프로젝트 목록 관리 (추가/수정/삭제)
- **납품일정**: 캘린더 형태로 납품 일정 확인
- **D-day 우선순위**: D-day 기준 정렬 및 드래그로 우선순위 변경

## 진행상황 자동 계산

- **착수**: 착수일이 오늘인 프로젝트
- **진행**: 착수일이 오늘이 아니고 최종납품일이 없는 프로젝트
- **납품**: 최종납품일이 입력된 프로젝트

## 로컬 개발

```bash
# 의존성 설치
npm install

# 개발 서버 실행
npm run dev

# 빌드
npm run build
```

## Netlify 배포 방법

### 방법 1: GitHub 연동
1. 이 프로젝트를 GitHub에 push
2. Netlify에서 "Add new site" → "Import an existing project"
3. GitHub 저장소 선택
4. 빌드 설정은 자동으로 감지됨 (netlify.toml)
5. "Deploy site" 클릭

### 방법 2: 수동 배포
1. `npm run build` 실행
2. Netlify에서 "Add new site" → "Deploy manually"
3. `dist` 폴더를 드래그 앤 드롭

### 방법 3: Netlify CLI
```bash
# Netlify CLI 설치
npm install -g netlify-cli

# 로그인
netlify login

# 배포
netlify deploy --prod
```

## 기술 스택

- React 18
- Vite
- Tailwind CSS
- Lucide React (아이콘)

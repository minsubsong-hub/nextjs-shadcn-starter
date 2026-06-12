# Next.js Shadcn Starter

Next.js 15 + TypeScript + Tailwind CSS + shadcn/ui 기반 스타터킷

## 기술 스택

| 기술 | 용도 |
|------|------|
| Next.js 15 | 프레임워크 (App Router) |
| TypeScript | 타입 안전성 |
| Tailwind CSS | 스타일링 |
| shadcn/ui | UI 컴포넌트 |
| Zustand | 전역 상태관리 |
| React Hook Form + Zod | 폼 검증 |
| next-themes | 다크모드 |

## 시작하기

```bash
# 의존성 설치
npm install

# 개발 서버 실행
npm run dev
```

브라우저에서 [http://localhost:3000](http://localhost:3000) 접속

## 예제 페이지

- `/` — 홈 (스타터킷 소개)
- `/examples/counter` — Zustand 카운터 예제
- `/examples/form` — React Hook Form + Zod 폼 예제

## 프로젝트 구조

```
src/
├── app/                   # Next.js App Router
│   ├── layout.tsx
│   ├── page.tsx
│   └── examples/
│       ├── counter/
│       └── form/
├── components/
│   ├── ui/                # shadcn/ui 컴포넌트
│   ├── common/            # 공통 컴포넌트
│   └── providers/         # Context Provider
├── lib/
│   ├── utils.ts           # cn() 유틸
│   └── schemas/           # Zod 스키마
├── stores/                # Zustand 스토어
└── types/                 # TypeScript 타입
```

## 새 컴포넌트 추가 (shadcn/ui)

```bash
npx shadcn@latest add [컴포넌트명]
# 예: npx shadcn@latest add table
```

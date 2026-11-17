# zetlabs

ZetLabs 공식 홈페이지 — [zetlabs.net](https://zetlabs.net)

Astro 정적 사이트. main push 시 GitHub Actions가 Cloudflare Pages(`zetlabs` 프로젝트)로 배포한다.

## 문서

> Notion 문서 추가 시 이곳에 인덱스를 유지한다.

- (없음)

## 개발

```bash
pnpm install
pnpm dev        # http://localhost:4321
pnpm build      # dist/ 빌드
```

## 배포

- Platform: Cloudflare Pages (Direct Upload)
- CI: GitHub Actions — `.github/workflows/deploy.yml`
- Secrets: `CLOUDFLARE_API_TOKEN` (Pages Edit), `CLOUDFLARE_ACCOUNT_ID`
- DNS: [cloudflare-dns](https://github.com/deuxksy/cloudflare-dns) — `zetlabs.net` CNAME → `zetlabs.pages.dev`

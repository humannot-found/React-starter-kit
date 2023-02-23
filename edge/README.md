# CDN edge endpoint

CDN edge endpoint powered by [Cloudflare Workers](https://workers.cloudflare.com/) that serves the front-end app.

## Directory Structure

`├──`[`dist`](./dist) — The compiled output<br>
`├──`[`global.d.ts`](./global.d.ts) — Global TypeScript declarations<br>
`├──`[`index.ts`](./index.tsx) — API entry point<br>
`├──`[`package.json`](./package.json) — The list of dependencies<br>
`├──`[`tsconfig.ts`](./tsconfig.json) — TypeScript configuration ([docs](https://www.typescriptlang.org/tsconfig))<br>
`├──`[`vite.config.ts`](./vite.config.ts) — JavaScript bundler configuration ([docs](https://vitejs.dev/config/))<br>
`└──`[`wrangler.toml`](./wrangler.toml) — Wrangler CLI configuration ([docs](https://developers.cloudflare.com/workers/wrangler/configuration/))<br>

## Getting Started

```
$ yarn workspace app build
$ yarn workspace edge build
$ yarn workspace edge deploy [--env #0]
```

## Scripts

- `build` — Build the app for production
- `test` — Run unit tests
- `coverage` — Run unit tests with enabled coverage report
- `deploy [--env #0]` — Deploy the app to Cloudflare (CDN)

## References

- https://hono.dev/ — JavaScript framework for CDN edge endpoints
- https://developers.cloudflare.com/workers/ — Cloudflare Workers docs
- https://www.typescriptlang.org/ — TypeScript reference
- https://vitejs.dev/ — Front-end tooling (bundler)
- https://vitest.dev/ — Unit test framework

### [Remix](https://remix.run/)

Focused on web standards and modern web app UX, you’re simply going to build better websites

### 記事
[一休レストランで Next.js App Router から Remix に乗り換えた話](https://user-first.ikyu.co.jp/entry/2023/12/15/093427)

- Next.js App Routerの課題：
   - History API の state を触れない
   - Cache-Control ヘッダを自由に設定できない
   - 継続的なアップデートに懸念

- Remixを採用する理由：
   - History APIの効果的な活用
   - Cache-Controlヘッダの柔軟な設定
   - 継続的なアップデート
      - メモリ使用量の削減
      - キャッシュ効率の向上
      - コンテナ起動時間の短縮

### Base of Remix
- Route
- Loader
- Action


### [quickstart](https://remix.run/docs/en/2.9.2/start/quickstart)
```
> npx create-remix@latest quickstart
Need to install the following packages:
create-remix@2.9.2
Ok to proceed? (y) y

npm warn deprecated inflight@1.0.6: This module is not supported, and leaks memory. Do not use it. Check out lru-cache if you want a good and tested way to coalesce async requests by a key value, which is much more comprehensive and powerful.
npm warn deprecated glob@7.2.3: Glob versions prior to v9 are no longer supported

 remix   v2.9.2 💿 Let's build a better website...
      ◼  Directory: Using quickstart as project directory

      ◼  Using basic template See https://remix.run/guides/templates for more
      ✔  Template copied

   git   Initialize a new git repository?
         No

  deps   Install dependencies with npm?
         Yes

      ✔  Dependencies installed

  done   That's it!

         Enter your project directory using cd ./quickstart
         Check out README.md for development and deploy instructions.

         Join the community at https://rmx.as/discord

> npm run build

vite v5.3.1 building for production...
✓ 84 modules transformed.
build/client/.vite/manifest.json                1.12 kB │ gzip:  0.32 kB
build/client/assets/root-BFUH26ow.css           5.36 kB │ gzip:  1.61 kB
build/client/assets/_index-B6hwyHK-.js          0.94 kB │ gzip:  0.40 kB
build/client/assets/root-Caf2gBYg.js            1.44 kB │ gzip:  0.84 kB
build/client/assets/jsx-runtime-56DGgGmo.js     8.11 kB │ gzip:  3.05 kB
build/client/assets/entry.client-_ocQGTuM.js   11.63 kB │ gzip:  4.09 kB
build/client/assets/components-hXNuMGC1.js    224.07 kB │ gzip: 72.46 kB
✓ built in 649ms
vite v5.3.1 building SSR bundle for production...
✓ 6 modules transformed.
build/server/.vite/manifest.json               0.22 kB
build/server/assets/server-build-BFUH26ow.css  5.36 kB
build/server/index.js                          7.19 kB
✓ built in 30ms

> npx remix-serve build/server/index.js
[remix-serve] http://localhost:3000 (http://192.168.11.9:3000)
GET / 200 - - 20.353 ms

```

### [remix tutorial](https://remix.run/docs/en/2.9.2/start/tutorial#remix-tutorial)

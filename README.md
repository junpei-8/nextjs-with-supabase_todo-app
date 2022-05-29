# Todo App（Next.js with Supabase）

講座 URL: https://www.udemy.com/course/nextjs-supabase-web-tailwindcss/learn/lecture/31686566

講座 Github: https://github.com/GomaGoma676/todo-app-supabase-nextjs

Notion レポート： https://www.notion.so/itnav/Nextjs-Supabase-Web-1db9ae02cb354fc0a1f687d3d8d2dda8

Notion レポート（このセクションのみ）： https://www.notion.so/itnav/Todo-App-SSG-CSF-e91ef986d99f44259910e7a7ef22e245

## 使い方

### env.local ファイルの追加

env.local ファイルを生成し、Supabase の情報を変数に代入する必要がある。

```env
NEXT_PUBLIC_SUPABASE_URL=[左タブの Settings > API ページから URL を確認できる]
NEXT_PUBLIC_SUPABASE_API_KEY=[左タブの Settings > API ページから Public key を確認できる]
```

### パッケージのインストール

パッケージライブラリに`pnpm`を使用することを個人的に推奨している。

```
pnpm install
```

### Dev サーバーの起動

すべて SSR としてサーブされるため、SSG や ISR の正確な挙動は確認できない。

```
pnpm dev
```

### Prod サーバーの起動

SSG や ISR の挙動を確認する場合は、こちらでないと正確な挙動を確認することができない。

```
pnpm build && pnpm start
```

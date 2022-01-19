## 概要
- ビンゴアプリケーション(https://bingo-app-lake.vercel.app/) で公開中。

## 使用技術
- TypeScript : 可能な限り型安全に開発を行えるようにするために採用しました。
- React Hooks (Next.js) : Hooks を利用して開発します。 Next.js の SSG により、パフォーマンスの指標となる lightScore の点数を向上させています。
- Chakra UI : 柔軟な記法ができる上に汎用性の高いコンポーネントを提供しているため採用しました。
- Jest : 各モジュールや Hooks などのビジネスロジックに関するテストを行うため採用しました。
- GitHub Actions : PR作成時に `yarn test` , `yarn lint` , `yarn build`　が通るか確認するために採用しました。
- Vercel : 手軽にSSGを行えるほか、PR 作成時にプレビューを確認できたり、main ブランチマージ時に自動的にデプロイ出来る機構を提供しているため採用しました。

## 使用方法
- `yarn dev` : Next.js を開発モードで実行します。
- `yarn start` :  Next.js の本番サーバーを起動します。
- `yarn build` : 本番用にビルドします。
- `yarn lint` : eslint と prettier の lint を走らせます。
- `yarn format` : eslint と prettier の formatを走らせます。
- `yarn test` : Jest によるテストを実行します。

## 感想
- 案外複雑なロジックだったがテストを書いて開発したため重いバグに直面することがなかった。
- Vercel や Next.js を個人で利用するのははじめてだったが特に躓くことがなく開発できた。
- 興味のあった技術を触ったり、開発フローを考えたりすることができたのでよいアウトプットにすることができた。

## 反省点
- データ構造をもう少し簡単にできたかもしれない。
- Figma でデザインを作成してから開発しようと考えていたが時間がなかったのでやめてしまった。

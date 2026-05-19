# プロジェクトルール

## 技術スタック
- React 18 + TypeScriptを使用
- Viteをビルドツールとして使用
- React Router v6でルーティング
- Vitest + React Testing Libraryでテスト

## コーディングスタイル
- 関数型コンポーネントのみ使用（クラスコンポーネントは禁止）
- TypeScriptの型定義を必ず使用
- JSX内での変数は `{}` で囲む
- propsはinterfaceで型定義

## コンポーネント構成
- コンポーネントは `src/components/` に配置
- ページコンポーネントは `src/pages/` に配置
- 共通のロジックや状態管理は Context API (`src/context/`) を使用

## 命名規則
- コンポーネントファイル：PascalCase (例: `ProductCard.tsx`)
- ユーティリティ・ヘルパー関数：camelCase (例: `formatPrice.ts`)
- 定数ファイル：UPPER_SNAKE_CASE (例: `API_ENDPOINTS.ts`)

## インポート順序
1. React関連
2. 第三者ライブラリ
3. 内部コンポーネント/モジュール

## テスト
- すべてのコンポーネントと重要な関数にテストを書く
- テストファイルは `__tests__` ディレクトリまたは `.test.tsx` / `.test.ts` サフィックス
- テストには `describe`, `it`, `expect` を使用

## スタイリング
- インラインスタイルは最小限に
- CSSは `App.css` または各コンポーネント専用のCSSファイルを使用

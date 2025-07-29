# Figma MCP 404ページテンプレート

このプロジェクトは、Figma MCP（Model Context Protocol）を活用して404ページのテンプレートを作成したWordPressブロックテーマです。

## 概要

Figmaのデザインファイルから直接コードを生成し、WordPressのブロックエディター（Gutenberg）に対応した404ページテンプレートを作成しました。

## WordPressブロックテーマのディレクトリ構造

```
figma-demo/
├── templates/           # テンプレートファイル
│   ├── index.html      # メインテンプレート
│   └── 404.html        # 404ページテンプレート
├── parts/              # テンプレートパーツ
│   ├── header.html     # ヘッダー
│   └── footer.html     # フッター
├── patterns/           # ブロックパターン
│   └── 404-error.php   # 404ページ用パターン
├── style.css           # テーマのスタイルシート
├── theme.json          # テーマ設定
└── README.md           # このファイル
```

## 作成されたファイル

### 1. `templates/404.html`
- WordPressのブロックエディター用の404ページテンプレート
- Figmaから取得したデザインを忠実に再現
- レスポンシブ対応
- テンプレートパーツ（header, footer）とパターンを使用

### 2. `patterns/404-error.php`
- 404ページ用のブロックパターン
- PHPを使用した国際化対応
- テンプレートタイプとして404を指定
- 再利用可能なコンポーネント

### 3. `style.css`
- 404ページ用のカスタムCSSスタイル
- Figmaのデザイン変数に基づいたスタイリング
- Noto Sans JPフォントの読み込み
- ホバーエフェクトとアニメーション

### 4. `theme.json`
- WordPressテーマの設定ファイル
- Figmaのカラーパレットとフォント設定を反映
- レイアウトサイズの最適化

## Figma MCPの活用

### 使用したツール
- `mcp_Figma_get_code`: Figmaデザインからコードを生成
- `mcp_Figma_get_image`: デザインの画像を取得
- `mcp_Figma_get_variable_defs`: デザイン変数を取得

### デザインソース
- Figma URL: https://www.figma.com/design/ifZ4OxnZnMP8Mg3ackxUZt/Amimoto-Website-Renewal?node-id=1113-24029&t=5lVXNPHso1J3NRXU-4
- ノードID: 1113:24029

## 特徴

### デザインの忠実性
- Figmaのデザインをそのままコードに変換
- 正確なカラー、フォント、スペーシングの再現
- レスポンシブデザイン対応

### WordPressブロックテーマ対応
- 正しいディレクトリ構造に従った配置
- テンプレートパーツの活用
- ブロックパターンの使用
- 国際化対応

### ユーザビリティ
- 404エラー時の適切なナビゲーション
- CTAセクションでのユーザーエンゲージメント向上
- アクセシビリティに配慮したデザイン

## 使用方法

1. このテーマをWordPressサイトにインストール
2. テーマを有効化
3. 存在しないURLにアクセスして404ページを確認
4. 必要に応じてカスタマイズ

## カスタマイズ

### カラーの変更
`theme.json`ファイルの`settings.color.palette`セクションを編集

### フォントの変更
`theme.json`ファイルの`settings.typography.fontFamilies`セクションを編集

### レイアウトの調整
`templates/404.html`または`patterns/404-error.php`を編集

## 技術仕様

- WordPress 6.8以上
- ブロックエディター（Gutenberg）対応
- PHP 7.4以上
- レスポンシブデザイン
- 国際化対応

## ライセンス

GNU General Public License v2 or later

## 作者

digitalcube 
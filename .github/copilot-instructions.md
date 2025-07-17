# Copilot Instructions for abc-storage.github.io

## プロジェクト概要
- 静的Webサイト（GitHub Pages運用）で、`asset/unity/`配下にUnity WebGLビルド成果物、`src/`配下にHTML・JS・CSSなどのWebリソースを配置。
- 英語・日本語のしりとりゲーム（`ultimate_shiritori`/`ultimate_shiritori_english`）やチャット機能（`src/chat.html`）など複数のWebアプリを同居。

## ディレクトリ構成と役割
- `asset/unity/ultimate_shiritori/`：日本語しりとりUnity WebGLビルド
- `asset/unity/ultimate_shiritori_english/`：英語しりとりUnity WebGLビルド
- `src/`：静的Webページ（`index.html`、`chat.html`、`english.html`）、共通JS（`script.js`）、CSS
- `src/TemplateData/`や`asset/unity/ultimate_shiritori/TemplateData/`：Unityビルドのテンプレート画像・スタイル

## コミットメッセージ規則
- `.github/instructions/test.instructions.md`および`.github/prompts/commit-message-rules.prompt.md`に従い、
  - `Fix: ...`（修正）
  - `Add: ...`（追加）
  - `Update: ...`（更新）
  - `Remove: ...`（削除）
  - `Refactor: ...`（リファクタリング）
  - `Other: ...`（その他）
- すべて日本語・簡潔明瞭に記述。

## 開発・運用のポイント
- Unityビルド成果物は`Build/`や`StreamingAssets/`配下に配置。不要なビルドファイルは定期的に削除。
- 静的HTML/JS/CSSは`src/`で管理。ページ追加時は`src/`にHTML・JS・CSSを配置。
- 外部依存は基本的に無し。UnityビルドやWeb標準技術のみ。
- テストやビルド自動化は特に導入されていない（2025年7月時点）。

## 例外・注意点
- Unityビルド成果物のパスやファイル名はビルドごとに変わる場合があるため、削除・追加時は慎重に。
- コミットメッセージ規則は必ず遵守。

---

### 参考ファイル
- `.github/instructions/test.instructions.md`：コミットメッセージ規則
- `.github/prompts/commit-message-rules.prompt.md`：コミットメッセージ規則
- `README.md`：プロジェクト概要
- `asset/unity/`、`src/`：主要な実装・リソース

---

不明点や例外があれば、既存コミットやディレクトリ構成を参照し、プロジェクトの一貫性を保つこと。

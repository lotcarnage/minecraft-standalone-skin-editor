# Minecraft Standalone Skin Editor

Copyright (c) 2026 lotcarnage

本リポジトリは、Minecraft 用スキンをブラウザ上で編集するための **スタンドアロン・スキンエディター** を開発・公開するものです。  
外部ライブラリやビルドツールに依存せず、単一の HTML ファイルとして動作することを前提に設計されています。

[Minecraft Standalone Skin Editorを使う](https://lotcarnage.github.io/minecraft-standalone-skin-editor/minecraft-standalone-skin-editor.html)

---

## 特徴

- ブラウザのみで動作するスタンドアロン構成
- ドット絵ツールとしての直感的な操作と作業性
- Minecraft スキン仕様に基づいた正確な編集機能
- 2D 編集と 3D 表示の両立
- ローカルストレージを用いた編集状態の保持
- 将来的な拡張を前提とした内部設計

---

## ドキュメント構成

本リポジトリでは、開発者向けドキュメントを明確に分離しています。  
実装に着手する前に、必ず以下の文書を一読してください。

### 開発者向けドキュメント

- **[SPECIFICATION.md](./docs/SPECIFICATION.md)**  
  本ツールの目的、機能仕様、設計上の前提条件をまとめた仕様書です。  
  実装はこの文書を正とします。

- **[REFACTORING_GUIDELINES.md](./docs/REFACTORING_GUIDELINES.md)**  
  命名、スコープ、コメント、構文などに関するリファクタリング方針をまとめたガイドラインです。  
  コードを修正する際の判断基準として使用してください。

---

## リポジトリ構成（概要）

```text
.
├─ skin_editor.html        # スキンエディター本体（スタンドアロンHTML）
├─ docs/
│  ├─ SPECIFICATION.md     # 仕様書（開発者向け）
│  └─ REFACTORING_GUIDELINES.md
└─ README.md
```

---

## 開発方針

本プロジェクトでは、以下の方針を採用しています。

- 初期設計と命名を最重要視する
- 動作を変えないリファクタリングを段階的に行う
- アドホックな修正や場当たり的最適化を避ける
- Git による履歴管理を前提とし、ファイル名にバージョン番号を含めない

これらの方針はすべて、`SPECIFICATION.md` および  
`REFACTORING_GUIDELINES.md` に明文化されています。

---

## ライセンス

本ソフトウェア（minecraft-standalone-skin-editor.html）は MIT ライセンスで提供します。

## 補足

Minecraftのスキン画像テンプレートファイルは[公式サイト](https://help.minecraft.net/hc/en-us/articles/4408894664461-Minecraft-Java-Edition-Skins)からダウンロードできます。

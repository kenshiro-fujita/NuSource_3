# CLAUDE.md - プロジェクト指示書

## プロジェクト概要

- **プロジェクト名**: Nu Source
- **概要**: Nulab主催の新規事業創出プログラム「Nu Source」への応募プロジェクト。「創造を易しく楽しくする」プロダクトを企画・開発する
- **プログラム**: [Nu Source](https://nusource.nulab.com/ja/) — プロトタイピングから事業化までを支援
- **開発者**: Fujita Kenshirou
- **開発手法**: BMAD-METHOD によるアジャイルAI駆動開発
- **応募締切**: 2026年3月13日（金）

## Nu Source プログラムについて

- Nulabのミッション「To make creating simple and enjoyable」に沿ったプロダクトが対象
- XR、Web、IoT、AI、Web3 などのテクノロジーを活用したサービス
- Backlog の 14,000+ チーム顧客基盤を活用した早期検証が可能
- 初期段階では事業計画書不要、プロダクトへの情熱を重視

## コミュニケーション

- 日本語でやりとりすること
- コミットメッセージ・PRタイトルは英語（conventional commits 形式）
- 敬語で返答する
- 体言止めは使わない
- カスタマイズ・設定変更の内容は都度ユーザーに確認すること
- 困ったら `/bmad-help` で次のステップを確認

## 開発フェーズ

```
0. アイデア出し → 1. リサーチ → 2. 分析・計画 → 3. 設計 → 4. 実装 → 5. 振り返り
```

- 現在はフェーズ 0（アイデア出し）から開始
- 実装前に未知の技術があれば必ずリサーチフェーズを挟む

## コミット規約

Conventional Commits 形式:

```
<type>(<scope>): <description>

[optional body]

Co-Authored-By: Claude Opus 4.6 <noreply@anthropic.com>
```

**type**: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`, `ci`

## ブランチ戦略

- `main` — メインブランチ（直接pushしない）
- `feature/<説明>` — 新機能・新プロダクト
- `fix/<説明>` — バグ修正
- `chore/<説明>` — メンテナンス作業

## ファイル構成

```
NuSource_3/
├── .claude/                  # Claude Code 設定
│   └── commands/             # BMAD コマンド
├── _bmad/                    # BMAD フレームワーク
├── _bmad-output/             # BMAD 成果物
│   ├── planning-artifacts/   # 計画フェーズの成果物
│   └── implementation-artifacts/ # 実装フェーズの成果物
├── docs/                     # ドキュメント・リサーチ資料
├── .claudeignore             # Claude 除外設定
└── CLAUDE.md                 # このファイル
```

# my-skills-mng

自分用の Claude Code スキル / サブエージェント集。

## ディレクトリ構成

スキルは `skills/` 配下のバケットフォルダで整理されています。

- [`engineering/`](skills/engineering/) — 日常のコード作業
- [`productivity/`](skills/productivity/README.md) — 日常のコード以外のワークフローツール
- [`misc/`](skills/misc/) — 残してはあるが、ほとんど使わないもの
- `personal/` — 自分自身のセットアップに紐づくもの、公開対象外（README には載せない）
- `in-progress/` — まだリリース準備が整っていないドラフト（README には載せない）
- `deprecated/` — もう使われていないもの（README には載せない）

サブエージェントは `agents/` 配下にフラットに配置されています。

## スキル一覧

### productivity

- [requirements-design-generator](skills/productivity/requirements-design-generator/SKILL.md) — 業務資料のディレクトリを分析し、要件定義書と設計書（初版）を Markdown で生成する。

### engineering

（未登録）

### misc

（未登録）

## サブエージェント一覧

- [business-document-analyzer](agents/business-document-analyzer.md) — 業務資料を読み、構造化サマリを返す専用 SubAgent。`requirements-design-generator` から並列起動される前提。

## 運用ルール

- `engineering/`、`productivity/`、`misc/` のスキルは、このトップレベル README と `.claude-plugin/plugin.json` の両方に登録する。
- `personal/`、`in-progress/`、`deprecated/` のスキルはどちらにも登録しない。
- 各スキルエントリは、スキル名を該当の `SKILL.md` へのリンクにする。
- 各バケットフォルダ直下にも README.md を置き、配下スキルを 1 行説明付きで列挙する。

  スキルは skills/ 配下のバケットフォルダで整理されています。
  
  - engineering/ — 日常のコード作業
  - productivity/ — 日常のコード以外のワークフローツール
  - misc/ — 残してはあるが、ほとんど使わないもの
  - personal/ — 自分自身のセットアップに紐づくもの、公開対象外
  - in-progress/ — まだリリース準備が整っていないドラフト
  - deprecated/ — もう使われていないもの

  engineering/、productivity/、misc/ にあるすべてのスキルは、トップレベルの README.md に参照を、そして .claude-plugin/plugin.json にエントリを持たせる必要があります。personal/、in-progress/、deprecated/
  にあるスキルは、これらのどちらにも記載してはいけません。

  トップレベルの README.md の各スキルエントリは、スキル名を該当の SKILL.md へリンクさせる必要があります。

  各フォルダには README.md があり、そのフォルダ内のすべてのスキルを1行の説明とともにリストし、スキル名は該当の SKILL.md へリンクされている必要があります。
# AI-Skills

各種AIエージェント（Claude Code、Codex など）で共通利用するスキルとコマンドを管理するリポジトリ。

## セットアップ

`skills/` と `commands/` を各AIエージェントのグローバル設定ディレクトリへシンボリックリンクすることで、全プロジェクトで使用できるようになる。

```sh
# Claude Code
ln -s /Users/kentosato/workspace/personal-tools/AI-skills/skills /Users/kentosato/.claude/skills
ln -s /Users/kentosato/workspace/personal-tools/AI-skills/commands /Users/kentosato/.claude/commands

# Codex
ln -s /Users/kentosato/workspace/personal-tools/AI-skills/skills /Users/kentosato/.codex/skills
ln -s /Users/kentosato/workspace/personal-tools/AI-skills/commands /Users/kentosato/.codex/commands
```

## プロジェクト固有のスキル

プロジェクト特有のスキルを作りたい場合は、そのプロジェクト配下の `.claude/skills/` ディレクトリに作成する。

## 注意事項

- `.claude/skills/.system` は Codex が自動作成するディレクトリのため、編集しない。git管理からも外す。

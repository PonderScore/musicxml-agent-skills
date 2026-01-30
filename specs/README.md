# 仕様リファレンス

このディレクトリには、MusicXMLとAgent Skillsの公式仕様がGit submoduleとして含まれています。

## 含まれる仕様

### MusicXML
- **ディレクトリ**: `musicxml/`
- **公式リポジトリ**: https://github.com/w3c/musicxml
- **公式サイト**: https://www.musicxml.com/
- **現行バージョン**: 4.0（W3C Community Group Final Report）
- **主要ファイル**:
  - `schema/musicxml.xsd` - XMLスキーマ定義
  - `docs/` - 仕様ドキュメント

MusicXMLは、楽譜データを交換するための標準オープンフォーマットです。
W3C Music Notation Community Groupが管理しています。

### Agent Skills
- **ディレクトリ**: `agent-skills/`
- **公式リポジトリ**: https://github.com/agentskills/agentskills
- **公式サイト**: https://agentskills.io/
- **仕様ドキュメント**: https://agentskills.io/specification
- **主要ファイル**:
  - `docs/specification.mdx` - 仕様ドキュメント

Agent SkillsはAIエージェントに新しい能力を与えるためのオープンフォーマットです。
Anthropicが開発し、Microsoft、OpenAI、GitHub等が採用しています。

## 仕様の更新方法

### 全てのsubmoduleを最新版に更新
```bash
git submodule update --remote
```

### 個別に更新
```bash
# MusicXMLのみ更新
git submodule update --remote specs/musicxml

# Agent Skillsのみ更新
git submodule update --remote specs/agent-skills
```

### 更新後のコミット
```bash
git add specs/
git commit -m "Update spec submodules to latest"
```

## 初回クローン時の注意

このリポジトリをクローンした際は、以下のコマンドでsubmoduleを初期化してください:

```bash
git submodule update --init --recursive
```

または、クローン時に `--recursive` フラグを使用:

```bash
git clone --recursive <repository-url>
```

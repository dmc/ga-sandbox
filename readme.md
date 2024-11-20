# GitHub Actions Test Repository

このリポジトリはGitHub Actionsの動作検証用のリポジトリです。各ブランチには異なるGitHub Actionsワークフローが配置され、それぞれのブランチで特定の機能やパターンを検証します。

## ブランチ構造

```
main
├── skip-if-no-changes     # 更新がない場合のスキップ機能検証
├── matrix-strategy        # マトリックスビルドの検証
├── custom-actions        # カスタムアクション作成検証
└── conditional-workflow  # 条件付きワークフロー検証
```

## ブランチ命名規則

- 機能検証用ブランチ: `feature/[検証内容]`
- バグ修正検証用ブランチ: `bugfix/[検証内容]`
- GitHub Actions検証用ブランチ: `actions/[検証内容]`

## ブランチごとのREADME構造

各ブランチのREADMEには以下の情報を含めます：

```markdown
# [検証名]

## 目的
このブランチで検証するGitHub Actionsの目的を記述

## 検証内容
具体的な検証項目や検証したい動作を記述

## ワークフロー
`.github/workflows/`に配置されているワークフローファイルの説明

## 使用方法
ワークフローのトリガー方法や必要な設定を記述

## 検証結果
検証結果や注意点を記述
```

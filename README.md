# GitHub Docs Sync

GitHub上のドキュメントやソースコードを取得し、Googleドライブへ自動保存するGoogle Colabノートブックです。

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1cmGI_kG3qd46SA0YjpBJa4GOwkaN-8mH#scrollTo=JHKmCFrZfIPe)

## 概要

指定したGitHubリポジトリ（または特定のサブディレクトリ）のデータを取得し、Google Driveに保存します。ローカル環境構築不要で、ブラウザのみで完結します。

**主な用途**
*   **AI用データ準備**: NotebookLM, Claude Projects, GPTs等のナレッジとして読み込ませるためのデータ収集。
*   **ドキュメント管理**: 公式ドキュメントやWikiページのアーカイブ、社内ナレッジの蓄積。

## ファイル
`github_docs_sync.ipynb`

## 使い方

1.  上の **[Open In Colab]** バッジをクリックしてノートブックを開きます。
2.  **設定フォーム**に必要事項を入力します。
    *   `repo_url`: 取得したいGitHubページのURL（特定のフォルダURLも可）
    *   `drive_folder`: 保存先のGoogleドライブフォルダ名
3.  左上の再生ボタン（▶）を押して実行します。
4.  Googleドライブへのアクセス許可を求められたら「接続」を選択してください。

## 特徴

*   **部分取得に対応**: リポジトリ全体だけでなく、必要なフォルダ（例: `/docs` のみ）だけを指定して高速に取得できます。
*   **履歴管理**: 保存フォルダには自動で「リポジトリ名_日時」の名前が付くため、過去のバージョンと混ざりません。
*   **一括処理**: 最大5つのURLを一度に処理可能です。

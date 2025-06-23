---
tags:
  - instructor-manual
  - evergreen
  - version-control
  - Phrases
last_modified: 2025-04-21
---
Key version‑control terms with Japanese equivalents.  
主要なバージョン管理用語と日本語訳。

| Term / 用語                    | Definition                                                                          | 定義                                         |
| ---------------------------- | ----------------------------------------------------------------------------------- | ------------------------------------------ |
| Repository (Repo)            | A database that stores all project files and their revision history.                | プロジェクトのファイルとその変更履歴を保存するデータベース。             |
| Commit                       | A snapshot of tracked files at a point in time, saved with a unique ID (SHA).       | 追跡対象ファイルの状態を記録するスナップショット。固有 ID（SHA）で識別される。 |
| Branch                       | A movable pointer to a series of commits, enabling parallel lines of development.   | 一連のコミットを指し示す可動ポインタで、並行開発を可能にする。            |
| Merge                        | Integrates changes from one branch into another.                                    | あるブランチの変更を別のブランチに統合する操作。                   |
| Merge Request / Pull Request | A request to merge code; includes diffs, reviews, and CI checks.                    | コード統合を依頼する仕組み。差分表示、レビュー、CI 検証を含む。          |
| Clone                        | Creates a full local copy of a remote repository.                                   | リモートリポジトリを完全に複製し、ローカルに作成する操作。              |
| Fork                         | Copies a repository to your own account, letting you propose changes independently. | リポジトリを自分のアカウントに複製し、独立して変更提案できるようにすること。     |
| Staging Area (Index)         | An intermediate area where changes are prepared before committing.                  | コミット前に変更を整理・選別する中間領域。                      |
| Remote                       | A reference to a repository hosted elsewhere (e.g., GitLab, GitHub).                | 別の場所（GitLab など）にあるリポジトリへの参照。               |
| Checkout                     | Switches the working directory to a specified commit or branch.                     | 作業ディレクトリを指定したコミットやブランチの状態に切り替える操作。         |
| Conflict                     | Occurs when incompatible changes touch the same lines during a merge/rebase.        | マージやリベースで同じ行が異なる変更を受け、Git が自動統合できない状態。     |

> [!action] Expand Glossary  
> To do: Add advanced VCS terms such as “cherry‑pick”, “rebase”, and “detached HEAD”, including EN definitions and JA translations.  
> cherry‑pick」「rebase」「detached HEAD」などの上級バージョン管理用語を、英語定義と日本語訳とともに追加しましょう。

#tags/glossary

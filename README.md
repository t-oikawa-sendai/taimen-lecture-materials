<!--
Program Name: Taimen Lecture Materials Root README
Language: Markdown
Function: 対面指導教材Repositoryの目的・対象・管理対象・管理方針を示す
Created: 2026-09-19
Last Updated: 2026-09-20
Author: Takashi Oikawa
AI: Cursor Grok 4.6
Memo: Repository基盤の初期README。教材本編は含まない
-->

# taimen-lecture-materials（対面指導教材）

<!-- Document Info（文書情報） -->
| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | TLM-README-001 |
| Version（バージョン） | 0.2 |
| Status（ステータス） | Draft |
| Created Date（作成日） | 2026-09-19 |
| Last Updated（最終更新日） | 2026-09-20 |
| Owner（管理者） | Takashi Oikawa |
| Related Documents（関連文書） | project-notes/CURRENT.md / project-notes/DECISIONS.md |

---

## Purpose（目的）

職業訓練校で実施する対面指導用教材を一元管理するRepository。
個別に作成した場合の整合性の問題、バージョン管理の問題を回避することを主たる目的とする。
カリキュラムを意識しながら不足、補足教材の制作を管理する。

## Target（対象）

IT初学者向けの対面指導教材。

ただし、「初心者向けだから専門用語を使用しない」という方針にはしない。

実務で使用される専門用語は必要に応じて使用し、初出時に簡潔な説明を加える。

## Managed Targets（管理対象）

- DB設計
- コード設計
- AIセットアップ
- 今後追加される対面指導テーマ

## Management Policy（管理方針）

- 教材テーマごとにRepositoryを増やさない
- テーマ単位でdirectoryを分離する
- 確定事項はGitHub側の文書を正本とする
- AIとの会話のみを正本にしない
- 現在地点は `project-notes/CURRENT.md`
- 重要な設計判断は `project-notes/DECISIONS.md` または個別Decision文書に記録する

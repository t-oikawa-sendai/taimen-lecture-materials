<!--
Program Name: Taimen Lecture Materials DECISIONS
Language: Markdown
Function: 対面指導教材Repositoryの確定済みDecisionを記録する
Created: 2026-09-19
Last Updated: 2026-09-20
Author: Takashi Oikawa
AI: Cursor Grok 4.6
Memo: DecisionはD-001からD-005。教材本編は含まない。D-005はRepository Purpose = LEARNING
-->

# DECISIONS（決定事項）

<!-- Document Info（文書情報） -->
| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | TLM-DECISIONS-001 |
| Version（バージョン） | 0.2 |
| Status（ステータス） | Draft |
| Created Date（作成日） | 2026-09-19 |
| Last Updated（最終更新日） | 2026-09-20 |
| Owner（管理者） | Takashi Oikawa |
| Related Documents（関連文書） | README.md / project-notes/CURRENT.md |

---

## D-001 Management Unit of Face-to-face Lecture Materials（対面指導教材の管理単位）

Decision（決定）:
教材単位ではなく、対面指導全体を1Repositoryで管理する。

Repository（リポジトリ）:
`taimen-lecture-materials`

Reason（理由）:
DB設計、コード設計、AIセットアップ等が今後増えるため、テーマ単位でRepositoryを作ると管理対象が過度に分散する。

## D-002 Introduction of DB Design D1（DB設計D1の導入）

Decision（決定）:
受注データをExcelの1枚表で管理していた状態から開始する。

Problem Example（問題発生例）:
顧客住所変更時に検索・置換を行ったが、全角・半角等の表記揺れにより一部レコードの更新が漏れ、古い住所へ発送して荷物が返送される。

Important（重要）:
Excelを原因としない。原因は同じ情報を複数箇所に重複保持するデータ構造にある。

## D-003 Handling of DB Technical Terms（DB専門用語の扱い）

Decision（決定）:
DB専門用語の使用を禁止しない。

Candidate Terms（使用候補）:

- データベース
- テーブル
- カラム
- レコード
- マスタ
- トランザクションデータ
- 主キー
- 外部キー
- 正規化

Rule（規則）:
必要な用語を使用し、初出時のみ初心者向けの説明を付ける。

## D-004 Teaching Material Setting for Product Prices（商品価格の教材設定）

Decision（決定）:
販売時点ではメーカー希望価格と販売価格を同額とする。

その後メーカー希望価格が値上げされることで、現在の商品価格を過去の注文にもそのまま使用する設計の問題を示す。

Lecture Goal（講義上の到達点）:
現在値と取引時点の値は意味が異なり、保存場所・管理方法を分ける必要があることを理解させる。

## D-005 Set Repository Purpose to LEARNING（Repository Purpose を LEARNING とする）

Decision（決定）:
taimen-lecture-materials の Repository Purpose を LEARNING とする。

Rationale（根拠）:
職業訓練校の対面指導教材を管理するRepositoryであり、
DEVELOPMENT向け設計7文書を必須としない
LEARNING Document Profileを適用するため。

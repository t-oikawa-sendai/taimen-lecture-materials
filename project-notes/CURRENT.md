<!--
Program Name: Taimen Lecture Materials CURRENT
Language: Markdown
Function: 対面指導教材Repositoryの現在地点・完了事項・次作業・ブロッカーを記録する
Created: 2026-09-19
Last Updated: 2026-09-20
Author: Takashi Oikawa
AI: Cursor Grok 4.6
Memo: Purpose = LEARNING。D-005反映。Governance Profile整理中。教材本編シナリオは含まない
-->

# CURRENT（現在地点）

<!-- Document Info（文書情報） -->
| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | TLM-CURRENT-001 |
| Version（バージョン） | 0.2 |
| Status（ステータス） | Draft |
| Created Date（作成日） | 2026-09-19 |
| Last Updated（最終更新日） | 2026-09-20 |
| Owner（管理者） | Takashi Oikawa |
| Related Documents（関連文書） | README.md / CONSTITUTION.md / AGENTS.md / DECISIONS.md |

---

## Purpose（目的）

Purpose = LEARNING。職業訓練校の対面指導教材を管理する。

## Completed（完了）

- 対面指導教材を単一Repositoryで管理する方針を決定
- Repository名を `taimen-lecture-materials` に決定
- DB設計D1の導入ストーリーについて以下を決定
- DB設計D1で現在確定している内容
  - 最初の受注データはExcelの1枚表で管理していた設定とする
  - Excelそのものを問題原因とはしない
  - 問題の本質は、同じ意味のデータを複数箇所に重複保持しているデータ構造
  - 顧客住所変更時にExcelの検索・置換を使用する
  - 全角・半角などの表記揺れにより一部レコードが置換対象から漏れる
  - 古い住所が残り、そのデータを使用して発送した結果、荷物が返送される
  - 表記揺れについては講義中の補足事項として説明する
  - 「表記揺れを直せば解決」ではなく、データ構造そのものを問題として扱う
  - ここからDB設計へ移行する
  - DB専門用語は必要に応じて使用可能
  - テーブル、レコード、カラム、マスタ、主キー、外部キー、正規化などを禁止事項としない
  - 専門用語は初出時に初心者向けの短い説明を加える
  - 商品価格については販売時点ではメーカー希望価格 = 販売価格とする
  - 後日メーカー希望価格が値上げされたことで、現在の商品価格と販売時点の価格を同一視できない問題を発生させる
  - 最終的に「現在の値」と「取引時点の値」を分けて設計する必要性へつなげる
  - 消費税は今回のD1教材では扱わない

## Current（現在）

- Governance Profile 整理中。Repository Purpose を LEARNING として中央Governance SSOTへ整合させる（関連：D-005）
- DB設計 D1 対面指導教材の再設計中。

## Next（次作業）

- DB設計D1の講義シナリオを上記方針で全面再設計
- 生徒提示資料を新シナリオに合わせて再設計
- D1確定後、D2 / C1 / C2へ展開

## Blockers（ブロッカー）

- なし

## Related Decisions（関連判断）

- D-005
- D-001 / D-002 / D-003 / D-004

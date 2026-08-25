# paper-knock — 論文ノック

論文を毎日1本読む習慣のための台帳。**記録の本体は GitHub Issues(1論文=1 Issue)**で、mdファイルには索引と規約だけを置く。

## 読み方の2つの型

論文はすべて同じ深さで読まず、2つの型を使い分ける。

| 型 | 割合の目安 | 何をするか | ラベル |
|---|---|---|---|
| **ノック**(アブスト水準) | 8割 | 問題意識・手法・結果を自分の言葉で3行に書く。テーマの関心範囲を掴むのが目的 | `d: アブスト` |
| **精読** | 2割 | [a1da4/paper-survey](https://github.com/a1da4/paper-survey) の7セクション形式で書く。構成(各節の分量配分)まで把握し、テーマの土地勘と重要パートを掴むのが目的 | `d: 精読` |

ノックした論文は後から精読へ格上げできる(同じIssueの本文を7セクションへ拡張し、ラベルを付け替える)。

## 運用

- **ペース: 平日ノック2本+精読 週2本**。書くのは **自分の言葉で**(コピペしない)。問題意識は明文化して腑に落ちるまで書き、そのテーマにおいてその問題意識がクリティカルかを問う。
- 選書は自分の目で行う(alphaXiv・arXiv新着・curated list)。推薦機能に任せない。
- 読み始めに、書誌(`0. Paper`)を埋めたIssueを起票する。本文は読み手本人が書く。読み終えたらIssueをclose(closedでも追記できる)。
- 索引= [knocks.md](knocks.md)(番号・タイトル・Issueリンクの一覧のみ。本文はIssueにだけ書く)。索引と進捗表の更新はmainへの直コミットで行い、PRは使わない。
- **分担**: 読む・書くのは本人(green-caviar)。AIアシスタント(green-caviar-bot)が起票・書誌の検収・索引と進捗表の更新を担う。Issueコメントでの議論もこの2アカウントで行い、アイコンで発言者が区別できる。

## ラベル

接頭辞で系統を分ける。命名は小文字が既定(略語・固有表記のみ大文字)。必要になった時に追加する。

| 接頭辞 | 意味 | 例 |
|---|---|---|
| `c:` | 出典・会議 | `c: arXiv` |
| `t:` | トピック | `t: agent`・`t: LLM` |
| `y:` | 年 | `y: 2025` |
| `d:` | 読解深度 | `d: アブスト`・`d: 精読` |
| `zz:` | 補助 | `zz: survey` |

補助にラベル `😃favorite`(お気に入り)・`🤔???`(消化しきれていない)も使う。

## テンプレート

### ノック(`d: アブスト`)

```markdown
## 0. Paper

(書誌: タイトル・著者・venue/年・alphaXiv・arXiv)

## 問題意識

## 手法

## 結果

## 吟味

- クリティカルか:
- 手段として適切か:
- 答え切ったか:

```

### 精読(`d: 精読`・[a1da4/paper-survey](https://github.com/a1da4/paper-survey) 形式)

```markdown
## 0. Paper

(書誌: タイトル・著者・venue/年・alphaXiv・arXiv)

## 1. What is it?

## 2. What is amazing compared to previous works?

## 3. Where is the key to technologies and techniques?

## 4. How did evaluate it?

## 5. Is there a discussion?

## 6. Which paper should read next?

## 7. personal comment

```

## 目標と進捗

`t: agent`(LLMエージェント関連)を **100本、2026-10-25まで(2ヶ月)**。内訳の目安= ノック80本・精読20本。中間チェックポイント= 09-24 にノック40・精読10。

| 対象 | 本数 |
|---|---|
| t: agent | 0 / 100 |
| 総数 | 0(読み中 2) |

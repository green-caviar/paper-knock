# paper-knock — 論文ノック

論文を毎日少しずつ読むための台帳。**記録の本体は GitHub Issues**(1論文=1 Issue)。

## 2つの型

先輩の100本ノックのやり方に倣い、読み方を2段に分ける。

| 型 | 割合の目安 | 何をするか | ラベル |
|---|---|---|---|
| **ノック**(アブスト水準) | 8割 | 問題意識・手法・結果を自分の言葉で3行に書く。テーマの関心範囲を掴む | `d: アブスト` |
| **精読** | 2割 | [a1da4/paper-survey](https://github.com/a1da4/paper-survey) の7セクションで書く。**構成(各節の分量配分)まで把握**し、テーマの土地勘と重要パートを掴む | `d: 精読` |

ノックした論文を後から精読に格上げしてよい(同じIssueの本文を7セクションへ拡張し、ラベルを付け替える)。

## ルール

- **平日1日1本**。書くのは **自分の言葉で**(コピペしない)。問題意識は明文化して腑に落ちるまで — そのテーマにおいてその問題意識がクリティカルかを問う。
- 選書は自分の目で: alphaXiv・arXiv新着・curated list。おすすめ機能に任せない。
- 読み始めに書誌(`0. Paper`)入りのIssueを起票し、本文を本人が埋める。読み終えたらIssueをclose(closedでも追記できる)。
- ラベルは接頭辞で: **`c:`(出典・会議)/ `t:`(トピック)/ `y:`(年)/ `d:`(読解深度)**+補助(`zz: Survey`・`😃favorite`・`🤔???`)。必要になった時に追加する。
- 索引= [knocks.md](knocks.md)(番号・タイトル・Issueリンクの一覧のみ。本文はIssueにだけ書く)。索引と進捗表の更新はmainへ直コミット・PRは使わない。
- **議論はIssueのコメントで**: 本人の発言は green-caviar・AIアシスタント(Claude)の回答は **green-caviar-bot** が投稿し、アイコンで発言者が分かれる。索引の管理と起票もClaudeが担う。

## テンプレート

### ノック(`d: アブスト`)

```markdown
## 0. Paper

(書誌: タイトル・著者・venue/年・URL)

## 問題意識

## 手法

## 結果

```

### 精読(`d: 精読`・[a1da4/paper-survey](https://github.com/a1da4/paper-survey) 形式)

```markdown
## 0. Paper

(書誌: タイトル・著者・venue/年・URL)

## 1. What is it?

## 2. What is amazing compared to previous works?

## 3. Where is the key to technologies and techniques?

## 4. How did evaluate it?

## 5. Is there a discussion?

## 6. Which paper should read next?

## 7. personal comment

```

## 目標

- `t: agent`(LLMエージェント関連)を **100本**(ノック8割・精読2割の目安)。

## 進捗

| 対象 | 本数 |
|---|---|
| t: agent | 0 / 100(1本目読み中) |
| うち精読 | 0 |
| 総数 | 0 |

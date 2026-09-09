[README_SQL用語集.md](https://github.com/user-attachments/files/31994412/README_SQL.md)
# SQL対策ノート（応用情報技術者試験）README

## Description（概要）

応用情報技術者試験のSQL分野に対応した学習用リファレンスノート。基本情報技術者試験レベルの基礎構文（SELECT / WHERE / JOIN など）から、応用情報技術者試験で問われる発展的なSQL（外部結合・サブクエリ・CASE式・ビュー・トランザクション制御・参照制約・GRANT/REVOKE・ウィンドウ関数など）までを1ページに集約。ページ上部の検索ボックスにSQL文やキーワードを入力すると、該当する解説箇所へワンクリックでジャンプできる。

## これは何か

もとは基本情報技術者試験向けに作られたSQL解説ページ（`SQL基礎解説_応用情報技術者試験.html`）を、応用情報技術者試験の出題範囲までカバーするよう拡張したものです。単なる用語の羅列ではなく、各キーワードについて「動作の説明」「具体的なSQL例」「実務での使われ方・注意点」をセットで掲載しています。

## 収録内容

**基礎（元ファイルから継承）**
SELECT/FROM、WHERE（比較・LIKE・BETWEEN・IN・IS NULL）、ORDER BY、GROUP BYと集計関数（COUNT/SUM/AVG/MAX/MIN）、HAVING、DISTINCT、JOIN/INNER JOIN

**応用情報技術者試験レベル（今回追加）**
外部結合（LEFT/RIGHT/FULL OUTER JOIN）、自己結合（SELF JOIN）、集合演算（UNION/UNION ALL/INTERSECT/EXCEPT）、副問合せとEXISTS/NOT EXISTS、ALL/ANY（SOME）、CASE式、ビュー（CREATE VIEW）、データ更新（INSERT/UPDATE/DELETE）、トランザクション制御（COMMIT/ROLLBACK/SAVEPOINT）、テーブル定義と制約（CREATE TABLE、PRIMARY KEY、FOREIGN KEY、UNIQUE、CHECK、DEFAULT、NOT NULL）、参照制約の動作（ON DELETE/ON UPDATEにおけるCASCADE・RESTRICT・NO ACTION・SET NULL・SET DEFAULT）、インデックス（CREATE INDEX）、アクセス権限の制御（GRANT/REVOKE）、ウィンドウ関数（OVER/PARTITION BY/ROW_NUMBER/RANK/DENSE_RANK）

全25セクション構成。目次（ページ上部）から該当セクションへ直接ジャンプできます。

## 使い方

1. ページ上部の検索ボックス（🔍 SQLキーワード検索）に、SQL文の一部やキーワード単体（例：`SELECT * FROM 商品表 LEFT JOIN 売上表 ON ...` や `CASCADE`）を入力する。
2. 入力内容に含まれるキーワードが自動検出され、チップ（丸いリンク）として一覧表示される。
3. チップをクリックする、または「最初のキーワードへジャンプ」ボタンを押すと、該当する解説セクションへスムーズにスクロールし、該当箇所が一瞬ハイライトされる。
4. ページ内の解説文中のキーワードも、下線付きのリンクになっておりクリックでジャンプ可能。

## 入手方法

- **オンライン版（推奨）**：ブラウザで開いて繰り返し参照できるページとして公開済み。何度でも開き直して学習に使えます。
- **ファイル版**：同内容のスタンドアロンHTMLファイルとしても提供済み（オフラインで開く場合や、他の場所に保存しておきたい場合用）。

## 出典・作成経緯

- ベースとなった基本情報レベルの内容：ユーザー提供の`SQL基礎解説_応用情報技術者試験.html`
- 参照制約の動作（CASCADE/RESTRICT/NO ACTION/SET NULL/SET DEFAULT）の記述：ユーザー指定の内容をそのまま反映
- そのほかの応用情報レベルの追加項目：応用情報技術者試験のSQL出題範囲に基づき作成

## 作成ツールについて

本ページの構成・追加解説文・検索機能の実装は、Anthropic社のAIアシスタント「Claude」を使用して作成しました。

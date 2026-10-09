# CP932とUNICODEの一対一の対応表

## 名称
CP932とUnicodeの一対一の対応表

## 説明
CP932とUnicodeの対応関係を示すデータです。

CP932内には、重複して登録されている文字があります。そのため、CP932からUnicodeへの変換は成立しますが、UnicodeからCP932への変換において、一部の文字については複数の候補があるため、CP932コードを確定できません。

本表では、bestfit932.txt に基づき、UnicodeからCP932への変換先を確定しています。

なお、CP932 1バイト部に対応したUnicode(半角英数字記号0x20-0x7eの95文字、半角カナ0xA1-0xDFの63文字、計158文字)、および CP932 2バイト部に対応したUnicode(7326文字)、計7484文字が対象です。

## 構造

データは**タブ区切り**です。

| 項目 | 内容 |
|---|---|
| CP932の文字コード | CP932における文字コード |
| Unicodeコードポイント | Unicodeのコードポイント |
| UTF-8コード | Unicode文字をUTF-8で表したバイト列 | 
| 文字 | 対応する文字 |
| Unicode文字名 | Unicodeで定義された文字名 |
| 東アジアの文字幅特性 | East Asian Widthの特性値 |
| 文字幅 | 表示幅を1または2で表した値 |

## 文字幅

`文字幅` は、日本語環境下における一般的な表示幅を示します。

- `1` : ASCII、半角カナなど
- `2` : 上記以外の文字

## データ出典

- CP932.TXT
- EastAsianWidth.txt
- bestfit932.txt

## 関連項目

[CP932⇔Unicode/UTF-8文字コード表](https://moginwc.sakura.ne.jp/other_cp932map.html)

EOF

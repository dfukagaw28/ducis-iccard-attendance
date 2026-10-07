# CSVまとめツール

複数のCSVファイルを読み込んで1つに結合し、CSVで保存するツールです。

処理はすべてブラウザ内で完結し、データは外部に送信されません（CSPで通信を禁止しています）。

## ツール

- `index.html` 出席取りまとめ：出席簿（Excel）の「学生ID」「表示用氏名」と出席データ（CSV）を照合し、出席／欠席の列を付けてCSVで保存
- `merge.html` CSVまとめ：複数のCSVを1つに結合

Excelの読み込みには [SheetJS](https://sheetjs.com/) 0.20.3（`vendor/xlsx.full.min.js`、Apache-2.0）を同梱して使っています。外部CDNからは読み込みません。

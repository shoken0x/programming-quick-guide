# CLI (Command Line Interface)

## 今日のゴール

bashスクリプトで以下のプログラムにチャレンジ

1. コマンドラインで画像をダウンロードしてみる
  - ワンライナーでダウンロード
  - テキストファイルを読み込んでダウンロード
2. タイピングゲームを作る
  - 標準入力をそのまま表示させるエコープログラム
  - テキストファイルを読み込んでタイピングゲーム


## TerminalでのCommandデモ

- w3mコマンドによるWebブラウジング
- mailコマンドでメール
- スクレイピング: 画像のダウンロード

## 参考

### bashスクリプトの実行方法

shコマンドの引数にbashスクリプトのファイル名を与える

`sh ファイル名`

### for文

```bash
for line in `cat xxx.txt`; do
  curl -O ${line}
done
```

### if文

```bash
if [ "xxx" = "input" ]; then
  echo "success!"
else
  echo "failed"
fi
```

### 標準入力を読み込む

```bash
echo "何か入力してください"
read input
sleep 1
echo $input
```

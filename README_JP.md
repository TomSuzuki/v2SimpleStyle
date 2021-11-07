# v2SimpleStyle
Beamerのためのシンプルなテーマ。  

<div align="right">
    <a href="./README.md">English</a> | <a href="./README_JP.md">日本語</a>
</div>
  
[見本](./sample/sample.pdf)  

[豆知識。](./豆知識.md)

## コマンド
### テーマカラーの変更
```tex
\definecolor{themeColor}{HTML}{E03200}
```
- このサンプルではカラーコードを `E03200` に変更しています。
- 他の色に変更したい場合はカラーコード（RGB）を変更してください。

### フレーム内に引用を表示する
```tex
\pagereference{\cite[???] ??????? ???????????}
```
- フレーム下部に引用を表示します。
- 詳細はこちら(`./sample/02_sample.tex`)。
- このコマンドは textpos absolute を使用しています。レイアウト崩壊に注意してください。

## 必要なコマンド
- `xelatex`, `pbibtex`, `xdvipdfmx`

## PDF化
```shell
make
```
- makefileを使うと簡単にできます。

## LICENSE
- MIT License
  - 改変したら `from v2SimpleStyle` とか `use v2SimpleStyle` とか書いて欲しい。
  - スライドテーマに使うなら書かなくてもいいよ。

## 注意？
- 参考文献が無いとエラー吐くかも。

## 参考文献
- [Beamer を使ってみる](http://www-an.acs.i.kyoto-u.ac.jp/~fujiwara/tex/beamer.html)

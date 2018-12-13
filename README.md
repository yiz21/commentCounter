# CommentCount

C/C++のソースコードのコメントをカウントします。

## 主な機能
フォルダを指定し、そのフォルダ配下にあるすべてのソースコードに対してそれぞれ下記を求めます。
* 全行数
* 有効行数
* コメント行数

下記のように有効行とコメント行が１行に存在する場合は、それぞれ１行としてカウントします。

```C
/* comment */ enabletext //comment
```

この場合、（全行数≠有効行数＋コメント行数）とはなりません。

上記例を有効行としてカウントしたい場合は（有効行数+コメント行数）- 全行数をコメント行数から引いて計算してください。

## 動作環境
Python3.7.0

## 利用方法
$python main.py
により、Windowが立ち上がるので後はフォルダを指定するだけです。

### インストール
下記ライブラリに依存しています。各自pipによりインストールしてください。
* re
* unicodedata
* glob
* os
* tkinter



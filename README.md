
にぽんご
========

なにこれ？
---------

同一ワークスペース上に既にある gVim でファイルを開くためのコマンドです。
gVim が存在しなれば新しく開き、複数あれば選択をせまられます。

表示されていないワークスペースの gVim は無視してくれる仕様です。


いるもの
--------

- percol https://github.com/mooz/percol
- zenity
- xprop
- xdotool

percol と zenity はどっちでも可。


つかいかた
----------

svim を適当な場所において、パスの通ったところにリンクを貼ります。

    $ ln -s /tekito-place/svim s     # 現在のタブで開くコマンド
    $ ln -s /tekito-place/svim t     # 新しいタブで開くコマンド

あとは、

    $ t something-file-1

とかすればいいです


かんきょうへんすう
------------------

設定しなくてもいいよ

    SVIM_FOCUS_COMMAND - ウィンドウにフォーカスするためのコマンド名を指定する
    SVIM_SELECTOR - ウィンドウを選択するのに使うコマンド ( percol みたいなのいれとき )
    SVIM_COMMAND_NORMAL - 現在タブで開くコマンド名 ( s が嫌なとき )
    SVIM_COMMAND_TAB - 新しいタブで開くコマンド名 ( t が嫌なとき )


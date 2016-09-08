# 20160908-gitbootcamp

Git Boot Campの成果物です

## git add
ファイルを追加する

##commit
###git commit
変更点を保存する。
commitを行うには、事前にaddコマンドで対象とするファイルを指定する必要がある。

###git commit -a
変更が加えられたファイルを自動的に検出して保存する。
（新規作成ファイルはコミット対象外）

###git commit -m <コミットメッセージ>
コミットメッセージを指定して保存する。

## remote add
リモートリポジトリを追加する。
remote add <name> <url>
同時にfetchを行う場合は、「-f」オプションをつける。

###git checkout -b fix/42
ブランチ fix/42 を作成すると同時に切り替える

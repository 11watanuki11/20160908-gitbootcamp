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

## commit --amend
直前のコミットをやり直す
Aをコミット後、git commit --amendすると、A'として再度コミットされる（Aは見えなくなるが.gitに残る？）
コミットする→ファイルを追加して同じコミットをやり直したくなったときに使う？

###git checkout -b fix/42
ブランチ fix/42 を作成すると同時に切り替える

## git branch fix/42
ブランチ fix/42 を作成する。HEADは動かない。


## git branch -f xxx

HEADにブランチxxxを移動します。

## git clone
リモートリポジトリをローカルにコピーする。

## git init
.git を作成する　（リポジトリの初期化）
リモートリポジトリをローカルにコピーする。

## git push
リモートリポジトリに変更内容を反映する

## pull --rebase
fetch + rebaseとして実行。
「--rebase」はgit pullコマンドのオプション。
git pullはfetch + mergeとして実行してくれるが、
mergeするかわりにrebaseしてくれる。

## commit --amend
直前のコミットをやり直す
Aをコミット後、git commit --amendすると、A'として再度コミットされる（Aは見えなくなるが.gitに残る？）
コミットする→ファイルを追加して同じコミットをやり直したくなったときに使う？

###git checkout -b fix/42
ブランチ fix/42 を作成すると同時に切り替える

###reset --hard master
リモートのブランチにローカルを強制一致させたい時に使用する。

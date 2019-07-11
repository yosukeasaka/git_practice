# Gitの使い方


## git init : Creats new Git repository
　作業ディストリクトにGitを使いますよと宣言する。

## git status : Inspects the content of working directory
  現在の状態を確認

## git add filename : Adds file from working directory to stagging area
　ステージングエリアに指定のファイルを加える。
 **git add .** : 作業ディストリクトにある全てのファイルをステージングに加える

## git commit -m "message" : Permanently stores file changes from stangging area
　メッセージと共にステージングエリアにあるファイルをコミットする。

## git log : shows a list of all previouse commits
　ログ（変更履歴）を確認する。Resetするときになどに必要になるSHAの7桁の番号はここで表示できる。

## git --version : check git verstion
　Gitのバージョンを確認できる。
###  git log --oneline ：Logを簡潔に表示


## git show HEAD : Show status of commit
　


## git checkout HEAD filename : Discards changes in working directory


## git reset HEAD filename : reset your change after you add file. (should be before commit)


## git reset commit_SHA : from git log, get 7 character of words. and reset to the log. 

## git config --global user.name "userName" : create user Name for global
　Gitを使用するときのユーザー名を作成


## git config --global user.email "userEmail" : create user Email for global
　Gitを使用するときのメールアドレスを登録


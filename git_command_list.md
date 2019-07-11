# Gitのコマンド一覧


## git init : Creats new Git repository
 - 作業ディストリクトにGitを使いますよと宣言する。
 

## git status : Inspects the content of working directory
 - 現在の状態を確認
 
 
## git diff : See the difference between added file's before & after
 - Addした後の変更点を確認できる。


## git add filename : Adds file from working directory to stagging area
 - ステージングエリアに指定のファイルを加える。
 - **git add .** : 作業ディストリクトにある全てのファイルをステージングに加える


## git commit -m "message" : Permanently stores file changes from stangging area
 - メッセージと共にステージングエリアにあるファイルをコミットする。


## git log : shows a list of all previouse commits
 - ログ（変更履歴）を確認する。Resetするときになどに必要になるSHAの7桁の番号はここで表示できる。


## git --version : check git verstion
 - Gitのバージョンを確認できる。
 - **git log --oneline**：Logを簡潔に表示


## git show HEAD : Show status of commit
 - コミットの詳細を表示


## git checkout HEAD filename : Discards changes in working directory
 - 前の状態に戻る。
 - **git checkout -- filename**：こちらのコマンドでも可。
  

## git reset HEAD filename : Reset your change after you add file. (should be before commit)
 - Addした変更内容を取り消す。


## git reset commit_SHA : from git log, get 7 character of words. and reset to the log. 
 - 指定のログの状態まで戻す。戻したあと**git checkout HEAD filename** をして作業ディストリクトもその指定のログの状態に戻す。
 

## git config --global user.name "userName" : create user Name for global
 - Gitを使用するときのユーザー名を作成


## git config --global user.email "userEmail" : create user Email for global
　Gitを使用するときのメールアドレスを登録


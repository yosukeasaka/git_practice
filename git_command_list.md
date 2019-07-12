---
# Gitのコマンド一覧
---

## init
 - ```git init``` 
 - Creats new Git repository
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


## git branch : Check hwat branch you are currently on.
 - 現在どのブランチにいるか確認できる
 
 
## git branch new_branch: Create new branch
 - 新しいブランチの作成
 - **git checkout new_branch_name : 作成したブランチに移動**


## git branch -d : Delete branch after merge
 - マージした後ののブランチの削除
 
 
## git branch -D : Delete branch before merge
 - マージする前のブランチの削除
 
 
## git merge : Merge new_branch into master
 - マスターのブランチに作成したブランチを統合させる 


## git clone remote_location clone_name : Make clone
 - クローンの作成


## git remote : Check new remote location(origin)
 - **git remote -v** : Show list of remote
 - 新しく作ったクローンの場所を確認


## git merge : Merge new_branch into master
 - マスターのブランチに作成したブランチを統合させる 


## git fetch : Bring the changes down to your local copy
 - 元のデータを自身のローカルに持ってくる


## git merge origin/master : Make your local maser branch update
 - 自身のローカルのマスターブランチをアップデートさせる

## git push origin your_branch_name : Push your branch up to the remote
 - 自身で作成したブランチを元の場所にあげる  


 
 
 
 


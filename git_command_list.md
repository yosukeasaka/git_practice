---
# Gitのコマンド一覧
---


## init
#### 作業ディストリクトにGitを使いますよと宣言する
 - ```git init``` 
 - Creats new Git repository
---
 

## status
#### 現在の状態を確認
 - ```git status``` 
 - Inspects the content of working directory
---
 
 
## diff
### Addした後の変更点を確認できる
 - ```git diff```
 - See the difference between added file's before & after
---


## add
#### ステージングエリアに指定のファイルを加える
 - ```git add filename``` : Adds file from working directory to staging area
#### 作業ディストリクトにある全てのファイルをステージングに加える
 - ```git add .``` : Adds all files from working directory to staging area
---


## commit
#### メッセージと共にステージングエリアにあるファイルをコミットする
 - ```git commit -m "message"``` : Permanently stores file changes from stanging area

---

## log
#### ログ（変更履歴）を確認する
 - ```git log``` : shows a list of all previous commits
 - *Resetするときになどに必要になるSHAの7桁の番号はここで表示できる*

#### Logを簡潔に表示
 - ```git log --oneline```：show a log in one line
---


## version
#### Gitのバージョンを確認できる
 - ```git --version``` : check git version

---


## show HEAD
#### コミットの詳細を表示
 - ```git show HEAD``` : Show status of commit

---

## checkout HEAD
#### 前の状態に戻る
 - ```git checkout HEAD filename``` : Discards changes in working directory

#### こちらのコマンドでも可。
 - ```git checkout -- filename```：Work same as above
---
  

## reset HEAD
#### Addした変更内容を取り消す
 - ```git reset HEAD filename``` : Reset your change after you add file. (should be before commit)

---

## reset commit_SHA
#### 指定のログの状態まで戻す
 - ```git reset commit_SHA``` : from git log, get 7 character of words. and reset to the log. 
 - 戻したあと ```git checkout HEAD filename``` をして作業ディストリクトもその指定のログの状態に戻す。
 ---


## config
#### Gitを使用するときのユーザー名を作成
 - ```git config --global user.name "userName"``` : create user Name for global

#### Gitを使用するときのEmailを登録
 - ```git config --global email.name "userEmail"``` : sign up user Email for global

---

## branch
#### 現在どのブランチにいるか確認できる
 - ```git branch``` : Check hwat branch you are currently on.

#### 新しいブランチの作成
 - ```git branch new_branch```: Create new branch

#### 作成したブランチに移動
 - ```git checkout new_branch_name``` : move new_branch_name

#### マージした後ののブランチの削除
 - ```git branch -d``` : Delete branch after merge

#### マージする前のブランチの削除
 - ```git branch -D``` : Delete branch before merge
---
 
 
## merge
#### マスターのブランチに作成したブランチを統合させる 
 - ```git merge``` : Merge new_branch into master

#### 自身のローカルのマスターブランチをアップデートさせる
 - ```git merge origin/master``` : Make your local maser branch update

---

## clone
#### クローンの作成
 - ```git clone remote_location clone_name``` : Make clone
---


## remote
#### 新しく作ったクローンの場所を確認
 - ```git remote``` : Check new remote location(origin)

#### リモートのリストを表示
 - ```git remote -v```: Show list of remote

---

## fetch
#### 元のデータを自身のローカルに持ってくる。しかし持ってくるだけでそれ以外は何もしない。
 - ```git fetch``` : Bring the changes down to your local copy
 - *ローカルのmasterには一切手を触れないため、masterとorigin/masterは別のコミットを指す*
   - この状態で```git checkout master```すると```Switched to branch 'master'
Your branch is behind 'origin/master' by 2 commit, and can be fast-forwarded.```などと表示される
 - ↑上記の時は```git merge origin/master```で統合すればよい
---


## push
#### 自身で作成したブランチを元の場所にあげる 
 - ```git push origin your_branch_name``` : Push your branch up to the remote

---

## pull
#### 他のリポジトリのデータを取得し、ローカルのブランチに統合
 - ```git pull```
 - ```git pull origin master``` : *こちらのが一般的に使われる*
 - ```git fetch```と```git merge origin/master```までを全部まとめてやってくれる

---
 
 
 


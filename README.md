# EfficientPoints

https://eztas.github.io/GithubTest/index.html

# gitの手順
## リモートリポジトリをローカルにクローン。作業時はcdを忘れずに。
```
git clone https://github.com/Eztas/EfficientPoints.git
cd EfficientPoints
```

## 変更をリモートに反映
リモートにないブランチを反映する場合はエラー文にあるgitコマンドを入力すればよい
```
git add .
git commit -m "メッセージを書いて下さい！"
git push
```

## 変更をリモートから反映
originがないとリモートの変更を取得できないので注意
```
git fetch origin
git pull
```

## branchに関する作業(checkout含む)

### 新しいブランチを切りだし

```
git checkout -b {your-feature-branch}
```

### ブランチを削除(主に自分のブランチ作業終了時)

```
git branch -d branch1
```

### リモートのブランチをローカルへ落とし込む(ローカルにbranch1がない)
```
git fetch origin
git checkout -b branch1 origin/branch1
```

### リモートのブランチをローカルのブランチに反映(ローカルにbranch1がある)
```
git fetch origin
git checkout branch1
git merge origin/branch1
```

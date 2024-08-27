# EfficientPoints

https://eztas.github.io/EfficientPoints/index.html

# gitの手順
## リモートリポジトリをローカルにクローン。作業時はcdを忘れずに。
```
git clone https://github.com/Eztas/EfficientPoints.git
cd EfficientPoints
```

### リモートのブランチをローカルへ落とし込む(ローカルにbranch1がない)
```
git fetch origin
git checkout -b branch1 origin/branch1
```
### 変更をリモートに反映

```
git add .
git commit -m "メッセージを書いて下さい！"
git push
```

### ブランチを削除

```
git branch -d branch1
```
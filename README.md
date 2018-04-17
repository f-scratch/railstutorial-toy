## 運用方法
各個人ごとにbranchを作成し、各個人はそのbranchに向けて作成物のアップロードを行う。

## 手順(git使用方法)
### 初期設定
1. railsプロジェクトのrootパスに移動する。

```
$ cd {個人のプロジェクトのrootパス}
```

2. リポジトリを作成し、実行パスとその配下のファイル群をgit管理下とする。

```
$ git init
```

3. 自身が使用するブランチを作成する。

```
$ git checkout -b develop/{ githubユーザー名 }
```

(もしgit管理を行いたくないファイルが存在する場合はgitignoreファイルを編集する。)

```
($ vim .gitignore)
```

4. ローカルブランチに現在の編集内容を保存する。

```
$ git add .
$ git commit -m "Initial Commit"
```

5. リポジトリとリモートブランチの設定を変更する。

```
$ git remote add origin git@github.com:f-scratch/railstutorial-hello.git
```

6. リポジトリにローカルブランチをアップロードする。

```
$ git push -u origin develop/{ githubユーザー名 }
```

### 通常のアップロード方法
1. 保存したい編集内容を選択する。

```
$ git add {変更対象のファイル}
```

2. 選択した編集内容をローカルブランチに保存する。

```
$ git commit -m "{変更内容を一言で記述}"
```

3. リポジトリにローカルブランチをアップロードする。

```
$ git push origin develop/{ githubユーザー名 }
```

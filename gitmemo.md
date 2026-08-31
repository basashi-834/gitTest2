# Git Memo(初心者向け)

## 初期設定

- Gitの初期設定を確認

```
$ git config --global --list
```

- アカウント名登録

```
$ git config --global uset.name アカウント名
```

- noreplyメールアドレスの登録

```
$ gitconfig --global user.email アドレス名
```

- コミットコメント入力用エディタをvsCodeに指定

```
$ gitconfig --global core.editor "code --wait"
```

- デフォルトブランチ名をmasterではなくmainに設定

```
$ gitconfig --global init.defaultBranch main
```

- 設定が反映されていることを確認

```
$ git config --list
    user.name=「GitHub アカウント名」
    user.email=「GitHub 提供のnoreply メールアドレス」
    core.editor=code --wait
    init.defalutbranch=main
```

\*設定項目名の取り消し

```
$ git config --global --unset 設定項目名
```

# ファイルを編集した後

```
git status  // 何が変わったか確認
```

```
git add .   // 変更をステージング
```

```
git commit -m "変更内容"  // コミット
```

### コミット操作

- ローカルリポジトリの初期化  
  $ `git init`
- 現在の状態を見る  
  $ `git status`
- コミットしたいファイルを、先にステージングエリアに追加  
  $ `git add <ファイル名>`
- ステージングエリアにあるファイルのコミット  
  $ `git commit`
- 同ファイルのコミット(コマンドと一緒にコミットメッセージを入力)  
  $ `git commit -m "コミットメッセージを入力"`

### ブランチ操作

- ブランチ一覧を表示  
  $ `git branch`
- 新しいブランチを作成  
  $ `git branch <ブランチ名>`
- ブランチを切り替え  
  $ `git switch <ブランチ名>`
- ブランチの作成と切り替えを同時に行う  
  $ `git switch -c <ブランチ名>`
- ブランチをマージ  
  $ `git merge <ブランチ名>`
- マージ済みブランチを削除  
  $ `git branch -d <ブランチ名>`

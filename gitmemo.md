# Git Memo

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

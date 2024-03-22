gitの設定には範囲がいくつかある
* プロジェクト
* グローバル
* システム

グローバルの設定を追加するコマンド
```bash
% git config --global user.name "username"    
% git config --global user.email "myname@example.com"
```

このコマンドにより以下のファイルが作られる

`~/.gitconfig`
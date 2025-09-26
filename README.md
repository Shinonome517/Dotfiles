# Dotfiles

## Shell Configuration

1. `zsh` が未インストールの場合は導入します（macOS には標準で含まれています）．
2. `which zsh` で `zsh` のフルパスを確認します．
3. `zsh` をログインシェルとして設定します．
   ```sh
   chsh -s $(which zsh)
   ```
4. 変更を反映させるため，ログアウトして再ログインするか，ターミナルを再起動します．

## Create Symbolic Links

このリポジトリの dotfiles をシェルで利用できるようシンボリックリンクを作成します．

```sh
ln -s /path/to/Dotfiles/.zshrc ~/.zshrc
```

- `/path/to/Dotfiles` はこのリポジトリの絶対パスに置き換えてください．
- 既存のファイルを上書きする場合は `ln -sf` を利用します．

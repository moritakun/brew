# Git

* インストール
  * brew install git
* インストール確認
  * git --version
    ```
    git version 2.24.3 (Apple Git-128)
    ```
    →(Apple Git-128)と表示されているのは、macにデフォルトでインストールされているgitを表している。
  * brew info git
    ```
    ==> git: stable 2.42.1 (bottled), HEAD
    Distributed revision control system
    https://git-scm.com
    /usr/local/Cellar/git/2.42.1 (1,637 files, 49.6MB)
    Poured from bottle using the formulae.brew.sh API on 2023-11-03 at 16:55:13
    From: https://github.com/Homebrew/homebrew-core/blob/HEAD/Formula/g/git.rb
    License: GPL-2.0-only

    --長いので省略--

    ```

* HomebrewのGitのパスを通す
  * 使用しているシェルの場所を確認
    * echo $SHELL
        ```
        /bin/bash
        ```
    →bashを使用している
  * .bash_profileを編集
    * vi ~/.bash_profile

        以下を追記する
        ```
        #HomebrewのGitを使うパス
        export PATH=/usr/local/bin/git:$PATH
        ```
* シェルを再起動
  * exec $SHELL -l



* 環境変数を追加して、lsやcdコマンドが打てなくなった場合（bash: sed: command not found）
  * export PATH=/bin:/usr/bin:/usr/local/bin
  * vim ~/.bash_profile
  * 参考→ [こちら](https://qiita.com/annts095/items/90bc9b4746f1ae9a83c3)


* デフォルトの対話型シェルはzshになりました。と表示された場合。
    ```
    The default interactive shell is now zsh.
    To update your account to use zsh, please run `chsh -s /bin/zsh`.
    For more details, please visit https://support.apple.com/kb/HT208050.
    ```
  * ログインシェル属性を変更する
    * chsh -s /bin/zsh
        ```
        Changing shell for moritahiro.
        Password for moritahiro: 
        ```

* git初期設定
  * cat ~/.gitconfig
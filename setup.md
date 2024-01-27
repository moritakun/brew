# homebrew
macOSのパッケージ管理ソフト（パッケージマネージャ）
[公式サイト](https://brew.sh)

* バージョン確認
  * brew -v
    ```
    ~ $ brew -v
    Homebrew 4.1.7
    Homebrew/homebrew-core (git revision b4047f14bff; last commit 2023-08-31)
    Homebrew/homebrew-cask (git revision 127e49af6a; last commit 2023-08-31)
    ```
* アップデート
  * brew update
    ```
    Installing from the API is now the default behaviour!
    You can save space and time by running:
        brew untap homebrew/core
        brew untap homebrew/cask
    Updated 3 taps (homebrew/cask-versions, homebrew/core and homebrew/cask).

    --長いので省略--
    
    You have 19 outdated formulae installed.
    You can upgrade them with brew upgrade
    or list them with brew outdated.
    ```

* インストールされているformulaeを全てアップグレード
  * brew upgrade
  ```
  ==> Downloading https://formulae.brew.sh/api/formula.jws.json
  ##O=- #      #
  ==> Upgrading 19 outdated packages:
  pyenv 2.1.0 -> 2.3.31
  gdbm 1.21_1 -> 1.23
  icu4c 69.1 -> 73.2
  readline 8.1.1 -> 8.2.1
  lz4 1.9.3 -> 1.9.4
  sqlite 3.36.0 -> 3.43.2
  xz 5.2.5 -> 5.4.4
  grep 3.8_1 -> 3.11
  openjdk 16.0.1 -> 21.0.1
  ca-certificates 2021-09-30 -> 2023-08-22
  zstd 1.5.0 -> 1.5.5
  mysql 8.0.26 -> 8.1.0
  pcre2 10.40 -> 10.42
  libevent 2.1.12 -> 2.1.12_1
  tfenv 2.2.2 -> 3.0.0
  openssl@1.1 1.1.1l_1 -> 1.1.1w
  six 1.16.0_2 -> 1.16.0_4
  protobuf 3.17.3 -> 25.0
  python 3.11.6_1
  
  --長いので省略--

  ```

* 古いformulaeを削除
  * brew cleanup
* brewのセキュリティ状態確認
  * brew doctor

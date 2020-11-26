## Linux備忘録

- サービス一覧の確認
  ```
  systemctl list-units --type=service
  ```
  
- ファイル比較（並べて表示）
  ```
  diff -y file1 file2
  ```

-  ユーザー切り替え
  ```
  sudo su - : root
  su user : userアカウント
  ```

- ポートの状態の確認
  ```
  ssコマンド(netstat)オプション(ipv4)           ex.)ss -nat4
  -t : 確立済TCPソケットを表示する　
  -l : リスニングソケットを表示する
  -a : リスニングソケットとそれ以外のソケットを表示する
  -n : サービス名をポート番号で表示する
  -p : ソケットを使っているプロセスを調べる
  -u : UDPソケットを表示する
  ```

- プロセスの一覧表示

  ```
  ps aux
  pstree
  ```

- プロセス名に対応するプロセスIDの確認

  ```
  pgrep python
  ```

- ターミナル（プロンプト）の文字色変更

  - .bash_profileに以下を記述

  ```.bash_profile
  export PS1='\[\e[32m\]\u:\W \$ \[\e[0m\]'
  
  # \[\e[32m\] : 色指定
  # \u:\W : プロンプトにユーザ名と現在のディレクトリ表示
  # \$ : $or#の表示
  # \[\e[0m\] : 色指定のリセット
  ```

- ユーザ関連

  ```
  /etc/passwd : ユーザ一覧
  /etc/group : グループ一覧
  /etc/shadow : パスワード一覧
  ```

  
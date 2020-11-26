## Python備忘録

- VScodeでコマンドパレットの表示
  ```
  Ctrl+Shift+P
  ```
- ライブラリの確認
  ```
  (python -m) pip list
  ```

- ライブラリのインストール
  ```
  (python -m) pip install "ライブラリ名"
  ```

- フォントライブラリの確認

  ```
  dir c:\Windows\Fonts
  ```

- pyenvによるPythonのバージョン管理

  ```
  sudo pyenv global 3.8.6 : 3.8.6に切り替え（全体）
  sudo pyenv local system : system(2.7.5)に切り替え
  sudo pyenv versions : 利用可能なバージョン確認
  ```

- Pythonからhttpサーバの起動

  - カレントディレクトリがドキュメントルートになる

  ```
  python -m http.server 8000
  python -m http.server --bind 127.0.0.1 8000
  ```

  
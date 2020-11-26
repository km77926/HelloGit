## Docker備忘録

- イメージ一覧表示

  ```
  docker images
  ```

- コンテナ一覧表示

  ```
  docker ps : 起動中のコンテナ
  docker ps -a : 停止中も含めた全てのコンテナ
  ```

- コンテナの作成

  ```
  docker run -d -it -p 8080:80 --name python1 python:3
  ```

- コンテナの起動と停止

  ```
  docker start python1
  docker stop python1
  ```

- コンテナ・イメージの削除

  ```
  docker rm python1 : コンテナの削除
  docker rmi python1 : イメージの削除
  　　※起動中のコンテナがある場合削除できない
  ```

- コンテナの実行

  ```
  docker exec -it centos2 bash
  ```

  
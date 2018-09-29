## Docker Swarmを用いた実践的なアプリケーション構築
`Docker Swarm`を用いてアプリケーションを構築していきます．
## 概要
以下のようなアーキテクチャを構築していきます．  
アプリは，`web`アプリケーションとして，`Todo`アプリを作ります.  
`mysql`は，`Master-Slave`構成で構築します，`INSERT/UPDATE/DELETE`などのクエリ(`WRITE`)は，`MasterDB`で行い，`SELECT`のクエリは，`SlaveDB`で行い，負荷分散をします．
## アーキテクチャ

![architecture](https://github.com/mytheta/TodoApp/blob/master/architecture.png)
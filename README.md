# todo_app

## 参考
https://github.com/rrousselGit/riverpod/tree/master/examples/counter

## このリポジトリの目的
- チュートリアルを振り返ることで、基礎的な状態管理の仕組みの理解を深める。
- 清書をしていきながら、RiverPodの導入について理解する。


## 学んだこと
- TodoListクラスで、stateを管理及び、ステートの変更にメソッドを入れると、viewが太らない。
- 今回のviewの書き方の構成は
  - importするライブラリ群のimport
  - 状態管理をするHook類
  - view
  - viewで利用するHookEffect
- グローバルに、入力されたデータを管理をしたい場合は、Providerを利用する。
- ユーザーの挙動を管理したい場合はhookを用いている。
  - flutter_hookを用いるポイントとして、フォーカスに関する情報の管理など、上記で作ったProviderとは関係せずアプリケーションの動作管理を行いたい時は、
  - Flutter_hookを利用している模様。
  - Providerはあくまでデータ管理であり、アプリケーションの動作管理は、Flutter依存のものを利用しているっぽい。

## 業務で使えそうなポイント
- 今まで一番混乱していたポイントが「データ管理」と「ユーザーの動作管理」が一緒くたにしていたことで理解が追いついてなかったっぽい。
  - データを管理、保存、更新するのは、Providerを利用する。
  - ユーザーの動作を管理するのは、flutterの動作挙動をハンドリングできるflutter_hookを利用する。


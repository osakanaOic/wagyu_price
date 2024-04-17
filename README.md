# Git Lesson

## リモートリポジトリとローカルリポジトリとはそれぞれ何でしょうか？

リモートリポジトリ：専用のサーバに配置して複数人で共有するためのリポジトリ
ローカルリポジトリ：ユーザ一人ひとりが利用するために、自分の手元のマシン上に配置するリポジトリ

## プッシュとマージの違いは何でしょうか？
プッシュ：ローカルリポジトリの変更をリモートリポジトリに反映させる
マージ：分岐した履歴を戻して統合する


## コミットとプッシュの違い
コミット：ローカルリポジトリに変更を記録する操作
プッシュ：ローカルリポジトリの変更をリモートリポジトリに反映させる



## コミットのメッセージはどのように書いてあげるのが最適でしょうか？
何を変更したか誰が見ても一目で分かるように書く

プレフィックス：接頭辞で、コミットメッセージの先頭に特定の文字をつけること。
メッセージからコミットの内容を予想しやすくなりレビュアーの負荷を下げられる
プレフィックスを意識することでコミット粒度を自然と適度に分割できるようになる
後でログからコミットを探しやすくなる

プレフィックスの例：
fix	既存の機能の問題を修正する場合に使用する。
hotfix	緊急の変更を追加する場合に使用する。
add	新しいファイルや機能を追加する場合に使用する。
feat	新しい機能やファイルを追加する場合に使用しまする。
update	既存の機能に問題がないが、修正を加えたい場合に使用しまする。


## ローカルでマージするフローと、プルリクエストでマージするフローの違いは何でしょうか？
ローカルでマージするフロー：ソースコードの変更部分を明確に表示できない。
プルリクエストでマージするフロー：ソースコードの変更部分を明確に表示できる。 また、プルリクエストの作成者は、ソースコードの意図や補足事項をコメントとして伝えることができる。 これらによって、レビュー担当者の負担を減らせることができる。


ローカルでマージするフロー：変更部分は確認できるが、レビューが細かく確認できないまま、モートリポジトリに送られる
プルリクエストでマージするフロー：レビュ-がしっかり確認でき、リモートリポジトリーでの再現性も高い。


## コンフリクトを起こしてしまった場合、どう対処すべきですか？
・変更をコミットする
. 変更をスタッシュする
. 変更を破棄する


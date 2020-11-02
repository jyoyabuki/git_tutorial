# 「ワークツリー」-->> 「ステージ」 -->> 「リポジトリ」

# 変更
## 「ワークツリー」-->> 「ステージ」
    git add <ファイル名>

## 「ステージ」 -->> 「リポジトリ」
    git commit

# 差分を確認
## 「ワークツリー」-->> 「ステージ」
    git diff

## 「ステージ」 -->> 「リポジトリ」
    git diff --staged

# コミットした履歴の確認
    git log

# ファイルを削除する（すべての場所から）
    git rm <ファイル名>
#  ファイルの移動を記録する（名前を変更する）
    git mv <旧ファイル名> <新しいファイル名>
          |
          V  これと同じこと
    mv <旧ファイル名> <新しいファイル名>    : ファイル名を変更
    git rm <旧ファイル>　                   : 旧ファイルを削除
    git add <新ファイル>　　　　　　　　　　　: 新ファイルをaddする

# リモートリポジトリ（GitHub）を新規に追加する
    git remote add origin https://github.com/user/repo.git

# リモートリポジトリへ送信する
    git push <リモート名> <ブランチ名>
    git push origin master

# GitHubで新規リポジトリを作成
    1. 右上のアイコンから「Your profile」を開く
    2. 「Ripositories」を開く
    3. 「New」で新規作成する
    4. 作成するリポジトリ名を入力
    5. 「Create repository」をクリック
    6. 「…or push an existing repository from the command line」の1行目（リポジトリのURL）をコピーしておく
    7. ターミナルに貼り付け（リモートリポジトリを新規に追加）
    8. push（リモートリポジトリへ送信）する
        git push -u origin master

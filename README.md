# SAKELOG
Ruby on Rails(5.2.4)を用いて、日本酒レビューのアプリを作成いたしました。
シンプルなUI(投稿写真が映えるようモノトーンに統一されたデザイン)と明快なUXにこだわりました。

<img width="840" alt="スクリーンショット 2020-05-07 18 36 05" src="https://user-images.githubusercontent.com/47711244/81289277-184c2800-90a1-11ea-875e-c1a0a9edbc5f.png">

# URL
https://www.sakelog.net

閲覧の際はヘッダーの【ゲストログイン(閲覧用)】をご利用ください。

## 制作の背景
居酒屋等のネットでのレビュー・口コミと、実際に訪問した際のギャップを感じることがしばしばあり、友人や知り合いの飲んだことのあるお酒・お店がすぐに確認できるツールがあれば良いと思い、開発しました。
今後の改良方針としては、

- GooglemapAPIを用いた、レビューしたお酒を飲んだ場所の記録。
- 日本酒の名前をDBに格納(もしくはAPIを利用)してサジェスト表示する。
- Rspecを用いたテストの充実
- CI/CDパイプラインの構築

等のアップデートを考えています。

## 言語・使用技術

- バックエンド
  - Ruby 2.6.2
  - Rails 5.2.4
  - MySQL 5.7
  
- フロントエンド
  - html
  - Scss
  - bootstrap
  - JavaScript
  - jQuery
  
- インフラ
  - ローカル
    - Docker
    - docker-compose
  - デプロイ
    - Capistrano
  - AWS
    - VPC
    - EC2
    - RDS
    - ALB
    - Route53
    - ACM
    - S3
    - Nginx
    - unicorn

<img width="698" alt="スクリーンショット 2020-05-07 19 34 08" src="https://user-images.githubusercontent.com/47711244/81289327-30bc4280-90a1-11ea-8f53-9db44b5db46c.png">

## 機能一覧

- ユーザー機能
  - 新規登録・ログイン・ログアウト機能
  - マイページ・登録情報編集機能
  - ユーザーフォロー機能
  - ユーザーの一覧表示
- 投稿機能
  - 投稿編集機能
  - 本番環境の画像の保存先にS3を採用
  - 写真のプレビュー機能
  - 投稿のブックマーク機能
- お気に入り・フォロー機能のajax化
- お気に入りの一覧表示


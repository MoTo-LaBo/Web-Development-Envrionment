# README
- 制作 APP
> https://moto-labo-product-register.herokuapp.com/
## Web Development Environment
- Docker を使ってweb application を開発 Flow を掴む
  - 今回はあくまでも、**web app 開発の時全体の流れをつかむという事にFOCUS** している
- Docker と wed をどう効率よく利用するかに重点を置く事
- web app 作成の為のフレームワーク
  - RAILS
  - Postgre SQL
  - docker comopose
  - docker
  - GitHub と Travis は連携させる
- Test and Deploy (CICD : パイプライン)を自動化
  - Travis CI
  - HEROKU
## Docker を使用して CICD パイプライン 作成
- 実際の業務に対応出来る Levelに設定
  - Docker
  - GitHub
  - CICD パイプライを組む
  - Heroku に deploy まで自動化
## GitHub repository に Travis CI 同期
- repository に push されると自動で Travis CI で CI tool が動く
  -  test を自動化 / deploy を自動化
- 今回は Ralis の test を Travis CI 上で実行させて、問題がなければ Heroku の方に deploy させている
- Heroku に postgres とか環境変数を設定
- Heroku の deploy 自体も Docker container を使用
- Heroku 上で app を動かす

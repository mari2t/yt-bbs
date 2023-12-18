# study-log

## 2023/12/17

1. スニペット拡張インストール
2. routes.rb の下記はデフォルトの正常動作確認用ルーティング  
   get "up" => "rails/health#show", as: :rails_health_check
3. controller を作成するコマンドがある  
   (ex) rails generate controller Posts
4. .erb がルビー形式のファイルとなる。(ex)index.html.erb
5. DB 作成はコマンドがある  
   (ex) rails generate model Posts title:string content:text
6. migrate コマンドがある
   rails db:migrate
7. @posts のように@を付けると view で呼び出せるようになる
8. Ruby v0.1.7 Shopify 　を入れたところ文字に色がついた
9. private 以降の記述はその html でしか呼び出せないもの
10. 投稿ボタンを押しても投稿できないエラー。原因はタイプミス。  
    〇 def new  
    ✕ def def new
11. %=だと値を返す。条件文は%。
12. ruby は delete ではなく destroy
13. edit ページが表示されないエラー。  
    （エラー）Couldn't find Post with 'id'={:params=>[:id]}  
    （原因）  
    〇　@post = Post.find(params[:id])　  
    ✕ 　@post = Post.find(params:[:id])

## 2023/12/16

1. 作成
2. MVC モデル(model,view,controller,)
3. rails server でサーバーが立ち上がる
4. サーバーが立ち上がらないエラー。原因は保存場所。以下保存場所を改善したらサーバーが立ち上がった。
   1. onedrive 外（onedrive は同期するのでうまくいかない、と見つけたため）
   2. パスに英数字のみ（パスにデスクトップと入っていたため）

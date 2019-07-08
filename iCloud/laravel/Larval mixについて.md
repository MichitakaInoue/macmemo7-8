# Larval mixについて


通常　viewをjsにコンパイルしたりsassをcssにコンパイルするために
Gulpランナーなどのタスクランナーをしようしてpackege.json
でコンパイルするコードを書かなければならなかったが、


タスクランナーを覚えるのも面倒なので

Laravel Mixというライブラリであれば完結にコードを書くことができる




なので、そういった基本的な設定コードはデフォルトで記述される




・nom run dev //全タスク実行

・npm run production //全タスクを実行し出力を圧縮

・nom run watch //ファイルの変更を監視し自動タスクを実行する




タスクはweb pack.mix.jsに記述されている
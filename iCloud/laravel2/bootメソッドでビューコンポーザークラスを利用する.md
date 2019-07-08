# bootメソッドでビューコンポーザークラスを利用する



必要な処理を書くこと



namespaceに必要なクラス、
ビューで常に行われる処理を書くこと


—>config/app.phpに設定を追加


Config/app.phpのprovidersにcomposerに
ComposerServiceProviderを追加することで
ComposerServiceProviderをLaravelが自動で読み込んで実行できるようにする



ここまでできたら、ビューで表示させるだけ！
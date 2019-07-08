# ServiceProviderクラスの作りかた


ServiceProviderクラスは


Php artisan make:provider ComposerServiceProvider





サービスプロバイダ　とはアプリケーションの準備段階で何かしらの処理や設定を行うためのクラス
リクエストが来てからアクションが呼ばれるまでの準備段階のときの話


今回はコンポーザーを提供するためにサービスプロバイダ を作る

その場合、ComposerServiceProviderとする
こんな名前が実務でもつけることができる


App/Providers/ComposerServiceProvider.php

の中にファイルあできる



ビューコンポーザーで使う場合はboot()に処理を書くこと
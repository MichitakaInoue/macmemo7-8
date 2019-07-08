# Route::get('/drills/{id}/edit', 'DrillsController@edit')->name('drills.edit…


URIに文字列が入ってくると、エラーになる


ここで、GETパラメータが数字であるかチェックしなければならない


コントローラでデータをやりとりしたものが、viewに入ってくるので

その変数にものが入っている前提で
ルーティングしようとしてしまうので、


Trying to get property of non-object


オブジェクトじゃないものから受け渡される 500エラー
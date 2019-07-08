# DB接続　について


ここの処理の流れを


DBとlaravelの接続をするには
作成したユーザーに対して権限を与える


DB作成

mysql -u root //MySQLに接続 
create database 'db_name'; //DB作成 
show databases; //DBが作成されたか確認 




ユーザーを作成しデータベースに権限を
//ユーザー作成。
create user 'user_name’@‘localhost’ identified by 'password'; 
// %はワイルドカードで、どんなホスト名がここに入ってもOKということになる。

//ユーザーに権限を付与。
GRANT ALL ON db_name .* TO 'user_name’@‘localhost’; 

//どんな権限がどこに付与されているのか確認。
show grants for 'user’@‘localhost’; 

//設定を確実に反映させる。
flush privileges 





Mysql 8の認証方式の変更

alter user 'username’@‘localhost’ identified with mysql_native_password by 'password';


php artisan migrate





重要！！！

**## .envの変更を反映させる**
.envを変更した後に、こちらを実行すると反映されます。 
php artisan config:cache



_https://hirona-bys.hatenablog.com/entry/2019/02/05/152610_
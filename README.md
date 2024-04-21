# subject-220420

## Apache の設定ファイルの構文チェック
```
httpd -t
```


## MySQL の設定
### C:\xampp\mysql\bin\my.ini

![image](https://user-images.githubusercontent.com/1501327/156976420-7b22dfbb-96e9-4d79-ad49-b5e7dba1845e.png)

22/04/20
```
## UTF 8 Settings
#init-connect=\'SET NAMES utf8\'
#collation_server=utf8_unicode_ci
character_set_server=utf8
#skip-character-set-client-handshake
#character_sets-dir="C:/xampp/mysql/share/charsets"
sql_mode=NO_ZERO_IN_DATE,NO_ZERO_DATE,NO_ENGINE_SUBSTITUTION
log_bin_trust_function_creators=1

character-set-server=utf8mb4
collation-server=utf8mb4_general_ci
[mysqldump]
max_allowed_packet=16M
```

# C:\xampp\mysql\bin で cmd を実行( カレントで処理 )

## ログイン
```
mysql -h localhost -u root --password=
```

## データベース作成
```sql
create database lightbox;
exit
```

## インポート
### lightbox.sql をダウンロード
```
mysql -h localhost -u root -D lightbox --password= < lightbox.sql
```

## VSCode MySQL ツール
![image](https://user-images.githubusercontent.com/1501327/164140853-2bd4ab93-14c1-40ed-ae74-f90983125fd7.png)


## さくらエディタのインストール

![image](https://user-images.githubusercontent.com/1501327/164349789-0c0bc1c2-4b3d-4d81-8270-065ab5d754ce.png)



## ODBC ドライバ( MySQL 用 32ビット )のインストール

![image](https://user-images.githubusercontent.com/1501327/164349950-7b868130-5045-4f47-9179-d297cfaa96ee.png)

![image](https://user-images.githubusercontent.com/1501327/164349987-24ea469d-bd25-456a-906e-44ff1510f479.png)



## SQL の窓のインストールと MySQL で動作確認

![image](https://user-images.githubusercontent.com/1501327/164350059-237e1337-3614-489a-be57-d663ebd3c131.png)

![image](https://user-images.githubusercontent.com/1501327/164350117-dbc7afaa-d970-4b69-a3a0-926b1762fe98.png)


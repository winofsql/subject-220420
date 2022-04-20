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


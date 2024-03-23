# 課題3

###  APサーバーについて調べる

---

* APサーバーの確認

```
$ rails s
```

![APサーバー確認](lecture-img/aplog.png)
APサーバーは、pumaでした。

<br>
<br>

* バージョンを確認

```
$ puma
```

![APサーバー](lecture-img/puma.png)
pumaのバージョンは5.6.8

<br>
<br>

* puma(APサーバー)を停止するとアプリが起動しなくなり、再起動させるとアプリが動作することを確認。

![サーバー停止](lecture-img/apstop.png)

<br>
<br>

---


### BDサーバーについて調べる

---

* DBサーバーの確認

```
$ rails dbconsole
```

![DBサーバー](lecture-img/dblog.png)
DBサーバーは、MySQLで、バージョンは8.0.36でした。

<br>
<br>

* MySQL(DBサーバー)を停止すると、エラーが出て処理がうまくいかない様子。

```
$ sudo service mysqld stop
```

![DBサーバーの停止](lecture-img/mysql_stop.png)

<br>
<br>

* MySQL(DBサーバー)を再起動させると、アプリが正常に動作しました。

```
$ sudo service mysqld restart
```

![DBサーバーの再起動](lecture-img/mysql_restart.png)

<br>
<br>

* Gemfileを確認すると、構成管理ツールはBundlerが使用され、様々なGemファイルが管理されていました。

![構成ファイル](lecture-img/bundler.png)


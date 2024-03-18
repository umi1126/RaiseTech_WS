# 課題3

###  APサーバーについて調べる

---

* APサーバーの確認

```
$ rails s
```

![APサーバー確認](/RaiseTech_WS/lecture-img/aplog.png)
APサーバーは、pumaでした。

<br>
<br>
<br>

* バージョンを確認

```
$ puma
```

![APサーバー](/RaiseTech_WS/lecture-img/puma.png)
pumaのバージョンは5.6.8

<br>
<br>
<br>

* puma(APサーバー)を停止するとアプリが起動しなくなり、再起動させるとアプリが動作することを確認。

![サーバー停止](/RaiseTech_WS/lecture-img/apstop.png)

<br>
<br>
<br>

---


### BDサーバーについて調べる

---

* DBサーバーの確認

```
$ rails dbconsole
```

![DBサーバー](/RaiseTech_WS/lecture-img/dblog.png)
DBサーバーは、MySQLで、バージョンは8.0.36でした。

<br>
<br>
<br>

* MySQL(DBサーバー)を停止すると、エラーが出て処理がうまくいかない様子。
![DBサーバーの停止](RaiseTech_WS/lecture-img/mysql_stop.png)

<br>
<br>
<br>

* MySQL(DBサーバー)を再起動させると、アプリが正常に動作しました。
![DBサーバーの再起動](RaiseTech_WS/lecture-img/mysql_restart.png)

<br>
<br>
<br>

* Railsの構成管理ツールは
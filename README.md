# SQLインジェクションによる認証回避練習問題

SQLインジェクションによる認証回避はよく見かけますが、たいていのケースではパスワードが平文保存されている前提です。この練習問題はパスワードがハッシュ値で保存されているので、よくある ' OR 'a'='a などではうまくいきません。adminでログインできれば、攻撃成功です。

# インストール方法
Dockerがインストールしてある環境で、以下でインストール可能です。

```
$ git clone https://github.com/ockeghem/SQLi-to-bypass-auth.git
$ cd SQLi-to-bypass-auth
$ docker compose up -d
```

http://localhost:7890/ にアクセスしてください。ログインフォームが表示されます。adminでログインできれば攻撃成功です。

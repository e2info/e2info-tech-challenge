# Step7 Web API

情報提供を目的としたWeb APIを実装します。

## 作業内容

* Restful Web APIの実装

## 前提条件

* masterブランチから派生した以下のブランチを作成し、作業を進めること
```
e2info-[lastname]-step7
```

* Markdown形式のAPIドキュメントを作成すること
    * ```/e2info-[lastname]/doc/api.md```

## 仕様

* WebアクセスによるAPI
* レスポンスはJson形式
* /api以下へのアクセスにはBasic認証によるアクセス制限がかかること
    * Basic認証はApache等のミドルウェア層ではなく、PHPで設定すること
    
### プロフィールの取得
    
* /api/profileへのGetアクセスで以下の情報が返却されること
    * /api/profile/[userid]でもよい

```
HTTP/1.1 200 OK
Content-Type: application/json
{
    "name": "山田 太郎",
    "email": "yamada@example.com",
    "profile": "食べることがすき\r\n寝ることも好き"
}
```

※上記以外の項目（ユーザーIDなど）を含めても良い    

### 年表の取得

* /api/historyへのGetアクセスで以下の情報が返却されること
    * /api/history/[userid]でもよい
```
HTTP/1.1 200 OK
Content-Type: application/json
{
    "history" : [
        {
            "year" : 2010,
            "month" : 12,
            "text" : "ブランコから落ちて骨折",
            "tension" : 40,
            "photo" : "https://example.com/20101201/xxxx.jpg"
        },
        {
            "year" : 2011,
            "month" : 3,
            "text" : "結婚",
            "tension" : 100,
            "photo" : "https://example.com/201110301/xxxx.jpg"
        }
    ]
}
```
※上記以外の項目（ユーザーIDなど）を含めても良い

## ゴール

* Basic認証を正常に通過した場合、ログイン済みユーザーではなくても利用できること
* APIでユーザープロフィールを取得できること
* APIで年表を取得できること

## 成果物

以下の成果物をgitにPUSHする

* 動作するプログラムソースコード(```/e2info-[lastname]/src```)
* APIドキュメント(```/e2info-[lastname]/doc/api.md```)

gitリポジトリが以下の状態になっていること

* ```master```ブランチに対して```e2info-[lastname]-step7```ブランチのプルリクエストが送られている状態
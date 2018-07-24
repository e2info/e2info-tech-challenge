# Step1 準備

以下の手順に従って事前準備を進めて下さい

## PhpStormの用意

* [PhpStorm](https://www.jetbrains.com/phpstorm/download/)をダウンロードしてインストールします。ライセンスは会社より貸与します

### 完了条件

* PhpStormが起動したら完了

## Webサーバ／データベースの用意

* [XAMPP](https://www.apachefriends.org/jp/index.html)最新版をインストール
    * すでにインストール済みで開発要件を満たす環境がある場合はインストール不要

### 完了条件

* XAMPPコントロールパネルよりApache,MySQLを起動できることを確認
* ブラウザで以下のURLが表示できたら完了
    * http://localhost/
    * http://localhost/phpMyAdmin/
* ※すでに業務で利用しており、設定変更により上記が表示できない場合は完了としてよい

![git](https://raw.githubusercontent.com/e2info/e2info-tech-challenge/master/Challenge1/images/step1_xampp.png)

## gitクライアントのインストール

* [Git GUI Clients](https://git-scm.com/download/gui/windows)をインストールします

### 完了条件

* コマンドプロンプト／PowerShell／terminalでgitコマンドが実行できることを確認

![git](https://raw.githubusercontent.com/e2info/e2info-tech-challenge/master/Challenge1/images/step1_gitcuiclient.png)

## リポジトリからプロジェクトをpull

* gitリポジトリからプロジェクトをpullする（リポジトリ情報は個別に連絡）
* masterブランチからブランチを作成する
    * ブランチ名はe2info-[lastname]-step1とする
* 作成したブランチにディレクトリを作成する
    * ディレクトリ名は、e2info-[lastname]とする
* 作成したディレクトリにファイルを作成する
    * ファイル名は、README.mdとする。内容は空でよい
* 上記のファイルをgitリポジトリにPUSHした後、masterブランチに対してプルリクエストを送る

## ゴール

* PhpStorm上にプロジェクトが完成すること

## 成果物

gitリポジトリが以下の状態になっていること

* e2info-[lastname]-step1ブランチにe2info-[lastname]/README.mdが存在する
* masterブランチに対してe2info-[lastname]-step1ブランチのプルリクエストが送られている状態
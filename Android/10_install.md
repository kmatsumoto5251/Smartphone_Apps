## Android端末へのインストール（Google Play以外）

作成したAndroidアプリをGoogle Playに申請する前に実機（Android端末）にインストールします。
仕組みとしてはapkファイルをスマホ内に持ち込みし、実行すればよいようです。

最も簡単な方法はパソコンとスマホをUSBで直結する方法と思われます。
この手順を作成している環境下ではパソコンとスマホを繋ぐことができないため、手順を以下を参照してください。
- [実機（Android端末）へのインストールと動作確認【Androidアプリ開発】](https://pg.akihiro-takeda.com/android-install-apk/)

ここではapkファイルの作成までを実施します。

## 目次
- [apkファイルを作成する](#anchor1)
- [apkファイルを実機へコピーする](#anchor2)
- [他のインストール方法](#anchor3)

<a id="anchor1"></a>
## apkファイルを作成する
- 対象のプロジェクトを開く
- ビルド > Genarate Signed Bundle... をクリックする。

  ![image](https://user-images.githubusercontent.com/87625373/213069405-0138d6f0-4b3d-4032-963c-2322bbb4a855.png)

- APK を選択して次へをクリックする。

  ![image](https://user-images.githubusercontent.com/87625373/213069852-ec4327df-3f4a-4209-b569-47dda0127f7b.png)

- Key store path > Create newをクリックする。

  apkファイルをインストールする際にはapkが署名済みである必要があり、そのために必要なアプリ署名鍵を作成します。詳細は[こちら](https://qiita.com/WisteriaWave/items/dd6f74b24852438a90df)

  ![image](https://user-images.githubusercontent.com/87625373/213070436-50b5f7b1-c2e8-48d2-9043-c4826c88d5e0.png)

- Key store path欄のフォルダマークをクリックする。

  ![image](https://user-images.githubusercontent.com/87625373/213070736-62376dfd-22ea-4b03-ab0f-b248eb612c23.png)

- キーの保存先とキーストア名を指定して次へをクリックする。
  
  今回はアプリケーションフォルダの直下にアプリケーションと同じ名前で保存する。
  
  ![image](https://user-images.githubusercontent.com/87625373/213071220-5ce70177-5ce0-47fa-88cb-f7e078ebad59.png)

- パスワード、エイリアス、証明書情報など任意の値を入力する。

  ※パスワードはapkファイルの再作成時に必要となるため忘れないようにしましょう。 
  
  ※Aliasについては[こちら](https://blog.aroundit.net/android-keystore-alias/)を参照してください。
  
  ※証明書欄はいずれか1つへの入力が必須となっています。本番で作成するときは正しい情報を入力しましょう。

  ![image](https://user-images.githubusercontent.com/87625373/213075382-96e18790-f821-4f09-93db-4969eddc6bbb.png)

- 次へをクリックする。

  ![image](https://user-images.githubusercontent.com/87625373/213075492-22e43f60-bd90-46f3-9339-1b633339ad05.png)

- debugを選択して完了をクリックする。

  ※releaseはおそらくGoogle Playにアップロードする際に選択するものです。このあたりは[こちら](https://developer.android.com/studio/publish/app-signing?hl=ja)を参照してください。

  ![image](https://user-images.githubusercontent.com/87625373/213076648-0f54e52b-15dc-47b5-aec2-312f8a1f44fc.png)


<a id="anchor2"></a>
## apkファイルを実機へコピーする

<a id="anchor3"></a>
## 他のインストール方法
メール、オンラインストレージ、Webページ公開などいくつか方法があるようですが、
結局はapkファイルをダウンロードできればいいようです。

 - https://qiita.com/kusokamayarou/items/9397cc15e8dfe4d7510a

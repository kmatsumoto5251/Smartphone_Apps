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

 ![image](https://user-images.githubusercontent.com/87625373/213070436-50b5f7b1-c2e8-48d2-9043-c4826c88d5e0.png)

- Key store path欄のフォルダマークをクリックする。

 ![image](https://user-images.githubusercontent.com/87625373/213070736-62376dfd-22ea-4b03-ab0f-b248eb612c23.png)

- キーの保存先と名前を指定して次へをクリックする。
  今回はアプリケーションフォルダの直下にアプリケーションと同じ名前で保存する。
  
  ![image](https://user-images.githubusercontent.com/87625373/213071220-5ce70177-5ce0-47fa-88cb-f7e078ebad59.png)


<a id="anchor2"></a>
## apkファイルを実機へコピーする

<a id="anchor3"></a>
## 他のインストール方法
メール、オンラインストレージ、Webページ公開などいくつか方法があるようですが、
結局はapkファイルをダウンロードできればいいようです。

 - https://qiita.com/kusokamayarou/items/9397cc15e8dfe4d7510a

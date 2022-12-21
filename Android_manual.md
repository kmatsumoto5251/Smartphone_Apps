## Andoroidアプリを作成する（Windows）
## 目次
- [Android Studioインストール](#anchor1)
- [Android Studio日本語化](#anchor2)
- [プロジェクト作成](#anchor3)

- [メモ](#anchor99)

<a id="anchor1"></a>
## Android Studioインストール
- [https://developer.android.com/studio/](https://developer.android.com/studio/)にアクセスする
- 「Download Android Studio」をクリックする
- ポップアップ画面の最下部にある同意のチェックボックスにチェックしダウンロードボタンをクリックする
- ダウンロードしたインストーラーを実行してインストールする（インストールメニューは全てデフォルト）
- インストールが完了したら自動起動する（コンフィグインポートをポップアップで聞いてくるが必要ない）
- セットアップ画面で「No Send」選択しNext、「Standard」を選択しNext、お好みのUIを選択してNextをクリックする
- ライセンス同意画面で各ライセンスをクリック後、右下の「Accept」をクリックする（左側のツリーのトップ階層をクリックして選択する）
- 全てのライセンスで「Accept」をクリックすると「Finish」が活性かするためクリックしてインストールを完了する

<a id="anchor2"></a>
## Android Studio日本語化
- Android Studioを起動する
- 画面左下の歯車 > aboutをクリックし、バージョンを確認する

　　![image](https://user-images.githubusercontent.com/87625373/208794823-21b746d8-899b-451e-a465-849a38111bde.png)
　　![image](https://user-images.githubusercontent.com/87625373/208795180-9e6c35bb-6bd2-40ec-8a89-fd5353562655.png)

- [https://plugins.jetbrains.com/plugin/13964-japanese-language-pack------/versions](https://plugins.jetbrains.com/plugin/13964-japanese-language-pack------/versions)にアクセスする
- バージョンが一致するプラグインをダウンロードする（メジャーバージョンのみ一致すればよい）

　　![image](https://user-images.githubusercontent.com/87625373/208795818-2c21a8c4-6e28-4b61-92e8-241bc92142e1.png)

- ダウンロードしたzipファイルを解凍し、「C:\Program Files\Android\Android Studio\plugins」にフォルダごと配置する
- Android Studio の Plugins > 右上の歯車 > Install Plugin from Disk を選択する

　　![image](https://user-images.githubusercontent.com/87625373/208794100-c1d7e6e5-942e-4483-bfb1-2511743273b3.png)

- プラグイン配置したフォルダ内にある「ja.xxx.jar」を選択し、OKをクリックする

　　![image](https://user-images.githubusercontent.com/87625373/208796680-2f47eb23-489e-4836-b001-110467e76747.png)

- 「Restart IDE」と表示されるので、Android Studio を再起動する
- 再起動が完了すると日本語になる

<a id="anchor3"></a>
## プロジェクト作成
- プロジェクト > New Projectをクリックする
- 画面レイアウトのテンプレートを任意で選択し次へをクリックする
- Nameにアプリ名、Package nameにパッケージ名を入力して完了をクリックする
  - パッケージ名はストアに表示されるため、プロジェクトの規則に従って適切な名称とする
- プロジェクトが作成されるとネットワーク環境によってはサーバ証明書の警告が表示されるため、内容を確認し「承認」をクリックする
  - 複数回表示される可能性あり
- インターネット接続にプロキシサーバを経由する場合はプロキシ設定を行う
  - プロキシ設定を行わないとhttp403エラーなどが発生する可能性あり
- ファイル > 設定 > システム設定 > HTTPプロキシ に遷移し、IPアドレスやポート番号を入力後、OKをクリックする

    ![image](https://user-images.githubusercontent.com/87625373/208830056-f54e6b07-59c4-4c8f-8a44-1fc9a1644871.png)

- プロキシサーバの情報はコマンドプロンプトやPowerShellから以下のコマンドで確認が可能
```
netsh winhttp show proxy
```
- プロキシサーバ設定後、下記のようなネットワーク関連のエラーが発生する場合はLAN内のSSLデコード除外などが必要となる

    ![image](https://user-images.githubusercontent.com/87625373/208832806-330b3082-b8b2-4256-9db7-dfaf2e8a880f.png)


<a id="anchor99"></a>
## メモ

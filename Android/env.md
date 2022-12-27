## Andoroidアプリを作成するその１（Windows）
## 環境構築
## 目次
- [Android Studioインストール](#anchor1)
- [Android Studio日本語化](#anchor2)
- [SDK追加](#anchor3)

- [メモ](#anchor99)

<a id="anchor1"></a>
## Android Studioインストール
- [https://developer.android.com/studio/](https://developer.android.com/studio/)にアクセスする。
- 「Download Android Studio」をクリックする。
- ポップアップ画面の最下部にある同意のチェックボックスにチェックしダウンロードボタンをクリックする。
- ダウンロードしたインストーラーを実行してインストールする。
  - インストールメニューは全てデフォルト
- インストールが完了したら自動起動する。
  - コンフィグインポートをポップアップで聞いてくるが必要ない。
- セットアップ画面で「No Send」選択しNext、「Standard」を選択しNext、お好みのUIを選択してNextをクリックする。
- ライセンス同意画面で各ライセンスをクリック後、右下の「Accept」をクリックする。
  - 左側のツリーのトップ階層をクリックして選択する。
- 全てのライセンスで「Accept」をクリックすると「Finish」が活性化するためクリックしてインストールを完了する。

<a id="anchor2"></a>
## Android Studio日本語化
- Android Studioを起動する。
- 画面左下の歯車 > aboutをクリックし、バージョンを確認する。

　　![image](https://user-images.githubusercontent.com/87625373/208794823-21b746d8-899b-451e-a465-849a38111bde.png)
　　![image](https://user-images.githubusercontent.com/87625373/208795180-9e6c35bb-6bd2-40ec-8a89-fd5353562655.png)

- [https://plugins.jetbrains.com/plugin/13964-japanese-language-pack------/versions](https://plugins.jetbrains.com/plugin/13964-japanese-language-pack------/versions)にアクセスする。
- バージョンが一致するプラグインをダウンロードする（メジャーバージョンのみ一致すればよい）。

　　![image](https://user-images.githubusercontent.com/87625373/208795818-2c21a8c4-6e28-4b61-92e8-241bc92142e1.png)

- ダウンロードしたzipファイルを解凍し、「C:\Program Files\Android\Android Studio\plugins」にフォルダごと配置する。
- Android Studio の Plugins > 右上の歯車 > Install Plugin from Disk を選択する。

　　![image](https://user-images.githubusercontent.com/87625373/208794100-c1d7e6e5-942e-4483-bfb1-2511743273b3.png)

- プラグイン配置したフォルダ内にある「ja.xxx.jar」を選択し、OKをクリックする。

　　![image](https://user-images.githubusercontent.com/87625373/208796680-2f47eb23-489e-4836-b001-110467e76747.png)

- 「Restart IDE」と表示されるので、Android Studio を再起動する。
- 再起動が完了すると日本語になる。

<a id="anchor3"></a>
## SDK追加
SDKの追加が必要な場合は以下のメニューからダウンロード・インストールする。
- プロジェクト作成前
  - 画面右上のケバブメニュー（3つの点）からSDK Managerをクリックする。
  - 右下のShow Package Details にチェックを入れて詳細を表示する。
  - 上部のタブでPlatform/Toolsなど遷移し、必要なパッケージにチェックを入れOKをクリックする。
  - 確認ダイアログでOKをクリックするとダウンロード・インストールが始まる。
  - 完了画面で完了をクリックし終了する。

![image](https://user-images.githubusercontent.com/87625373/209634147-d09ed3c9-8cfd-4e6a-8e01-49df391ec483.png)

![image](https://user-images.githubusercontent.com/87625373/209634422-d8c37b29-9a5b-4b5b-83cb-ac4497884bcf.png)

- プロジェクト作成後
  - 左上のファイル > 設定 > システム設定 > Android SDKに遷移する。
  - あとはプロジェクト作成前と同じ。

<a id="anchor99"></a>
## メモ
- [Android Developers](https://developer.android.com/?hl=ja)
- [Kotolinで始めるAndroidアプリ入門](https://qiita.com/k-ysd/items/4efdecdfd60afe333a3a)
- [新規プロジェクトを作成する方法](https://original-game.com/develop-android-app-2/)
- [エミュレータの作成とコード実行](https://pouhon.net/android-avd/4698/)
- [エミュレータのシステム要件と操作方法](https://developer.android.com/studio/run/emulator?hl=ja#requirements)
- [HUAWEI製デバイスで実機テストするための準備](https://pouhon.net/android-connection/4619/)
- [KotlinのWeb実行環境](https://developer.android.com/training/kotlinplayground?hl=ja)
- [Androidアプリの画面作っていくには](https://qiita.com/cawmate_hitomi/items/35ae7c218090ae8f60b1)
- [Android Stdioプロジェクトのディレクトリ構成](http://gmonsoon.blog96.fc2.com/blog-entry-107.html)

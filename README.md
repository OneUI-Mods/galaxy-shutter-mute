# Galaxy Shutter Mute

Galaxyのカメラのシャッター音設定を切り替えるアプリです。導入・権限設定には[Galaxy Shutter Mute Manager](https://github.com/OneUI-Mods/galaxy-shutter-mute-manager)を使用します。

## 対応環境

Samsung Galaxyの対応するシャッター音設定が利用できる環境向けです。従来の確認範囲はAndroid 9〜16 / One UI 1〜8.5です。Android 17での動作確認は、このREADME更新では追加していません。端末・地域・カメラアプリの版により設定が利用できない場合があります。

## インストール・使い方

1. [ManagerのReleases](https://github.com/OneUI-Mods/galaxy-shutter-mute-manager/releases)からManagerをインストールします。
2. Shizukuを起動し、Managerへのアクセスを許可します。
3. ManagerからGalaxy Shutter Muteをインストールして、必要な権限を付与します。
4. Galaxy Shutter Muteを開き、シャッター音のスイッチを変更します。

本体アプリは対象の設定へアクセスする都合で古い互換設定を使用します。新しいAndroidでは通常のAPKインストールが制限されるため、Manager経由で導入してください。

## 配布・停止

本体の配布物は[Releases](https://github.com/OneUI-Mods/galaxy-shutter-mute/releases)にあります。設定を戻す場合はスイッチをONにしてください。設定が反映されない場合は、対応するカメラアプリを開き直して確認します。

## 開発者向け・ライセンス

ビルド、内部構造、検証方法は[開発者向けガイド](docs/development.md)に分けています。不具合報告は[Issues](https://github.com/OneUI-Mods/galaxy-shutter-mute/issues)へ、端末・OS・対象アプリの版と再現手順を添えてください。

本体のライセンスは[LICENSE](LICENSE)、依存ライブラリの表記はアプリ内または同梱の第三者ライセンスを参照してください。Samsungの公式アプリではありません。

[OneUI Modsのアプリ一覧](https://github.com/OneUI-Mods)

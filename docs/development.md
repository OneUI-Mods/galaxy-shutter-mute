# 開発者向けガイド

利用者向けの説明は[README](../README.md)にあります。公開先は[galaxy-shutter-mute](https://github.com/OneUI-Mods/galaxy-shutter-mute)です。

## ソースとビルド

Android SDKのコンパイル対象は35です。JDK・Gradle・依存関係の版は、リポジトリ内のGradle設定とwrapperを基準にしてください。

```sh
./gradlew :app:assembleRelease
```

配布にはrelease variantを使い、配布鍵による署名とAPKの構造を検証します。debug APKやテスト専用画面を含むAPKを配布しません。署名鍵・パスワード・端末ログ・外部アプリのバイナリをGitへ追加しないでください。

## 設計・検証

未確認のOS・端末・対象アプリの版を対応済みと記載しないでください。実測・実機確認と、コード上で準備した互換処理を区別して記録します。READMEは機能、導入、更新、制約を説明し、内部API・フック・測定値はこのディレクトリに記録します。

本体のtargetSdk 21はシャッター音設定への互換性のため意図的に維持されています。コンパイルSDKと混同せず、対象設定へのアクセスを確認せずに引き上げないでください。

## ドキュメント一覧

- [実装と過去の検証の補足](architecture-and-validation.md)

## 2026-10-30のビルド確認

Android実装は元からKotlinです。固定されていたGradle版のwrapper一式を追加し、releaseビルドとlintを確認しました。API 21でも動く権限確認と、Shizukuによる特権付与を表すlint注記を整理しました。
端末上の画面操作・音声操作は実施していません。SDK・設定・署名の識別は変更しません。

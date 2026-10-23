---
title: "Flutter のコードプッシュを Shorebird と Codemagic で自動化する"
url: "https://blog.codemagic.io/how-to-set-up-flutter-code-push-with-shorebird-and-codemagic-cicd-jpn/"
date: "2025-02-25"
feed_url: "https://blog.codemagic.io/index.xml"
---
本記事は、佐藤将来が執筆しました。 この記事で出来るようになること Shorebird を Codemagic へ連携することで、ストアからのインストールを必要とせずに Dart コードの変更をコードプッシュするワークフローを組み込むことが出来るようになります。 以下の例では、 アプリの UI 上に表示しているテキストの変更が即時反映されています： Shorebird とは Shorebird は Flutter アプリケーション専用のコードプッシュ機能を提供するサービスです。コードプッシュによって、開発者はストアへのリリースを必要とせずにユーザーのデバイスに直接アップデートを反映することができます。つまり、Shorebird を活用することで、Flutter 開発者は Play Store や App Store といった各プラットフォーム上でのガイドラインに準拠しながら効率的にアプリの Dart コードのアップデートを管理することが出来ます。 Shorebird 初期設定 まずは、Shorebird へサインアップして、以下の手順で CLI ツールを使ってみましょう： こちら より、 Shorebird の無料アカウントを作成します。 Shorebird の CLI を自身の PC へインストールしましょう。 以下のコマンドをターミナルで実行します： curl --proto 

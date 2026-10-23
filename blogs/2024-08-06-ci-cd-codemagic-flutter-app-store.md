---
title: "CI/CD ツール(Codemagic) を使って Flutter アプリを App Store へ公開する"
url: "https://blog.codemagic.io/publishing-flutter-apps-to-appstore-jpn/"
date: "2024-08-06"
feed_url: "https://blog.codemagic.io/index.xml"
---
本記事は、佐藤将来が執筆しました。 本記事では、CI/CD ツールである Codemagic を用いてApp Store へ Flutter アプリをリリースする手順をご紹介します。 「現状、Xcode を用いて手動で App Store Connect へアプリをアップロードしているけど、その手順を簡略化したい」という方に是非読んでいただけると幸いです🙌 この記事で出来るようになること この記事の手順に沿ってセットアップしていただくと、App Store Connect への対象のアプリのアップロードを自動化出来るようになります。 つまり、日々の開発の際には以下のような流れでストアへのリリースを行えるようになります： GitHub 上でトリガーとなる PR をマージする(下記例では develop → main ブランチへのマージ時) 数分後、Codemagic 上でアプリのビルドが完了する App Store Connect 上にアプリがアップロードされ、リリース申請が行えるようになる 前提条件 本記事の手順に沿っていただくには、以下のものが事前に必要です： macOS の搭載されたPC Apple Developer Program へのメンバーシップ登録 App Store Connect 上でのアプリ登録 事前準備 まず事前準備として、Codemagic のワークフロー作

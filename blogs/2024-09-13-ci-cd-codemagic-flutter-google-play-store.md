---
title: "CI/CD ツール(Codemagic) を使って Flutter アプリを Google Play Store へ公開する"
url: "https://blog.codemagic.io/publishing-flutter-apps-to-playstore-jpn/"
date: "2024-09-13"
feed_url: "https://blog.codemagic.io/index.xml"
---
本記事は、佐藤将来が執筆しました。 本記事では、CI/CD ツールである Codemagic を用いてGoogle Play Store へ Flutter アプリをリリースする手順をご紹介します。 「現状、手動で Google Play へアプリをアップロードしているけど、その手順を簡略化したい」という方に是非読んでいただけると幸いです🙌 この記事で出来るようになること この記事の手順に沿ってセットアップしていただくと、Google Play への Flutter 製の Android 用アプリのアップロードを自動化出来るようになります。 つまり、日々の開発の際には以下のような流れでストアへのリリースを行えるようになります： GitHub 上でトリガーとなる PR をマージする(下記例では develop → main ブランチへのマージ時) 数分後、Codemagic 上でアプリのビルドが完了する Google Play 上にアプリがアップロードされ、リリース申請へ進めるようになる 前提条件 本記事の手順に沿っていただくには、以下のものが事前に必要です。 Google Play デベロッパーアカウントの登録 Google Play ストアでのリリースには、有料の アカウント登録 が必要になります。 Google Play コンソール 上へのアプリ登録 Google Play コ

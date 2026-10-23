---
title: "Mac を使わずに iOS アプリを Flutter と Codemagic で配布する"
url: "https://blog.codemagic.io/how-to-develop-and-distribute-ios-apps-without-mac-with-flutter-codemagic_jpn/"
date: "2024-11-25"
feed_url: "https://blog.codemagic.io/index.xml"
---
本記事は、佐藤将来 が執筆しました。 Mac コンピューター無しで iOS アプリを開発することは難しいと思われるかもしれません。実際この状況がすぐに変わる兆しはありませんが、Mac を持っていなくてもアプリ開発者が iOS アプリをビルドして App Store にリリースする方法は存在します。この投稿では、Linux または Windows コンピュータしか持っていない場合でも Flutter と Codemagic を使用して iOS アプリをビルドして公開する方法をご紹介します。 この記事の手順と Codemagic を使用して Flutter アプリを iOS 向けにビルドすることは可能ですが、iOS シミュレーターや実機でアプリをデバッグする場合には Mac が必要になります。 必要なもの まず事前に以下のものを準備しましょう： Apple Developer Program へのメンバーシップ登録 アプリのコード署名や公開を行うために必要です。 iOS デバイス 本記事の手順を終えた後には、アプリの挙動を実際にテストするためのデバイス用意することをお勧めします。 iOS アプリの署名や Apple App Store への公開が初めての方には、 専用チュートリアル （英語）をご用意しています。 まず本題に入る前に、今回の作業を通して何が出来るようになるのかを明確にしま

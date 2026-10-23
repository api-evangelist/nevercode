---
title: "Codemagic CI/CD でリリースノートを自動更新する"
url: "https://blog.codemagic.io/automate-release-notes-jpn/"
date: "2025-04-30"
feed_url: "https://blog.codemagic.io/index.xml"
---
本記事は、佐藤将来が執筆しました。 ストアへのレビュー提出時、毎回同じ文言のリリースノートを記入するのを少し面倒に感じたことはありませんか？ この記事では、そんなちょっとした手間を自動化する方法をご紹介します。 とても簡単に導入出来るため、ぜひご覧下さい💡 この記事で出来るようになること 以下のように、Git 管理したリリースノート用のテキストファイルがストアへのアプリアップロード時に自動で記入されるようになります。 Codemagic とは まず初めに、簡単に Codemagic についてご紹介します。 Codemagic とは、Flutter 開発に特化した、テストやビルド、デプロイを自動化する CI/CD ツールです。iOS, Android や React Native など、様々なプロジェクトにおいて利用できますが、Flutter プロジェクトでは Workflow Editor という GUI ツールを用いることが出来ます。これにより、yaml ファイルなどの専用ファイルの作成を必要とせずに直感的な操作による開発が可能です。 個人利用であれば無料で使い始めることが出来、十分な無料枠(毎月500分)を提供しています。料金の詳細については こちら をご覧ください。 前提条件 リリース済みのアプリが App Store Connect 及び Google Play Conso

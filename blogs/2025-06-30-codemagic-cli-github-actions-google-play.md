---
title: "Codemagic CLI ツールと GitHub Actions で Google Play へアプリをデプロイする"
url: "https://blog.codemagic.io/deploy-your-app-to-google-play-with-codemagic-cli-tools-and-github-actions-jpn/"
date: "2025-06-30"
feed_url: "https://blog.codemagic.io/index.xml"
---
本記事は、佐藤将来が執筆しました。 以前の記事にて、 Codemagic CLI ツールと GitHub Actions で App Store Connect へアプリをデプロイする方法 について解説しました。Codemagic チームはこの CLI ツールを継続的に改良し、Google Play Console への Android リリース機能を拡張しました。 Codemagic CLI ツールとは Codemagic CLI ツール は、Codemagic の CI/CD プラットフォームを内部的に動かしている無料のオープンソースツールです。このツールの利用により、アプリのビルド、コード署名、ストアへのデプロイメントなど、モバイル開発ワークフローの効率化が可能になります。 このツールはクロスプラットフォーム対応であり、iOS と Android の両方のプロジェクトで同じツールセットを使用できます。Codemagic のクラウドベースの CI/CD サービスとは異なり、こちらの CLI ツールでは開発マシン上でローカルにビルドを実行したり、GitHub Actions などの任意の CI/CD プラットフォームと統合したりと柔軟な開発が可能です。ユーザーフレンドリーな設計を意識しており、初心者から上級者まで幅広い層に利用をお勧め出来ます。 この記事では、この CLI ツール

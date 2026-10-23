---
title: "Codemagic CLI ツールと GitHub Actions で App Store Connect へアプリをデプロイする"
url: "https://blog.codemagic.io/deploy-your-app-to-app-store-with-codemagic-cli-tools-and-github-actions-jpn/"
date: "2025-05-31"
feed_url: "https://blog.codemagic.io/index.xml"
---
本記事は、佐藤将来が執筆しました。 モバイルアプリのビルドからコード署名、公開までのプロセスは、特に QA エンジニアとビルドを共有しているような大規模なチームにおいては、多くの手間と時間を要します。そこで Codemagic では、最小限の設定でワークフロー全体を自動化できるクラウドベースの CI/CD サービスを提供しています。しかし、Codemagic の機能をローカル環境や他の CI/CD 環境（例：GitHub Actions）で使いたい場合にはどうすれば良いでしょう？そんな時に便利なのが Codemagic CLI ツール です。 Codemagic CLI ツールとは Codemagic CLI ツール は、Codemagic の CI/CD サービスの裏側で使われている、無料かつオープンソースのコマンドラインツール群です。このツールを使うことで、モバイルアプリ開発に関する様々な作業（ビルド、コード署名、公開など）に簡単に着手することが出来ます。ドキュメントも充実しており、Codemagic チームや外部のコントリビューターによって常に最新の状態に保たれています。 Codemagic CLI ツールの大きな特徴は、プラットフォームに依存しない点にあります。複数の OS で利用でき、iOS・Android の両方に対応しているため、ストアごとに異なるツールを用意する必要

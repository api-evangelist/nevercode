---
title: "CI/CD ビルド速度ベンチマーク：Codemagic vs GitHub Actions vs Bitrise"
url: "https://blog.codemagic.io/build-speed-benchmark-comparison-jpn/"
date: "2026-03-27"
feed_url: "https://blog.codemagic.io/index.xml"
---
本記事は、佐藤将来が執筆しました。 CI/CD を導入しているチームにとって、ビルドマシンのスペックは開発の生産性を大きく左右する要素です。ビルドが速ければ修正・検証のサイクルが短くなり、開発全体のスピードアップにつながります。しかし、各 CI/CD サービスが実際にどの程度の速度を出すのかは、同じ条件で比較してみないとなかなかわかりません。 本記事では、同一の Flutter プロジェクトを用いて GitHub Actions 、 Bitrise 、 Codemagic の iOS ビルド速度を実測し、コストパフォーマンスまで含めて比較します。 ベンチマークの条件 テスト対象 今回のベンチマークでは、オープンソースの瞑想アプリ Medito を使用しました。多くのレビューがストアに寄せられており、プロダクションレベルの Flutter アプリとして十分な規模のプロジェクトかと思います。 測定方法 各サービスで flutter build ios --release --no-codesign 相当の iOS リリースビルドを実行し、ビルド開始から終了までの所要時間を比較対象としました。 各ビルドのログは公開リンクで確認可能です。 ビルド速度ベンチマーク それでは、各サービスのベンチマーク結果を見ていきましょう。 GitHub Actions GitHub Actions は Gi

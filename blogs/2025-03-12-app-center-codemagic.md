---
title: "さようなら App Center、はじめまして Codemagic！"
url: "https://blog.codemagic.io/goodbye-app-center-hello-codemagic-jpn/"
date: "2025-03-12"
feed_url: "https://blog.codemagic.io/index.xml"
---
本記事は、同内容の 英語版記事 を 佐藤将来 が翻訳したものになります。 Microsoft で多くのユーザーを抱えた CI/CD プラットフォームである App Center は、2025 年 3 月 31 日にサービスを終了することが発表されました。これにより、多くのモバイル開発者やチームが代替策を探すこととなりました。おそらく最も影響を受けるのは、CodePush による OTA (Over The Air) アップデートのために App Center に依存していた React Native コミュニティでしょう。 この記事では、App Center とは何か、開発者に好まれていた点及び好まれていなかったであろう点について簡単にご説明します。その上で、モバイルアプリのビルドやテスト、ストアへのデプロイ、CodePush による OTA アップデートの送信にも対応した優れた代替手段として Codemagic について説明します。 App Center について App Center は、Thomas Dohmke 氏によって設立され 2011 年にリリースされた HockeyApp というオープンソースプロジェクトとして始まりました。当初は、TestFlight を通じた正式なアプリ提出プロセスを経ることなく、iOS アプリを第三者に迅速に配布する方法として考案されました。 

# KataGo棋譜検索システム
- 現在katagoのページから棋譜を少しずつ集めていますが、アーカイブがあるようなので、それを利用する方法を模索中
- sgfノード管理にモジュール変数を使っていたのをやめて、配列にしました。　メモリ上限問題解決。

Katagoのrating自己対戦の棋譜を集めていますが、数百-数千visitsで打たれた棋譜（人間でいえば第一感、５秒碁ぐらいのイメージでしょうか）なので、
正解を打っているとは限りませんが、人間よりははるかに強いです。

寝る前に自動再生で眺めて強くなろう！というコンセプトで作っています。

本プログラムにはAIを動かす機能はありません。あくまで、棋譜鑑賞、検索用です。

[My Study Logs on GitHub Pages](https://hosinobu.github.io)

***
囲碁AI、KataGoのサイト  
https://katagotraining.org/

KataGoを動かす検討ソフトを導入する場合、seventeenさんが開発されている、BadukMegapackがおすすめ。私もこれを使っています。  
https://github.com/wonsiks/BadukMegapack

# Katago棋譜検索システム
- 現在katagoのページから棋譜を少しずつ集めていますが、アーカイブがあるようなので、それを利用する方法を模索中
- 特定条件下で、メモリが確保できなくなる問題について調査中。（発生した場合はPCを再起動すると直る場合あります）
- 64bit版への移行を検討中
  - DLLを変更が必要？（hspext, hspda, hspinet)
  - 各モジュールを６４bitに対応させる　(mref i,2 -> mref i, 4), memcpyの計算が変わる？

Katagoのrating自己対戦の棋譜を集めていますが、わずか数百visitsで打たれた（人間でいえば第一感、５秒碁ぐらい？）の棋譜とのことですので、
完全に正解を打っているわけではありません。
lizzieなどの検討ソフトで深く読ませると最善ではないことが分かることもありますが、人間よりははるかに強いです。

寝る前に自動再生で眺めて強くなろう！というコンセプトで作っています

***
囲碁AI、KataGoのサイト  
https://katagotraining.org/

KataGoを動かす検討ソフトを導入する場合、こちらのメガパックがおすすめ。私もこれを使っています。  
https://github.com/wonsiks/BadukMegapack

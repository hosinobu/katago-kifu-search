---
title: "検索機能についての悩み。いずれかの表現"
date: 2025-03-10
layout: post
---

この地点とこの地点（またはエリア内）のいずれかに黒石一つある。という表現はできるようにしたいと思えている。

また、ここに黒またはここに白みたいな表現もあれば便利だなぁ。

石情報自体をグループ化できるようにしてしまうのがいいのか？

んで検索中そこに見つかったら、パターンからその石グループを取り除いて、パターン自体もキューに突っ込むようにすればいいのかな。

あ、よく考えたら今もパターンはキューに突っ込んでるからパターンから取り除くってのをすればいいだけか。案外簡単そう？？？？わからん。

まあ、焦らないでいいか。

しかし石の色情報もメモ化してるから取り除いたらわけわからんことになるなｗｗｗうーむｗ

パターンから取り除くのではなく、
石情報のメモ化のときに、その石（グループ）がカウント済みかの情報もメモ化しちゃえばいいのかしら？

まだ未メモ化状態の時に着手地点の色情報を参照する際、えーーと。。何を記録したらいいんだろ。

今まではヒットしたか。　そしてそこが空点も許容してるかどうかを記録してたな。

ヒット済みかどうかと、そうでないときはヒットしたかと、空点許容（カウントしない）の３つを記録するとすると。。。

うーんと。

でもその情報をグループ内に共有しないといけないよなぁ。

ヒット済みのところにもう一度ヒットしたらfalseを返さないといけないから。。うーん。

ヒット済みかどうかはパターン側に書き込むか！

・・・・うん。いけそうなきがしてきた。

まとめると。石情報をグループ化する（１個のものでも）ヒット済みの石グループかのフラグをパターンに持たせる。でいいかな。

検索時にヒット済みの石グループをヒットすると即falseでいいかしら？

相変わらず抜き後系のことは考えてない（笑）

せっかくsgfモジュールにbitboardを組み込んだんだけどなぁ。bitboardを使った検索はまた１から書かないとだから後回しかなぁ（汗汗

３２bitだとあまり速くならなそうと思ってるのもある。やってみたら爆速だったとかもありそうだけどｗ

パターンの構造が変わるから、言うて色々変更しないとあかんなー。

またUI的にも指定方法がわかるようにせなあかんし。

ん－ｗどうしよ

あー。グループが矩形をまたがっちゃう可能性があるな―。うーん。石自体にグループ番号を持たせるべきかな。

今日はここまで。

---
title: 罪滅ぼし8月号
created_at: 2019-08-30
tags: 
 - workshop
 - coding
category: develop
---

## 👆何やねんこれ?

この記事は罪滅ぼしとなっております

こんにちは、shuta(did0es) です

何の罪滅ぼしかと言うと、まず僕は<a href="http://www.rcc.ritsumei.ac.jp/" target="_blank">RCC</a>という団体(まあ大学のサークルみたいなもんです)に所属しています。

そこでは「夏期勉強会」という、有志が色々情報系(別に作曲とかイラスト制作みたいな感じで多岐にわたります)のことを夏季休業期間に教えるイベントがあります。普通のコミュニティや社内の勉強会みたいなものです

<br>

んで、僕は今回ゴリゴリ先輩風を吹かせてやろうと思い「Creative Coding(Generative Art)」をテーマにやっていきをしていたのですが、予定管理や人生に失敗しそれどころでは無くなったので罪滅ぼしをしようと記事を書いています、いま

<br>

> Q. この記事はRCC会員向けなんですか？

> A. いいえ　こうやってブログにしているので不特定な読者を想定しています。質問や投石等お気軽にこちらまで → <a href="https://twitter.com/did0es" target="_blank">@did0es</a>

<br>

## 内容の要約

これは「Creative Coding(Generative Art)」についての僕の考えや全く知らない人が入門するために催す予定だった内容を記事として記しています。

Creative Codingと銘打ちつつも内容はほぼ全部「Generative Art」の話です。Generative Artとは何か全くわからない人向けにちょっとしたワークショップのような形でGenerative Artについてのお話しをします

大きく以下の構成に分けられます

- Generative Artとは何なのか

- 何故僕がGenerative Artに没頭していたのか

- ワークショップ

対象読者は
　
- RCCで僕の勉強会に参加登録していた方(本当に申し訳ないです、これで矛をお収め下さい)

- Generative Artに興味があるものの、ぼく/わたしってどうしたらいいですか？ な人

- 多少なりともコード書いたことがある人(プログラミングの初歩さえ分かれば読めます、なぜならそこまでコーディングの話しないので)

です

既にGenerative Artに精通している方からすると退屈な内容になるかもしれません。ざーっと流して何かの暇つぶしにでもどうぞ。マサカリを投げるために準備運動でも良いです、生暖かく見守って下さい。

コーヒーやお茶の用意はできましたか？割とくどくど色々書くつもりなので眠くなったらこれらのものを顔にかけたりしながら読んで下さい。
## 執筆中(未定)
<!--
## 本体

### Generative Artとは何なのか

まずは「Generative Art」という言葉でgoogle画像検索をかけてみましょう(作品見たほうが説明はやいので)

> 検索結果：<a href="https://www.google.com/search?rlz=1C5CHFA_enJP843JP843&biw=2100&bih=1173&tbm=isch&sa=1&ei=g2VpXam9IYjh-AaN_67QAw&q=Generative+Art&oq=Generative+Art&gs_l=img.3..35i39j0i30l9.1651.4032..4269...0.0..0.79.441.6......0....1..gws-wiz-img.......0i8i30.Y-0sVbcM6to&ved=0ahUKEwjpiurJl6vkAhWIMN4KHY2_CzoQ4dUDCAY&uact=5" target="_blank">https://www.google.com/search?rlz=1C5CHFA_enJP843JP843&biw=2100&bih=1173&tbm=isch&sa=1&ei=g2VpXam9IYjh-AaN_67QAw&q=Generative+Art&oq=Generative+Art&gs_l=img.3..35i39j0i30l9.1651.4032..4269...0.0..0.79.441.6......0....1..gws-wiz-img.......0i8i30.Y-0sVbcM6to&ved=0ahUKEwjpiurJl6vkAhWIMN4KHY2_CzoQ4dUDCAY&uact=5</a>

ズラーッと並んでいますが大体こういう感じのものを想像していただくと良いです。

Generative Art とはそういった活動で制作された作品や芸術活動自体を指しています。

<br>

なんと言ってもGenerative Artで肝要なのは、

1. コードを書く

2. 予測不可能性

3. 芸術と呼ぶこと

以上の3つだと僕は思っています。

思っています とか言っちゃってるんですが、大体ここでする話は Matt Pearson著の <a href="https://www.amazon.co.jp/%E6%99%AE%E5%8F%8A%E7%89%88-%E3%82%B8%E3%82%A7%E3%83%8D%E3%83%A9%E3%83%86%E3%82%A3%E3%83%96%E3%83%BB%E3%82%A2%E3%83%BC%E3%83%88%E2%80%95Processing%E3%81%AB%E3%82%88%E3%82%8B%E5%AE%9F%E8%B7%B5%E3%82%AC%E3%82%A4%E3%83%89-%E3%83%9E%E3%83%83%E3%83%88%E3%83%BB%E3%83%94%E3%82%A2%E3%82%BD%E3%83%B3/dp/4861009634/ref=sr_1_1?__mk_ja_JP=%E3%82%AB%E3%82%BF%E3%82%AB%E3%83%8A&keywords=%E3%83%9E%E3%83%83%E3%83%88%E3%83%94%E3%82%A2%E3%82%BD%E3%83%B3&qid=1567185191&s=gateway&sr=8-1" target="_blank">ジェネラティブ・アート - Processingによる実践ガイド </a> で言及されているものに影響を受けています。(もし、というかGenerative Artをがっつりやりたいならまずこの本を読むことを勧めます。また色々後述します)

<br>

では、3つそれぞれの説明に入ります。

1. コードを書く

先程の検索結果のような画像はおそらく、クリエイターが Illustrator や Photoshop などのツールで制作した と思われるかもしれませんが、僕が今話しているGenerative Artはそのようなツールを用いたものではなく **コードを書き、計算機に生成させた作品** のようなものを指しています。

コードを書くことで計算機に処理を行わせることができます。また、計算機は人間の脳ではほとんどできないような回数の繰り返しや複雑な条件分岐を処理することができます。これらを利用してGenerative Artをやっていき することができます。
> 別にコードを用いないでやるGenerative Artもあるみたいなんですが、僕はやったことないです。ただ アルゴリズムを組む 部分をGUIでやるみたいな感じらしいので大体やってること一緒です、おそらく

ただし、計算機は無限回の実行には弱いです。筐体のスペックによってはかなりの計算量を回せたりしますが、流石に無限回実行を行うのは無理です。

Generative Artはとりあえず無限回繰り返してやろう みたいな感じでやると破滅します、なぜなら計算機でやってるので。

また、ひたすら繰り返すだけだと面白みがなかったりするので、うまくやっていきをする必要があります(フラクタル構造などを利用する場合は別ですが)

ここで `2.` に繋がります

2. 予測不可能性

Generative Artをする前の最初で最後の忠告なんですが、 **なんでも思い通りになると思わないほうが良い** です。

思い通りに作品を生成できるような猛者は確かにいます(しらんけど)が、最初からそれを求めてやると本当に 無理 という感じになってくるので、やめたほうが良いです。これは色々な先人の方も言っているのでマジです、というかGenerative Artやるとよ〜〜〜〜〜く分かります。

もし思い通りに何か作りたいならデザインツールの使い方を覚える方がよっぽど生産的だし仕事とかにも役立つのでさっさとこんな記事読むのやめてYouTubeでツールの使い方でも見て、自分で好きにやって下さい。

<br>

話戻るんですが、**大体思い通りにならない** ことがGenerative Artの醍醐味だったりします。

は？ という感じになると思うので少し説明を加えますが、こんな コーディングで計算機にただ処理させるプログラムを生成すること を何が芸術したらしめているのかと言えば、

**時々、いい感じの軌跡や模様が生まれてうれしいので満足するまでいっぱいやる**

みたいなざっくりしたアレです。

砕け過ぎな感じがしますが、この ***時々いい感じ*** と ***満足するまでいっぱいやる*** みたいなのが、どうも創作じみてて僕はGenerative Artだなぁみたいな気分になります。

<br>

先程、`1.` で計算機は複雑な処理ができると言いました。つまりそれは人間の予想を外れた結果をもたらします。

ただ、やはり繰り返しや条件分岐だけだと味気ないので、適宜 ノイズ や 数式 を利用することになります。

ここで使用する ノイズ も 数式 もプログラマー(つまり、Generative Artをするあなたです)が選択でき、なんなら自作することもできます。

この2つによって、さらにプログラムは予測不可能なものに変わっていくのでかなり興味深い結果を得られるようになります。

興味深い結果を得られるまで、ひたすら改良し、自分の好きな満足するところで止める このような工程が非常に芸術性を持っていると僕は思います。

3. 芸術と呼ぶこと

これはもうなんかコーディング云々の話でもなんでもないので流しながらで良いです。

これは上で紹介した ジェネラティブ・アート - Processingによる実践ガイド でも言及されていたのですが、簡単に言うと

「今から私は 自分の行動 を 芸術 とします！」

と言ってしまえば、歯を磨いたりご飯食べたりするようなことでさえもすべて芸術活動となり、ご飯を食べることで発生したゴミは芸術作品と呼べ得ます(←本当に？)(なんかシュールレアリスムの行き着く先みたいで面白いですね)

つまり自分の行っている、そのエディタ上の文字を目を細めてにらめっこする工程を芸術活動だとすることでArtが成立します(多分)。

とにかく自分はこういう感じでArtをしています、いま みたいな感じで後半のワークショップもやっていきましょう。

形や雰囲気から入るのも大事です。Generative Artしてるぞ〜みたいな気持ちでコード書いてると楽しいですよ

---

### 何故僕がGenerative Artに没頭していたのか

ワークショップに入る前に、僕がGenerative Artをはじめた話をちょっとだけします。隙あらば自分語りしたい病気なので許して下さい

何回も挙げまくってる <a href="https://www.amazon.co.jp/%E6%99%AE%E5%8F%8A%E7%89%88-%E3%82%B8%E3%82%A7%E3%83%8D%E3%83%A9%E3%83%86%E3%82%A3%E3%83%96%E3%83%BB%E3%82%A2%E3%83%BC%E3%83%88%E2%80%95Processing%E3%81%AB%E3%82%88%E3%82%8B%E5%AE%9F%E8%B7%B5%E3%82%AC%E3%82%A4%E3%83%89-%E3%83%9E%E3%83%83%E3%83%88%E3%83%BB%E3%83%94%E3%82%A2%E3%82%BD%E3%83%B3/dp/4861009634/ref=sr_1_1?__mk_ja_JP=%E3%82%AB%E3%82%BF%E3%82%AB%E3%83%8A&keywords=%E3%83%9E%E3%83%83%E3%83%88%E3%83%94%E3%82%A2%E3%82%BD%E3%83%B3&qid=1567185191&s=gateway&sr=8-1" target="_blank">例のジェネラティブアートの本</a> やその他の本や記事でも度々<a href="https://processing.org/" target="_blank">Processing</a>という言語が使用されています。

僕の通う大学ではプログラミング入門にこの言語が使用されています。

ただ、正直なところ授業ではあまり面白みを感じれなかったので、あれこれ調べているうちにProcessingでGenerative Artをやっている人の作品に行き着き、見様見真似で始めました。

情報系に進学したのが、そういう(主に当初は音声でしたが)クリエイティブな活動をPCを使ってやっていきたい という意思だったのでProcessingでのGenerative Artはかなりハマる感じの内容でした。

また大学入学時点では、てんで素人だった僕でもProcessingは非常に扱いやすくすんなり入門もできたため、かなり :good: でやってました。

こんな感じでGenerative Artに没頭し毎日溶かしていました

また、作った作品を公開するためにWebフロントやらの技術回りもガジガジ囓り始めました。(最近はもうこればっかりになっていますが)

> こちらは作品を並べたWebサイトです、ちらほらProcessingでのGenerative Art作品があります → <a href="https://did0es.me/garelly" target="_blank">GARELLY</a>

また、これは僕のGenerative Artの話とはあまり関係ないんですが、最近良く(というか前から) プログラミング初心者は〜をやるべき みたいな ~~不毛な~~ 論争をよく見かけます。僕は結構ProcessingでのGenerative Artを勧めます。(不毛と言いつつも論争に参加していくお気持ち)

なぜなら、ドキュメントや入門記事、入門書が結構充実している(最後らへんに僕が良いなと思った記事や書籍をいくつか紹介します)のと、結果が目に見てわかって楽しいので。あとはProcessing自体Javaという ~~36億のデバイスを汚す~~ かなり有名で実績のある言語をベースに作られているのでいい感じにプログラミングの基礎やそれ以上の内容に手をかけることもできます。

芸術や画像とかの加工に興味がある人には特に楽しくやれると思うので是非この記事を見かけた初心者の方は次のワークショップで一度手を動かしてProcessingを書いてみてください。プログラミング学習の一助になれば幸いです。

既にProcessingを書いたことがある方でも、こういう感じのことができるんだ〜みたいなアレで読んで頂けると嬉しいです。

---

### ワークショップ(執筆中)

ここからは やっていき が始まります

今回作るものはこんな感じです

[いい感じの画像1]

[いい感じの画像2]

[いい感じの画像3]

~~正直そこら辺の記事とか本読みあさってできるのだとアレなので、ぐぇぇぇと体内からひねり出してアレをアレしてやっています~~

無からひねり出すのが苦行過ぎたのでGitHubをあれこれ巡って見つけたいい感じの表現を色々インポートしたみたいなアレをやっていきます。(ちゃんと最後に参考のリンク貼ります)

後はコード自体のバグは是非 @did0es に石投げて貰えれば良いんですが、 *ハード関連(特にmacのGPUらへんのバグとか)* は僕に聞かないで下さい、ハード層力(ぢから)が皆無なので

はじめていきます

---

まずはProcessingのインストールからはじめていきます、そんな仰々しいアレじゃないので楽に終わります

Windows/Linux/macOS も大体一緒な感じだと思われます、僕はmacOSを使用しているのでmacを想定して進めていきます

Windows/Linux の方は [こちら]() の記事を参考に進めて下さい(未検証です、すみません でも多分大丈夫)

<br>

1. 　Processing入りzipのダウンロード

<a href="https://processing.org/download/" target="_blank">https://processing.org/download/</a> から os に合ったzipをダウンロードします(macなのでmac用を落としてきます)

2. 起動

落としてきたzipを展開し、中に入っている`Processing`を`アプリケーション`に移動させます

おわり

<br>

java うんぬんのエラーで死んでしまった場合は <a href="https://www.oracle.com/java/technologies/javase-jsp-downloads.html" target="_blank">https://www.oracle.com/java/technologies/javase-jsp-downloads.html</a> からjavaの実行環境諸々インストーラを取ってきて自分で頑張ってください　応援しています

それでもなお、なんやこいつ動かんやんけ！クソが！！！！！！みたい感じになっていたらPCを叩く前に <a href="https://twitter.com/did0es" target="_blank">@did0es</a> まで連絡をば

---

ではざっくりProcessingについての文法をやっていきます

これまでに何か他の言語(手続き型とか)を書いたことある方であればそう難しいものではない というか多分簡単な部類に入ると思います

最初に`型`のお話しです。コードを書く際に以下のような`変数`を宣言し、使用できます

これは勝手で申し訳という感じなんですが、そんなに(僕が)使わない型は省いています(全部見たい人は [公式リファレンス](https://processing.org/reference/) 見てください、英語ですが )

```processing
// 数値を扱う
int numInt = 1;
float numFloat = 0.05;

// 文字を扱う
char chr = "a";
String str = "元気笑顔出社";

// 配列
int[] intArray = { 1, 10, 100, 1000 };
float[] floatArray = { 0.1, 0.02, 0.03, 0.04 };
char chr[] = "おうちかえりたい"; // String型とほぼ同じと思って貰っていいです

// 色を扱う
color rgb = color(255, 255, 255);
color colorCode = #FFFFFF;
```
まあこれだけあればとりあえず困らないです、`color`型があるのがちょっと一見変わっています。

`=`を使用すると宣言した変数に、変数の型と同じ型のデータを代入することができます。

宣言した変数に初めてデータを入れることを`初期化`と呼びます。

<br>

次にProcessingのローカルルールみたいなものの説明をします。

こう書いたらこう動くみたいなのを並べていきます

```processing
// 初期化用関数
void setup() {
    // 800*800のキャンバスの表示
    size(800, 800);
    // 背景色の設定
    background(0, 0, 0);
}

// Main関数(Loop)
void draw() {
    // 白で塗りつぶす
    fill(255, 255, 255);
    // 中心に大きさ10の円を描画
    ellipse(width / 2, height / 2, 10, 10);
}

// キーボード入力がトリガーで実行される関数
void keyPressed() {
    // 何かしらの処理
}
```

この2つが主要な関数です。`setup()` はコードを実行した際に`初めに一度だけ`呼び出される関数です

そのため`setup()`には初期化の処理やキャンバス(絵を描画するところ)を表示する処理を記述します。

`draw()` は実行すると無限ループで中の処理が呼び出されます。

これを利用して簡単にアニメーションを実装していくことができます

ループが煩わしいのであれば`setup()`の内部に `noLoop()` を記述することでループを止められ、一回だけ実行に変更できます。

また `noLoop()` を書くと実行するたびに ウインドウ閉じてまた実行してウインドウ閉じて... みたいな不毛をする羽目になるので `keyPressed()` の内部に以下のような記述をすると任意の入力に応じて `draw()` を再度呼び出すことができます

```processing
// 初期化用関数
void setup() {
    // 800*800のキャンバスの表示
    size(800, 800);
    // 背景色の設定
    background(0, 0, 0);
}

// Main関数(Loop)
void draw() {
    // 白で塗りつぶす
    fill(255, 255, 255);
    // 中心に大きさ10の円を描画
    ellipse(width / 2, height / 2, 10, 10);
}

// キーボード入力がトリガーで実行される関数
void keyPressed() {
    // これなんか書いておいて
}
```
-->
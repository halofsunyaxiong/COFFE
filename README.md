# SUNCOFFEEについての説明書

## 前書き

- 本文の「プログラムについて」は主にindex.htmlとstyle.cssを図解します。javascriptのwow.jsの紹介もあります。
- 自分の能力は不足なので、ミスや良いアイデアがあれば、わたくしにご指摘しください。
- このプロフィールサイトのプログラミング言語はHTMLとcssです。
- このプログラムはCSS3.0 grid layout に使われたので、下記のブラウザの実行環境で実行できません。
  - Internet Explorer 11 以下
  - Edge 15 以下
  - Firefox 52 以下
  - Safari とiOS Safari 10.1 以下
  - Chrome 57 以下
  - Samsung Internet 6.2 以下
- このプログラムの開発環境は Visual Studio Code です。

## プログラムについて

- 作者：孫亜雄
- 内容：SUNCOFFEEのサイトなど。
### プログラムのファイル

-  contact.html
-  index.html
-  menu.html
-  order.html
-  README.md
- css:

      -animate.css
      -contact.css
      -index.css
      -menu.css
      -order.css
      -reset.css
      -style.css

- images:

      -1.jpeg
      -2.jpeg
      -3.jpeg
      -americano.jpg
      -bg.jpg
      -CafeBreve.jpg
      -CaffèLatte.jpg
      -Cappuccino.jpg
      -coffee0.jpg
      -EspressoConPanna.jpg
      -facebook.png
      -flatwhite.jpg
      -instagram.png
      -IrishCoffee.jpg
      -line.png
      -logo1.png
      -logo2.png
      -macchiato.jpg
      -seat.jpg
      -tiktok.png
      -VienneseCoffee.jpg
      -coffee_shop.jpg

- javascript:

        js.js
        wow.min.js


        
- index.htmlとstyle.cssのプログラムの構造

![プログラムの構造の図解](https://i.imgur.com/5zTD1Zr.png)

- この図はプログラムおおざっぱなりんかくです。
- 主にcss3.0のflexとgirdに使われた。



## CSSのanimate.css, javascriptのwow.js について説明
### 1.animate.css と　wow.js 導入する方法。

<br>


- [animate.css](https://animate.style/)からanimate.cssダウンロードします。offlineで導入 
```
<link rel="stylesheet" href="animate.css">

```
  - あるいはonlineで導入
``` 
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css">
  
```

<br>


- [wow.js](https://wowjs.uk/)からwow.jsダウンロードします。offlineで導入

```
<script src="wow.min.js"></script>
```



  - あるいはonlineで導入

```
<script src="https://cdnjs.cloudflare.com/ajax/libs/wow/1.1.2/wow.min.js"></script>

```

### 2. low elementにanimate.css と　wow.js の　class特徴を　追加します。

#### 01.追加し方法。 
　　　
- まず、low elementに class を入力します。
```
<p class="">low elementにanimate.cssとwow.jsのclass特徴を追加し方法 </p>
```
- 次は、animate_animated animate_動作名詞 wow　を入力します。動作名詞はいろいろがあるので、[animate.css](https://animate.style/)のサイトをご覧ください。
- 他の特徴を追加することもできます。
     - data-wow-duration="1.0s"指定した秒数かけて要素を表示させることができる。
     - data-wow-delay="1.0s"スクロールで要素まで達したとき、指定した秒数、遅らせて表示させる。
     - data-wow-offset="10" 画面に表示されてから、アニメーションを開始する距離を指定。基準位置は画面下になる。- - - -
     - data-wow-iteration="10" 指定した回数分、アニメーションを繰り返し動作させる。


```
<p class="animate_animated animate_fadeInLeft" data-wow-iteration="3" data-wow-duration="5.0s">low elementにanimate.cssとwow.jsのclass特徴を追加し方法 </p>

```

- 最後は、scriptの中に実例をリセットします。
```
<script>
    new WOW().init();
</script>
```





#### 02.　large elements　と　root elements にanimate.css と　wow.js の　class特徴を　追加することできません。

```
<!--これはダメです!!!!!! -->
<body>
  <main class="animate_animated animate_fadeInLeft">
     <!-- your coding -->
  </main>
</body>

```
```
<!--これはダメです!!!!!! -->
== <body class="animate_animated animate_fadeInLeft"> ==
  <main>
    <!-- your coding -->
  </main>
</body>

```
#### 03.例文

 ```
<!DOCTYPE html>
<html lang="ja">
<head>
  <title>wow.js+animate.css</title>
  <meta charset="UTF-8">
  
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css">
  <!-- もしくは <link rel="stylesheet" href="animate.css"> -->
</head>
<body>
  <h1 class="text-center">wow.jsとanimate.cssを使ったテスト</h1>
  <h2 class="animate_animated animate_fadeInLeft" data-wow-iteration="3" data-wow-duration="5.0s">bounceInUp!</h2>
  <h2 class="animate_animated animate_fadeInRight" data-wow-iteration="1000000" data-wow-duration="1.0s">fadeInLeftBig!</h2>

</body>
<script src="https://cdnjs.cloudflare.com/ajax/libs/wow/1.1.2/wow.min.js"></script>
<!-- もしくは <script src="wow.min.js"></script> -->
<script>
    new WOW().init();
</script>

</html>
````


### 開発のツール について

- VS CODE 
- Copilot
- Microsoft Whitleboard
- Imgur
- Pexels

## 著作権
- seat.jpg coffee_shop.jpgの著作権はpexels.comのライセンスに基づいて。
- link.jpg、facebook.jpg、ins.jpg、tiktok.jpgの著作権はgoogle deveioper fontsです。
- 参考した文章や説明書などの著作権の所有は元作者だけです。
## 参考

1. [READMEについて](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes)
2. [MAKEDOWNの記法](https://gist.github.com/mignonstyle/083c9e1651d7734f84c99b8cf49d57fa)
3. [CSS GRID LAYOUT](https://developer.mozilla.org/ja/docs/Web/CSS/grid)
4. [CSS FLEX LAYOUT](https://developer.mozilla.org/ja/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox)
5. [IMGUR.COM](https://imgur.com/)
6. [PEXELS.COM](https://www.pexels.com/ja-jp/)
7. [wow.js](https://wowjs.uk/)
8. [animate.css](https://animate.style/)
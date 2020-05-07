# bali-wp

> 2020/05/07

# HTML

## サイト構成

- top
    - 表示構成
- 404
    - よくあるパターンを探す
- 会社情報
    - よくあるパターン探す
- News
- property
    - テンプレで入れるもの
- land
    - テンプレで入れるもの
- 問い合わせ


## 想定

- 実直につくる
    - 一部コピペで

## 制作メモ

### タグ

[参考サイト](https://qiita.com/maccotsan/items/20c6ea274b0190dc2c05)

- `nav`
    - リストにする
    - ヘッダーメニュー、サイドメニュー、パンくずリスト


``` nav.html
<nav>
  <ul>
    <li><a href='/'>サイトトップ</li>
    <li><a href='/about'>このサイトについて</li>
    <li><a href='/contact'>お問い合わせ</li>
  </ul>
</nav>
```


    - 複数のセクションを置く場合
        - `section`要素
        - `aside`要素



``` multi.html
<!-- section -->
<nav>
  <section>
    <h3>カテゴリーから選ぶ</h3>
    <ul>
      <li><a href='/category/all'>全て</li>
      <li><a href='/category/book'>書籍</li>
      <li><a href='/category/game'>ゲーム</li>
    </ul>
  </section>
  <section>
    <h3>売り上げランキング</h3>
    <ul>
      <li><a href='/ranking/all'>全て</li>
      <li><a href='/ranking/book'>書籍</li>
      <li><a href='/ranking/game'>ゲーム</li>
    </ul>
  </section>
</nav>

<!-- aside -->
<aside>
  <nav>
    <h3>カテゴリーから選ぶ</h3>
    <ul>
      <li><a href='/category/all'>全て</li>
      <li><a href='/category/book'>書籍</li>
      <li><a href='/category/game'>ゲーム</li>
    </ul>
  </nav>
  <nav>
    <h3>売り上げランキング</h3>
    <ul>
      <li><a href='/ranking/all'>全て</li>
      <li><a href='/ranking/book'>書籍</li>
      <li><a href='/ranking/game'>ゲーム</li>
    </ul>
  </nav>
</aside>
```




- `article`
    - 単独の記事としてふさわしいか？



``` article.html
<article>
  <h1>記事タイトル</h1>
  <p>本文</p>
  <section>
    <h2>この記事へのコメント</h2>
    <article>
      <h3>名無しさん</h3>
      <p>...</p>
    </article>
  </section>
</article>
```


- `section`
    - 見出しをつける




``` section.html
<section>
  <h1>見出し</h1>
  <p>本文</p>
</section>
```

# CSS

## 構成

`import url();` で連携させる

- style
    - Responsive
- reboot

### reboot

とりあえず、reboot が慣れてるので入れてる


## 想定

- WordPress のcss 構成
- Js よりも、css で、動かす
- flexbox でやる


# Js

## 思いつきメモ

- なるべくVanilla で書きたい？
- jQuery がどこまで影響があるか
- WordPress 移行時に設定ができればいいかも？
    - 基本css で解決できそうなものはcssで
- 検索関係は、要検討
    - WordPress に入ってからかな？
- 早く表示させるのはここかな？

# WordPress

- 分割することの想定
- N予備校 のやつやる
- ログイン処理
    - 情報をまとめる
    - どんな情報いれる？
        - どのsns と連携させるか
    - セキュリティ関係

## テスト置き場

- プラグイン？
- ディレクトリとか、ちゃんとしないと


## メモ

- ブロックエディタだと、オリジナルはなぜ面倒？


# その他

## アイコン

- png かsvg か
    - フリーなやつ

## 参考サイト

- 要素の洗い出し
- リンクまとめる

## 参照デザイン

- リンク貼る


## 対応ブラウザ

- 要確認

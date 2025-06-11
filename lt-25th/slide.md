---
marp: true
theme: default
paginate: true
size: 16:9
style: |
  /* 基本スタイル */
  section {
    color: #2c3e50;
    font-family: 'Helvetica Neue', Arial, sans-serif;
  }

  /* タイトルスライドは画像背景 */
  section.title-slide {
    background-image: url('./images/Slide1.jpg');
    background-color:rgba(255,255,255,0.2);
    background-blend-mode:lighten;
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    color: #fff;
  }

  /* その他のスライドは明るい背景 */
  section:not(.title-slide) {
    background: 
      linear-gradient(135deg, rgba(199, 224, 247, 0.95) 0%, rgba(230, 245, 255, 0.95) 50%, rgba(178, 220, 252, 0.9) 100%),
      url('./images/Slide2.jpg');
    background-size: cover, cover;
    background-position: center, center;
    background-repeat: no-repeat, no-repeat;
    position: relative;
    color: #2c3e50;
  }

  section:not(.title-slide)::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-image: 
      linear-gradient(90deg, #3498db 0%, #3498db 20%, transparent 20%, transparent 30%, #3498db 30%, #3498db 50%, transparent 50%, transparent 60%, #3498db 60%, #3498db 80%, transparent 80%),
      linear-gradient(0deg, #3498db 0%, #3498db 10%, transparent 10%, transparent 20%, #3498db 20%, #3498db 30%, transparent 30%);
    background-size: 200px 20px, 20px 200px;
    background-position: 0 20px, 0 0;
    opacity: 0.15;
    pointer-events: none;
  }

  section:not(.title-slide)::after {
    content: '';
    position: absolute;
    top: 0;
    right: 0;
    width: 0;
    height: 0;
    border-left: 200px solid transparent;
    border-top: 100px solid rgba(52, 152, 219, 0.2);
    pointer-events: none;
    z-index: 1;
  }

  /* h1とh2のスタイル */
  h2 {
    position: fixed;
    top: 30px;
    left: 30px;
    font-size: 1.2em;
    margin: 0;
    padding: 10px 20px;
    background: rgba(52, 152, 219, 0.15);
    border-radius: 5px;
    border: 1px solid rgba(52, 152, 219, 0.3);
    z-index: 10;
    color: #2980b9;
    font-weight: 600;
  }

  h1 {
    position: static;
    font-size: 3em;
    text-align: center;
    margin-top: 200px;
    background: none;
    border: none;
    padding: 0;
    color:rgba(255, 194, 53, 0.89);
    font-weight: 700;
  }

  p {
    text-align: center;
    font-size: 2em;
  }

  ul {
    font-size: 1.3em;
    line-height: 1.8;
    color: #2c3e50;
  }

  ul ul {
    font-size: 1em; /* ネストした箇条書きのフォントサイズを統一 */
  }

  li {
    margin-bottom: 15px;
  }

  p.small {
    font-size: 20px;
    z-index: 100;
  }
---

<!-- _class: title-slide -->

# 25卒LT会

中岡暉

---

## 自己紹介

- 名前：中岡暉（なかおかあきら）
- 出身：大阪府高槻市
- 所属：DIGITALIO Tech Unit ユーザーチーム
- 経歴：大阪府立大学 生命環境科学域 緑地環境科学類

<div style="position: absolute; top: 200px; right: 100px; width: 200px; height: auto;">
  <img src="./images/secrets/スクリーンショット 2025-06-11 11.26.05.png" alt="写真" />
</div>

---

## 専攻

- 大学では農学を専攻
- 研究は気象学
  - CH<sub>4</sub>とC<sub>2</sub>H<sub>6</sub>を測定

<div style="display: flex; justify-content: center; height: 300px;">
  <img src="./images/eddy-covariance.png" alt="渦相関法" />
</div>

<p class="small">https://www.cger.nies.go.jp/cgernews/201204/257003.html</p>

---

## 課外活動

- ボランティア団体で活動
  - 中古教科書の回収・再販売
  - 予約サイトや在庫管理システムを立ち上げ
- 大学の情報戦略課でシステム開発のバイトも
  - GoでPHPシステムのリプレイスなど

<div style="position: absolute; top: 200px; right: 100px; width: 150px; height: auto;">
  <img src="./images/sft.png" alt="sft" />
  <p style="position: absolute; font-size: 12px;">https://github.com/study-for-two</p>
</div>
<div style="position: absolute; top: 400px; right: 100px; width: 150px; height: auto;">
  <img src="./images/omu-sp.png" alt="omu-sp" />
  <p style="position: absolute; font-size: 12px;">https://github.com/omu-sp</p>
</div>

---

## 好きな技術

- TypeScript、PHP、Go、Pythonとかは触れます
- Rustもやりたい

<div style="display: flex; justify-content: center; height: 250px;">
  <img src="./images/rust-and-go.png" alt="rust-and-go" />
</div>

<p class="small">https://bitfieldconsulting.com/posts/rust-and-go</p>

---

## 趣味-1

- モンスターハンター
  - PS2以外で出たやつは大体やってる
    - P,P2(G),P3,3(G),4(G),X(X),W(I),Rise(SB),Wilds,F
  - シリーズ通算10,000時間↑

<div style="display: flex; justify-content: center; height: 220px;">
  <img src="./images/dreadking.png" alt="dreadking" />
  <img src="./images/boltreaver.png" alt="boltreaver" />
</div>

<p class="small">https://www.monsterhunter.com/stories2/ja/monster/</p>

---

## 趣味-2

- ドライブ
  - 大学の同期と小旅行に行くのが年2〜3回の楽しみ

<div style="display: flex; justify-content: center; height: 350px;">
  <img src="./images/65050DDF-0BEE-400D-BB0E-8A9914549C20.jpeg" alt="koyasan" />
  <div style="width: 50px;"></div>
  <img src="./images/IMG_2515.png" alt="yamaguchi" />
</div>

---

## 趣味-3

- コーヒー
  - 豆の種類とか焙煎の知識まで知れると面白そう
  - 最近はピーチティーっぽい香りがする豆を買った

<div style="display: flex; justify-content: center; height: 300px;">
  <img src="./images/hario.png" alt="koyasan" />
</div>

<p class="small">https://shop.hariocorp.co.jp/collections/dripper</p>

---

## やりたいこと-1

- 運動習慣をつけたい
  - 部活経験：空手・剣道
  - カジュアルなスポーツがやりたい
  - 最近ボルダリングをちょくちょくやってる

---

## やりたいこと-2

- 仕事はもろもろ頑張る
  - 足りていない知識や経験は積極的に取りに行く
  - 手を動かすだけでなく、座学も大事に

---

## おわりに

<p>これからよろしくお願いします！</p>

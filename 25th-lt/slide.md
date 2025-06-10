---
marp: true
theme: default
paginate: true
size: 16:9
style: |
  /* 基本スタイル */
  section {
    color: white;
    font-family: 'Helvetica Neue', Arial, sans-serif;
  }

  /* タイトルスライドは画像背景 */
  section.title-slide {
    background-image: url('./images/Slide1.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
  }

  /* その他のスライドはCSS背景 */
  section:not(.title-slide) {
    background: 
      linear-gradient(135deg, rgba(44, 62, 80, 0.8) 0%, rgba(52, 73, 94, 0.8) 50%, rgba(44, 62, 80, 0.8) 100%),
      url('./images/Slide2.jpg');
    background-size: cover, cover;
    background-position: center, center;
    background-repeat: no-repeat, no-repeat;
    position: relative;
  }

  section:not(.title-slide)::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-image: 
      linear-gradient(90deg, #00ffcc 0%, #00ffcc 20%, transparent 20%, transparent 30%, #00ffcc 30%, #00ffcc 50%, transparent 50%, transparent 60%, #00ffcc 60%, #00ffcc 80%, transparent 80%),
      linear-gradient(0deg, #00ffcc 0%, #00ffcc 10%, transparent 10%, transparent 20%, #00ffcc 20%, #00ffcc 30%, transparent 30%);
    background-size: 200px 20px, 20px 200px;
    background-position: 0 20px, 0 0;
    opacity: 0.3;
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
    border-top: 100px solid rgba(128, 128, 128, 0.3);
    pointer-events: none;
    z-index: 1;
  }

  /* h1とh2のスタイル */
  h2 {
    position: fixed;
    top: 40px;
    left: 40px;
    font-size: 1.2em;
    margin: 0;
    padding: 10px 20px;
    background: rgba(0, 255, 204, 0.2);
    border-radius: 5px;
    border: 1px solid rgba(0, 255, 204, 0.5);
    z-index: 10;
  }

  h1 {
    position: static;
    font-size: 3em;
    text-align: center;
    margin-top: 200px;
    background: none;
    border: none;
    padding: 0;
    color: rgba(0, 255, 204, 0.5);
  }

  p {
    text-align: center;
    font-size: 2em;
    margin-top: 50px;
  }

  ul {
    font-size: 1.3em;
    line-height: 1.8;
  }

  ul ul {
    font-size: 1em; /* ネストした箇条書きのフォントサイズを統一 */
  }

  li {
    margin-bottom: 15px;
  }

  /* ページ番号のスタイル調整 */
  section:not(.title-slide) footer {
    color: rgba(255, 255, 255, 0.7);
    z-index: 10;
    position: relative;
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

---

## 専攻

- 大学では農学を専攻
  - 理科の教員免許が取りたかった
- 研究は気象学
  - 渦相関法ってガス測定法がございまして
  - 大阪府堺市のCH4、C2H6を定量化

---

## 課外活動

- ボランティア団体で活動
  - 中古教科書の回収・再販売
  - 予約サイトや在庫管理システムに携わる
- 大学の情報戦略課でシステム開発のバイトも
  - Goで既存のPHPシステムをリプレイスするなど

---

## 好きな技術

<div class="large-text">

- TypeScript、PHP、Go、Pythonとかは触れます
- 最近はGoとRustが楽しい

</div>

---

## 趣味-1

- モンスターハンター
  - PS2以外で出たやつは大体やってる
    - P,P2(G),P3,3(G),4(G),X(X),W(I),Rise(SB),Wilds,F
  - シリーズ通算10,000時間↑

---

## 趣味-2

- ドライブ
  - 大学の同期と小旅行に行くのが年2〜3回の楽しみ
  - たぶん夏もどっか行く

---

## 趣味-3

- コーヒー
  - 豆の種類とか焙煎の知識まで入れられると面白そう
  - 最近はピーチティーの香りがするやつを買った

---

## やりたいこと

- 運動習慣をつけたい
  - 空手と剣道しか通らなかったからカジュアルなやつがやりたい
  - 最近ボルダリングをちょくちょくやってる

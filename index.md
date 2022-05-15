---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: "QLANET -量子陣取り-"
#layout: home
#list_title: 更新情報
---

<img src="https://github.com/QuantumComputerStudy/qlanet/blob/main/assets/images/qlanet_logo.PNG?raw=true">

## ゲームの概要
QLANETは9つの量子惑星を巡る二人対戦の陣取りゲームです。  
それぞれの量子惑星に、それを操作するためのゲートカードを使用して自陣営の領地とすることを目指します。  
近年話題の**量子コンピュータ**を背景にデザインされている点が本ゲーム最大の特徴です。  
量子について知らない方でも楽しんでいただけるのでQlanetから量子に興味を持っていただけたら幸いです。

## プレイ人数
2人
## 推奨年齢
8才以上
## プレイ時間
10~15分

## 動画

<iframe width="560" height="315" src="https://www.youtube.com/embed/Ny17yqxpFA4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<!-- [youtube](https://youtu.be/Ny17yqxpFA4) -->

## ルール説明

### 用語

- 量子惑星
    - 場には9つの量子惑星が存在し、プレイヤーは量子惑星を自分の領地とすることで勝利を目指します。
    - 量子惑星には7つの状態「確定０、０、-、+、1、確定1、？」があり、状態「確定1」は1陣営の領地、「確定0」は0陣営の領地を意味します。

| 量子惑星の状態 | | | | | | 
| --- | --- | --- | --- | --- | --- | 
| <img src="https://github.com/QuantumComputerStudy/qlanet/blob/main/assets/images/QubitsZero.png?raw=true"> | <img src="https://github.com/QuantumComputerStudy/qlanet/blob/main/assets/images/QubitsPlus.png?raw=true">| <img src="https://github.com/QuantumComputerStudy/qlanet/blob/main/assets/images/QubitsMinus.png?raw=true">| <img src="https://github.com/QuantumComputerStudy/qlanet/blob/main/assets/images/QubitsOne.png?raw=true">| <img src="https://github.com/QuantumComputerStudy/qlanet/blob/dev_igc/assets/images/QubitsUnknown.png?raw=true"> | <img src="https://github.com/QuantumComputerStudy/qlanet/blob/dev_igc/assets/images/QubitsEntangle.png?raw=true"> |
| 0状態 | ＋状態 | －状態 | 1状態 | 不明な状態 | もつれ状態 | 

- ゲートカード
    - プレイヤーは手札となる「ゲート」を量子惑星に使うことで、量子惑星の状態を操作することができます。
    - 「X,H,Z,M,CX0,CX1,SW,BM」の8種類が存在します。

量子惑星の状態の詳しい説明は以下の通りです。

| 惑星 | 状態 | 意味 |
| ---- | ---- | ---- |
| <img src="https://github.com/QuantumComputerStudy/qlanet/blob/main/assets/images/QubitsZero.png?raw=true"> | 0状態 | ほぼ0陣営の領地 |
| <img src="https://github.com/QuantumComputerStudy/qlanet/blob/main/assets/images/QubitsPlus.png?raw=true"> | ＋状態 | 五分五分の領地。やや0陣営が優勢 |
| <img src="https://github.com/QuantumComputerStudy/qlanet/blob/main/assets/images/QubitsMinus.png?raw=true"> | －状態 | 五分五分の領地。やや1陣営が優勢 |
| <img src="https://github.com/QuantumComputerStudy/qlanet/blob/main/assets/images/QubitsOne.png?raw=true"> | 1状態 | ほぼ1陣営の領地 |
| <img src="https://github.com/QuantumComputerStudy/qlanet/blob/main/assets/images/QubitsUnknown.png?raw=true"> | ？ | 状態がわからない領地 |
| <img src="https://github.com/QuantumComputerStudy/qlanet/blob/main/assets/images/QubitsEntangle.png?raw=true"> | もつれ | 二つの量子惑星が連動している状態 |


### ゲームの準備

- 各プレイヤーに4枚ずつ量子ゲートカードを表向きに配り、9つの量子惑星を並べた状態でゲームを開始します。

### ゲームの流れ
- プレーヤーの手番を繰り返すことでゲームが進行します。手番は手札の量子ゲートカード1枚を量子惑星に作用させた後に手札を1枚ランダムに補充して終了します。次の手番プレーヤーはゲーム中に使用した量子ゲートカードの総コストが少ないプレーヤーになります。手番決定時に総コストが同じ場合は直前に手番だったプレイヤーが連続で手番となります。

(ここにゲーム画面の画像)

- 各ゲートカードの効果とコストは以下の通りです。

| ゲート | 効果 | コスト | カード |
| ---- | ---- | ---- | ---- |
| X   | ０状態と１状態を入れ替える | 6 |  <img src="https://github.com/QuantumComputerStudy/qlanet/blob/main/assets/images/X.png?raw=true"> |
| H   | ＋状態と０状態、または－状態と１状態を入れ替える  | 3 |  <img src="https://github.com/QuantumComputerStudy/qlanet/blob/main/assets/images/H.png?raw=true"> |
| Z   | ＋状態と－状態を入れ替える | 2 |  <img src="https://github.com/QuantumComputerStudy/qlanet/blob/main/assets/images/Z.png?raw=true"> |
| M   | 量子惑星を確定０または確定１にする。１状態または０状態の場合は100%で確定１または確定０にし、＋、－、もつれの場合は50%の確率で確定１か確定０となる。 | 10 | <img src="https://github.com/QuantumComputerStudy/qlanet/blob/main/assets/images/M.png?raw=true"> |
| CX0 | 二つの量子惑星に対して使用する。一つ目の量子惑星が０状態の時二つ目の量子惑星の０状態と１状態を入れ替える。  | 3 |  <img src="https://github.com/QuantumComputerStudy/qlanet/blob/main/assets/images/CX0.png?raw=true"> |
| CX1 | 二つの量子惑星に対して使用する。一つ目の量子惑星が１状態の時二つ目の量子惑星の０状態と１状態を入れ替える。 | 3 |  <img src="https://github.com/QuantumComputerStudy/qlanet/blob/main/assets/images/CX1.png?raw=true"> |
| SW | 二つの量子惑星に対して使用する。二つの量子惑星の状態を入れ替える。 | 4  |  <img src="https://github.com/QuantumComputerStudy/qlanet/blob/main/assets/images/SW.png?raw=true"> |
| BM | 二つの量子惑星に対して使用する。二つの量子惑星をもつれ状態にする。もつれ状態の片方にMゲートを使うと50％で確定０(確定１)になり、残りの量子惑星は０状態または１状態となる。もつれ状態はBMゲート使用者のみが知ることができる秘密の暗号であり、相手プレイヤーからは？に見える。 | 8  |  <img src="https://github.com/QuantumComputerStudy/qlanet/blob/main/assets/images/BM.png?raw=true"> |

### 勝利条件

いずれかのプレーヤーの手番が修了したとき、次のどちらかの条件が満たされたプレーヤーは勝利します。
- 縦横斜めのいずれか一列の３惑星を自陣営の領地とする。
- 過半数の5惑星を自陣営の領地とする。

(ここに画像)

### ゲームのコツ
- ０陣営（１陣営）プレイヤーは０状態（１状態）の惑星にMゲートを使うことで確実に自分の領地にできます。  
ゲートカードを駆使して０状態（１状態）にした量子惑星にMゲートを使い領地を確定させていくのが基本の動きになります。
- CX0、CX1、BMは使うのが難しいですがその分強力な効果になっています。  
これらは量子コンピュータでも重要な役割を担っているゲートです。
- ゲートカードの特徴的な効果とカード使用コストに応じて手番が決まるシステムにより9つの量子惑星を同時に争う駆け引きが魅力です。  
一つの量子惑星の領地争いに負けても他の惑星で有利にゲームを進めて勝つことも可能です。


### 量子コンピュータについて ～より高みを目指す人へ～

- QLANETの背景

量子コンピュータは情報を保持する量子ビットと計算を行う量子ゲートから構成されており、QLANETにおいては量子惑星が量子ビット、ゲートカードが量子ゲートの概念と対応しています。
- 量子ビットとは
「０でもあり１でもある不思議な状態」を扱える量子コンピュータ上での情報の最小単位です。  
量子力学における重ね合わせ現象を利用しています。  
0と1の情報を同時に扱って計算できることが量子コンピュータが速い理由です。  
測定（Mゲート）で確率的に０か１に定まった値が最終的な計算結果となります。
- 量子ゲートとは
「０と１の重ね合わさり方」を変化させる計算を行います。  
量子ビットを観測した時の０か１に定まる確率に影響します。
- もつれ状態とは  
量子もつれとは、二つの量子ビットの間に相関関係がある状態のことを指します。  
一つの量子ビットを測定し状態が確定すると、もう一方の量子ビットは測定せずとも状態が確定します。  
例えば、「００と１１」の重ね合わせ状態にある量子ビットの一つ目を測定して「０」が得られれば、二つ目も必ず「０」となります。  
本ゲームではベル測定（BMゲート）を使用することでこの状態を作り出すことができます。  
- BMゲートとCX０（CX１）ゲートのコンボ
「００と１１」の重ね合わせ状態にCX０ゲートを使用すると２つ目の量子ビットは必ず状態１になります。  
これは重ね合わさっている００と１１がどちらもCX０ゲートで２つ目の量子ビットが状態１になるためです。  
BMゲートで発生させたもつれ状態とCX０（CX１）ゲートを正しく組み合わせられるとゲームを有利に進められるでしょう。

## Twitter (ご意見・ご要望はこちらまで)

<a class="twitter-timeline" href="https://twitter.com/qlanet_game?ref_src=twsrc%5Etfw">Tweets by qlanet_game</a> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

## ゲームデザイナー
サークルQLANET

---

Copyright © 2022 サークルQLANET All Rights Reserved.

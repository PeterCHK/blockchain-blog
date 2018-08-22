---
title: 第二課-Merkle-Root
date: 2018-08-23 00:27:00
tags:
---

區塊鏈是由一個連結一個區塊的鏈

H() 是以Hash來加密的意思
blockID (區塊的身份) 就是以下3個結合加密組成的
{% asset_img Merkle_Root1.jpg %}

PREV BLOCK HASH 是用來連結之前的區塊鏈
NONCE 是一個數字記號
MERKLE ROOT 是交易的集合

{% asset_img Merkle_Root3.jpg %}
交易 》 加密 》 加密其他交易 》 。。。 》 Merkle Root

{% asset_img Merkle_Root4.jpg %}
掘礦解碼就是要找出一個數值少於“目標值”

目標值的計算（課堂補充）：
{% asset_img Merkle_Root5.jpg %}
{% asset_img Merkle_Root6.jpg %}

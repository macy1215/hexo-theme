---
title: 對新手小白像佛地魔存在的魔王-Javascript
subtitle: 想當前端工程師你一定要知道
layout: post
author: Macy
date: 2023/11/30
cover: /images/article-image4.png
tags:
- Javascript
---
轉職成為前端工程師時，除了畫面的版型需要進行切版。但我們的資料呢？資料絕對不是寫成靜態網站的方式寫死在網站上，通常我們會透過後端提供的 API ，將資料從遠端撈回網站中並使用。那資料這時該怎麼辦呢？這時候就會需要用到 Javascript 的資料處理方法（還有更進階的語法，但在初期使用 Javascript 是最基礎的一處理資料的方法）。學習Javascript 絕對不是幾個月就可以學會的語法，常常做練習才能真的學以致用。


## Javascript 基礎知識
Javascript 的語法大量的借鑒了 C 語言與其他類似 C語言的語法。在 Javascript 的基礎先認識:

<h5>變數</h5>
<ul>
  <li>變數基礎規則：變數的開頭可以是 英文字母、底線 <strong>（ _ ）</strong>、<strong>錢字符號($)</strong>，後面可以是英文字母、底線、錢字符號、數字。<strong>（記住：變數開頭不能是數字！）</strong></li>
  <li>變數名稱不可以是保留字跟關鍵字。（保留字為目前 JS 沒有使用但未來可能會被拿來當關鍵字的英文單字，關鍵字為JS語法中已有特聽用法的英文單字）</li>
  <li>Javascript 是有大小寫分的，例：(app 與 App 是不同的變數。)</li>
  <li>中文也可以命名變數 <span class="text-danger">（較不符合開發習慣，所以不建議唷！）</span></li>
</ul> 
<br>

## 宣告變數關鍵字

話說10年前學習基礎的程式語言時常常在 DW 中看到 Var，卻不知道那個是什麼。直到這一年學習才知道 Javascript 在 ES6以前常常使用到 var 來宣告變數。 在ES6 後被分為了常數與變數。宣告變數可以使用 Var、let、const。
但！宣告又是什麼呢？宣告簡單來說就是需要告訴你的電腦你宣告了一個變數去放你的值。那我們該如何檢視變數呢？可以使輸入 console.log(變數的值) 
例如：
<div>
  <p class="mb-0 code-header py-1 px-3">javascript</p>
  <p class='ps-2 code-body py-3 ps-5'>
    例：宣告 abc = '英文';</br>
    var abc = '英文';</br>
    console.log(abc) // 會跑出 英文</br>
    var def; </br>
    m = 1; </br>
  </p>
</div>
<div class="mb-5">宣告後可以直接給值，也可以只進行宣告不放值，但沒有宣告的變數就統一被視為 var。宣告變數後就可以依照你宣告的變數去存放你的值了！那這三項分別的差異為何呢？</div>

##### var
var與let 最大的差別是變數的作用範圍（這個我們等等再來說）。var 的宣告是全域作用域，全域就是指整個專案都可吃到這個變數，他不侷限在哪一個區域中。
var 還可以重複宣告，是可以被改變值的。但 var 因為很不嚴謹所以真的很不建議用唷！ 
<div>
  <p class="mb-0 code-header py-1 px-3">javascript</p>
  <p class='ps-2 code-body py-3 ps-5'>
   var abc = 'Hello world';</br>
   var abc = 'Haha World'
  </p>
</div>

##### let 
let 的宣告是屬於區塊作用域，他指侷限在該區域中。
let 也可以重新賦予他的值。但無法重複宣告。
<div>
  <p class="mb-0 code-header py-1 px-3">javascript</p>
  <p class='ps-2 code-body py-3 ps-5'>
    let abc = 'Hello world';</br>
    abc = 'Haha World'
  </p>
</div>

##### const
const 的宣告是屬於區塊作用域，只能宣告一次，並只能為唯一值，唯獨的意思。所以當我們希望我們的變數不想被更改時可以使用 const。

Javascripe 基礎概念網路上有很多大神提供各種說明。真的很謝謝各位學長姐的無私知識，也有很多網站有提供 Javascript 的練習。學習的路途還很長遠，只能透過不斷的學習與撞牆增加自己的知識。
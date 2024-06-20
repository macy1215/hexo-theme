---
title: 手刻 Css 還是 交給Bootstrap呢？ 
layout: post
date: 2023/09/20
cover: /images/article-image2.png
tags:
- 切版設計
---
在上一份工作時，自己學習了很基礎的切版觀念，話說「金魚都能懂的 Css 必學屬性」，真的陪伴在疫情學時的我。轉職學習的路上很推薦大家自己做筆記（雖然我的筆記很亂..）。用自己的話將知識轉換成自己熟悉的文字會更加強記憶（但還是要常常碰，不然一定會忘記QQ）

在10年前還在用 Dreamweaver 的年代當時在學習時就有 Bootstrap 就開始有人在大推，對當時剛學會 Css的我不理解他的用法跟優點。當初的我如果學起來現在應該...。基礎的 Css 可以依照畫面需求調整比如說：
<div>
  <p class="mb-0 code-header py-1 px-3">HTML/Css</p>
  <p class='ps-2 code-body py-3 ps-5'>
    <span class="mb-1"> ..class='box'>box1...</br></span>
    .box{ </br>
        <span style="white-space:pre">
        backgroung-color: red;</br>
        height:100px;</br>
        width:100px;</br>
        </span>
    }
  </p>
</div>

我們依照相對應的 class 來寫出她的樣式需求，是依照主體客製化他的 css 屬性。所以只要有使用到 box 的class 就會吃到樣式。

Bootstrap 就比較針對功能來去命名與設定。比如說 margin/padding ，依照功能分類。
<div>
  <p class="mb-0 code-header py-1 px-3">HTML/Css</p>
  <p class='ps-2 code-body py-3 ps-5'>
    <span class="mb-1"> ..class='mt-0 px-2'>box1...</br></span>
   
    ```
        .mt-0 {
            margin-top: 0 !important;
        }

        .ms-1 {
            margin-left: ($spacer * .25) !important;
        }

        .px-2 {
            padding-left: ($spacer * .5) !important;
            padding-right: ($spacer * .5) !important;
        }

        .p-3 {
            padding: $spacer !important;
        }
    ```

  </p>
</div>

所以當我們想要統一調整某一個值的時候，就可以只調整一次就可以全部吃到。這真的是很棒的一個功能 QQ。
想像一下，當你今天收到任務，老闆說：「 請把公司的網站主色系調整成另一個顏色唷! 請下班前完成」。看了時鐘離下班只剩20分鐘..
這時候就會發現 bootstrap5 的功能分類的方法非常好整理。

手刻的Css 跟 Bootstrap 到底哪一個比較好呢？先來說說他們各自的優缺吧！

<table class="table">
  <thead>
    <tr>
      <th scope="col"></th>
      <th scope="col"> Css </th>
      <th scope="col"> Bootstrap</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">獨立性</th>
      <td>單一使用</td>
      <td>只要有需求都可以使用到</td>
    </tr>
    <tr>
      <th scope="row">整理性</th>
      <td>依照畫面整理</td>
      <td>依照功能整理</td>
    </tr>
    <tr>
      <th scope="row">實用性</th>
      <td>寫一套後，未來可重複使用</td>
      <td>依照功能套用，未來可重複使用</td>
    </tr>
    <tr>
      <th scope="row">編譯複雜度</th>
      <td>改一個屬性，全部都要修改</td>
      <td>修改單一特定功能就可以全部修改掉</td>
    </tr>
  </tbody>
</table>

這樣看下來， Bootstrap5 不愧是全世界目前還是很受歡迎的前端框架，對於開發者來說它將流變格線規劃得非常完整，要做RWD（響應式設計）變得相對簡單容易！
目前我還在努力學習 Tailwind 中，如果有任何心得會跟大家進行分享唷！
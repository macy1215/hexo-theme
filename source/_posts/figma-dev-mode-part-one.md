---
title: Sass 與 Scss 解析，讓你的畫面更乾淨！
subtitle: 切版議題討論
layout: post
date: 2023/08/12
cover: /images/article-image3.png
tags:
- 切版設計
---
大家比較常聽到的 Css 是最基本的樣式撰寫網頁裡特定或一群元素指定一系列的規則。通常會依照功能。
Sass 與 Scss 的不同之處其實在網路瀏覽器是沒有辦法直接吃到的，需要透過編譯的方式讓 Sass/Scss 去轉換成 css 的樣式。 

Sass 是一種程式語言，有兩種格式寫法
1. Scss （較多人使用）較適合初學者，跟 css 比較類似
2. Sacc

![圖片出處六角學院](<https://firebasestorage.googleapis.com/v0/b/portfolio-1cfc7.appspot.com/o/article.png?alt=media&token=5d8abb18-20bc-439b-9b1e-da9eb2dec813> "圖片出處六角學院")

#### Scss
寫法較類似於 css 他是透過一層一層去撰寫。
```
.menu {
	// 第一層 {}
	li{
        font-size:30px;
            // 第二層 {}
            a{
                color:red;
            }
	}
}
```

#### Sass
sass 每一個樣式前，用兩個空白鍵（一個teb）做推進分層。每一個分號後面一定要留一個空白。
並且不能用分號！
```
.menu
  font-size: 30px
  li
    a
        color: red
        letter-spacing: 5px
```

## **Sass 編譯方式**
我們可以透過什麼樣的方式在開發時使用 Ｓass/Scss 呢？可以透過下面的方式
1. 透過特定軟體編譯：Prepros
2. 網頁常用：glup、webpack 前端打包工具
3. 網頁編輯器內建的插件：VScode套件-安裝Sass compiler

<span class="fs-6 text-secondary ">參考Sass官網：https://sass-lang.com/install/</span>

我比較常使用到 Vscode中的套件。這樣就可以編開發檢查自己的 Scss 有沒有需要調整的地方！大家可以再研究一下網路上常見的方法唷～
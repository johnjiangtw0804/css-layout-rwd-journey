# Day 1 — CSS 排版基礎：Box Model + Display + Margin Collapse

## 🎯 目標
- 理解 Box Model 的結構（margin / border / padding / content）
- 掌握 `display` 類型（block / inline / inline-block）
- 理解 `box-sizing` 的差異
- 了解 margin collapse 現象

## 📘 核心概念

### Box Model 結構圖：
[見圖](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model)

建議一律使用：
```css
* {
  box-sizing: border-box;
}

# Source materials
[參考] (https://www.w3schools.com/css/css_boxmodel.asp)

你是否理解 padding、border、margin 的佔據空間？
✅ 可以。padding 在 content 外面，border 包住 padding，margin 是元件與外部的距離。

你知道為什麼加上 box-sizing: border-box 後寬度比較好算？
✅ 因為這樣 width 就包含了 padding 和 border，不用額外再加總。

你能分辨出 block、inline、inline-block 差在哪裡？
✅ block 會換行、獨占一排；
✅ inline 和 inline-block 可以一排排很多個；
✅ inline-block 可以設定寬度與高度，inline 不行。

你是否有觀察到 margin collapse 的現象？
✅ 有，像兩個元素上下 margin 會合併成較大的那一個。

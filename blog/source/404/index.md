---
title: '404 - Oops! 你迷路了嗎？ '
date: 2022-01-03 22:39:19
comments: false
permalink: /404.html
---

<!-- markdownlint-disable MD039 MD033 -->

## 這是一個不存在的頁面

很抱歉，你所存取的頁面並不存在。

預計約在 <span id="timeout">5</span> 秒後，或是 **[點選此處](https://prysline.github.io/)** 返回首頁。

<script>
let countTime = 5;

function count() {
  
  document.getElementById('timeout').textContent = countTime;
  countTime -= 1;
  if(countTime === 0){
    location.href = 'https://prysline.github.io/'; // 記得改成自己網址 Url
  }
  setTimeout(() => {
    count();
  }, 1000);
}

count();
</script>
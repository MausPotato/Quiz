### Q2: 廣告只剩圖片沒有文字
2-1. 請描述原因是什麼? <br>
2-2. 為了讓廣告正常你有哪些解決辦法?
#### Ans: 
2-1. 打開開發者工具可以直接看到.adBlock裡面有個font-size: 0px;<br>
2-2. 把該行拿掉或將.adBlock這層拿掉<br>
### Q3: 蓋板廣告點了[X]卻不會關閉
3-1. 請使用原生JavaScript實作一段code, 讓[X]按鈕可以關閉廣告<br>
3-2. 還有其他種解法可以達到同樣效果嗎?
### Ans:
3-1. 
document.querySelector(".CloseBtn").addEventListener("click", function() {
  document.querySelector(".fixBottomAd").style.display = "none";
});<br>
3-2. 有, 可以使用css的checkbox + label達到同樣的效果<br>
     https://codepen.io/maus-poteto/pen/bGGaorL
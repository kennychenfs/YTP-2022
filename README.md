# YTP專題實作想法

## 主題選擇
我想要做AI相關的研究，目前的想法是做圖神經網路和NLP結合，讓AI能夠讀取一段句子或文章，並從其中選出關鍵字，把字當作節點，用邊把它們連接起來，邊代表字之間的各種關係。

## 動機
我不太喜歡做太簡單的事情，如果有別人做過的我也覺得沒什麼意思，因此我想到了在COSCUP聽到的圖神經網路，我覺得把資料推廣到圖這種非歐的空間很有意思。

## 未來性
1. 用AI找出關鍵字與它們的關聯可以讓我們很快的大概知道內容，因為現在資訊爆炸的時代人們總是沒空好好看一段文字甚至幾分鐘的影片，如果能用圖像化的方式整理出來可以讓人更快理解。
1. 未來這樣的圖或許也可以讓AI更好的理解語言，例如比較不同文章的內容等等。

## 需要的知識
* 規定標記資料的標準，比如哪些字會是關鍵字，以及關係如何描述
* 生成GNN的知識，目前我只會用簡單的GraphRNN做監督式學習

## 需要的工具和實作
如果找不到現成的資料（我們的需求是把文章對應到圖），可能就需要自己收集資料。
* 爬蟲，收集文章，可能主要來自於新聞
* 標記圖的工具，可能是app或網頁，因為需要標記大量的資料，必須做得很方便
* AI，讀取文字後輸出圖，可能是用簡單的GraphRNN做監督式學習，或用其他我來沒看過的東西

## 連結們

https://www.python.org  
https://code.visualstudio.com  
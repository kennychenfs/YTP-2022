# YTP 第七屆專題競賽  
組名：兩個電神和一個廢物的奮鬥  
成員：王民人、陳仲肯、謝牧懷  
就讀學校：建中  
指導老師：師大科技系蔡芸琤老師  
指導業師：精誠科技 (誠志)  

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

## 每週進度
|週次|主題|成果|
|---|---|---|
|1|GitHub & VSCode 開發環境安裝與設定|**待補**|
|2|爬蟲|[範例程式](https://github.com/kennychenfs/YTP-2022/blob/main/Week%202:%20%E7%88%AC%E8%9F%B2.py)|

## Todo
抓取新聞文字：  
從新聞主頁擷取新聞的連結和標題，然後擷取個別的新聞，**只留下標題和內文，並整理好儲存在檔案**  
或是直接用網址進到新聞內頁  
目前找的新聞來源：  
中央社，網址範例  
https://www.cna.com.tw/news/aopl/202210010004.aspx  
後面數字是yyyymmdd和四位數流水號  
自由時報，網址範例  
https://news.ltn.com.tw/news/life/breakingnews/4084112  
https://ec.ltn.com.tw/article/breakingnews/4083708  
前面網址說明類別，後面則是流水號  
  
資料預處理流程：  
爬蟲收集資料->Jeiba斷詞->Tf-idf找關鍵字->App或其他工具做圖的連接（標籤）  

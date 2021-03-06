# namecard-demo
## 名片 demo

此 demo 的動畫效果僅為示意，請以此文件文字內容為主  


請使用 chrome developer tool 觀看此 demo  
或使用手機開這個網頁  
https://tl-vivian.github.io/namecard-demo/
此 demo 理應忠實呈現名片頁在不同尺寸螢幕上面的行為  


![](https://paper-attachments.dropbox.com/s_0243D5CDCA730DAAAF37F1260A6EE631E374860C1D5CF91767A98580D9FE0F1F_1567594901969_image.png)


### 名片內容如何影響捲動長度
  
直播主簡介雖然有限制字數，但是可以有很多空行。  
當簡介因此變得很長時，簡介所在的範圍便會隨著內容擴張而變長，捲動的長度便會增加。  
想要模擬此行為，可以刪減及增加簡介裡面的內容來觀察當簡介很長的時候，畫面的捲動行為。  


## 動畫效果
- 上面三張名片照輪播
    - 雖然 demo 播到第三張會反向滑回第一張，但應該要無限向右輪播
    - 一旦頁面開始滑動，輪播就停止，也無法手動左右 swipe


- 捲軸動畫
    - 名片照放大
    - 照片以中心點放大 120%
    - 往下捲觸發動畫
    - 捲到底結束動畫
    - 動畫的進度是以捲動位置控制的，也就是說捲到一半停下來，大約就放大到 110%   
![](https://paper-attachments.dropbox.com/s_0243D5CDCA730DAAAF37F1260A6EE631E374860C1D5CF91767A98580D9FE0F1F_1567584386498_image.png)

![](https://paper-attachments.dropbox.com/s_0243D5CDCA730DAAAF37F1260A6EE631E374860C1D5CF91767A98580D9FE0F1F_1567589654701_image.png)

- Navigation Bar 由透明變成 Black25
    - 當下方白色漸層捲到畫面頂部的時候觸發
    - duration 300ms
    - 往上捲到觸發位置時變回透明
   
![](https://paper-attachments.dropbox.com/s_0243D5CDCA730DAAAF37F1260A6EE631E374860C1D5CF91767A98580D9FE0F1F_1567589759774_image.png)



## Loading 狀態

loading 狀態時的名片照使用一張灰色的名片預設圖（當直播主沒有設定名片照時使用）  
此時無法按按鈕、往下捲動、左右滑動名片照  
名片照都 load 完才會結束此狀態  
此處灰色方塊的動畫請參考：  
https://codepen.io/yunusekim/pen/XaBoNZ


![](https://paper-attachments.dropbox.com/s_0243D5CDCA730DAAAF37F1260A6EE631E374860C1D5CF91767A98580D9FE0F1F_1567589101976_image.png)




## 直播中標籤動畫

當直播主正在直播的時候，開播時間的位置會顯示一個直播中標籤


![](https://paper-attachments.dropbox.com/s_0243D5CDCA730DAAAF37F1260A6EE631E374860C1D5CF91767A98580D9FE0F1F_1567590545155_image.png)

此處動畫請參考：
https://codepen.io/tl-vivian/pen/JjPOEQW



## 喜歡按鈕動畫
- 點擊愛心時，愛心會放大 1.1 倍隨即變回原來大小，按住的話會維持放大狀態
- 一般愛心按鈕跟 pressed 狀態的愛心按鈕可以在這裡下載：
https://drive.google.com/drive/folders/1QkpZiLqqnR8Ck_ReWP94eCLuAnbgpq5t  

- 點擊愛心時會從喜歡按鈕為源頭
    噴發動態那邊的動畫，動畫會飛到畫面頂端消失，跟現在動態按喜歡相同  
    按住時，持續噴發動畫，但是按讚數量只算一次  
![](https://paper-attachments.dropbox.com/s_0243D5CDCA730DAAAF37F1260A6EE631E374860C1D5CF91767A98580D9FE0F1F_1567594608304_IMG_C5B6AFBFE513-1.jpeg)
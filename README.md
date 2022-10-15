# homework

homework-cs

liunx

Linux是一種自由開放原始碼的類似Unix 的作業系統，其廣泛運用於伺服器和嵌入式系統中。具有可移植性的Open Source的作業系統，它的程式碼可以被修改適合在各種機器上。運行目前主流的 Linux 發佈版本包括：Debian、Fedora、CentOS、Ubuntu 等。 

![](https://i.imgur.com/MWJxUon.png)

 Linux背景知識-發展與線上升級

Linux的內核版本編號：2.6.32-358.el6.x86_64(通過命令uname -a可以看到)
                            
                                   （主版本.次版本.釋出版本-修改版本）
                            
版本會分為：1.開發中版本範例(主、次版本為奇數)：2.5.x
			  
               2.穩定版本範例(主、次版本為偶數)：2.6.x

![](https://i.imgur.com/dEVwXgu.png)


linux  背景知識-檔案系統目錄結構


![](https://i.imgur.com/3iD5zS6.png)

 Linux各個目錄存放的內容
/：根目錄，所有檔案皆從根目錄開始，只有root使用者具該目錄的許可權

/root：該目錄為系統管理員，也稱作超級許可權者的使用者主目錄

/bin：存放著經常使用的命令

/boot：系統啟動時必須讀取的檔案, 包括系統核心

/home：存放普通使用者的家目錄，每個使用者都有自己的家目錄

/etc：放置與系統設定、管理相關的檔案

/usr：這是一個非常重要的目錄，使用者的應用程式和檔案都放在這個目錄下，類似與windows下的program files目錄

/media：可用來做為光碟、軟碟片、隨身碟與其他分割區的自動掛載點

/tmp：供全部使用者暫時放置檔案的目錄

/var：系統執行時, 內容經常變動的資料或暫存檔(log file), 都會放置在這個目錄裡




### linux指令
touch建立檔案

vi編輯檔案

ls顯示目錄下的所有檔案


![image](https://user-images.githubusercontent.com/112846166/195986510-682ca481-cb47-43a9-a0cf-fa44c03db9fd.png)


ls-al顯示目錄下的所有檔案(包含隱藏檔)詳細資訊
![](https://i.imgur.com/WF5Bl29.png)


cat查看檔案內容

pwd顯示目前的目錄位置

cp複製

cd變換目錄

mv重新命名，移動

rm刪除檔案

rm-r強制刪除

rmdir刪除一個裡面是空的目錄

mkdir建立一個新目錄

mkdir -p同時建立多個目錄

chown可修改檔案或目錄的擁有者及群組

i編輯文件

![](https://i.imgur.com/kRS5SKq.png)


Esc離開編輯頁面

![](https://i.imgur.com/CUdqRC3.png)


:w 將編輯的資料寫入硬碟檔案中

:q離開

:q!強制離開不儲存

:wq儲存後離開

chown可修改檔案或目錄的擁有者及群組

![](https://i.imgur.com/bESNWAO.png)


### Linux背景知識-資料傳輸

![](https://i.imgur.com/A4qKRm6.png)





![](https://i.imgur.com/WB0uB7Y.png)


#### Port
通訊埠號是 TCP/UDP 與上層通訊的通道，當 TCP/UDP 要傳送訊息時，會指定要由哪一個通訊埠號來接收。一些常用的服務會使用特定的埠號來等待要求的訊息。埠號是由 16 個位元所組成的號碼，0 ~ 255 為保留號碼，256 ~ 65535 則可自行設定。 


![](https://i.imgur.com/z4XwLYu.png)

![](https://i.imgur.com/WJRRWWc.png)

#### TCP/IP
TCP/IP提供了點對點的連結機制，將資料應該如何封裝、定址、傳輸、路由以及在目的地如何接收，都加以標準化。它將軟體通信過程抽象化為四個抽象層，採取協議堆疊的方式，分別實作出不同通信協定。協定套組下的各種協議，依其功能不同，被分別歸屬到這四個階層之中，常被視為是簡化的七層OSI模型。


##### 當瀏覽器輸入網址，發出一個 GET 請求時，過程中發生了哪些事情？
1.TCP三向交握
在瀏覽器送出請求之後，瀏覽器和伺服器就會開始初步溝通，確定雙方的溝通管道順暢，以便後續請求的執行

2.瀏覽器請求、資料傳輸、渲染畫面
如同前面所提，當三項交握結束後，瀏覽器和伺服器便會開始執行請求、資料傳輸與渲染畫面的過程

3.TCP四次揮手，結束連線
在網頁成功渲染之後，瀏覽器就會和伺服器進行最後的溝通，確認傳輸過程已完成，準備結束連線





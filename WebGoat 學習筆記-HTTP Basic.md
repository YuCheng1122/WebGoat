# WebGoat 學習筆記-HTTP Basic
## HTTP 的概念
超文本傳輸協定HTTP(HyperText Tansfer Protocol)，用來傳輸超媒體文件的[應用層][http://ithelp.ithome.com.tw/m/articles/10000021]協定，被設計來讓瀏覽器和伺服器進行溝通，但也可做其他用途。HTTP遵循標準[主從式架構][http://zh.m.wikipedia.org/zh-tw/主從式架構]模式，由客戶端連線以發送請求，然後等待接收回應，HTTP是一種[無狀態通訊協定][http://medium.com/麥克的半路出家筆記/筆記-http-cookie-和-session-使用-19bc740e49b5]，意思是伺服器不會保存任兩個請求間的任何資料。儘管作為TCP/IP的應用層，HTTP亦可應用於其他可靠的傳輸層，只要不會無聲無息消失就好。

## 請使用者在欄位輸入名字
畫面會將您輸入的東西**顛倒顯示**
![Screenshot (517)](https://github.com/YuCheng1122/WebGoat/blob/master/Screenshot%20(517).png)

根據程式碼我們可以發現這個表格是使用**POST**的方式傳出去
![Screenshot (516)](https://github.com/YuCheng1122/WebGoat/blob/master/Screenshot%20(516).png)

接著我們會發現**Request**裡竟然包含一個叫做**magic_num的參數**，這個表單裡有個隱藏的表單欄位，並存了**magic_num**的值在其中。

![Screenshot (518)](https://github.com/YuCheng1122/WebGoat/blob/master/Screenshot%20(518).png)

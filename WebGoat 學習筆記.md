# WebGoat 學習筆記
## 前言
Webgoat是專門用來練習漏洞的Web應用程式，所以裡面的網頁都是漏洞百出，因此官方建議使用WebGoat練習時，最好要把網路中斷。此外WebGoat只供教育使用，在裡面學到的任何技術都不能拿去測試外面的網頁，以免觸法。
***
## WebGoat怎麼安裝
Github上可以看到，安裝WebGoat有四種方法:
> 1. Standalone
> 2. Run using Docker
> 3. Run from the sources
> 4. Run with custom

這邊我使用的是第一種
## 一、首先要先確定電腦裡有裝JRE
[Java SE Downloads][https://www.oracle.com/java/technologies/downloads/]

## 二、到Github上下載最新的WebGoat

[WebGoat Downloads][https://github.com/WebGoat/WebGoat/releases]

## 三、執行下載的檔案
	java -jar webgoat-server-8.1.0.jar [ — server.port=8080] [ — server.address=localhost]
**出現這個頁面就是成功喔!** 到這裡的朋友已經成功一半了:)

![WebGoat Downloads](https://github.com/YuCheng1122/WebGoat/blob/master/Screenshot%20(510).png)

## 四、輸入上述所設定的Port及Server網址
[WebGoat][http://localhost:8080/WebGoat]
## 五、心得
其實我在做這個練習的過程中花最多時間的就是安裝WebGoat，來來回回應該就花了兩天的時間，雖然是斷斷續續的但其實不知不覺就花了好幾個小時，原因大致分為: 
> 1.第一次自己使用這種 Command Prompt的介面安裝程式
>
> 2.找錯方向

## 1. 沒有自己使用 Command Prompt 安裝程式的經驗
雖然看似很蠢，但我覺得沒有相關使用經驗，同時又沒有人教的時候，真的會犯一些看似很低級的錯誤，因此這邊提供一些淺見給一些毫無經驗的人
## 要開 Windows Powershell 去做安裝
找到你下載的路徑右鍵點選 Open in Terminal ，**一般來說會在Downloads**
![PowerShell](https://github.com/YuCheng1122/WebGoat/blob/master/Screenshot%20(511).png)

## 廣泛閱讀找資料很重要
盡最大的努力從GitHub、Medium等等網站去找學習資源，問人是很好的方法，從小到大我們都被鼓勵有問題就應該去問，然而並不是隨時都有人可以問，因此在現在這個網路資源豐富的時代，我們其實應該盡可能去找資料，訓練自己獨立解決問題，從中可以提升你兩個能力:
>1.下關鍵字的準確度
>
>2.閱讀能力
>
>3.讀懂電腦回傳給你哪些錯誤

## 2. 找錯方向

在找錯誤的過程中，曾經有一度以為是環境變數的問題，隨然現在還不確定是不是因為環境變數，但從錯誤中也學到另一個看問題的角度，可能未來有相關問題的時候就會把環境變數列為其中一個需要注意的要素。
	
![JRE_Home](https://github.com/YuCheng1122/WebGoat/blob/master/Screenshot%20(513).png)![Path](https://github.com/YuCheng1122/WebGoat/blob/master/Screenshot%20(514).png)![Java_Home](https://github.com/YuCheng1122/WebGoat/blob/master/Screenshot%20(512).png)

Arduino 介紹

## 參考網址 
https://www.arduino.cc

## Arduino 來源
原始的Arduino硬體是從一間義大利公司Smart Projects製造，有些Arduino硬體則是被官方授權由美國公司SparkFun Electronics和Adafruit Industries設計。
https://www.youtube.com/watch?v=hjRSwBcLcSU

國內教學 : https://www.youtube.com/watch?v=3mw-1Bvv0WU&list=PLdckmk1Jf8MYOED98iY13wdGi52h-O69X

## Arduino 開發版
參考 : https://www.arduino.cc/en/Main/Products
![](https://github.com/derricktsai0904/Arduino/blob/master/00.Arduino%E5%9F%BA%E6%9C%AC%E4%BB%8B%E7%B4%B9/ArduinoProduct.PNG?raw=true)

## Arduino 相關應用

### 1.擴充板 
>![](https://github.com/derricktsai0904/Arduino/blob/master/00.Arduino%E5%9F%BA%E6%9C%AC%E4%BB%8B%E7%B4%B9/ArduinoShield.PNG?raw=true)
>![](https://github.com/derricktsai0904/Arduino/blob/master/00.Arduino%E5%9F%BA%E6%9C%AC%E4%BB%8B%E7%B4%B9/ArduinoShield2.PNG?raw=true)
<hr>

### 2.通訊模組
>![](https://github.com/derricktsai0904/Arduino/blob/master/00.Arduino%E5%9F%BA%E6%9C%AC%E4%BB%8B%E7%B4%B9/ArduinoCommunication.PNG?raw=true)
>![](https://github.com/derricktsai0904/Arduino/blob/master/00.Arduino%E5%9F%BA%E6%9C%AC%E4%BB%8B%E7%B4%B9/ArduinoCommunication2.PNG?raw=true)
<hr>

### 3.感測器
>![](https://github.com/derricktsai0904/Arduino/blob/master/00.Arduino%E5%9F%BA%E6%9C%AC%E4%BB%8B%E7%B4%B9/ArduinoSensor.PNG?raw=true)
>![](https://github.com/derricktsai0904/Arduino/blob/master/00.Arduino%E5%9F%BA%E6%9C%AC%E4%BB%8B%E7%B4%B9/ArduinoSensor2.PNG?raw=true)
>![](https://github.com/derricktsai0904/Arduino/blob/master/00.Arduino%E5%9F%BA%E6%9C%AC%E4%BB%8B%E7%B4%B9/ArduinoSensor3.PNG?raw=true)
>![](https://github.com/derricktsai0904/Arduino/blob/master/00.Arduino%E5%9F%BA%E6%9C%AC%E4%BB%8B%E7%B4%B9/ArduinoSensor4.PNG?raw=true)
<hr>

### 4.實例應用
>![](https://github.com/derricktsai0904/Arduino/blob/master/00.Arduino%E5%9F%BA%E6%9C%AC%E4%BB%8B%E7%B4%B9/ArduinoApplication.PNG?raw=true)
<hr>

<br><br><br>

<hr><hr>

<br><br><br>

<b><font size=32>【Arduino 開發環境安裝】</font></b>

#### 1.下載Arduino ide Tool
##### 1.1 請到以下網址下載最新開發軟體，作業系統可建置在Mac OS、Linux、Windows 32位元及64位元
參考網址 : https://www.arduino.cc
>![](https://github.com/derricktsai0904/Arduino/blob/master/01.Arduino%E9%96%8B%E7%99%BC%E7%92%B0%E5%A2%83%E5%AE%89%E8%A3%9D/Arduino_Download.PNG?raw=true)
>![](https://github.com/derricktsai0904/Arduino/blob/master/01.Arduino%E9%96%8B%E7%99%BC%E7%92%B0%E5%A2%83%E5%AE%89%E8%A3%9D/Arduino_Download2.PNG?raw=true)
<hr>

##### 1.2 開發介面介紹
##### 1.2.1 Adruino IDE 介面

【基本按鈕】
>![](https://github.com/derricktsai0904/Arduino/blob/master/01.Arduino%E9%96%8B%E7%99%BC%E7%92%B0%E5%A2%83%E5%AE%89%E8%A3%9D/ArduinoInstall.PNG?raw=true)

【檢查裝置管理員是否有偵測到 Arduino開發板】
>![](https://github.com/derricktsai0904/Arduino/blob/master/01.Arduino%E9%96%8B%E7%99%BC%E7%92%B0%E5%A2%83%E5%AE%89%E8%A3%9D/ArduinoInstall1.PNG?raw=true)

【電腦接上 Arduino 開發板.USB連線方式】
>![](https://github.com/derricktsai0904/Arduino/blob/master/01.Arduino%E9%96%8B%E7%99%BC%E7%92%B0%E5%A2%83%E5%AE%89%E8%A3%9D/ArduinoInstall2.PNG?raw=true)

【設定使用開發板】
>![](https://github.com/derricktsai0904/Arduino/blob/master/01.Arduino%E9%96%8B%E7%99%BC%E7%92%B0%E5%A2%83%E5%AE%89%E8%A3%9D/ArduinoInstall3.PNG?raw=true)

【設定使用開發板連結埠】
>![](https://github.com/derricktsai0904/Arduino/blob/master/01.Arduino%E9%96%8B%E7%99%BC%E7%92%B0%E5%A2%83%E5%AE%89%E8%A3%9D/ArduinoInstall4.PNG?raw=true)

##### 1.3 Arduino開發板腳位說明
>![](https://github.com/derricktsai0904/Arduino/blob/master/01.Arduino%E9%96%8B%E7%99%BC%E7%92%B0%E5%A2%83%E5%AE%89%E8%A3%9D/ArduinoPoint.PNG?raw=true)




<br><br><br>

<hr><hr>

<br><br><br>



<h1>【練習題目 : LED 控制】</h1>

## 準備材料 : 
>1. Arduino Nano 板(CH340驅動程式.USB:MicroUSB)
>2. MicroUSB 連接線 X 1
>3. LED 一顆
>4. 杜邦線數條
>5. 麵包板 X 1
===
 
>![](https://github.com/derricktsai0904/Arduino/blob/master/02%20Arduino%20%E5%9F%BA%E6%9C%AC%E6%84%9F%E6%B8%AC%E5%99%A8%E5%AF%A6%E4%BD%9C%E7%AF%84%E4%BE%8B/A.LED%E6%8E%A7%E5%88%B6/Arduino_LED.PNG?raw=true)

## LED控制電路圖

>![](https://github.com/derricktsai0904/Arduino/blob/master/02%20Arduino%20%E5%9F%BA%E6%9C%AC%E6%84%9F%E6%B8%AC%E5%99%A8%E5%AF%A6%E4%BD%9C%E7%AF%84%E4%BE%8B/A.LED%E6%8E%A7%E5%88%B6/Arduino_LED_Circuit.PNG?raw=true)

## 相關函式 : 無

## 程式說明

[以下程式來源 Blink.ino ]:https://github.com/derricktsai0904/Arduino/blob/master/02%20Arduino%20%E5%9F%BA%E6%9C%AC%E6%84%9F%E6%B8%AC%E5%99%A8%E5%AF%A6%E4%BD%9C%E7%AF%84%E4%BE%8B/A.LED%E6%8E%A7%E5%88%B6/Blink.ino "Blink.ino"
[以下程式來源 Blink.ino ]
``` arduino
int LED = 13; // 宣告 Arduino 連結 LED 腳位
void setup() {  // Arduino 啟始函式，只會執行一次
 pinMode(LED, OUTPUT); //設定腳位為輸出訊號
}  

void loop() { //Arduino 主要迴圈，執行無窮多次，直到關機為主
 digitalWrite(LED, HIGH);   // 設定 LED 亮
 delay(1000);               // 延遲一秒  
 digitalWrite(LED, LOW);    // 設定 LED 關
 delay(1000);               // 延遲一秒
}  

```

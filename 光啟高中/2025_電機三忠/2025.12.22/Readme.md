<h1>【練習題目 : 超音波距離感測 + 蜂鳴器 】</h1>

## 準備材料 : 
>1. Arduino Nano板(CH340驅動程式.USB:MicroUSB)
>2. MicroUSB 連接線 X 1
>3. HC-SR04 超音波感測器 X 1
>4. 蜂鳴器 3-6V X 1
>5. 8Ω 0.5W 喇叭 X 1
>6. 1k ohm 電阻 X 2
>7. 麵包板 X 1
===

## Arduino Nano 腳位圖 

<img src="https://github.com/derricktsai0904/Arduino/blob/master/03%20Arduino%20%E9%80%B2%E9%9A%8E%E5%AF%A6%E4%BD%9C%E7%AF%84%E4%BE%8B/03%20%E8%AA%9E%E9%9F%B3%E6%92%AD%E6%94%BE/Arduino_NANO.jpg" width=600 height=400 />

## ㄈㄥa<h1>【練習題目 : 超音波距離感測 + 蜂鳴器 】</h1>

## 準備材料 : 
>1. Arduino Nano板(CH340驅動程式.USB:MicroUSB)
>2. MicroUSB 連接線 X 1
>3. HC-SR04 超音波感測器 X 1
>4. 蜂鳴器 3-6V X 1
>5. 8Ω 0.5W 喇叭 X 1
>6. 麵包板 X 1
===

## Arduino Nano 腳位圖 

<img src="https://github.com/derricktsai0904/Arduino/blob/master/03%20Arduino%20%E9%80%B2%E9%9A%8E%E5%AF%A6%E4%BD%9C%E7%AF%84%E4%BE%8B/03%20%E8%AA%9E%E9%9F%B3%E6%92%AD%E6%94%BE/Arduino_NANO.jpg" width=600 height=400 />

## 蜂鳴器 腳位圖 

<img src="https://github.com/1104405103/Course/blob/main/%E5%85%89%E5%95%9F%E9%AB%98%E4%B8%AD/2025_%E9%9B%BB%E6%A9%9F%E4%B8%89%E5%BF%A0/2025.12.22/buzzer.jpg" width=300 height=300 />

## HC-SR04 超音波感測器腳位圖

<img src="https://github.com/derricktsai0904/Course/blob/main/2025.09%20%E8%BF%91%E4%BB%A3%E9%9B%BB%E5%AD%90%E7%B3%BB%E7%B5%B1/11.%20%E8%B6%85%E9%9F%B3%E6%B3%A2.mp3%E6%92%AD%E6%94%BE/HCSR04.jpg" width=300 height=300 />

## 超音波距離感測+ 蜂鳴器控制電路圖

<img src="https://github.com/1104405103/Course/blob/main/%E5%85%89%E5%95%9F%E9%AB%98%E4%B8%AD/2025_%E9%9B%BB%E6%A9%9F%E4%B8%89%E5%BF%A0/2025.12.22/playbob.jpg"  width=800 height=600 />

## 相關函式 : 無
>1. Arduino.h
>2. SoftwareSerial.h

## 程式說明

``` arduino

//使用軟體Serial
int const trigPin= 12;
int const echoPin= 11;
int const buzzer=7;
int Duration;
int Distance;
int first;

void setup() 
{
  Serial.begin(9600); //啟用監控視窗
  Serial.println("initializing...");

  // 超音波
  pinMode(trigPin,OUTPUT);
  pinMode(echoPin,INPUT);

  // 蜂鳴器腳位
  pinMode(buzzer,OUTPUT);

  digitalWrite(trigPin,LOW);
}

void loop() 
{
    digitalWrite(trigPin,HIGH); //發射超音波
    delay(1);
    digitalWrite(trigPin,LOW);
    Duration = pulseIn(echoPin,HIGH); //超音波發射到接收的時間
    Distance = Duration*0.034/2; //計算距離(cm)
    if ( Distance <= 15 && Distance!=0){
         Serial.print("play= HRS-04 =>");
         Serial.println(Distance);
         digitalWrite(buzzer,HIGH);
         delay(1000);
         digitalWrite(buzzer,LOW);
         delay(1000);
    }
    delay(10);
}


```







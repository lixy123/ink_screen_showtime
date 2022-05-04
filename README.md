# ink_screen_showtime

<b>一.功能：</b><br/>
墨水屏显示时间，每分钟刷新一次<br/>

最终效果：<br/>
  <img src= 'https://github.com/lixy123/ink_screen_showtime/blob/main/time1.jpg?raw=true' /> <br/>
  <img src= 'https://github.com/lixy123/ink_screen_showtime/blob/main/time2.jpg?raw=true' /> <br/>
  <img src= 'https://github.com/lixy123/ink_screen_showtime/blob/main/time3.jpg?raw=true' /> <br/>
  <img src= 'https://github.com/lixy123/ink_screen_showtime/blob/main/time4.jpg?raw=true' /> <br/>
  
<b>二.硬件：</b><br/>
1.lilygo ESP32 墨水屏驱动板 T5_V2.4 <br/>
2.微雪3.7 寸黑白墨水屏 支持局刷 <br/>
3.DS3231时钟模块(ESP32默认I2C引脚连接 IO21,IO22) <br/>
4.锂电池1500mah <br/>


<b>三.软件代码:</b><br/>
A.arduino 版本 1.8.13<br/>
B.库文件:<br/>
ESP32库 arduino-esp32 版本 1.0.6<br/>
墨水屏库 https://github.com/ZinggJM/GxEPD2 <br/>
ds3231时钟模块驱动 RTClib https://github.com/adafruit/RTClib <br/>
C.其它：<br/>
制作字库参考： http://oleddisplay.squix.ch/<br/>


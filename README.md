# ink_screen_showtime

<b>一.功能：</b><br/>
墨水屏显示时间，每分钟刷新一次<br/>
1.此屏局刷效果好，刷屏无闪烁<br/>
2.利用了休眠节能，休眠待机功耗约3ma左右，其中DS3231时钟模块用电2ma，不太容易进一步节能<br/>
3.需要显示的汉字点阵较大，汉字字库点阵程序做不了那么大的字库，显示汉字处用图片代替<br/>
4.初步估算，1500ma充满电后能使用0.5-1月，待测试<br/>

最终效果：<br/>
  <img src= 'https://github.com/lixy123/ink_screen_showtime/blob/main/time1.jpg?raw=true' /> <br/>
  <img src= 'https://github.com/lixy123/ink_screen_showtime/blob/main/time2.jpg?raw=true' /> <br/>
  <img src= 'https://github.com/lixy123/ink_screen_showtime/blob/main/time3.jpg?raw=true' /> <br/>
  <img src= 'https://github.com/lixy123/ink_screen_showtime/blob/main/time4.jpg?raw=true' /> <br/>
  
<b>二.硬件：</b><br/>
1.lilygo ESP32 墨水屏驱动板 T5_V2.4 https://github.com/Xinyuan-LilyGO/T5-Ink-Screen-Series <br/>
2.微雪3.7 寸黑白墨水屏 支持局刷 <br/>
3.DS3231时钟模块 (注：孔距不匹配，用钳子将4引脚夹一下，直接焊接) <br/>
  ESP32 ==>DS3231<br/>
  GND GND<br/>
  5V 5V<br/>
  21 SDA<br/>
  22 SCL<br/>
4.锂电池1500mah (注：参考原理图，直接到墨水屏驱动板的5V/GND 23/2引脚， 1/24两引脚夹断，容易电池短路 )<br/>

<b>三.软件代码:</b><br/>
A.arduino 版本 1.8.13<br/>
B.库文件:<br/>
ESP32库 arduino-esp32 版本 1.0.6<br/>
墨水屏库 https://github.com/ZinggJM/GxEPD2 <br/>
ds3231时钟模块驱动 RTClib https://github.com/adafruit/RTClib <br/>
C.其它：<br/>
制作字库参考： http://oleddisplay.squix.ch/<br/>


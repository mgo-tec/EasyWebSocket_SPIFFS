# EasyWebSocket_SPIFFS BETA ver 1.45
Simple library for WebSocket communication with ESP-WROOM-02(ESP8266) and smartphone browser.  
This requires the Arduino core for ESP8266 WiFi chip library.  
https://github.com/esp8266/arduino  
This use SPIFFS file system.

My Blog: https://www.mgo-tec.com
# Change log:

(1.45)  
A watchdog timer of ESP8266 to create a grace period to operate, has been added here and there yield ().  
As a result, I think the operation is stable.  
Sample sketch also has been corrected.  

-NEW class-  
EWS_BrowserReceiveTextTag2  
EWS_Status_Text2  
EWS_WebSocket_Reconnection_Button2  
EWS_Close_Button2  
EWS_Window_ReLoad_Button2  

(1.39)  
*It added support for SoftAP mode.

(1.37)  
*I the suggestions for improvement from Visyeii's on twitter, I was allowed to adopt because it was very effective.  
Mr. Visyeii, Thank you very much.

*And speed of loading the spiffs_01.txt file in SPIFFS file system at the time of access from the first of the smartphone browser is much up, display of the browser is now faster.  
*Fixed a WebSocket reconnect button in (confirmed by ver 9.3.1) iOS.  
*Connections at the time I was allowed to divert the handleClient function from the library WiFiServer.cpp of Arduino core for ESP8266 WiFi chip in. I think the connection has become more reliable.  

(1.35)  
*From the Web to GET requests, add a function to extract the text by analyzing the HTML tags.  
*Add to reconnect button of WebSocket communication only.

(1.3)  
*Brush up the WebSocket handshake method.  
*Reconnection is now easier to.  
*Reload button Add Library.  
*Momentary button Add Library.  
*Text box send Add Library  
(However, up to 120 bytes, including the ID string)  
*Canvas_Slider was so that data transmission in only touched without slide.  
*Updated the HTML header file "spiffs_01.txt" be read by SPIFFS file system.

【更新履歴】(Japanese)   
(1.45)  
ESP8266のウォッチドッグタイマを作動させる猶予時間を作るために、所々 yield() を追加しました。  
それにより、多少動作が安定したと思います。
サンプルスケッチも修正しました。

-NEW class-  
EWS_BrowserReceiveTextTag2  
EWS_Status_Text2  
EWS_WebSocket_Reconnection_Button2  
EWS_Close_Button2  
EWS_Window_ReLoad_Button2  

(1.39)  
ESP-WROOM-02 (ESP8266) の SoftAPモードに対応しました。詳しくはサンプルスケッチをご覧ください。

(1.37)  
ツィッター上でVisyeiiさんから改善提案をいただき、とても有効でしたので採用させていただきました。  
Visyeiiさん、ありがとうございました。

・初回のスマートフォンブラウザからのアクセス時にSPIFFSファイルシステムでspiffs_01.txtファイルを読み込む速度が格段にアップし、ブラウザの表示が早くなりました。  
・iOS(9.3.1で動作確認済み)でのWebSocket再接続ボタンを修正しました。  
・コネクション時にArduino core for ESP8266 WiFi chip のライブラリ WiFiServer.cpp から handleClient()関数を流用させていただきました。コネクションがより確実になったかと思います。  

(1.35)  
・WebからGETリクエストして、HTMLタグを解析してテキストを抽出する関数を追加。  
・WebSocket通信のみの再接続ボタンを追加。

(1.3)  
・WebSocketハンドシェイク方法をブラッシュアップ  
・再接続がしやすくなりました。  
・再接続(Reload) ボタンライブラリ追加  
・瞬時ボタン（モーメンタリーボタン）ライブラリ追加  
・テキストボックス送信ライブラリ追加  
（※ただし、ID文字列も含め120バイトまで）  
・Canvas_Slider をスライドしなくてもタッチしただけでデータ送信するようにしました。  
・SPIFFSファイルシステムで読み出すHTMLヘッダファイル spiffs_01.txt を更新しました。  
# Credits and license
*Licensed under the GNU LESSER GENERAL PUBLIC LICENSE Version 2.1

*Copyright (c) 2016 mgo-tec

Other usage is Japanese, please visit my blog.

My Blog:  https://www.mgo-tec.com  
(ver1.39) https://www.mgo-tec.com/blog-entry-softap-esp8266-easywebsocket139.html  
(ver1.35) https://www.mgo-tec.com/blog-entry-wroom-websocket-messageboard-05.html  
(ver1.3) https://www.mgo-tec.com/blog-entry-easywebsocket-beta13.html
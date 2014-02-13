#AcceliteController   
  
Acceliteに搭載されているスイッチモジュール「AcceliteController」の仕様  
  
Device：USB ClassHID Joystick  
Input：SlideSwitch*4，PushSwitch*1  
  
  
JoystickNumber：  
※ubuntuとwinでは数値の始まりが異なります．  
|    | ubuntu |  win |  
|:--:|:------:|:----:|  
| S1 |   1    |   2  |  
| S2 |   2    |   3  |  
| P3 |   3    |   4  |  
| S3 |   4    |   5  |
| S4 |   %    |   6  |  
S*：SlideSwitch*　P*:PushSwitch*

ubuntu側のソフトウェア問題対処の為  
P1を押すと，すべてのSlideSwitchが論理反転しP1を離すとリアルコンフィグへ戻ります.  
  
  
ブートローダとファームウェアについて  
内部プログラムにUSBブートローダ機能が実装されています.  
PushSwitchを押し込んだままUSBDeviceを接続すると，ブートモードに入ります.  
ファームウェア（JoystickProgram）はブートモードからUSB経由で書き込みが可能です.  
  
  
「AcceliteController.zip」  
・AcceliteController ProductVersion　：　EagleCAD電子回路データ  
・Bootloader　：　ブートローダ書き込みツール(for win , for Linux)  
・Project　：　MPLABプロジェクト  
・Verification　：　シミュレーションソフト  
  
  



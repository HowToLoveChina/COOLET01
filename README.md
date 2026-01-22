### COOLET01-216 
#### 智能插座 北京国电通网络技术有限公司

. 来源小黄鱼  

面对ESP8266EX模块天线向上，插口在左边自上向下，自左向右各定义如下


| 位置 | 编号 | 说明 |
|-----|-------|-----|
| 左上1 | 1 | VCC 供电 |  
| 靠1 | 2 | 板上LED   PIN12,GPIO13 |
| 上中 | 3 | TOUT  PIN6 |
| 上右 | 4 | RSTB  PIN32 |
| 左2 | 5 |   GPIO02,PIN14 |
| 左3 | 6 |   GPIO00,PIN15 |
| 左下1 | 7 | GPIO04,PIN16 |
| 下2 | 8 |   GND  |
| 下3 | 9 |   U0RXD,PIN25  |
| 下4 | 10 |  U0TXD,PIN26   |


外接双排11焊点定义如下

| 位置 |  模组连接 | 插座连接 | 说明 | OOOO | 对侧 | 
| ---  | -------  | ------- | ----- |---  | --- |
|  1   | GPIO14,PIN10| CF   | 计量脉冲 | OOOO | 无 |
|  2   | GPIO15,PIN13| MOS  | 继电器吸合 | OOOO | 无 |
|  3   | GPIO13,PIN12| NC   | 与模组LED连接 | OOOO | VCC |
|  4   |   GND       | 共地   |  | OOOO | VCC |
|  5   | GPIO05,PIN24| IR.1   | 红外接收 | OOOO | GND |
|  6   | 经R6接地| LED负 |  无功能 | OOOO | GND |
|  7   | VDDPST,PIN17,11| IR.3   | 红外供电 | OOOO | 无 |


RSTB与GPIO16短接才能低功耗

VCC,GND,U0RXD,U0TXD 接串口，GPIO0接地，刷写模块成功

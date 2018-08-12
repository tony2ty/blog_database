## usb msc 枚举过程



### 概述

1. 枚举是控制传输的过程



### 抓包过程

#### 获取设备描述符

##### 令牌包

![1533175261964](C:\Users\zhenglili\Desktop\Remote SVN\11_Communication_Protocol\04_USB\02_document\picture\1533175261964.png)

##### 数据包

![1533175409748](C:\Users\zhenglili\Desktop\Remote SVN\11_Communication_Protocol\04_USB\02_document\picture\1533175409748.png)

##### 握手包

![1533178992930](C:\Users\zhenglili\Desktop\Remote SVN\11_Communication_Protocol\04_USB\02_document\picture\1533178992930.png)



#### 获取配置描述符

##### 令牌包

![1533178949998](C:\Users\zhenglili\Desktop\Remote SVN\11_Communication_Protocol\04_USB\02_document\picture\1533178949998.png)

##### 数据包

![1533179154801](C:\Users\zhenglili\Desktop\Remote SVN\11_Communication_Protocol\04_USB\02_document\picture\1533179154801.png)

##### 握手包

![1533178992930](C:\Users\zhenglili\Desktop\Remote SVN\11_Communication_Protocol\04_USB\02_document\picture\1533178992930.png)

#### 获取配置接口端点描述符

##### 令牌包

![1533179258513](C:\Users\zhenglili\Desktop\Remote SVN\11_Communication_Protocol\04_USB\02_document\picture\1533179258513.png)



##### 数据包

![1533179574643](C:\Users\zhenglili\Desktop\Remote SVN\11_Communication_Protocol\04_USB\02_document\picture\1533179574643.png)



##### 握手包

![1533179613251](C:\Users\zhenglili\Desktop\Remote SVN\11_Communication_Protocol\04_USB\02_document\picture\1533179613251.png)





问题

1. 当前来看枚举过程起始的SETUP令牌包阶段，应该是IN令牌包，根据IN令牌包的要求，需要包含设备地址和端点号，目前来看并未包含？





如何识别各种包的类型

![1533178248321](C:\Users\zhenglili\Desktop\Remote SVN\11_Communication_Protocol\04_USB\02_document\picture\1533178248321.png)

![1533178365995](C:\Users\zhenglili\Desktop\Remote SVN\11_Communication_Protocol\04_USB\02_document\picture\1533178365995.png)
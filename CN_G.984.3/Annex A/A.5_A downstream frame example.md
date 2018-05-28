# A.5 一个下行帧例子

该下行帧 test vector 的目的是提供：

- CRC on PLOAM 的例子， PLend and US Bwmap access.
- 一个traffic 载荷的例子 mapping into GEM fragments
- Frame scrambling 的 例子

 

该例子 includes 一个GTC 下行帧的前138字节。它includes PCBd 和 两个 GEM 分片（zero ATM portion）. 该 PCBd includes 一个 "Key_Switching_Time" PLOAM 消息和两个 US Bwmap accesses.

 

Fields 不同的参数细节是：

- Ident field: Super-frame counter is      0x00051276 and FEC ind is 0

- PLOAM 消息：      'Key_Switching_Time'(type 0x13) 消息 addressed to ONU-ID 0x12

- US BWmap：

  ​                Alloc-ID      Flags      StartTime    StopTime

   Access 1   0x10        0x000     0x1000        0x1500

   Access 2   0x150       0x400     0x1600        0x1700

- GEM 分片：

  1) 第一个分片： 64 byte 以太网包 where:

  ​    DA=FF-FF-FF-FF-FF-FF, SA=00-0E-7F-5F-F1-DF

  2) 第二个分片： Unstructured data.

  

NOTE 1 - AES is not applied to GEM 分片（fragments）。

NOTE 2 - BIP field is NA in the example.

 

Frame before scrambling:

+--------------+-----+--------------+-------------------+

|…             |…    |…

…

 

 

Frame after scrambling:

+-------------+-----+--------------+--------------------+

|…            |…    |…

…
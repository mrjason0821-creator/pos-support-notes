1. 找到Kp后台（如果没有准备TeamViewer)
2. 查看新机器的SN，检查商家是否已经Batch,然后在Kp的后台检查（Check Batch）。Check Batch大部分数字是0，则代表已经过账成功，具体情况具体分析。
3. 通知Harris或其他有激活权限的人，确认Pax系列刷卡机的升级激活权限。
4. 确认激活之后，让商家将刷卡机重启。（重新插拔电源即可）
5. 重启之后，一般来说IP会跳转到新的IP地址。这边先查看IP地址，然后固定IP，再Ping一下，确认有网络之后。查看刷卡机的MID。如果没有网络，再次查刷卡机的ECR，然后再试着Ping。
6. ECR,（communication-----Ethernet------出现一个数字之后点OK）。 Kp绑定的是第二个HTTP GET,其他系统选第一个TCP/IP。
7. SP30 查刷卡机MID: F -> 4. Host Setting -> 1.Hosts Parameters -> 1.Merchant ID

SP30 PING：F -> 6. Communcation -> 8. Lan Parameters -> PING

SP30 查刷卡机IP： F -> 6. Communcation -> 8. Lan Parameters ->2. IP address

SP30 固定IP： F -> 6. Communcation -> 8. Lan Parameters ->1. LAN Type -> 2.static（如果static后Ping还是不行，就先改为DHCP再Ping，再改回static，然后查看新的IP）

SP30 查刷卡机ECR：F -> 6. Communcation -> 9.ECR comm.Type -> 选择网路方式 ->如果是KP系统选择HTTP GET，如果是其他系统选择TCP/IP

KP后台查看电脑的IP（Tools左上角或者远程到电脑进行cmd），确定电脑IP后在后台绑定刷卡机IP

检查device status刷卡机是否正常（如果不正常通过电脑Ping刷卡机IP，Ping不通则检查电脑的IP看能否通过加IP网段解决）


8. 通过电脑点餐测试是否可以进行刷卡
9. Void掉测试单

 
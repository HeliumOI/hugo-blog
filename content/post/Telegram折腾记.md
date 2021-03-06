title: Telegram折腾记
abbrlink: 3581552066
tags:
  - 网络安全
  - 网络
  - Telegram
categories:
  - 网络
date: 2020-08-05 22:32:00
---
出于一些众所周知的原因，一些即时通讯软件不能很好地满足我们的需求：

- QQ/WeChat，国产+闭源+黑历史，不存在的
- WhatsApp/iMessages，闭源的商业软件，再加上某Prism，不存在的
- Signal/Jabber，在国内比较小众，用户数量太少

## Telegram是什么

以下内容摘自维基百科：

> Telegram是跨平台的即时通信软件，其客户端是自由及开放源代码软件，但服务器是专有软件。用户可以相互交换加密与自毁消息，发送照片、影片等所有类型文件。官方提供手机版（Android、iOS、Windows Phone）、桌面版（Windows、macOS、Linux）和网页版等多种平台客户端；同时官方开放应用程序接口（API），因此拥有许多第三方的客户端可供选择，其中多款内置中文。

在墙越来越高的今天，许多软件都被证实并不可靠，前段时间升至爆出过腾讯一个数据方面的小主管就能调取聊天记录的新闻。于是乎，Sophon开始找在某些方面更优秀的IM（即时通讯）软件，然后就找到了Telegram。

Telegram有以下几个优势：

- 完全免费，多平台不限制同步消息，比微信QQ之流不知高到哪里去了
- 跨平台，支持Windows，macOS，Linux，iOS，Android，和Web端
- 分享单个文件最大可达1.5G（更新后为2G）
- 客户端开源，放心
- 可以选择端到端加密并销毁数据
- 服务器端虽然储存平时聊天的记录，但Telegram骨头硬啊，俄罗斯政府曾经找Telegram要密钥，被Telegram一句话怼回去了，后来被逐出俄罗斯也不松口
- Signal之类的软件或许比Telegram更安全，但是如果你注册了，你会惊喜得发现，没什么人用，最后放在硬盘里吃灰

## Telegram的安装

Telegram当然可以直接从官网下载，但大多数人是访问不了Telegram官网的，所以就要另辟蹊跷：

1. Telegram被托管在GitHub上，因此可以从GitHub上下载Telegram，具体来说是https://github.com/telegramdesktop/tdesktop/releases

但是，请注意，GitHub在国内是属于半被墙状态，因此可能要使用多线程下载器之类的“奇技淫巧”来克服困难了。

2. 如果你是Apple用户并且又一个美区AppleID，恭喜你，你可以直接从App Store下载Telegram

当然，如果以上方案都不行，你还是老老实实用梯子吧，也不贵，有机场圈的朋友介绍的话就更简单了

![](https://cdn.jsdelivr.net/gh/HeliumOI/HeliumOI.github.io/images/1582504823938.jpg)

## Telegram的注册

因为Sophon酱在用macOS，所以暂时只有macOS的图例

![](https://cdn.jsdelivr.net/gh/HeliumOI/HeliumOI.github.io/images/1583162215202.jpg)

首先在这里输入你的手机号码，然后你就会很惊喜的发现……

无法连接

原因不言而喻，毕竟由于墙的存在，这类软件基本不可能直接连接，用VPN等梯子就能简单的解决这个问题；

当然，如果您实在是没钱，Telegram还提供了另一个选项：使用公益MTProxy代理

（不用担心，代理服务器看不到你的聊天内容）

比较靠谱的代理频道有@onessr @socks5list 等

顺带一提，MTPProxy代理经常会被屏蔽，所以平时最好多准备几个订阅频道以及梯子

连接上之后可以订阅代理频道，获取长期可用的链接

当然有条件的话最好还是用自己的代理

第一次打开时是无法设置代理的，这时不要慌，直接正常输入自己的电话号码，然后会弹出要求你设置代理的提示，按要求填写就可以了。

注册成功后会要求你填写自己的姓名~~（当然不用填真名~~

## Telegram的概念解释

毕竟 ~~露西娅酱~~ 毛子开发的软件，在很多操作习惯上都和国人有区别，具体说来如下：

### Telegram的好友机制

国内的IM中，QQ，微信等都有“好友”的概念，但Telegram中没有。Telegram的概念是“联系人”，是单向的，即：你可以将对方加为你的联系人，但你不一定是对方的联系人。

### Telegram的群组

Telegram群组其实就和QQ群，微信群差不多，但Telegram群组最大容量有20万人

同时，Telegram的公开群组有所谓“分享链接”，这意味着你不需要像微信那样发个二维码，直接用链接就能分享。即使是非公开群组，也有“邀请链接”，但“邀请链接”需要管理员才能查看。

另外，Telegram上的公开群组是可以在Google上被搜索到的，直接搜索“关键词 site:t.me”即可

### Telegram的频道

“频道”其实和群组没有本质差别，但区别在于：“频道”中只有一个用户，即管理用户能发言

## Telegram的注意事项

### Telegram汉化

根据官方介绍，Telegram提供 英语， 西班牙语， 德语， 荷兰语， 意大利语， 葡萄牙语， 朝鲜语， 俄语， 法语， 印尼语， 马来语， 波斯语， 乌克兰语的界面文字，但偏偏就不提供中文的，暂时还不知道原因。

不过，虽然官方不提供，也有第三方的热心人士自己对Telegram的界面进行了翻译；使用方法如下：

进入频道@zh_CN

![](https://cdn.jsdelivr.net/gh/HeliumOI/HeliumOI.github.io/images/1583165079891.jpg)

点击“点击此处安装语言包”

### Spam用户

大概是由于某些“币圈”人士经常用Telegram来推广比特币，+86手机号注册后会被官方直接判断为Spam（垃圾）账号，判断自己是否是Spam账号的方法是向其他用户发送私聊信息时是否显示“只能发信给双向联系人”

如果你注册时使用的是大陆的手机号，那么你已经被判定为Spam用户了。要解封也不难，联系官方账号@SpamBot，说明情况（用英文）即可

## 关于Telegram的一些问题

### Q:Telegram默认没有端到端加密，这是否意味着Telegram的安全性比WhatsApp、Facebook Messenger更低？

当然不是！

首先要明白一个概念，如果你进行真正的「端到端加密」，你的信息是无法在不同设备之间同步的。对于这一点，用过XMPP通讯的朋友应该很清楚，当你结束一次XMPP加密通讯后，在林一个地方登录账号，查看你的聊天记录时，只能看到一堆乱码。

这也是XMPP，Signal这类软件小众的原因之一，普通用户一半都有同步自己聊天记录的需求。

在WhatsApp等常用的通讯软件（微信、QQ等直接红牌罚下场，原因不言而喻）中，即使你选择了端到端加密，你的密钥也是保存在服务器端的，在你查看聊天记录是会使用保存的密钥解密。这意味着该软件公司或NSA等部门可以随时查看你的信息。

关于这一点的具体情况，大家可以下载爱德华·斯诺登的著作[《永久记录》的电子版](https://a.temporaryrecord.com/Permanent_Record_-_CN_edition_with_underlined_redactions.pdf)来看，里面有很多关于大规模监听的内容。

而Telegram是如何处理这一点的？在默认情况下，Telegram也和普通的通讯软件一样，将密钥保存在云端。（没人愿意自己的聊天记录一下线就消失！）但Telegram也可以选择「加密对话」，在这种情况下，加密通讯的密钥会在对话结束之后销毁。

在这里Sophon酱给大家一个小建议，如果真的不希望某些聊天记录被别人知晓，最好还是用「加密对话」的方式进行。虽然Telegram公司曾经因为密钥的事和俄罗斯联邦安全局打过官司，但一定要记住一句话：在信息安全方面，除了自己之外，不要相信任何人。

### 我注册了Telegram账号，我可以去/看那些地方？

推荐几个Telegram群组或频道：

[洛谷TG群（非官方）](https://t.me/joinchat/Gueflk8USNj6n68rA7aCEw)，这里是洛谷OIer的交流群，但不太活跃（大陆用户人数少

[OI WIki群](https://t.me/joinchat/GaEGzlAec5HRSoSxW7o2kg)，OI Wiki的群组，~~其实里面主要是几个大佬在处理工作。~~

退役OIer交流群，各种现役/退役OIer的聚集地。邀请链接暂时没有，可以找别人邀请加入

[Coder Offtopic 中文群](https://t.me/coder_ot)，关于技术的各种杂谈，里面有一些计算机技术方面的大神，讨论氛围不错

最后插一句，Sophon酱的用户是@SophonCI，有别的问题可以联系哦～
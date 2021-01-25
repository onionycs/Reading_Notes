[toc]

# preface

其实在读 *c primer plus* 的时候就已经开始了阅读 *computer networking a top down apporoach* 只是因为还没习惯document my work 所以就 拖到了**第二章第5节**来搞这个reading note。sry:cry::sob::sob::sob::sob:

之前的经历是学习了王道的自下网上的架构，感觉到很不能接受这种东西，接受的很慢，我认为的网络应该是与生活息息相关的， *computer networking a top down apporoach* 从应用层讲起，让我充满了兴趣。

> 网络的根本principle 是复杂的部分都在网络边缘(end system/host)实现

忘记这一句在书上哪一节看到的了..懒得找了...我觉得学网络学protocol就是去实现这些host.

http email dns P2P 我觉得超有意思. 但是还是想学更深的东西 比如shadowsocks的实现, clash 的实现等等.

keep in touch with the world 在别的地区可能很容易,我们(CN)要保持connection可太难了

现在<2021年1月12日11点43分>正在看BitTorrent(比特洪流协议)

稍等上传其余内容.至于之前的该怎么办，我觉得我之后还会再读一遍，到时候补上也可，但是我倾向是人生总要有点遗憾

不是吗？

## 2.5 Peer-to-Peer Applications 140

### 2.5.1 P2P File Distribution 140

看到这两级目录跟书上实际设置的目录不符。

First, which chunks should she request first from her neighbors? And second, to which of her neighbors should she send requested chunks? In deciding which chunks to request, Alice uses a technique called **rarest first**.最稀缺优先

aiming to (roughly) equalize the numbers of copies of each chunk in the torrent

在这个torrent（“洪流：分发互助小组”）中保证每个包的资源数基本一样，这就体现了算法在协议中的应用，在一个torrent中大家对话的对象是torrent的所有成员，看成一个整体就是整个小组成员，大家一起维护这个torrent中的资源（chunks）

> that are currently supplying her data at the highest rate.

给我(Alice)越多的我满足你的request越有较高的precedence

reciprocate = repay 报答

these four peers are said to be **unchoked**(疏通/好的关系).跟人情社会一样的,打通了的"关节"被称为unchoked

读到此处2021年1月12日15点11分我觉得BitTorrent这个协议是比较有趣的(因为拥有算法而且很仿真)我感觉在中国只能被别人**optimistically unchoked**因为我们成为不了别人的topfour. 

The effect is that peers capable of uploading at compatible rates tend to find each other. 聪明人跟聪明人玩?这个协议是一个赢家通吃的协议啊

choked = 阻塞 BitTorrent has a number of interesting mechanisms that are not discussed here, including pieces (minichunks), pipelining, random first selection, endgame mode, and anti-snubbing [Cohen 2003].这些东西感觉才是此协议的精髓部分

incentive 激励/提供动力,内部激励a thing that motivates or encourages one to do something.

tit for tat 针锋相对/复仇/报复/回报/一报还一报/有因必有果

circumvent = find a way around (an obstacle).破解bittorrent协议

variant = a form or version of something that differs in some respect from other forms of the same thing or from a standard. 变体/不同的版本

as the majority of the users would have been freeriders 每个人都讨厌freerider 白嫖

hash table 是一种用于查找的数据结构主要关注点在于怎么实现hash function, 应用层应用往往不是简单的一个协议就可以完成所有的事,例如此处的DHT, 和之前的DNS+web browser, DNS+email



我从来没看过配套网站的video真是遗憾啊,希望大家能有机会有时间去看看DHT的介绍



## 2.6 Video Streaming and Content Distribution Networks 147

the majority of the traffic = 主要流量/ 例如NetFlix?YouTube?

奈菲相当于漂亮国 只有订阅了才能上的 优酷爱奇艺,没有免费的资源,只付门票subscribe 提供正版高清的影视服务.

whopping = adjective very large.高达

### 2.6.1 Internet Video 148

为什么只提这些娱乐流式视频的供应商呢?我们的OCW不配拥有性命吗?

trade off = dispose of for compromise

off-the-shelf 现成的

salient = most noticeable or important.

envision (verb) imagine as a future possibility; visualize. 现在已经有8k了,但是我看的是第七版,哭了.

throughput 吞吐量/单位时间完成的量

### 2.6.2 HTTP Streaming and DASH 148

playback 回放

inception = the establishment or starting point of an institution or activity.

All clients receive the same encoding of the video, despite the large variations in the amount of bandwidth available to a client, both across different clients and also over time for the same client.

这只是写第7版的当时的youtube吧,现在已经有auto的清晰度选项了

The client dynamically requests chunks of video segments of a few seconds in length.

看来所谓的streaming也是表面的在微观来看也是几秒钟一段的小视频.

manifest file(告示文件)

a document giving comprehensive(全面的) details of **a ship** and its cargo(goods) and other contents, passengers, and crew for the use of customs officers.仓单

感觉今天记笔记有点用力过猛,之后的词汇就不往这上面记了,过于overkill了

### 2.6.3 Content Distribution Networks 149

assume 和 consumption

最屌的分享私货的方式就是搞一本书把自己觉得好的内容都夹带在里边。



### 2.6.4 Case Studies: Netflix, YouTube, and Kankan 153

proprietary = patent

novice = beginner 新手



## 2.7 Socket Programming: Creating Network Applications 157



### 2.7.1 Socket Programming with UDP 159

socket's identifier named **port name**



### 2.7.2 Socket Programming with TCP 164



## 2.8 Summary 170



## Homework Problems and Questions 171



## Socket Programming Assignments 180



## Wireshark Labs: HTTP, DNS 182



## Interview: Marc Andreessen 184




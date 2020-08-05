
## Wechat Block 微信封号

最近不知道怎么回事，被微信封号了。

理论上来说，微信封号我，我还真没有什么办法。

这个号，权利归属是谁的呢？

我估计，属于TX，虽然我没有去仔细研究，但是理该如此，否则宇宙最强法务部存在的意义是什么呢。

但是感情上来说，我不喜欢。

因为Control自我，是成熟人士的特征，遵守所在国家的法律法规，也是成熟人士的特征。

我认为，我是一个成熟人士。

那就去Fight吧。

```
仰天大笑出门去
我辈岂是蓬蒿人
```

---

### Update 20200804

其实，TX 对于 block 的用户，也不是什么都不能操作，还是可以 “受限” 登录的，只是 Social 功能无法使用。

具体来说，经过我这几天的观察，有如下规则

##### NO （那些你无法执行的动作，想法....可以有）

>发点对点消息，收点对点消息，加好友<br>
>建群，加群，发群消息，改群名，改群备注，加群成员<br>
>看服务号文章，看订阅号文章<br>
>邮箱看邮件内容（可以收到标题）

##### YES （人马合一，剑随人动）
>导出数据<br>
>特殊链接可以看（头条新闻、腾讯新闻等等，还在发现中）<br>
>选择文章然后发邮件（不理会连接错误的提示，继续操作，最后总能发出去的）<br>
>收群消息，退群<br>
>收点对点消息（某些人的消息可以收到，他们怎么操作的？电脑么？要测试一下）

我们从法律和技术两个角度来分析。

法律上看，微信号码，应该归属于 TX，因此它可以控制这个号码的使用，限制的行为，基本上都符合这个逻辑。
而这个号码产生的使用数据，则归属于用户，因此 TX 必须要允许用户导出自己的数据。

技术上看，IM通讯协议有很多种，XMPP是比价经典的，TX 的 Wechat 应该是有自己的扩展，但是核心框架应该差不多。
PUB-SUB 机制，TOPIC 分类。因此，限制某个 USER 的行为，是比较简单的实现，服务器的协议解析后，增加一个 Filter 逻辑搞定。

那么，为什么会有部分操作的逻辑存在矛盾？例如，可以“收群消息”，但是不能 “看服务号文章” ？

理论上来说，如果要限制 Social 访问，那么也要避免 block 的用户，作为一个 receiver 而接受其他人的消息，从而造成可能的潜在危害 :-O。

这个目标，不能 ”看服务号文章“ 实现了，但是 “收群消息” 却打破了，真是奇怪。

如果不是产品设计的问题，就是....测试时漏掉了:-)。

不过，挺好的。这个世界上，哪来那么多的坏人昵？

嗯，这篇文章 [枪口抬高一点](https://www.zhihu.com/question/20102444) 倒是挺有趣

```
休垂绝徼千行泪
共泛清湘一叶舟
```

### Update 20200803

这几天，TX 的客服不理我了。

自从上次他们 SMS 通知我以后，我再发Appeal，回答的基本上很快，晚上发....第二天早上....立刻回，明显是 “不再想理你” 的态度 :-C

我一直在询问，到底那条信息是 rumor，他们拒绝回答，只是重复到 “你违反XXX条款，请遵守XXX法律”。

好吧，我当然遵守XXX法律，否则 Policy 会请我去喝茶。既然 Policy 没有请我去喝茶，说明我没有违法，至少....还没有被证明违了法。

为了展现我的自信，我在 Appeal 中，痛心疾首地呐喊 “有事请报警”，千万不能放过坏人，对吧？

可惜，TX 依然不理我，依然是 “你违反XXX条款，请遵守XXX法律”，依然是冷漠的....客客气气，言辞让你觉得，是那么地....无可挑剔。

我估计，这应该是 TX 统一调教的客服应答规则：不理不睬，让投诉....自生自灭。

肿么办？我已经更换了 普通汉语/英语/法语/日语/德语 多种语法来 Appeal，然而....并没有什么用。

说句实话吧，我觉得我已经爱上 “你违法XXX条款，请遵守XXX法律” 这个修辞表达了，太 Adapative，太 General，太 Robust，太....无可奈何了 T_T

如果时光可以倒流，如果我们生活在星际救援五维宇宙中，我希望....能够早些....学会这句话掌握这句话说好这句话。
人世间，还有什么言语，比这句话，更加伟大昵？图灵测试....太 Native 了。

```
问世间情为何物
直叫人生死相许
```

### Update 20200728

嗯，很奇怪，今日 df595149790.github.io 无法访问了。

我试了试 github.io 这个域名，发现手机上都无法访问，包括 IPhone 和 Android，但是 Mac 的 Safari 可以访问。原因么....就不去猜测了。

那么，如何在 Appeal 中告知 TX 我的事件记录昵？只好用 github.com 的 md 文件路径了。

让我们看看 github.com 有没有可能，也无法访问？

```
无可奈何花落去
似曾相识燕归来
```

---

### Mainstream 20200725

```
金风玉露一相逢
便胜却人间无数
```

开始时，倒是没有记录的想法，不过时间长了，觉得维持现状，不是个办法，还是记录一下吧，万一....我要是不在了呢，对吧？

等记录多一些后，考虑进行程序处理，OCR识别图片后，进行一些数据分析，例如时间间隔、人员分布、自动整理写总结文章等等，看看技术，到底能改变多少世界 :-)



#### 缘起 

```
人生若只如初见
何事秋风悲画扇
```

早上一起来，打开微信，屏幕上看到这个提示

![image](/wechatblock/image/wb_1_logout.PNG)

What The Fxck? spreading rumor? 我怎么可能是这样的人呢？虽说 Country 限制的很严格，但我自己也管的很严格呀，最近说的话，也都是事实。

In general, I donnot like politicis。

继续操作，看到如下提示

![image](/wechatblock/image/wb_2_login_1.PNG)

继续，登录进来了，又显示如下提示

![image](/wechatblock/image/wb_2_login_2.PNG)

好吧，先 cancel 试试，结果发现无法给朋友发送信息。那 ok 又如何？进入了界面

![image](/wechatblock/image/wb_2_login_3.PNG)

![image](/wechatblock/image/wb_3_appeal_1.PNG)

![image](/wechatblock/image/wb_3_appeal_2.PNG)

然后......只好让朋友的手机扫码，来投诉喽


#### 缠绵

```
长宵无那欲西风
细雨敲窗问几更
```

20200717，开始了人生中的第一次。

根据伊的引导，一番摸索后，看到如下画面

![image](/wechatblock/image/20200717_0.jpg)

怎么办？反抗呀，发起了投诉如下

![image](/wechatblock/image/20200717_appeal.jpg)

看得出来，伊，一开始也是有些犹豫的，第二天晚上才互动了一下

![image](/wechatblock/image/20200717_reply.jpg)

嗯，没有抹平心头的冲动，反而泛起了更多涟漪。到底为什么呢？我决定....更加直接一些

![image](/wechatblock/image/20200718_appeal.jpg)

第二天，伊又答复我了，还是一样的羞涩

![image](/wechatblock/image/20200718_reply.jpg)

好吧，也许没有明白我的意思，我表达的太复杂了，简化一下语法，再次询问

![image](/wechatblock/image/20200720_appeal.jpg)

相同的反应....

![image](/wechatblock/image/20200720_reply.jpg)

怎么办？语言不通么？那换个通讯模型，再试试。English登场

![image](/wechatblock/image/20200721_appeal.jpg)

可惜结果....还是一样

![image](/wechatblock/image/20200721_reply.jpg)

我不知道，伊，到底有没有仔细观察我的发音，因为，伊的发音，倒是一模一样，这不像人类呀。

按照图灵测试来说，几番交互，我作为一个人类（虽然我难以自我证明，苏格拉底也不行），明显可以辨别，对方是愚蠢的 ifelse 代码，不是人类，更不属于 AI。

TX 的 NLP 技术，不可能这么差呀，对吧，否则，怎么能找到老干妈呢....

于是，我只好....尝试通过持之以恒的虔诚呐喊，期望有朝一日聆听到伊的无上真言。

策略么，就是在每次发音前，都带上一个日期，然后表达我的一些疑惑，例如

```
20200725：
I do not break any Law, 
or you can call the police and let the Law to make decision. 
So I think you should unblock my WeChat. 
Thanks.
```

嗯，伊，倒也不含糊，开始时，也是也是一样的发音

![image](/wechatblock/image/20200722_reply.jpg)

![image](/wechatblock/image/20200723_reply.jpg)

![image](/wechatblock/image/20200724_reply.jpg)

直到某一天，突然收到一条 SMS，重复了一下发音。

我....估计呢，伊还是被我的诚心所 touch 了一下。

同时呢，也担心我听不到伊过去已经重复无数遍的发音（虽然我听到了，但是我紧接着又发音了，But....我无法确定伊是否听到了我的发音）。

决定换个容貌来见我（就像....希腊神话中的戈耳贡三姐妹 Euryale，Stheno 和 Medusa 一样美丽），再次发出了相同的声音。

![image](/wechatblock/image/20200725_sms.jpg)

问题是，我始终没有明白，我到底错在哪里？而且，我并没有违法 Country 的法律，如果违法了，TX 可以报警呀？

那就让生活继续吧，也让我的发音继续，直到....某一天。


``` 
There are known knowns; 
there are things we know we know.
We also know there are known unknowns; 
that is to say we know there are some things we do not know.
But there are also unknown unknowns
the ones we don’t know we don’t know.
        -- Donald Rumsfeld
```

---

### TBD

BTW，其实没有Wechat的生活倒也不错。

我不想被打扰的人，不会主动打扰我，而我想去打扰的人，我会主动去打扰。








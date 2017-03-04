# 互联网安全：事与愿违的后门程序

>一些情报机构赞同在加密软件中放置后门程序，但是谁使用它们呢？

2016年1月2日

如果没有加密技术，互联网上传递的信息倒不如写在明信片上。因此，政府、银行和商业机构都对自己的信息加密，当然恐怖组织和犯罪团伙也是如此。

对情报机构而言，破解加密算法是一件优先事项。
使用计算机暴力破解的方式成本高昂且效率低下，因为编写加密程序比破解它们要容易得多。
一种替代方案是强迫企业们来帮助情报机构，破解客户的加密信息，一项旨在贯彻这一策略的新法律刚刚在中国通过，这种权力对西方情报机构来说也是梦寐以求的。
另一种选择是通过开后门的方式实现：在软件或硬件中保留缺陷用以猜解或窃取密钥。这些后门可能源于程序错误，在设计阶段形成（需要加密软件供应商的配合）或者通过未授权的代码改编——或者以上三者共同促成。


后门的问题就是这样，尽管它能让特工的工作更顺利，但也让互联网的每个人都失去了很多秘密。
近期Juniper公司（一家美国网络硬件和软件供应商）事件的启示，清楚地说明了这点。Juniper在12月紧急发布后门公告，最早可追溯到2012年，它使得任何人可以解读基于VPN软件的加密流量（虚拟私有网络），VPN广泛应用于全球的企业和政府机构，以透过公共互联网链接不同办公区。目前不清楚谁该为此事负责，但是可能是在一个情报机构安装后门程序后，其他人又秘密的修改过。
该后门涉及的加密标准包含一个有缺陷的随机数生成算法，它获得了美国国家安全局（NSA）的支持；另外一些线索指向中国或英国的情报机构。
 
针对不同侦查目标破解加密信息显然是情报结构的职责范围，这也是政府结构应当具备监测能力最好理由，当然是在国家安全利益和法律框架的情况下。为了侦查行动而引入后门程序，风险是可能被胡作非为的特工、敌国政府或者犯罪者滥用，而且是在合法的前提下。目前不清楚Juniper的后门程序是什么人安装、使用，结局是什么。
 
情报机构辩解称：该后门非常隐秘、足够复杂，他们未经授权而使用是不可能的。
但是外来者可能偶然发现或者窃取到这个漏洞的细节。特别是美国在安全储存保密数据方面的记录非常糟糕。
众所周知，在这个夏天，人事管理办公室发生泄密，包括20万以上联邦雇员（公务员）的敏感个人数据，据称是中国人干的。
有人称这一事件为美国情报史上最大的灾难。唯有Edward Snowden 泄密事件可以与之相比，（斯诺登：前国家安全局承包商雇员，目前居住在莫斯科）。（机场安全当局也不小心泄漏了万能钥匙——能打开大多数商业行李——一种物理上的后门）。


反击后门

因此强制性置入后门的观点应当抵制。他们可能被犯罪者利用、从整体上削弱互联网安全，亿万人民赖以进行银行和支付业务。
这种行为将损害公众对技术公司的信心，也使西方国家政府对独裁政权干涉互联网的批评更加困难。他们过分的要求在任何情况下都是徒劳的：没有后门的高性能加密软件，任何人在网上都可以免费获得。


与其通过后门程序削弱每个人的秘密，特工应当使用其他手段。
11月巴黎恐怖袭击之所以能成功，不是因为恐怖分子使用了高超的计算机技术，而是因为他们的活动信息没有被有效共享。
必要时，国家安全局和其他情报机构通常能用特殊方式在嫌疑人的计算机和手机上植入蠕虫病毒。这比使用一个通用的后门要困难和低效——但是它对别人更安全。


译者注释

NSA： National Security Agency
隶属美国国防部（DoD），办公地点在五角大楼，主管是现役军官。
和CIA工作的最大不同之处在于，后两者首要的工作是面向“人”的间谍活动，而NSA不能参与此类间谍活动
它的典型工作比如监视反越战活动，经济间谍活动，遭斯诺登泄露的公众信息是由NSA负责监控的。

a new law just passed in China
2015年7月1日，中国全国人大通过了新的《国家安全法》，首次提出“国家建设网络与信息安全保障体系”，“维护国家网络空间主权、安全和发展利益”

Juniper漏洞
 2015年12月发布紧急公告，称在对其NetScreen产品的内部代码审计过程中发现了两枚漏洞,可以让资深的攻击者获得对NetScreen设备的管理权限和解密VPN流量。








Internet security
When back doors backfire
Some spy agencies favour “back doors” in encryption software, but who will use them?
Jan 2nd 2016  | 



WITHOUT encryption, internet traffic might as well be written on postcards. So governments, bankers and retailers encipher their messages, as do terrorists and criminals.

For spy agencies, cracking methods of encryption is therefore a priority. Using computational brute force is costly and slow, because making codes is far easier than breaking them. One alternative is to force companies to help the authorities crack their customers’ encryption, the thrust of a new law just passed in China and a power that Western spy agencies also covet. Another option is to open “back doors”: flaws in software or hardware which make it possible to guess or steal the encryption keys. Such back doors can be the result of programming mistakes, built by design (with the co-operation of the encryption provider) or created through unauthorised tinkering with software—or some combination of the three.

The problem with back doors is that, though they make life easier for spooks, they also make the internet less secure for everyone else. Recent revelations involving Juniper, an American maker of networking hardware and software, vividly demonstrate how. Juniper disclosed in December that a back door, dating to 2012, let anyone with knowledge of it read traffic encrypted by its “virtual private network” software, which is used by companies and government agencies worldwide to connect different offices via the public internet. It is unclear who is responsible, but the flaw may have arisen when one intelligence agency installed a back door which was then secretly modified by another. The back door involved a faulty random-number generator in an encryption standard championed by America’s National Security Agency (NSA); other clues point to Chinese or British intelligence agencies.
Decrypting messages that involve one or more intelligence targets is clearly within a spy agency’s remit. And there are good reasons why governments should be able to snoop, in the interests of national security and within legal limits. The danger is that back doors introduced for snooping may also end up being used for nefarious ends by rogue spooks, enemy governments, or malefactors who wish to spy on the law-abiding. It is unclear who installed Juniper’s back door or used it and to what end.
Intelligence agencies argue that back doors can be kept secret and are sufficiently complex that their unauthorised use is unlikely. But an outsider may stumble across a weakness or steal details of it. America, in particular, has a lamentable record when it comes to storing secrets safely. In the summer it became known that the Office of Personnel Management, which stores the sensitive personal data of more than 20m federal employees and others, had been breached—allegedly by the Chinese. Some call that the biggest disaster in American intelligence history. It is rivalled only by the data taken by Edward Snowden, a former NSA contractor now living in Moscow. (The authorities responsible for airport security also let slip the details of master keys that can open most commercially available luggage—a form of physical back door.)
Push back against back doors
Calls for the mandatory inclusion of back doors should therefore be resisted. Their potential use by criminals weakens overall internet security, on which billions of people rely for banking and payments. Their existence also undermines confidence in technology companies and makes it hard for Western governments to criticise authoritarian regimes for interfering with the internet. And their imposition would be futile in any case: high-powered encryption software, with no back doors, is available free online to anyone who wants it.

Rather than weakening everyone’s encryption by exploiting back doors, spies should use other means. The attacks in Paris in November succeeded not because terrorists used computer wizardry, but because information about their activities was not shared. When necessary, the NSA and other agencies can usually worm their way into suspects’ computers or phones. That is harder and slower than using a universal back door—but it is safer for everyone else.

# [首页查询更多项目](https://github.com/GraduationProject-weixin) 包安装运行


# 50292wxapp微信小程序的民宿短租系统设计与实现

![picture](https://raw.githubusercontent.com/GraduationProject-springboot/.github/main/img/wx.png)

### 点击播放视频 ▼
[![Watch the video](https://i.sstatic.net/Vp2cE.png)]()


# 第1章 绪论](#_Toc11589_#_Toc11589_)
## 1.1课题开发背景
`   `目前我国已进入网络化时代，网络深入生活，给人们带来新的体验。现在很多的企业在办公中还是采用传统的方式，这是因为老的办公人员习惯传统的办公方式，认为新的办公方式使用不方便，没有传统的办公方式更有效率。企业加强培训使越来越多的员工接受新的办公方式。采用计算机和网络进行办公的新方式可以缩短工作时间，从而减轻工作压力[1]。

民宿是最基本的生活设备，对于外出旅游、出差人员来说非常重要。好的民宿不单是环境好、民宿配置好，更是价格合适、售后服务好。目前，人们找民宿都还是找中介进行，这种效率非常高，但往往是一性交易，售后没有保障。现如今中介跑路的例子比比皆是，中介最大的问题就是不能直接面对房主，所有的信息都是由中介在中间传达[2]。如果中介在中间添油加醋，对房主和租客都是致命的影响。对房主来说找租客没有有效的平台，也只能通过中介，被动性太强。民宿短租行业想要取得好的评价和拥有好的市场就需要进行变革[3]。
## 1.2课题研究现状
`    `目前民宿租赁大致可以分为几种方式，第一，张贴小广告，这种方式宣传效果不好，经常会被其它广告覆盖。还需要打印多张进行张贴，浪费时间和金钱，而效果却是最不好的[4]。第二，在物业登记出租信息，目前好的小区都有门禁，外人不会轻易进入。物业都设立在小区里，所以这种方式的效果也非常不理想。第三，找专业的民宿中介，这种方式效果好，但需要中介费用，而且不能直接对面房主、租客，中间信息的传达会造成以后售后的问题。第四，现在也有大量的民宿短租平台，像58同城、贝壳网。这类都属于第三方平台，想要获得展示和流量都得额外付费。而且目前这些民宿短租平台都被中介占领，发布的信息真实性令人怀疑[5]。
## ` `1.3课题研究内容
`   `本系统为免费的房主直对房客的民宿短租系统。在本平台里用户可以浏览所有的民宿信息，可以分地区进行民宿信息的查询、浏览。选择好民宿后可以实地看房，加快租赁效率。管理员可以管理民宿信息和用户的订单信息。房主可以发布自己的民宿和管理租赁自己的订单。本系统包括用户和管理员、房主三种身份。
## 1.4论文结构安排
`   `本篇论文为民宿短租系统的设计实现过程的描述。包括：

（1）摘要：简单介绍本论文的内容和本系统的内容；

（2）外文翻译：对摘要进行英文的翻译；

（3）目录：方便阅读人员快速找到需要的内容；

（4）第1章 绪论：描述课题的开发背景、现状和本课题的内容；

（5）第2章 系统开发技术和环境介绍：针对本系统开发时需要的语言、技术、环境等进行介绍；

（6）第3章 系统分析：本章包括需求分析，可行性分析，功能性分析和操作分析等；

（7）第4章 系统设计：本章主要包括系统的功能结构设计和数据库ER图设计，数据库表的设计；

（8）第5章 系统实现：本章从用户功能，管理员功能，房主功能进行界面实现的描述；

（9）第6章 系统测试：本章从系统的重要功能进行测试的描述；

（10）总结：总结全文做出自己的感想；

（11）参考文献：列出写出本篇论文时参考的所有资料和文献；

（12）致谢：列出想要感谢的人。
# 第2章 系统开发技术和环境介绍
## 2.1Java语言介绍
`   `Java语言是由sun公司在1995年开发的。自Java语言面市后，互联网的应用出现了新的生机，都提供了Java的虚拟机，在当前大多数的操作系统中都加入了Java的编译器[6]。Java语言可以实现虚拟机和应用编程进行接口，可以提供单独的标准。Java可以提供基本部分和扩展部分。在电脑里只要安装了Java平台，Java编写的项目就可以直接运行。现在大多数的操作系统里都支持Java程序。并且Java语言的兼容性特别强，非常受编程人员的喜欢[7]。
## 2.2Vue技术介绍
`  `Vue技术是属于Java的页面技术，是部署在服务器上的可以通过客户端进行反馈的技术。Vue可以生成html文档格式的页面，可以为用户提供http的服务。Vue技术可以应用到静态页面中[8]。通过静态页面的模板来生成动态页面。Vue技术可以不受平台的限制，在多个平台上运行。Vue技术还可以形成servlet代码，通过Java编译成servlet代码，然后再形成二进制的代码[9]。
## 2.3MySQL数据库介绍
MySQL数据库是一种关系型的数据库，属于MySQLab公司的产品。MySQL数据库通过不同的表将数据进行保存，实现了数据的灵活运用。MySQL数据库具有体积小、运行速度快、编译简单的特点[10]。并且MySQL数据库可以免费使用，减少开发人员的开发成本。MySQL数据库可以搭配多种平台使用，最常用的平台有visual studio和Java、php等。所以近几年来使用MySQL数据库的人非常多[11]。
## 2.4B/S框架介绍
B/S是一种web结构，统一了客户端，改变了固定端的要求。可能把系统都放到服务器上，用户只需要浏览器就可以运行。使系统的开发、运行、维护都更加简单[12]。随着网络的发展，C/S框架不再适应时代的要求。想要实现共连和随时随地的办公就需要采用B/S框架。B/S框架包括三层。第一层为浏览器，可以直接由浏览器进行信息的展示，第二层为web服务器，当用户有要求时可以把要求反应到服务器上，然后再由服务器将结果反馈到浏览器上。第三层为数据库服务器，数据库服务器可以存入大量的数据，当需要调用数据时就可以直接在数据库服务器中使用[13]。
## 2.5微信小程序介绍
微信小程序是一种不用下载就能使用的应用，也是一项创新，经过将近两年的发展，已经构造了新的微信小程序开发环境和开发者生态。微信小程序也是这么多年来中国IT行业里一个真正能够影响到普通程序员的创新成果，已经有超过150万的开发者加入到了微信小程序的开发，与我们一起共同发力推动微信小程序的发展，微信小程序应用数量超过了一百万，覆盖200多个细分的行业，日活用户达到两个亿，微信小程序还在许多城市实现了支持地铁、公交服务。微信小程序发展带来更多的就业机会，2017年小程序带动就业104万人，社会效应不断提升。












# 第3章 系统分析
## 3.1系统的需求分析
本系统的实现可以改变传统租赁民宿的问题。改变找中介租赁民宿不透明需要交中介费的问题，改变去物业登记、张贴广告效果低的问题，改变现在大部分民宿短租平台信息不真实，都是中介市场的问题。本系统是利用现代技术的新型系统，可以满足用户随时浏览民宿，随时在线预订的需求，也可以满足了解市场的需求，同时满足房主快速找到房客的需求，帮助管理人员管理信息的需求。
## 3.2系统可行性分析
系统的可行性包括系统在开发整个过程中可能遇到的所有问题的分析，本部分内容必不可少。一般系统的可行性分析包括经济可行性分析，技术可行性分析，操作可行性分析[14]。在此基础上，本人加上法律可行性分析和组织、管理可行性分析。
### 3.2.1技术可行性分析
`   `技术可行性通常下是指本系统的实现在开发时所需要的条件、环境是否支持。本系统在后期的维护、升级上所需要的条件、环境是否支持。本系统在开发时需要Java语言和MySQL数据库以及Vue技术等，这些技术都是常用的成熟技术，可以支持。本系统运行需要微信开发者工具软件，微信开发者工具软件可以在网上下载，而本系统运行需要的电脑也为常用的设备，所以本系统在技术可行性上分析是没有问题的。
### 3.2.2经济可行性分析
`    `经济顾名思义就是本系统在前期、中期和后期所需要的经济支持。本系统在开发前期需要电脑和编程软件，编程软件可以免费下载，电脑为本人上大学已购得，不需要再次购买。本系统在后期也不需要经济的支出。所以本系统在经济的可行性分析上是没有问题的。
### 3.2.3操作的可行性分析
`   `本系统在开发时参考了用户的操作习惯也设计了大量的提示操作。使本系统在使用时不用去培训就可以使用。本系统对于布局也参考了热门网站，相信本系统在操作的可行性分析上也是没有问题的。
### 3.2.4法律上的可行性分析
本系统在开发上，功能上，界面上等都没有抄袭其它系统，并且本系统也不会涉及到收费的问题。所以本系统在法律上的可行性分析上没有问题。
### 3.2.5组织和管理的可行性分析
`    `本系统的开发的根本在于人，也就是本人是否有能力开发本系统。社会是否支持本系统的开发。本系统在今后的使用中是否会被社会认可。所以本系统在开发时需要注意系统的可法性和生命周期性。
## 3.3系统性能方面分析
系统的性能主要表现在系统的扩展、升级，系统的数据反应，系统的完整性和开放性等。本系统的性能方面分析详情为：

1. 在开发系统时需要周全的想到系统开发后的扩展问题和系统的开发工作量问题。还要想到系统在后期的运行速度和用户使用后的反应速度。本系统在开发时充分预留接口[15]。
1. 系统中数据的安全非常重要。当用户操作后，数据要及时的进行更新、变化。当用户操作后也要进行及时的反馈，在系统开发的前期就要设定好标准，才可以使系统的后期维护简单。
1. 在开发系统时同样也要想到系统的开发语言和技术，不仅要选择自己熟练的，也要选择市场上有保障的[16]。
1. 系统中的数据要注意一致性和完整性以及安全性和共享性。
## 3.4系统功能方面分析
`   `通过调研现在已有的民宿短租系统和结合自己的能力以及用户的实际需求，设计出本系统的功能为民宿信息、公告信息、评论信息、预订信息、用户信息、收藏信息等。本系统包括管理员和用户、房主三种身份。
## 3.5系统流程分析
`   `本系统的流程为用户先进行注册，注册后可以进行登录。在首页用户可以看到民宿信息和公告信息，可以在线租赁。管理员负责公告信息的发布。用户可以实现我的预订管理和我的收藏管理，管理员负责更新管理公告和审核民宿、预订等。房主可以发布民宿和管理预订。本系统的管理员和用户、房主都是需要登录后才能进行相关操作。用户登录流程图如下图3.1所示：

![C:\Users\Administrator\AppData\Roaming\Tencent\Users\441709118\QQ\WinTemp\RichOle\5[GJ[(\_\_L65%EI6%$@)ICB1.png](/md/blog.001.png "5[GJ[(\_\_L65%EI6%$@)ICB1")

图3.1系统用户登录的流程图

（1）管理员的流程为审核民宿信息和用户信息，发布公告信息和管理房主信息、预订信息，管理房间类型信息等。管理员的流程图如下图3.2所示：

![](/md/blog.002.png)

图3.2管理员的系统操作流程图

（2）用户的流程为在线注册，然后登录。在首页浏览民宿、公告。在线预订和在线评论等。用户的操作流程图如下图3.3所示：

![](/md/blog.003.png)

图3.3用户的系统操作流程图

(3)房主可以发布民宿和管理预订。房主的流程图如下图3.4所示：

![](/md/blog.004.png)

图3.4房主操作流程图

(4)本系统中主要的功能为民宿浏览、民宿预订、民宿评价、预订管理。系统流程图如下图3.5所示：

![](/md/blog.005.png)图3.5系统流程图
1


# [第4章 系统设计](#_Toc8006_#_Toc8006_)
## [4.1系统设计的目标](#_Toc273815983)
系统设计的目标是满足用户的需求和满足系统实现所需要的所有要求。本系统收集了信息浏览、信息删除、信息添加、信息修改、信息查询为一体[17]。改变了用户民宿短租的方式，提高管理员管理效率以及用户预订的效率。为用户、房主提供专业的民宿短租系统。
## [4.2系统功能结构图设计](#_Toc273815983)
本系统的结构分为管理员、用户、房主三部分。本系统的功能结构图如下图4.1所示：

![](/md/blog.006.png)         图4.1民宿短租系统的功能结构图
## 4.3数据库设计
数据库为数据的存放地。集合着系统中所有的数据。可以单独设计。一个系统想要拥有快速的反应和保证数据的安全就需要一个好的数据库[18]。每种不同的数据都有属于它的数据库表。数据库设计包括数据ER图设计和数据库表设计。数据ER图里设计了实体以及实体的属性。数据库表设计了不同数据的类型、长短等[19]。
### 4.3.1数据E-R图
`   `数据ER图就是把抽象的数据进行建模，通过不同的图形来清晰化的表示数据。数据库设计的第一步就是数据ER图的设计。本系统中主要的数据为管理员信息、用户信息、民宿信息和预订信息等。

1. 管理员信息为管理员身份的资料，包括编号和密码、账号。管理员信息ER图如下图4.2所示：

![](/md/blog.007.png)

图4.2管理员信息ER图

（2）用户信息为用户身份的资料。用户身份的资料有账号、密码、电话、住址等。用户信息ER图如下图4.3所示：

![](/md/blog.008.png)

图4.3用户身份的ER图

（3）民宿信息可由房主进行发布，民宿信息包括面积、价格，装修等，民宿信息ER图如下图4.4所示：

![](/md/blog.009.png)

图4.4民宿信息ER图

（4）预订信息也是由用户产生，管理员审核，房主管理。预订信息包括类型、民宿户型、民宿面积等。预订信息ER图如下图4.5所示：

![](/md/blog.010.png)

图4.5预订信息ER图

（5）系统全局ER图如下图4.6所示：

![](/md/blog.011.png)

图4.6系统全局ER图
### 4.3.2数据库表设计
`   `数据库表是将数据ER图进一步细分和实现。数据库最终是以数据库表呈现。通过对不同的实体设置不同的字段类型和长短、标识来进行数据库表的实现。在数据库表设计中要注意数据的冗余问题和范式问题。本系统的数据库表有管理员信息表、民宿信息表、预订信息表和公告信息表等。本系统的数据库表如下表4.1-4.11所示：

表4.1 config

||
| :- |

|序号|列名|数据类型|长度|小数位|标识|主键|外键|允许空|默认值|说明|
| :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- |
|1|id|bigint|20| |是|是| |否| |auto\_increment|
|2|name|varchar|100| | | | |否| | |
|3|value|varchar|100| | | | |是| | |

||
| :- |
表4.2 discussminsuxinxi

||
| :- |

|序号|列名|数据类型|长度|小数位|标识|主键|外键|允许空|默认值|说明|
| :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- |
|1|id|bigint|20| |是|是| |否| |auto\_increment|
|2|addtime|timestamp| | | | | |否|CURRENT\_TIMESTAMP| |
|3|refid|bigint|20| | | | |否| | |
|4|userid|bigint|20| | | | |否| | |
|5|nickname|varchar|200| | | | |是| | |
|6|content|longtext| | | | | |否| | |
|7|reply|longtext| | | | | |是| | |

||
| :- |
表4.3 fangjianleixing

||
| :- |

|序号|列名|数据类型|长度|小数位|标识|主键|外键|允许空|默认值|说明|
| :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- |
|1|id|bigint|20| |是|是| |否| |auto\_increment|
|2|addtime|timestamp| | | | | |否|CURRENT\_TIMESTAMP| |
|3|fangjianleixing|varchar|200| | | | |是| | |

||
| :- |
表4.4 fangzhu

||
| :- |

|序号|列名|数据类型|长度|小数位|标识|主键|外键|允许空|默认值|说明|
| :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- |
|1|id|bigint|20| |是|是| |否| |auto\_increment|
|2|addtime|timestamp| | | | | |否|CURRENT\_TIMESTAMP| |
|3|fangzhuzhanghao|varchar|200| | | | |否| | |
|4|mima|varchar|200| | | | |否| | |
|5|fangzhuxingming|varchar|200| | | | |否| | |
|6|touxiang|varchar|200| | | | |是| | |
|7|xingbie|varchar|200| | | | |是| | |
|8|lianxidianhua|varchar|200| | | | |是| | |
|9|shenfenzhenghao|varchar|200| | | | |是| | |

||
| :- |
表4.5 minsuxinxi

||
| :- |

|序号|列名|数据类型|长度|小数位|标识|主键|外键|允许空|默认值|说明|
| :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- |
|1|id|bigint|20| |是|是| |否| |auto\_increment|
|2|addtime|timestamp| | | | | |否|CURRENT\_TIMESTAMP| |
|3|minsumingcheng|varchar|200| | | | |否| | |
|4|minsutupian|varchar|200| | | | |是| | |
|5|fangjianleixing|varchar|200| | | | |是| | |
|6|minsuxingji|varchar|200| | | | |否| | |
|7|yiwanjiage|int|11| | | | |是| | |
|8|minsudizhi|varchar|200| | | | |是| | |
|9|minsujieshao|longtext| | | | | |是| | |
|10|fangzhuzhanghao|varchar|200| | | | |是| | |
|11|lianxidianhua|varchar|200| | | | |是| | |
|12|clicktime|datetime| | | | | |是| | |
|13|clicknum|int|11| | | | |是|0| |

||
| :- |
表4.6 minsuyuding

||
| :- |

|序号|列名|数据类型|长度|小数位|标识|主键|外键|允许空|默认值|说明|
| :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- |
|1|id|bigint|20| |是|是| |否| |auto\_increment|
|2|addtime|timestamp| | | | | |否|CURRENT\_TIMESTAMP| |
|3|yuyuebianhao|varchar|200| | | | |是| | |
|4|minsumingcheng|varchar|200| | | | |是| | |
|5|minsutupian|varchar|200| | | | |是| | |
|6|fangjianleixing|varchar|200| | | | |是| | |
|7|minsudizhi|varchar|200| | | | |是| | |
|8|fangzhuzhanghao|varchar|200| | | | |是| | |
|9|yiwanjiage|int|11| | | | |是| | |
|10|ruzhuriqi|date| | | | | |是| | |
|11|ruzhutianshu|int|11| | | | |是| | |
|12|zongjine|int|11| | | | |是| | |
|13|yuyueshijian|datetime| | | | | |是| | |
|14|beizhu|varchar|200| | | | |是| | |
|15|yonghuzhanghao|varchar|200| | | | |是| | |
|16|yonghuxingming|varchar|200| | | | |是| | |
|17|shoujihaoma|varchar|200| | | | |是| | |
|18|sfsh|varchar|200| | | | |是|否| |
|19|shhf|longtext| | | | | |是| | |
|20|ispay|varchar|200| | | | |是|未支付| |
|21|userid|bigint|20| | | | |是| | |

||
| :- |
表4.7 news

||
| :- |

|序号|列名|数据类型|长度|小数位|标识|主键|外键|允许空|默认值|说明|
| :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- |
|1|id|bigint|20| |是|是| |否| |auto\_increment|
|2|addtime|timestamp| | | | | |否|CURRENT\_TIMESTAMP| |
|3|title|varchar|200| | | | |否| | |
|4|introduction|longtext| | | | | |是| | |
|5|picture|varchar|200| | | | |否| | |
|6|content|longtext| | | | | |否| | |

||
| :- |
表4.8 storeup

||
| :- |

|序号|列名|数据类型|长度|小数位|标识|主键|外键|允许空|默认值|说明|
| :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- |
|1|id|bigint|20| |是|是| |否| |auto\_increment|
|2|addtime|timestamp| | | | | |否|CURRENT\_TIMESTAMP| |
|3|userid|bigint|20| | | | |否| | |
|4|refid|bigint|20| | | | |是| | |
|5|tablename|varchar|200| | | | |是| | |
|6|name|varchar|200| | | | |否| | |
|7|picture|varchar|200| | | | |否| | |
|8|type|varchar|200| | | | |是|1| |
|9|inteltype|varchar|200| | | | |是| | |

||
| :- |
表4.9 token

||
| :- |

|序号|列名|数据类型|长度|小数位|标识|主键|外键|允许空|默认值|说明|
| :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- |
|1|id|bigint|20| |是|是| |否| |auto\_increment|
|2|userid|bigint|20| | | | |否| | |
|3|username|varchar|100| | | | |否| | |
|4|tablename|varchar|100| | | | |是| | |
|5|role|varchar|100| | | | |是| | |
|6|token|varchar|200| | | | |否| | |
|7|addtime|timestamp| | | | | |否|CURRENT\_TIMESTAMP| |
|8|expiratedtime|timestamp| | | | | |否|CURRENT\_TIMESTAMP| |

||
| :- |
表4.10 users

||
| :- |

|序号|列名|数据类型|长度|小数位|标识|主键|外键|允许空|默认值|说明|
| :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- |
|1|id|bigint|20| |是|是| |否| |auto\_increment|
|2|username|varchar|100| | | | |否| | |
|3|password|varchar|100| | | | |否| | |
|4|role|varchar|100| | | | |是|管理员| |
|5|addtime|timestamp| | | | | |否|CURRENT\_TIMESTAMP| |

||
| :- |
表4.11 yonghu

||
| :- |

|序号|列名|数据类型|长度|小数位|标识|主键|外键|允许空|默认值|说明|
| :- | :- | :- | :- | :- | :- | :- | :- | :- | :- | :- |
|1|id|bigint|20| |是|是| |否| |auto\_increment|
|2|addtime|timestamp| | | | | |否|CURRENT\_TIMESTAMP| |
|3|yonghuzhanghao|varchar|200| | | | |否| | |
|4|mima|varchar|200| | | | |否| | |
|5|yonghuxingming|varchar|200| | | | |否| | |
|6|touxiang|varchar|200| | | | |是| | |
|7|xingbie|varchar|200| | | | |是| | |
|8|shoujihaoma|varchar|200| | | | |是| | |

||
| :- |

#













# [第5章 系统功能的实现](#_Toc10150_#_Toc10150_)
## 5.1 系统界面实现
### 5.1.1界面设计原则
`   `系统的界面设计至关重要。良好的界面可以给人好的感受和良好的操作体验。在系统界面设计时需要遵守的原则为：

1. 不同的身份使用的功能不同，所以要设计不同的登录界面以便来区分不同的身份。在设计界面时首先要考虑好身份的区别和不同身份的界面功能，根据不同的身份来设计不同的操作界面；
1. 要采用尽可能减少手动输入的方式进行设计。对于某些信息如果可以减少输入就都自动生成，这样也可以减少用户手动输入时的错误；
1. 设置大量的帮助词和提示词来指导用户的操作，减少用户的记忆。
### 5.1.2数据输入界面设计
为了减少用户手动输入的次数，增加系统的容忍有力，在数据输入界面设计时就要注意以下几点：

1. 对于多种字段需要输入里可以采用列表框。比如在输入房间类型，租赁时间时，可以选择信息进行填写。对于需要大量文字描述的特定信息时可以选择特定缩写、数字等来代替；
1. 对于同一类型的信息在输入时可以采用统一的界面风格，可以培养用户的输入习惯。对于特定信息在输入时可以设定好数据类型，比如在输入手机号时只能输入数字，在输入数量时，只能输入数字。
## 5.2 主要功能模块实现
### 5.2.1用户登录功能模块的实现界面
本系统需要登录才可以使用相关功能。用户登录功能的操作步骤为，用户点击用户登录功能，可以跳转到用户登录的窗口界面里，在用户登录的窗口界面里输入账号和密码，然后点击登录按钮。用户登录窗口的界面实现如下图5.1所示：

![](/md/blog.012.png)

图5.1用户登录功能的窗口实现界面

用户登录的流程为当用户输入信息后，会自动进行数据的比对，当比对通过可以登录成功，当比对错误会提示账号或者密码错误，需要重新登录的提示。用户登录的流程图如下图5.2所示：

![](/md/blog.013.png)

图5.2用户登录的流程
### 5.2.2修改密码功能模块的界面实现
`   `修改密码可以保证账号的安全，本功能为基础功能。修改密码的实现如下图5.3所示：

![](/md/blog.014.png)图5.3修改登录密码的功能实现界面
### 5.2.3用户注册模块功能的实现
`    `用户注册功能可以实现成为本系统用户的作用。当用户点击用户注册功能时界面会进入新的注册界面。注册的流程为用户填写注册信息，数据库先进行判断数据是否正确，如果正确可以在数据库中插入用户信息，如果信息错误，则会提示注册失败。用户注册功能的流程如下图5.4所示：



![](/md/blog.015.png)

图5.4用户注册功能的实现流程

用户注册的实现界面如下图5.5所示：

![](/md/blog.016.png)

图5.5用户注册功能的实现界面
### 5.2.4评价功能模块的界面实现
用户评价的流程为用户点击评价功能，然后输入评价信息，当评价信息为有效时，可以评价成功，当评价信息为无效时，需要重新评价。用户评价的流程如下图5.6所示：

![](/md/blog.017.png)

图5.6用户评价的流程图

用户评价的实现界面如下图5.7所示：

![](/md/blog.018.png)

图5.7用户评价的实现效果界面
### 5.2.5新闻公告功能模块的实现界面
`     `公告信息是由管理员负责管理的，用户可以在前台看到公告的详细信息，在公告功能里，公告可以由列表进行标题、时间的展示。当想了解具体的公告信息时，可以点击标题进入公告详情界面。公告功能的实现界面如下图5.8所示：

![](/md/blog.019.png)

图5.8公告功能的实现界面
### 5.2.6民宿详情的功能实现界面
在民宿详情界面里可以看到详细的民宿信息，包括类型、户型、面积、价格等。民宿详情里有联系方式，用户可以实现在线预订。民宿详情的实现界面如下图5.9所示：

![](/md/blog.020.png)

图5.9民宿详情功能模块的实现界面
### 5.2.7在线预订功能模块的实现界面
用户在预订民宿时需要填写入住日期、入住天数和订单备注。在线预订信息的实现界面如下图5.10所示：

![](/md/blog.021.png)

图5.10在线预订功能的实现界面
### 5.2.8民宿预订管理功能界面的实现
用户预订成功后可以管理预订信息。民宿预订管理功能的实现界面如下图5.11所示：

![](/md/blog.022.png)

图5.11民宿预订管理功能的实现界面
## 5.3房主注册功能的实现界面
房主也可以通过注册实现系统的使用。实现界面如下图5.12所示：

![](/md/blog.023.png)

图5.12房主注册功能的实现界面
### 5.3.1房主功能界面的实现
`     `本界面分为图片、文字、标题、按键、列表等。房主可以发布民宿和管理预订信息以及个人信息。房主界面的实现效果如下图5.13所示：

![](/md/blog.024.png)

图5.13房主功能界面的运行实现效果 
## 5.4管理员功能的实现界面
管理员的功能为用户管理、房主管理、民宿管理、房间类型管理、预订管理和系统管理等。实现界面如下图5.14所示：

![](/md/blog.025.png)

图5.14管理员功能的实现界面












# 系











- ### 使用者需求概述

 **目标用户：**
 
分布地区：以一，二线城市为主

年龄区间：在20岁~50岁之间的博物馆游客

 **目标用户分类：** 

1.使用直观介绍工具的游客：喜欢直接通过博物馆直观的文字介绍去了解到博物馆展品信息的游客。

2.使用电子产品工具的游客：面对人多的情况部分游客喜欢直接使用搜索引擎搜索自己所感兴趣的展品信息。

3.既使用直观介绍又使用电子产品的游客：大部分展品通过博物馆直观的文字介绍去了解展品，遇到自己感兴趣的展品会使用搜索引擎去寻找更多有关展品的信息。


 **功能使用场景：** 

1.当人们在参观博物馆的时候面对拥挤的人群时并不想长时间的呆在展品前去查看相关的介绍时，他们可能会希望只需要用手机扫一扫展品便能跳转出展品的数据和相关的介绍信息，这样的操作不仅可以缓解博物馆人流，人们也不需要排队去看主管的展品信息，只需要用手机扫描一下展品便可以查看到相关的展品信息和拓展信息；

2.针对国外的游客，博物馆中直观的信息介绍通常只设置中文和英文两种语言，当外国游客想要了解展品却因为语言的障碍而无法了解到展品时，他们会希望能通过简单的手机操作就可以扫描出展品翻译后的信息，从而减少浏览过程中语言障碍的问题

3.针对年纪稍大的游客，他们的视力和听力功能可能不够灵敏，这类游客可以打开手机扫描展品，手机屏幕跳转至展品信息和拓展的知识，用户还可以根据自己的情况选择有声朗读功能。


- ### 产品主要概述总结

 **核心功能** 

我们产品 _以数据管理为基础，API服务为核心_ ，系统管理为支撑，将藏品信息、历史关联信息，管理人员信息，在数据共享及数据联动的基础上，实现文物识别、知识整合、语音翻译和语音合成的协同工作，旨在全面有效的提升参观者对于博物馆藏品的认知度，弘扬历史文化的博大精深。

 **产品背景** 

博物馆是非营利的永久性机构，对公众开放，为社会发展提供服务，以学习、教育、娱乐为目的。博物馆是对历史知识的系统整理、直观呈现，如今许多的参观者都会带着学习的态度对博物馆进行参观。随着数字化技术的不断成熟发展，各大博物馆也着手建立自己的线上博物馆。而技术落地难、技术使用成本高、用户互动不足等问题，让不少博物馆望而却步。

 **产品价值** 

1. API 对于现代企业而言至关重要，可以为其运营和产品以及合作伙伴战略等各方面增加新的功能。例如语音识别、语音合成API可以自动帮助用户识别并翻译文物信息，这样可以大大的节省下导游翻译的成本。

2. 以教育、研究和欣赏为目的，向公众展示人类活动和自然环境的见证物。在向游客展示文物的同时，讲解文物背后的各种奇幻故事，为游客提供一次精神上的“视觉盛宴”。

3. API 可以在企业的现有业务模式之外产生全新的商机。我们可以在帮助用户了解的文物的同时为用户推荐文物小周边，以此达到互利共赢的目的。

 **加值宣言** 

1. 结合 _API图像识别_ 对博物馆产品实现一个知识拓展的功能，可使得参观者了解到更多历史故事、传说、书籍等，为参观者的博物馆之旅带来丰富的知识体验。

2. 在文物拓展文本上结合 _API文本翻译_ 的功能，可以帮助不同国家的参观者解决语言不同的问题。

3. 拓展文本上结合 _API语音合成_ 的功能，可将文本内容转换为语音，使参观者可以实现边听边观看的观览体验。


 **成本分析：** 
- 技术支持成本：包括调用API需要给API平台支付的费用，对产品功能的设计、开发、雇用技术咨询人员的成本和对博物馆展品进行数据化和数字化并存储于云端的成本
- 维护管理成本：博物馆需要投入一定的人力、物力、财力进行定期维护，及时更新展品信息
- 风险成本：由于采用第三方API平台的服务，存在一定的不确定性，一旦第三方平台出现问题或产生纠纷，功能的可用性将大打折扣

 **效益分析：** 
- 通过知识拓展，帮助参观者更好地了解展品信息，可以丰富参观者的积极情感，提高用户体验，使参观者感到物超所值
- 完善博物馆的服务功能，继而提升用户评价，提升博物馆竞争力
- 吸引到更多的参观者，包括更多的外国游客，继而形成良好口碑效应，既能提高博物馆人流量，方便博物馆创收，又能让更多人更好地了解中国，体现社会教育价值
- 云端展品信息可以作为线上科普和博物馆宣传的信息来源，提高博物馆知名度


- ### 原型

![用户界面](https://images.gitee.com/uploads/images/2019/1116/133331_0934a28e_1648150.png "用户界面.png")

- ### 功能需求

#### 一、
##### 模块描述

 _知识拓展_ 

##### 功能描述
用户通过手机扫描文物，通过微软图像识别API，可查看到被扫描文物的基本信息和拓展信息。

##### 需求说明
1. 用户首次使用，通过手机扫描文物或展示台上的二维码后，打开语言选择的页面，语言选择成功后，打开知识拓展页面；若非首次使用，扫描文物或二维码后，打开知识拓展页面；
2. 若扫描不成功，打开空白页面，文字提示用户“暂无该展品信息，请重新扫描”；
3. 扫描框下显示文字“将二维码/文物放入框内，即可自动扫描”；
4. 若当前环境太暗，扫描框下显示文字“当前环境太暗”；扫描框底部显示“手电筒”图标；
5. 知识拓展页面标题为文物的名称，内容包括文物的图片、基本信息和拓展信息，标题下放置语音朗读模块和语言选择模块；
6. 引用部分设置超链接，可以让用户跳离该页面并打开超链接的页面；返回时，回到知识拓展页面；
7. 页面底部，用户可以对次介绍进行点赞、收藏、分享和评论；
8. 分享到微信等社交媒体时，会自动生成简单的介绍图文，图片默认为官方图片，用户也可以通过点击图片更改为自己拍摄的照片；
9. 记录用户的扫描数据，找到游客的兴趣点，根据兴趣点举办相关的活动和制作、销售相应的纪念品。并且通过推荐算法，为用户提供推荐的浏览路线、纪念品和相关活动；

#### 二、
##### 模块描述

 _语音朗读_ 

##### 功能描述
通过语音合成，为视力不好或不方便阅读的游客提供语音朗读服务，相当于一位便携导游，能够在游客观览展品时不必将目光长时间集中于繁多的文字上，而是可以边听边看。

##### 需求说明
1. 当用户阅读不便时，用户通过点击播放键便能听到文物知识拓展的介绍，此时播放键变为暂停键。点击暂停键，暂停语音朗读。
2. 用户点击播放键时显示文字提醒用户“仅支持听筒和耳机播放。为减少对其他游客的影响和给您更好的体验，建议您使用耳机聆听。”
3. 用户可以通过时间选择的滑块控件，选择想要听的部分。
4. 用户可以通过长按任一句子选择“朗读”，聆听该句子的语音。
5. 播放的字段高亮显示，手机息屏后依然可以播放。
6. 语音的语言根据用户选择的语言进行改变。

#### 三、
##### 模块描述

 _语言选择_ 

##### 功能描述
通过机器翻译，为国外游客提供可理解的文本翻译和语音服务。

##### 需求说明
1. 用户首次使用，扫描文物后打开语言选择页面，默认为“中文”选项，每项语言选择主要以其当地语言表示，辅以英文表示。
2. 语言选项以英文首字母A-Z进行排序，以下拉列表的形式展开。
3. 首次选择后，所有的知识拓展内容和语音朗读均默认为首次被选择的语言。
4. 若用户想要更改语言，进入知识拓展页面后，可点击语言选择模块，选择需要的语言，知识拓展页面的文字和语音朗读变为更改后的语言。
##### 需求列表
| 需求 | API | 重要程度 
| :-----| ----: | ----: 
| 查看到被扫描文物的基本信息和拓展信息。 |  微软图像识别API|重要
| 边听边看 | 语音合成|次要
| 为国外游客提供可理解的文本翻译和语音服务。 |  机器翻译|重要

- ### 功能总览流程图
[核心交互原型]( http://jackonz2017.gitee.io/bowuguan)
![功能总览流程图](https://images.gitee.com/uploads/images/2019/1118/131602_c32a2a88_1648150.png "功能总览流程图.png")

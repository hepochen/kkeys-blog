kkeys-blog
==========
原文链接：：[http://kkeys.me/post/20130218a](http://kkeys.me/post/20130218a)  

kkeys-blog 是我的[博客](http://kkeys.me)的模板，而我的博客使用的是Farbox的服务，具体Farbox是做什么，想必看官你已经知道了，不知道的在[Farbox](http://http://www.farbox.com/)的首页可以看到他们的宣传视频。

Farbox可以让你自己定制模板，也可以clone别人的模板，但是看来clone功能还不太好用（因为有几个人都问我是否开源了模板代码），而且我确实为这个博客做了很多定制。现在我的博客的模板已经开源了，这篇文章就是介绍下使用细节，有不懂的欢迎留言,我做了个[demo](http://test-kkeys.farbox.com/),可以先去看看效果如何。

文件结构：

    |---catalog  #把你的文章丢在这个文件夹下面，按时间放，2013年的文章丢2013文件夹下
    |      |---2013
    |      |---2014
    |---template       #这个文件夹下面放的是模板文件，如果要定制的话，来这看源码吧
    |       |---page                  #放about页面和catolog页面的模板
    |       |    |---about.html
    |       |    |---category.html
    |       |---errors                                  #404.html 错误页面
    |       |     |---404.html
    |       |---img        #这里面放了本站要用的一些图片，包括favicon，和你的头像
    |       |---css                                #如果你不懂，那也没必要懂了
    |       |---js                                                   #同上
    |---README.md                                                    #本文
    |---site.md                       #配置文件，如果你不定制，就只用改这一个文件
    |---domain.config         #你的独立域名，也可以用farbox任意未被使用的二级域名

**首先**  
准备两站图片，一张命名为favicon.ico（不懂？google吧），一张命名为face.png（你的头像），两张都放到template——img文件夹下面

**然后**  
在domain.config中写下你要用的域名，可以是自己的独立域名，也可以是Farbox的任何还没有被使用的二级域名
像这样就可以了：  
>kkeys.me

**接着**  
在site.md中填写相应项，选项有：
>site-name:"Your site name"  
name:"Your nickname"  
motto:"What you believe"  
\# **email**:"your email address"  
\# example：xxxx@gmail.com  
\# **twitter**:"your twitter account"  
\# example：https://twitter.com/kkeys_me  
\# **github**:"your github account"  
\# example：https://github.com/farmerworking

应该还蛮简明的吧，呵呵，打警号的是不会显示的信息，如果你想要显示，就填写过相应项后把警号去掉。（*ps：example前面的警号就不要去掉了*）

**最后**  
定义你自己的about页面之后，你的网站完成了，去你的网站看看效果如何吧，如果有bug，欢迎提交给我，然后别忘记了把READE.md（本文）删了，不然会显示在你的blog里面，现在可以开始享受写作了(ps:留言功能自己找disquz吧)。

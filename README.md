####一点点说明

这是[MingoZone.com](http://MingoZone.com)的个人首页说明
## 列一下目录内容
1. _config.yml <一些个人设置>
2. _includes <可以复用的一些模块,比如公共头部,脚步,导航.方便通过{ % include head.html %}（去掉前两个{中或者{与%中的空格，下同）灵活的调用。这条命令会调用_includes/head.html文件。>
3. _layouts <这是模板文件存放的位置。模板需要通过[YAML front matter](https://github.com/jekyll/jekyll/wiki/YAML-Front-Matter)来定义，{ { content }}标记用来将数据插入到这些模板中来。>
4. _posts <你的个人博客区域,命名是2016-04-07-artical-title.MARKUP这样的形式，MARKUP是你所使用标记语言的文件后缀名，根据_config.yml中设定的链接规则，可以根据你的文件名灵活调整，文章的日期和标记语言后缀与文章的标题的独立的。>
5. _site <这个是Jekyll生成的最终的文档，不用去关心。最好把他放在你的.gitignore文件中忽略它>
6. 其他文件夹 <你可以创建任何的文件夹，在根目录下面也可以创建任何文件，假设你创建了project文件夹，下面有一个github-pages.md的文件，那么你就可以通过yoursite.com/project/github-pages访问的到，如果你是使用一级域名的话。文件后缀可以是.html或者markdown或者textile>
7. 以上都是转的 =_=~

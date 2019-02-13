![每日美图](https://upload-images.jianshu.io/upload_images/13419832-b28223719a47c5d9.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
#介绍
在学完了sass语法之后我们可以正式开始学习bootstrap-4.0的源码啦，还不熟悉sass的读者可以查看我的[sass专题呀](https://www.jianshu.com/c/9c1d5608c810)。
在学习bootstrap之前我们也是一样需要下载bootstrap的源码，读者可以点击[链接](https://codeload.github.com/twbs/bootstrap/zip/v4.0.0)下载,下载完成之后同样需要导入webstrom中。
如果还不知道如何安装sass与webstorm的读者也可以点击[Sass开发环境安装](https://www.jianshu.com/p/7c9aa05782e6)进行查看并安装。
#初次尝试
在完成了环境安装之后，可以编写如下的test.html:cloud:
```html
<!doctype html>
<html lang="zh-cn">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS 此处引入本地sass源码编译后的css -->
	  <link rel="stylesheet" href="./bootstrap-4.0.0/scss/bootstrap.css">  

    <title>Bootstrap初探</title>
  </head>
  <body>
  <div class="container">
   <div class="alert alert-primary" role="alert">
    这是个测试
</div>
  </div>
   

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://cdn.bootcss.com/jquery/3.2.1/jquery.slim.min.js" integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN" crossorigin="anonymous"></script>
    <script src="https://cdn.bootcss.com/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>
    <script src="https://cdn.bootcss.com/bootstrap/4.0.0/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script>
  </body>
</html>
```
此处需要特别说明的是我们引入bootstrap.css是我们编译bootstrap-4.0.0源码后产生的本地css
![运行截图](https://upload-images.jianshu.io/upload_images/13419832-6738731cdbfd5385.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

接下来我们修改一下bootstrap源码目录scss/_variables.scss第37行的
`$blue:    #007bff !default;`变为`$blue:    #06fff6 !default;`
等待新的css文件编译完成后重新刷新页面我们发现原先的页面发生了变化
![修改后运行截图](https://upload-images.jianshu.io/upload_images/13419832-4021cd378bf25fad.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
至此我们已经初次对bootstrap进行了自己的定制化，接下来我们会针对bootstrap的css内容进行学习，明白它为什么可以实现响应式，为什么可以方便的定制化。

#总结
1. 需要安装配置sass编译环境，webstorm编辑工具；
2. 需要bootstrap-4.0源码；
3. 初次对源码进行修改，定制化bootstrap-4.0；
4. 该文章所有内容可点击[链接](https://github.com/OnlyPiglet/bootstrap4/tree/master/20190212)查看。

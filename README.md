# Video-background-page
仿墨迹天气视频首页
> 本文首发于效果预览：http://www.ethan997.com:8080/holiday_project/intro/intro.html<br/>
> github项目地址：https://github.com/sunshine940326/canvas-nest
> 

首先上效果图：
![最终效果图](http://upload-images.jianshu.io/upload_images/6089846-bcb7d0951503c5d4.gif?imageMogr2/auto-orient/strip)
>

实现起来也是很简单的， 按照我的步骤一步一步来就可以了~
# html代码
首先要制作我们的页面，用到的是html5的新标签video
```
<body>
   <video autoplay loop poster="polina.jpg" class="bgvid" id="bgvid">
          <source src="http://cdn.moji.com/websrc/video/video621.mp4" type="video/mp4">
    </video>
</body>
```
# css样式
css样式也没有什么好说的，只是要让视频充满屏幕、循环、无声、直接播放、隐藏按钮和不重复就可以了。
```
 body{
        background-color:gray;
        background:url("http://cdn.moji.com/websrc/video/video621.mp4") no-repeat center 0px;
    }
 video#bgvid {
        position: fixed; right: 0; bottom: 0;
        min-width: 100%; min-height: 100%;
        width: auto; height: auto; z-index: -100;
        background-size: cover;
    }	
```

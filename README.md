# Video-background-page
模仿墨迹天气首页，利用视频作为网页背景。
html核心代码：
<video autoplay loop poster="polina.jpg" class="bgvid" id="bgvid">
        <source src="http://cdn.moji.com/websrc/video/video621.mp4" type="video/mp4">
</video>
css核心代码：
video#bgvid {
   position: fixed; right: 0; bottom: 0;
   min-width: 100%; min-height: 100%;
   width: auto; height: auto; z-index: -100;
   background-size: cover;
		}

#HTML媒体标签
1. audio 音频
- src属性 
- controls 控制面板（要想显示 必须添加这个属性）
- autoplay 自动播放
- loop 循环
`<audio src="">`
2. video 视频
- src属性 
- controls 控制面板（要想显示 必须添加这个属性）
- autoplay 自动播放
- loop 循环
- width
- height
<!-- 设置宽高时 一般情况下 只会设置宽度或高度其中一个值 让其自动的等比缩放 如果同时设置宽度或者高度 那么视频不会自动调整到设置的宽高 除非设置的值刚好是等比例的  -->
<!-- 
  不同浏览器支持的视频格式不一样
  HTML5提供了source标签 可以准备多个格式的视频文件 让浏览器自动选择  
-->
- poster 当视频还没有完全下载 或者用户还没有点击播放前的默认显示的封面 默认情况显示当前视频文件的第一帧 可以手动设置图片为封面
`<video  src="" ></video>`
```
<video controls>
  <source src="" type="video/flv"></source>
  <source src="" type="video/mp4"></source>
  <!-- 当浏览器都不支持source里面的格式时  允许提示信息 -->
  您的浏览器不支持当前的视频播放
</video>
```
## 以前解决方案:

1.通过flash插件 增加学习成本 ios设备不支持flash
2.embed 直接插入视频音频文件 本质上是调用本机上已经暗转的软件  有兼容性问题

# 什么是HTML5
1. HTML5不是新的语言 而是html语言的第五次重大修改版本
2. 支持 ：所有的主流浏览器支持h5（chrome,firefox,safari）
    IE支持情况
      IE8以下都不支持  在ie8中不认识语义标签 无法解析 即所写样式无效
        解决方案：
         1. 在html中手动创建标签,以及将所创建的标签设置为块级元素
          ```
            <script>
              document.createElement('header')
            </script>
          ```
          2.引入第三方插件 就可以正常显示这些语义化标签
          `<scipt src="./html5shiv.min.js"></script>`
      IE9 部分支持（实现兼容：将语义化标签设置 display:block）
      IE10完全支持

3. 改变了用户与文档的交互方式 新增了许多多媒体标签 video,audio,canvas
4. 增加了其他新的特性 语义特性，本地存储特性，网页多媒体，二维三维，特效（过渡，案例）
5. 相对H4 
  - 进步 抛弃了一些不合理不常用的标记和属性
  - 新增一些标记和属性（表单）
  - 从代码角度看，h5的网页结构代码更简洁


# 语义化标签
1. 种类
- <header></header> 页眉
- <nav></nav> 导航
-  <main></main> 主体部分
- <article></article> 文章
- <section></section> 区块
- <aside></aside> 侧边栏
- <footer></footer> 页尾

2. 兼容性
- 语义化标签在ie9中被解析为行级元素 
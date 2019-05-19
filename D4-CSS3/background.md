## background
1. 添加背景颜色
background-color
2. 添加背景图片
  background-image：url("")
  如果图片大小大于容器的大小，则默认从左上角开始放置
  如果图片大小小于容器，那么图片默认会平铺
3.设置背景图片平铺
  background-repeat:no-repeat/repead/repead-x/repeat-y
  新增属性值：
    - round 会将图片进行缩放 再进行平铺
    - space 不会缩放图片 会在图片之间产生间距
4. 设置在滚动容器种背景的行为:跟随/固定
  background-attachment:fixed(固定)/scroll跟随滚动/local
  设置fixed之后 背景图片会默认平铺 
  fixed 背景图片的位置固定不变
  scroll 当滚动容器时 背景图片也会跟随滚动
  local与scroll的区别
  前提：滚动当前容器的内容
  在容器中：
  local：背景图片会跟随内容一起滚动
  scroll：背景图片不会跟随内容一起滚动
  5. background-size:设置背景图片的大小
  宽度 高度 /宽度 auto
  建议：要确定图片宽高比与容器宽高比一致 不然图片会变形
  设置百分比 是参照父容器的宽 高 50% * width 即最后图片显示的宽
  contain：  
  auto 自动/number 数值/percentage 百分比/cover 放大铺满（图片显示不全）/contain 缩小铺满（有可能造成空白效果）
  6.设置背景图片偏移
    background-position:
  **移动端响应区域**
  7.background-origin 设置背景图片坐标原点 默认是在容器左上角
    属性值：
      padding-box 设置从padding位置开始背景填充
      border-box 设置从border
      content-box 设置从content
  8.background-clip 设置内容裁切  设置的是裁切 控制的是显示
      
      border-box 显示border以内的内容
      padding-box 显示padding以内的内容
      content-box 显示content以内的内容


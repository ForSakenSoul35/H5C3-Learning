## flex 布局
1. 使用flex布局
  在父容器上设置flex display:flex;
2. 基本概念
  主轴：
  交叉轴：
2. 容器属性 设置在容器上的属性
  (1)flex-direction: 设置主轴的方向-即项目的排列方向
  属性值：
  - row 默认水平方向 起点在左端
  - column 垂直 方向  起点在上边
  - row-revere
  - column-recerse 

  (2)flex-wrap:设置是否换行 
  属性值： 
  - nowrap 不换行 默认
  - wrap
  - wrap-reverse 换行 第一行在下面

  (3)flex-flow: flex-direction flex-wrap的 简写方式 一般不用

  (4)justify-content:设置主轴对齐方式 （默认主轴方向为水平方向 即设置水平方向上的排列方式）
    属性值：
    - flex-start 靠左
    - flex-end 靠右
    - center  居中对齐
    - space-between  左右与容器盒子没有间距 中间平均分布
    - space-around  左右与容器盒子有间距  

  (5) align-items : 定义项目在交叉轴的对齐方式（默认交叉轴 为垂直方向，即为设置垂直方向上的排列方式）
   
  (6) align-content 定义了多根轴线的对齐方式 如果只有一根轴线，则不起作用
  默认情况下：主轴方向有多行
  属性值：
  - flex-start 与交叉轴的起点对齐(默认情况下 靠上对齐)
  - flex-end  与交叉轴的终点对齐 靠下排列
  - center 与交叉轴的中点对齐 居中排列
  - stretch 默认值  轴线占满整个交叉轴（每根轴平分交叉轴的空间）
  - space-around 每根轴线两侧的间隔都相等
  - space-between 与交叉轴两端对齐 轴线之间的间隔平均分布

  3. 项目的属性
  (1)order 定义项目的排序顺序 数值越小，排列越前面，默认为0
  (2)flex-grow 定义项目的放大比例 默认为0 即如果存在剩余空间，也不放大
    - 如果所有项目的flex-grow属性都为1 则它们将平分所有剩余空间，如果有的话。如果一个项目的flex-grow为2，其他为1，则前者占据的剩余空间将比其他项多一倍
  (3)flex-shrink 定义项目的缩小比例 默认为1 即如果空间不足，该项目将缩小
  - 如果所有的项目flex-shrink都为1 当空间不足时，都按比例缩小，如果一个项目的flex-shrink为0 其他为1，则空间不足时，前者不缩小

  (4)flex-basis  定义了在分配多余空间时，项目占据的主轴空间。浏览器根据这个属性，计算主轴是否有多余空间。默认值是auto，即项目的本来大小
  - 他可以设置width或者height一样的值，则项目将占据固定空间
  (5)flex  是flex-grow flex-shrink flex-basis 三个值的简写 ,默认为0 1 auto。后两个属性可选。
  - 快捷值： auto （1，1，auto）  放大为1 缩小为1 主轴空间auto 表示自动撑满剩余空间
             none（0 0 auto） 不放大 不缩小 
  - 建议使用这个属性 而不是单独写三个分离的属性
  (6)align-self  允许单个项目有与其他项目不一样的对齐方式，可覆盖align-items属性
  - 默认为auto 表示继承align-items 如果没有父元素  相当于stretch
  - 属性值 除了auto 其他与align-items一致
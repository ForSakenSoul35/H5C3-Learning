# 表单新增type属性

1. type="email"  提供了默认的电子邮箱的完整验证
  需要包含@ 同时需要包括完整服务器名称 
  如果不能满足验证，则会阻止当前提交
2. type="tel"  并不是来实现验证，本质目的是为了在移动端打开数字键盘
  限制了用户只能数字
3. type="url"  对网址进行验证 只能输入合法的网址
  必须包括http；//
4. type="number"  只能输入数字，包含小数点 其他内容不可输入
  提供上下箭头 可以点击调整大小
  可以设置默认值 最大值 以及最小值
  <input type="number" value="1" max="10" min="0">
5. type="search" 是一个搜索框 右边会有一个清除输入内容的删除键
  提供更人性化的输入体验
6. type="range" 表示范围 有value，max，以及min属性
7. type="color" 提供颜色拾取 
<!-- 时间相关 -->
8.  type="time" 小时 分钟 秒钟
    type="month" 哪一年月份
    type="week" 哪一年第几星期
    type="date" 年月日  
    type="dateTime"  大多数浏览器一般不能用 只有safari能用
    type="dateTime-local" 年月日 时分秒

# 表单新增属性
- 提示文本：placeholder 
- 自动获取焦点： autofocus
- 自动填充： autocomplete="on/off" on打开 off 关闭
  使用前提 ： 
    1.必须成功提交一次之后 才会做记录
    2.当前添加autocomplete属性的元素 必须有name属性
- 必须输入 required  没有输入 则会阻止当前提交操作
- 正则验证： pattern="^(\+86)?1\d{10}$"
<!-- 
  正则：
    * 代表任意个
    ？ 代表0个或1个
    + 代表1个或多个
 -->
- 多个文件上传  multiple表示可以选择多个文件
 `<input type="file" multiple>`


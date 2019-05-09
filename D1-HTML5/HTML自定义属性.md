# 自定义属性
1. 如何定义
通过 data- 开头  至少有一个值
属性名称都使用小写 不包含特殊符号 数字 多个单词使用-连接
`<p data-info-name="xhb"></p>`
2. 如何取值
var p =document.quertSeletor('p');
<!-- 自定义属性 都放在dataset这个数组里面 通过驼峰命名法 取值-->
p.dataset['InfoName']
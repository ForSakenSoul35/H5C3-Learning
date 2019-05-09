# DOM操作
1. 获取元素
<!-- 通过索引值获取元素 不直观  -->
querySelector("")
querySelectorAll("")
2. 修改样式 通过classList 添加，切换，删除，判断
只能同时添加或者移除一个
remove 移除 只会移除样式 不会移除class属性
- 添加
document.querySelector("").classList.add("red")
- 删除
document.querySelector("").classList.remove("red")
- 切换 如果元素之前没有指定的class属性 则添加 如果有 则移除
document.querySelector("").classList.toggle("red")
- 判断是否包含指定的class 返回布尔值
document.querySelector("").classList.contain("red")

<!-- 对比之前对className的操作 -->
document.querySelector("").className="red"
 - 缺点 容易层叠掉 原来的类名 导致样式失效
 <!-- 操作行内样式  -->
 document.querySelector("").style.display=""
 - 只能操作行内样式
 - 写了行内样式   对应的元素上 才会有style属性 
 
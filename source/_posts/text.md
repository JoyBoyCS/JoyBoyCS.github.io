---
title: text
date: 2023-11-18 14:02:00
tags: [111] # 确保标签格式正确,使用方括号
categories: web
---

# Wang An Lei

## Sdasd

daaaaaaaaaaas

dsadddddddddds

<!--more-->
- 列表
- 列表2
  - 子列表 # 使用空格缩进表示层级关系
  - 子列表
- 列表3

<!-- 这里假设'caniuse获取'是自定义标签,需要对应的Hexo插件 -->
{% caniuse '获取' %} 

<div class="text-center"> <!-- 修正了div标签 -->
  <!-- 假设'btn'是自定义标签,需要安装适当的插件来支持 -->
  {% btn 'https://github.com', 'GitHub', 'fab fa-github fa-fw fa-lg', 'GitHub' %}
</div>

<!-- 同样,'gp'和'endgp'标签需要相应插件的支持 -->
{% gp '5-2' %} 
![](/images/next.svg) 
![](/images/next.svg) 
![](/images/next.svg) 
![](/images/next.svg) 
![](/images/next.svg)
{% endgp %}

[王](https://www.bilibili.com/)
<img src="https://github.com/JoyBoyCS/blog-img/blob/main/img/compressed.jpg?raw=true" width="400" height="400">

<!-- 对于'mermaid'支持也必须确保你的Hexo有对应的插件 -->
{% mermaid gantt %}
dateFormat YYYY-MM-DD
section 部分
已完成 :done, des1, 2014-01-06,2014-01-08 
Active :active, des2, 2014-01-09, 3d 
Parallel 1 : des3, after des1, 1d
Parallel 2 : des4, after des1, 1d
Parallel 3 : des5, after des3, 1d
Parallel 4 : des6, after des4, 1d
{% endmermaid %}

```flow
st=>start: 开始
ipt=>inputoutput: 输入一个x
op=>operation: x=x+1
cond=>condition: 溢出了吗?
sub=>subroutine: 重置x
io=>inputoutput: 输出x
e=>end: 结束

st->ipt->op->cond
cond(yes)->io->e
cond(no)->sub->op
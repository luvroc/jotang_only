# jotang_only
招新 
<h3>目录</h3>
<ul>
<li><a href="#process">学习历程</a></li>
<li><a href="#works">成果展示</a></li>
<li><a href="#unfinished">未完成部分思路</a></li>
</ul>
<h4 id="process">学习历程</h4>
<p>从军训开始看到synx的前端题，
本身有C语言学习基础，又想做一点和C语言很难做到的东西，
于是尝试从0开始入门web前端。<p>
一开始的学习很不规范，比如
<ul>
<li>学html学到div和span后戛然而止
<li>css和js一起学习，很快但未必掌握牢靠
</ul>
结果就是后面开始来补前面漏下的知识。
所幸经过拷打后再学，基础已经比开始好很多了。
<p>
<h4 id="works">成果展示</h4>
<ul>
<li><a href="https://github.com/luvroc/jotang_only/tree/main/reallyLuv">个人博客</a>：包含三页，完成度一般，个人的遗憾是写了很多效果未必好
<li><a href="https://github.com/luvroc/jotang_only/tree/main/bili">b站尝试</a>：暂时只写了样式，会把后续的完成思路写到下一节
</ul>


<h4 id="unfinished">未完成部分思路</h4>
<p>如果看到这里,建议先看完bili里的各个example,你可以从中一步步看出我搭建样式布局的过程.
从而更好理解后续的部分.
<p>1.悬停展示导航栏标签:<ul>
<li>首先提前写好一个盒子,同时填充内容且设置visibility为 none,之后js再获取元素,绑定onmouseenter和onmousedown,
从而做到悬停时改动element.style.visibility属性为可视
<li>另一种思路是在js里创建节点并填入内容(存储为数组),再绑定事件悬停展示.
</ul>
<p>
考虑到B站的导航栏展开内容很多样,个人偏向第一种,第二种更适合后续推荐视频的无限刷新
(当然内容就不会存储在js里,而是ajax获取)
<p>2.悬停播放视频(惭愧的是,练习时从未碰过视频音频,过)
<p>3.评论区制作(参考我自己博客里的)
<ul>
<li>要有头像,输入input\textarea,字数限制提示,以及一个提交按钮
<li>另外要有别人的评论展示,同时有点赞,踩,评论,分享之类(楼内评论和分享先饶过我吧)
<li>样式写好(不小的工作量)
<li>完成输入评论:绑定提交按钮的事件为:获取文本框的value,存入localStorage(setItem)
另外输入时以value的length属性填入到字数提示里.
<li>展示评论:getItem获取存储内容(键值对格式与存储评论一致),填入dom里(头像还是别存里面了)
<li>点赞互动:思路为存一个boolean变量,在点击时判断之使另一个加一,再次点击取消加一
</ul>

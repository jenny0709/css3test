# css3test
css3笔记

-------------------------

## css3选择器
	1.后代选择器
	- div p
	选中div元素里面的所有p元素;
	- div>p
	选中父元素div里面的所有子元素p;
	- .list li:only-child
	选中list中的作为唯一的li子元素存在;
	- .list :only-child
	选中list中的只有唯一一个子元素的元素;
	- p:nth-child(2)
	选中父元素中第2个子元素p,n可以是数字或公式(n是所有的,2n是偶数个,3n是3的倍数个,2n-1是偶数个);
	- p:nth-last-child(3)
	选中父元素中倒数第2个子元素p,同上;
	- p:first-child
	选中属于父元素中第一个子元素为p的每个元素;
	- p:last-child
	选中属于父元素中最后一个子元素为p的每个元素;
	- :root
	选择文档的根元素 
	- p:empty
	选中没有子元素的每个p元素(包括文本节点)
	
	2.同辈选择器
	- div+p
	选择紧跟在div之后的所有p元素
	- p~ul
	选择p元素之后的每个ul元素
	
	3.伪类选择器
	- :focus 匹配获得焦点的input元素
	- :first-letter 匹配p标签的第一个文字
	- :before 在每个p元素的内容之前插入内容(行内标签)
	- :after 在每个p元素的内容之后插入(行内标签)

> :before、:after 功能
> 1. 清除浮动
```css
/*清除浮动*/
.clf:after,.clf:before{
	content="";
	display:block;
	clear:both;
}
```
> 2. 做一些常用效果“”,背景图片




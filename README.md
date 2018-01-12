## 功能介绍

- 为html文档生成toc
- 右边浮动

## 用法

可以参考example.html：

```html
<script type="text/javascript">
//<![CDATA[
	var firstLvl = 2; // h2开始
	var lastLvl = 4;  // h4结束
	var divID = "TOC";
	var divToSearch = "articles";
	window.onload=function(){
			//参数控制
			// 参数一：起始level，默认为h2
			// 参数二：末位Level，默认为h3
			// 参数三：用于生成toc的divID，默认为TOC
			// 参数四：搜索headlines的divID
			toc(firstLvl, lastLvl, divID, divToSearch);
			diyStyle(divID);
			addNewStyle('.TOCSectNum {margin-right: 0.5em;}');
	}
//]]>
</script>
```

## 关于代码

本simpletoc代码主要修改自[这里](https://www.cnblogs.com/qiudeqing/p/3229583.html)，具体出处不明。
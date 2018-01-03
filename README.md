# markmapview
## 介绍

此插件的作用是，生成一个markdown文档的标题树。使用了svg和d3.js，所以只兼容IE9以上浏览器。
此插件通过修改markmap而来。

## 集成的工具

- 1、remarkable.js 1.6.0；用于解析markdown文档
- 2、d3.js 3.5.17；用于渲染标题树
- 3、markmap；将markdown文档标题树提取成json对象
- 4、自定义的init.js；定义了2个使用方法

	> TODO：方法的回调函数和返回值

## 使用方法

- 1、引入markmapview.js；在文档中插入一个svg标签
- 2、使用markmapviey函数生成markdown标题树

		//svgTagId string 插入到文档中的svg标签的id
		//text string markdown文档内容
		markmapview(svgTagId, text);

- 3、使用markmapvieyFromUrl函数生成markdown标题树。异步请求文档资源

		//svgTagId string 插入到文档中的svg标签的id
		//url string markdown文档资源链接
		markmapviewFromUrl(svgTagId, url);

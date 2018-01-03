# pagination

| selector  | totalPage |  currentPage | prev   | next   |  first     |   last     | jumpBtn |jumpBtn |pageOneLoad|count|showTotalPage
| :----: 	| :----:  	|  :----:      | :----: | :----: |  :----:    | :----:     | :----:  |:----:  | :----:  | :----:  | :----:  |
| 选择器（id）| 总页数  | 当前页(默认1)| 上一页 | 下一页 | 显示首页   | 显示尾页   |支持跳转 |支持跳转 |首页加载 |当前页前后显示的数量 |显示总页数 |
|  #page   	| 30    	|   1          |   <    |   >    | true/false | true/false | true/false| true/false| true/false| 2|true/false|


## 使用示例
> 通过js动态添加样式，class：pagination必须

```html
<div class="pagination" id="page1"></div>
```
```js
pagination({
	selector: '#page1', // 选择器
	totalPage: 30, // 总页数
	currentPage: 1, // 当前页
	prev: '上一页', // 上一页，可设置 <
	next: '下一页', // 下一页，可设置 >
	first: true, // 是否显示首页
	last: true, // 是否显示尾页
	showTotalPage: true, //是否显示总页数
	jumpBtn: true, // 需要跳转的输入框
	pageOneLoad: true, // 首页加载与否
	count: 2//当前页前后显示的数量
},function(val){
	// 当前页
	$.ajax({})
	console.log('page1当前页',val)
})
```


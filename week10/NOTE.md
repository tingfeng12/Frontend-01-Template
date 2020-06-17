# 每周总结可以写在这里
将元素的所有子元素逆序
	1.笨办法  将子元素倒序插到另一个元素上 在copy回来
	2.原地转换 （不新加元素）
		let el = document.getElementById('a');
		  function reverse(element) {
			let children = element.children;

			for (let i = children.length - 1; i >= 0; i--) {
			  element.append(children[i]);
			}
		  }
	3.标准答案
		1.取length
		2.while(l-- > 0)
		3. appendChild最后一个子节点元素
Range API（属于DOM API）
	代表DOM树中间的部分片段
	
	Range API有：
		XXX
		XXX
		XXX
	
	创建Range
		使用new  
	使用range
		.selectNodeContents
		
	使用Range的好处 
		只重排一次，（减少重排）
		
	
	
	
	
	
	
	
	
CSSOM
	document.styleSheets继承了StyleSheet
	Rule
	
	论如何用原始API写出后端懵逼的前端代码
	
	
	getComputedStyle
		window.getComputedStyle(elt,pseudoElt)
		elt想要获取的元素  pseudoElt可选，伪元素
	
range切割style		可以进行切割，不会报错	
range可以切割所有元素	
datauri

视口滚动
scroll 滚动到（位置）
scrollBy滚动（多少）
	
	

	
	
	
	
	
	
		

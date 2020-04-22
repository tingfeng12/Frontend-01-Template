# 每周总结可以写在这里
第二周笔记 JS部分
编程语言通识
	语言按语法分类
		1.语言形式（中文，英文）
		2.非形式语言（乔姆斯基谱系）{
			0型		无限制文法 
				等号左右可以有多个非终结符
			1型		上下文相关文法
				等号左右可以有多个内容，但是头尾固定
			2型		上下文无关文法
				语句在哪的意义都一样，不管在哪里都是这些产生的
			3型		正则文法
				只
			
	产生式（BNF）
		尖括号括起来的名称表示语法结构名
		语法结构分为基础结构和需要用其他语法结构定义的复合结构
			基础结构称终结符
			非基础结构称非终结符
		引号和中间的字符表示终结符
		可以有括号
		*表示重复多次  |表示或   +表示至少一次
		
		设计a,b两种组成的语言
		四则运算
			<Number> = "0" | "1" | "2" | ..... | "9"

			<DecimalNumber> = "0" | (("1" | "2" | ..... | "9") <Number>* )

			<PrimaryExpression> = <DecimalNumber> |
				"(" <LogicalExpression> ")"

			<MultiplicativeExpression> = <PrimaryExpression> | 
				<MultiplicativeExpression> "*" <PrimaryExpression>| 
				<MultiplicativeExpression> "/" <PrimaryExpression>

			<AdditiveExpression> = <MultiplicativeExpression> | 
				<AdditiveExpression> "+" <MultiplicativeExpression>| 
				<AdditiveExpression> "-" <MultiplicativeExpression>

			<LogicalExpression> = <AdditiveExpression> | 
				<LogicalExpression> "||" <AdditiveExpression> | 
				<LogicalExpression> "&&" <AdditiveExpression>
				
		正则分析四则运算
	其他产生式
		JS属于其他产生式
	现代语言的特例
		C++中 *可能表示乘号或指针，具体表示什么  取决于星号前的标识符是否被声明为类型	C++是非形式化语言
		VB中 <表示小于号也可能是XML直接量的开始，取决于当前位置是否接受XML直接量		
		python中 tab符和空格会根据上一行行首空白以一定规则处理成虚拟终结符indent或dedent
		JavaScript中/可能是除号也可能是正则表达式开头处理方式类似于VB字符串模板中也需要特殊处理}还有自动插入分号规则
		
	计算机语言分类
		按照语言用途分类
			数据描述语言
				JSON，HTML，XAML，SQL，CSS
			编程语言
				C，C++，Java，C#，Python，Ruby，Perl，Lisp，T-SQL，Clojure，Haskell，JavaScript
		按语言表达方式
			声明式语言
				JSON，HTML，XAML，SQL，CSS，Lisp，Clojure,Haskell
			命令式语言
				C，C++，Java，C#，Python，Ruby，Perl，JavaScript
	
图灵完备性	
	命令式
		goto
		if和while
		*有if-while就是图灵完备性
	声明式——lambda
		递归
		
动态语言和静态语言
	动态
		在用户的设备/在线服务器上
		在产品运行时
		runtime
	静态
		在程序员的设备上
		产品开发时
		compiletime
	
	少出bug更静态的语言好
	
类型系统
	动态类型系统与静态类型系统
	强类型和弱类型(有隐式转换的就是弱类型)
		String+Number
		String == Boolean
	复合类型
		结构体
		函数签名
	子类型
		逆变/列表
	
一般命令式编程语言
	atom
		identifier
		Literal
		
JavaScript
	Atom(原子)
	Expression(表达式)
	Statement(语句声明)
	Structure(结构)
	Program/Module(程序/模块)
	
	
	
	
	
	
#TypeScrip
>TypeScript 是微软开发的 JavaScript 的超集，TypeScript兼容JavaScript，可以载入JavaScript代码然后运行。TypeScript与JavaScript相比进步的地方 包括：加入注释，让编译器理解所支持的对象和函数，编译器会移除注释，不会增加开销；增加一个完整的类结构，使之更新是传统的面向对象语言。

##如何编译 TypeScript
1. 安装TypeScrip
	* 通过Visual Studio安装
	* 通过nodeJS安装
> npm install -g typescript

2. 新建typescript文件——index.ts
	```javascript
		function greeter(person: string) {
    		return "Hello, " + person;
		}

		var user = "Jane User";
		
		document.body.innerHTML = greeter(user); 
	```

3. 编译ts文件,
> tsc greeter.ts  

	```javascript
		function greeter(person) {
		    return "Hello, " + person;
		}
		
		var user = "Jane User";
		
		document.body.innerHTML = greeter(user);
	```

##语言扩展
* 类 Classes
* 接口 Interfaces
* 模块 Modules 
* 类型注解 Type annotations
* 编译时类型检查 Compile time type checking 
* Arrow 函数 (类似 C# 的 Lambda 表达式)

###类型批注和编译时类型检查
>TypeScript 通过类型批注提供静态类型以在编译时启动类型检查。这是可选的，而且可以被忽略而使用 JavaScript 常规的动态类型。

```javascript

	function greeter(person: string) {
        return "Hello, " + person;
    }

    var user = "Jane User";
    document.body.innerHTML = greeter(user);
```

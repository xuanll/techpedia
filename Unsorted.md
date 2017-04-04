# 未整理

## [lua](https://www.lua.org/about.html)
> Lua is a powerful, efficient, lightweight, embeddable **scripting** language. It supports procedural programming, object-oriented programming, functional programming, data-driven programming, and data description.

> Lua combines simple procedural syntax with powerful data description constructs based on **associative arrays** and **extensible semantics**. Lua is **dynamically** typed, runs by interpreting bytecode with a register-based virtual machine, and has automatic memory management with incremental garbage collection, making it ideal for configuration, scripting, and rapid prototyping.

## 脚本语言
解释执行，无需编译，运行效率不高，运行时更耗费内存。

## notepad++快捷键
- `Ctrl+Q`Win下，注释

### 格式化输出`%02d`输出带占位符0的数据
```
    string.format("  %02d", number)
```

### lua中调用父类方法
1. 父类 = require("父类")
2. 子类中 父类.方法名(self, param[])调用

### lua类变量不用local修饰
~~local~~ UITerritory.logic = nil

### Json对象字符串格式，最外层需要加`{}`

```Json
  {"title":{"str": "titleStr"}}
```

### UV
> UV 是一种标准化了的 2D 坐标系统，等同于 XY 坐标系统，为了不和 XY 混淆，用 U 和 V 分别表示对应的 X 和 Y。UV 系统中， (0, 0) 表示左纹理的下角，(1, 1) 表示纹理的右上角。
> [Rocky Lai's blog](http://blog.shuiguzi.com/2016/07/03/TilingAndOffset/)

### Code陷阱
- 判断和`or`的混用，下列情况判断语句永远为真（`or`后的字符串为true）；即使改成`cell.identifier == ("left" or "right")`也无济于事，后面代码语句等价于`cell.identifier == "left"`
```lua
	if cell.identifier == "left" or "right" then
		-- logics here
	end
```


### 边界值

- `int` 32位 $\ -2^{31}$ ~ $\ 2^{31}$ 即 -2147483648 ~ 2147483648(十亿级,10位数)

### ASCII

[ASCII在线工具](http://tool.oschina.net/commons?type=4)


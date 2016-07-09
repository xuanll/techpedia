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

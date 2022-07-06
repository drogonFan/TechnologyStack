## 2.1 名称

`go`有25个关键字

```
break default func interface select
case defer go map struct
chan else goto package switch
const fallthrough if range type
continue for import return var

常量：true false iota nil
类型：int int8 int16 int64
    uint uint8 uint16 uint32 uint64 uintptr
    float32 float64 complex128 complex64
    bool byte rune string error
函数：make len cap new append copy close delete
    complex real imag panic recover
```

如果一个实体再函数中声明，它只在函数局部有效。实体的第一个字母的大小决定其可见性是否跨包。

## 2.2 声明

4个主要的声明：变量`var`,常量`const`,类型`type`,函数`func`。

变量
```go
// 忽略类型允许声明多个不同类型的变量
var name type = expression
// 短变量声明
name := expression
```

短变量声明不需要声明所有在左边的变量。

`指针`的值是一个变量的地址。指针的零值是`nil`。
指针是可以比较的，当两个指针指向同一个变量或者两个指针都为nil时相等。

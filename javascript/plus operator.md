## what

一元正号 ( + ) 运算符位于其操作数前面，计算其操作数的数值，如果操作数不是一个数值，会尝试将其转换成一个数值，就是说如果不是一个number类型的数值，一元正号会将其转换成一个number类型的数值

***



## how

```js
+3 // 3
+"3" // 3
+true // 1
+false // 0
+null //0
+function(param) {return param} // NaN
+{name: 'balhblah'} // NaN
+[1, 2, 3] // NaN
+[] // 0
+[1] // 1
```



## why

一元正号 ( + ) 是转换其他对象到数值的最快方法，也是最推荐的做法。因为它不会对数值执行任何多余操作。它可以将字符串转换成整数和浮点数形式。如果它不能解析一个值，则计算结果为 [NaN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/NaN)。
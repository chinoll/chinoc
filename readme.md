# ChinoC编译器

## C编译器的子集实现

### 注意⚠️：该编译器不是成品，以下已发现的bug列表
* flex库存在内存泄露
### 以下是feature
* 将C代码转换为HIR(High IR)
* 初步的include支持

### 编译时注意事项
* 请在Linux环境下编译

### 其他注意事项
* 要读取c文件可以在main.c里修改yyin指针

## HIR的语法
* 将表达式转换为逆波兰表达式
* 将for循环转换为while循环
* 其他的和C一样
* 将指针/数组声明转换为以下形式,type [m][n] * name
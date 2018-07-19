# php
## 变量作用域
* 全局作用域 global
再所有函数外部定义的变量，拥有全局作用域，除函数外，全局变量可以被脚本的任何部门访问.如果要在一个函数内部访问全局变量，需要使用global关键字。
```php
<?php 
$x=5; // 全局变量 

function myTest() 
{ 
    $y=10; // 局部变量 
    echo "<p>测试函数内变量:<p>"; 
    echo "变量 x 为: $x"; 
    echo "<br>"; 
    echo "变量 y 为: $y"; 
}  

myTest(); 

echo "<p>测试函数外变量:<p>"; 
echo "变量 x 为: $x"; 
echo "<br>"; 
echo "变量 y 为: $y"; 
?>
```
* 局部作用域
在函数内部声明的变量是局部变量，仅在函数内部访问。
